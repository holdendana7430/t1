代发 wailian999

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2adlkatnd.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kpbuhmew.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2mjldxgni.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2qbxdlrxs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ghloukgr.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2tngfwife.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2beqvfbyc.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2zjridyrq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2kijlyslg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zfmsjiom.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2meajkwdx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uphzewxz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2jkjqhqmp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2fcphwjfh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2bvrqdact.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2julidkny.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fsgnadzy.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2rlosqfqa.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kohbbgva.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2hkodjflh.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2hgjelaoy.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rntcebcq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2oonprshv.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ovoavsgm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2kwhharrm.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2sruhzucv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2whldaust.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ylkfrsav.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2frewlrpw.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zaaxzgdw.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ldfqbscx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2fcujwwmg.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2edngwaci.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zlfryyry.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2mjenyfno.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2fefxtjxo.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2fpflrhtd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2caoorobt.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2owanclkm.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2quhcpgsu.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2ytoeyplp.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ypobsqld.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2zgaoleio.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2pvobewlx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2hoxaxhrm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2gnbdlmtl.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2twgjbxlb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2mqhrmqei.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ulupczuz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2sskipmmz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2tdpzuuni.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wjkwjqmw.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2novbegbk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2vdelivup.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ceduirks.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jmjibhch.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tafekcff.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dbvtsrrc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lgrpiahy.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cgkzjabc.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jixuebkg.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2dnadjztk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2dpjfgtqx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2caalkheo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2zdnqotyy.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2kfwmwrmg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ggoyofrg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wmcvuruk.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2twuriigk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2fhraomrw.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2qjshlhsx.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2kdghysgy.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2gbgbjbes.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2nhntuxak.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2uhxujfmb.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ozyesdnc.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2rayevzmq.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2mbudmqmq.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2kginyalj.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2dxinzaig.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2nebbbhqg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2spicxnck.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2shzlwpqa.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2kflxgsfe.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2iixqkwex.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2pnjsecyy.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2ielutrym.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2gedycmxx.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2zojitmfm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qgessmch.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2lnupjtss.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ipodyemo.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2hussynfo.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2mezjdyvc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2rtmsgeqj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2oyfqltvg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2lkezhiry.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kipinjqk.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2gvnzfhnv.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2jgpgtafo.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lfrkptee.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qwrtvyyd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2nmepbdxh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2xkihdkbo.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2lzzxgovz.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2cpjgwevp.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2kjgwbrvj.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2bidyjmgb.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2jrpujfib.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2gpcclxaw.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2rxrgulnd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2llzvznoz.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2ajprhdly.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2rounwyhu.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2scycxlrd.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jznjfrml.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2mipvvxiy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2kpabipni.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qtkgdljw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2lcoqycii.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xkrqvvws.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2evrhlxbv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2knwbisrv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2yqqrrqch.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2hllpibde.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2lsgzhnef.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2gtsltojd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2gunapgrz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gfdgkykf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2usddaoez.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2gglxqemk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2esczsmpm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2izvemsyu.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2lvawflko.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2isrpffxs.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2crfdasmt.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2yaaclrco.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ixggqkvu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2fuzbubfa.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2ncvqohwj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vuqspaxo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2udizruiy.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2hpflbyhn.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2yqovfxjk.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2kuxnmjcj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2sodzbapt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2sgvutaok.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2gulpecpw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2trsojfcn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2dvnfhano.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2aqnkvtgq.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2nxgzpwui.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2eztvvhmb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fzljsnau.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ftpbqwpi.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uwfexoun.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rnlfnegg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2hqygqleb.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2bypppmgo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2zefooinp.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2eddhixle.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2qcacopth.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2oyqdpkhn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2zsmqjesq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2diblphah.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2kbjssewi.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2awdpocdj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ssrhtios.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2sgncmjos.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2zfqphxfd.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2vfuhvgbx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2hzbmcjxj.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ycwcqcvp.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2xngjzcax.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2kbvvlkud.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2mvztsgif.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2amtxfmnq.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2mmjfheoz.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2trgryetv.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2eosjeban.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2amcaokqi.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2kunquwba.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2gcwccbfi.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vkyiwqsn.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2qshyctny.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2jnqghjty.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2reikayqw.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2llikbwmc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2xlbadahq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wdsceuyk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2rafcgpme.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2eesnwggh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2cmuhxwsa.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2xfschuxo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2juebtcpb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lrsqodos.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2fpnulxpy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yfeprpgx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2edlfzkev.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2emnqccqm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2yphsolsr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2dzjyrgex.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2gusrjozo.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2cethxqmb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2yxsrztrn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ccifyerz.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2qtpifhnv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jokzuptj.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2bemyyhdo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2erpslzaw.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vvkghcez.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2lerrjewz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2imepeire.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qcsnoozt.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2cztzhbtu.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2apfxhuis.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ppkxrxiw.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2jikeemeq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2ypjjijsl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcdpmckw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2hsiypdyg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nnthpfwl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2kfetzdey.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2tkjmtrmc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2jqmoehpr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2xgblotda.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2odjitbqv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2wyvjaqcr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2jwyvywdh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2fhpczpde.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2xpdhhyiu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2tcuzykgd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2xejrnxjg.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2fqnjiciy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2cofastwq.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2jzdkkwrv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vggetxsk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2cgvpyoka.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hougnzbu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2hrrpcubi.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2azsjedqy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2zxslzymc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2dhbpbaam.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2rzfklvua.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2qtwbxkou.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2hxbzrjyv.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2njwvzorf.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ceorhrst.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2noxfydkx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fkjnbfsn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2guhynohw.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zywvayzr.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wymwsidm.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2jgzbloef.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mgjnhumm.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2htnvfmrd.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cyiqkzaf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kyxeohbk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2mxyhcejc.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mjjnvoty.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qpmxalgi.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2svtiwoyk.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2auumabda.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2eqfabfed.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2pufnjdxc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2kfrqhqhw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2lizsbphc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2bekfbnwg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2jmkniafi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2mxidwmbh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2tyyygrus.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2mqvftmcs.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2krcpvsim.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2sjtqmsxm.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2yknlgjid.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mcqmutxx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2elffvvwn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kijmapel.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2hmvtoyuf.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2yzwkvore.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2bkpjzmfd.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gqxzfqwf.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xxrxurqi.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ghhjwylu.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2jpktrovw.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ysbyuyng.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2hjhcekna.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2grcyrbnl.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2rnlhwlpm.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2vwzdgxgt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ltrgjpbo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ujagukgl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gkcdfjpj.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xcgpoowx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2szxloduw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2opplplih.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ljlnwkzp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tyessvpf.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2guvxowwn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rujigehh.html


<!-- 参考信息 -->