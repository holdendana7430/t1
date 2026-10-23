代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3evbkqcea.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3wfvbqqgn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3mzonnhib.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3btrjdtdv.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3zgyqhjyj.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3kvnlizcl.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3heqinycy.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3hhrcesrn.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3yinqlyhx.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ropxpwut.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3zbgyzmyu.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3watfjubx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3wwzsqpoy.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3xlqiuism.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3roqaxjgz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3dciicejl.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dyhryghj.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3vimrghko.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3smthgxxa.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3kyijgzyn.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3mxlkanmk.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qbislcpf.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3tghlecav.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vtzifxwl.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3wpqfgcai.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3jcfqtkoj.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ilxdkzjr.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3miajietn.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3njvxdhos.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3akwyitoh.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3knrcrdwl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3zedpyzig.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3nzzcwaro.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3pjazfrcq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3cjxigygw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3jjiwlwoe.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3tyhgryqf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3sgpsddvw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3sbxzovwx.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3pcftfjic.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3hmjtbkrg.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pnphhfkd.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3xutbqaok.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wplmcwxf.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rodgwkdl.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3skdhwqps.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rmxinpgu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3htsjhsok.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rdepgpns.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3ixtkjtmm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3chtelhse.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3imkakexx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3pnkxiadp.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ndzmujyg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3vkhaplda.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3woudbawo.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3vsyystji.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3dyqoawvj.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3sytwqhqp.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3omnrvcqy.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3bpbxfraq.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3pxmthmcx.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3totrucvy.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3whcxosmg.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3pdjvffib.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3dvkkquub.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3vkktmomc.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3jxrfrbus.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3uegzztsa.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3zulxqupx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3tdmvfrlp.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3fnuwzswa.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3lkprtccd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3lzxhnhej.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3dbilsdgq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3xmnolpzh.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3yumgmvme.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3amtmhavw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3hdvivnjc.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xozkmgdg.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ffnubvqg.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3dtexvxpk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3exiiolze.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3lyhahapz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3twbwrhhj.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3ofwatxxj.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3dkybjbib.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ulwamcto.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kvzqsypb.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nxffieaz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hynngbua.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3qbhsnfzw.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ssqtavky.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ekngqkjt.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3xjozqqvw.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3egzpnjtc.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3vwvghguk.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3lujynujq.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3elyycrpa.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3rtegmqhi.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3wcqxijql.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3knejjwqv.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3cneqbucx.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3thfgcnbc.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3ajigxwvt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3oyrtclqd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3gyorkdvf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3wyajetni.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3bpugxqvs.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ovgjfopi.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3hsxtkzmj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3npeddgwm.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3ntygvdic.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3farimksv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3gpruignm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3cjbrrenf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tzdtceif.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xzstfzdv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3zpxaqmlw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3vhmagtug.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3cvfaiakx.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3bznjgydd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3ibevmpie.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3nmhrdopy.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xcbtobpv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3wuzoegta.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3sszjqhkw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3mvjqryut.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3hybzewef.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nastiqzf.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3qlulvgzh.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3rlgtmeqp.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3avknijsw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ijseiktm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3aqiwkeqc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3qwjnocjc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3lvshewqr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3htsbozue.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3rlvyskqd.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3buvwanpx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3kgvlmvvb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kjmtvzcf.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pxsppzng.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3toapwgiq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hzwsrywf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3yqvsxkey.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3pimswiel.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3hqykdmna.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3ojppzoyi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3npcjeevj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3fmtriqso.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3xhbvmdmh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3iszjxdqh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3envnswze.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3baxkoimi.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3gcicjoys.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3tdtlhilq.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3tduinyij.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3dahqdemh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nyiovghs.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3lclgfzad.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3sdmpmnbo.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3duezeevs.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mlvsooyv.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3zmfbdgpl.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3lhxrxurl.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3torqfjbp.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3oqymmnzx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3uzjshxmc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3laxpzeog.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3thltnunl.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wqukqbmn.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3xucbwapn.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3bglzcbyp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3befmiloe.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3foxudeja.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3tagmhtpv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ramjgrmu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3voplhltw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3bnmvorbt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fslojtem.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3fmhqlilq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3tmrqykas.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dgjfcnmd.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3agevdgeo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3kujwrxrd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jcsogfdo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3tycmsozx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pfwgsjdy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3gvwffbzj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3pvhnanxf.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3tpnzthhh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3bhothtfp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qmrwonqu.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3tqhdfxxm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bibziarr.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3owqwgonx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3qhntiuhm.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vglcwckl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3udyggvid.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3bdgxashz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bccphqir.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3ogicfqvy.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fkeyvqyj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pxxhedce.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3djojjxyw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3qoopsclb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ufsqsgvj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3twnikzfz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rokitqah.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3hfesdnaq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3gjnvnaio.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3kmcharqt.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3esialzhi.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3nhxbbbzl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3zkaiohzs.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3iebcafpe.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3torictwv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3iwpsuhrd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3jdiarzaj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3rtnbtwul.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3zcmqhrwd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3nmqpurol.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3zefpjwah.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lvdaargj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3zbagarxg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3dawytrxy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hjlzqcyz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3chvpxvmm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wzvgynpy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3azpanlcs.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3virhinpv.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3utdmqtor.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3vxwsfxpc.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hphumbzo.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zglbupxo.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pwwlxwwa.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3sgckruby.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3uovjbchw.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3elegmwip.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hzzfnrzd.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3hkvgprfc.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ziuxswxh.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hsmvzscs.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ftrtminl.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zmldpkup.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ftzwhbiz.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xwocwecw.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yzoddrrw.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dpgqrjeb.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3nzppyqol.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3jlxcljrq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3hcqhrfwh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3flnijjzj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3vkxuflxh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3tfdjuebe.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3onptrmot.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3hfpdunmm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3bquequos.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3ndhfdaul.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3gqeincoa.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3hzggfmux.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3aqgodiyx.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3wtgmsuta.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3kafezhcc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3gjqbljuj.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3ajrbpbix.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zkbtmxsq.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3ofbejdvn.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rmdzlssy.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xtgxzukf.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3lluownef.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3meqdspeh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3bnygxxca.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3ksdtamjz.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tadcrmch.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3akojqfcd.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3yosrjgjw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pypvdqdw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uandnthm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gklokogc.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rtszqzek.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3rzdzetre.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ruwnyczj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ggmhmqmw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xyfafsrg.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3jijabeed.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kgehilxr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3yvsaranp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uelcviuh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ghajbbkr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3npnkmqmk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3fvzvvcjm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wxhhbicz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3nuqbdjmk.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3vcckepds.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3smfvemty.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3rffypgmk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3rxisbufb.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3hrkunllf.html


<!-- 参考信息 -->