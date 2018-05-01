# JavascriptNotes

let vr = [{PN: "PN1"},{PN: "PN2"},{PN: "PN3"}]; let ls = [{lc: "en"}, {lc: "es"}];
var test1 = [].concat(...vr.map(v => ls.map(l => [].concat(v, l))));
var test2 = test1.map(e => let obj = {...e[0]}; obj.PN = e[0].PN+"_"+e[1].lc; return obj});
