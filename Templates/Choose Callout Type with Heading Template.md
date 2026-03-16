<%*
const promptType = await tp.system.prompt("Callout Type");
const promptHeading = await tp.system.prompt("Callout Heading");

let output = [];


output.push(`> [!${promptType}]- ` + promptHeading);
output.push("> ");

tR += output.join("\n");
-%>