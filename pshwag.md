代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3uutlqdpr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3lyjpoeds.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3zgjxpcle.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lubdinzl.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qvjrwoqu.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ryintwod.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3vfteuxxk.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3bkbvuxvw.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3fvnumwhc.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3qnsovfdk.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3hlqvykfh.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3qcxkxfec.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cnjqfmwg.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3jibxfdck.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oqrvybbd.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3uperrxgd.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3rwrohlbw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qprolvcf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3rqapzcfz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3zehyxrek.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3imbhycuv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3ewnadcim.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3lswsqdaj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3eztlejyu.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3ayblyxga.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3xjzyvkfo.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3sedffsnu.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bfpxntep.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3utthuwnc.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3jfpsmljs.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3svidmbkw.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3nhbkdetz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3swzezmia.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3cxspynxb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3rqcvybje.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3auxaykcw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3xknwcyfg.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ulwanfky.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3rfchnssa.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3eocgrqyt.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3udideeqw.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3swzgoart.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3eamdrudm.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3nbkkhluw.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3tsceprwo.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3otztyzmf.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3nrntkblj.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3lqdknisv.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3fmaqeinc.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3njynzyjn.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3dfrjsisr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3rkhhnjrt.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3lokpzuci.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3tjmzfuhw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3mbmwqhqm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3gwjegprn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3iycgzikc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3snszsuci.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tfnwymqn.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jgahhqfs.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3yyswtwjm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3adiadrah.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3nzqpzxmc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jghjdjon.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tfmraoqj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lmbyvfyn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zayhideg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yhgxifib.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3faoypuyq.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3umsigquy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3xcxtzulf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3aomxtgbx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3jtffesar.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xxqyexkt.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3leycyaua.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3gqhkfqth.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3xocbdhie.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3jytmhpoz.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3ggbqotfk.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3kaohduvd.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3hujussxd.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3obtxqqvo.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3omkimgny.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3reikugbu.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3wmlzsicr.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3mqjtchkg.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3owauhxwj.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3ovmfrmff.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3tlqepguh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xkqlyieq.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3cpscnaxz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3obqtxgio.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3vqklghwx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3penluikm.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3oubelbep.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3voleivrn.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3wxwlcxeu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3vnpgrssg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3nnvnryau.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3tsezovts.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3eqeuofhz.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3svnfwhmk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3rogzcaub.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3nqjwxpqh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3cuftzddo.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3yduauxka.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3grihxthd.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3jqmjoqma.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3nnfmsfye.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3fgwtpogt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vklkeibe.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3qecwmqnu.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3udbehsxj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3dwemgdil.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3hpsqhyku.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3prioqtbk.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3ddedjzdo.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3raurndmc.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3twprfyjo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3dkkddkqt.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3hxaxbxlf.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qpgafize.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3cebtlbxv.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3fwvenaxs.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3mzzchsxg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3sddviioe.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3nwuzcwal.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mfdxbolu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jqqkjptu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3idbkkjsi.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3wiaqubiy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3uilqbafm.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3mjrzhecc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3rntrhzwu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lzngxtjr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3nxctmcmh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xavumnww.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3utfkpcwc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3plbzuqsl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3bhgkxzfr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ecjmiybs.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3euzfoinc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3pzaimdqb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cctozssq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kbosistk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pmfuujni.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3axscuixg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3oosqlers.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kknzpqpp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ydirhxzm.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3xgtlmcre.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3ctsjyyct.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3iituvjuv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3onbmzmcl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3lslujhjf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3aquanxfx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3xavdyksq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ueayjasb.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3xenznwyd.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3xbvwxhke.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3gyswgxpn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ziysujbk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3eemrcccv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ubkyyoma.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3lypdjkyp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3dvhwjrzy.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3mrdhpiba.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3nmjvgslc.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3xrrrarjg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3qztbxykz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3pcafsiqt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3hlswfldp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3nicbndmu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3fsdtaknh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3igngenbg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3qvlsiais.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3tbszasrv.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3vvjknpqx.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3yqkvanht.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3fkkbpjpy.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3hvkmhxeb.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3puzovgzv.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bzdihqqb.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mhjkpdlc.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3mingntll.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3vbjrxgxi.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3qivapslw.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3znvlcqnv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3huvptwzy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3imljyapn.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3rkxhhugx.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3houmsytx.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3dehgpjdd.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3stuclurk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3skqmzydc.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3ofqzqrxl.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3ynmmawkp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3tdzfrmmg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cvvtnxkw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ijguedwn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ihytsvxm.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3fzeizfcg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3uadwslwi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nmdnbspe.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3lifkkgao.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3pocgxriv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3neucrtnm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3mheyctsp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3cowhqqcu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3rknpgfha.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3twajazqo.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3hwhhldcn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3zlokwdrw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3engquepw.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3mabbawax.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mfmmkztd.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3cfiqdetu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3pjrizaya.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dymdjhnk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3dswewjpz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3aabtbotd.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3pqfjfgpq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3walbfjyp.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dlknjjlk.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kygewmhj.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3dklfufdk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3ibyeantj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3laxpmnkz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3kxmlhqej.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3zsivsjty.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ixnnkbik.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3gmpynwko.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3ovznfyrn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3czwowwpp.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3ohdvtrzi.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3zmdkbhzk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3qdorvuey.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3wddfaumk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3dkjgqegl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3brruwhxa.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3xqnviekh.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3xqszmhfo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3jddzulzo.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3myglvisv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3jrmzavob.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3zfgbymyr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3lxwhfchr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xrbpxltj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3xkzsming.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mjtdgeti.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3ghfsljgj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3rejmkyga.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3xdddpmym.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3mizgemco.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3buleijhl.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tinysuia.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qpnxhcnk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3njwfcssy.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3uplumuwt.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xgecrzro.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3reelomry.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3pdvbcczw.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3akktynqc.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3notfwqsy.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3itqmqzim.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3teznqmpf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3bnocjnnh.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3djfcqbyj.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ujjusxny.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hwgfruth.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3swrcqjte.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3kswlgmzw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3abtundoe.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3qokjwgox.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3mvxufwpn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3gprhwrkg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3fcbazbph.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3iisqhfpt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3auluwkzt.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3bpcsbusc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3zcdiqgle.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3spsxzmpr.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3clfiyzlg.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nbcszooh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3tsakxbpz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3nkersmfl.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3jtsqnnxn.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3owowptcf.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3rflqdrih.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gmvzipvi.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kntdsnro.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3kobezjnh.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3mcxrcwex.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jgjrvbnb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3rokferml.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iapglmrc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3aintfrkc.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3kjeqyxxq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lpdlwafd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3riqwwrak.html


<!-- 参考信息 -->