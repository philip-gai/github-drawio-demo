# github-drawio

This repo shows how to use diagrams.net (draw.io) diagrams in your GitHub repo.

Reference: <https://github.com/jgraph/drawio-github>

## How to integrate diagrams.net (draw.io) with your GitHub repo

1. Open draw.io in GitHub mode (<https://app.diagrams.net/?mode=github>)
2. Authorize with GitHub\
    ![Authorize GitHub](assets/drawio-github-authorize.png)
3. Choose the file you would like to edit OR Create a diagram in a new location
    - File should be editable bitmap image png or svg
    ![Authorize GitHub](assets/drawio-github-createedit.png)
    ![Create diagram screenshot](assets/create-diagram-screenshot.png)
4. Make changes, save and commit
5. Your png or svg file is now in your repo and contains a copy of your diagram in its metadata
6. In your markdown
    1. Reference the image like you would to any image
    2. On click, have the user navigate to diagrams.net and begin editing

    ```markdown
    [![Test Embedding draw.io](./Test%20Embedding.drawio.png)](https://app.diagrams.net/#Hphilip-gai%2Fgithub-drawio%2Fmain%2FTest%20Embedding.drawio.png)
    ```

## Example

### PNG

[![Test Embedding draw.io](./Test%20Embedding.drawio.png)](https://app.diagrams.net/#Hphilip-gai%2Fgithub-drawio%2Fmain%2FTest%20Embedding.drawio.png)

### SVG

[![Test Embedding draw.io](./Test%20Embedding.drawio.svg)](https://app.diagrams.net/#Hphilip-gai%2Fgithub-drawio%2Fmain%2FTest%20Embedding.drawio.svg)

## Notes

- Images in markdown are cached and can take a few minutes to update
- The edit link has to reference what branch to edit the diagram on. In this case I used `main`
