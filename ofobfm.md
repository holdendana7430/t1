代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3iaitntrr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3wwozivio.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ihqzquwh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rtbwnmoj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3etzwuqou.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3fabjpzfq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3dknowtfh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kotmanmj.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rdilndke.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3egrranba.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3lcctsenq.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3nkypxikl.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3oabtluek.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3crflqxzi.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cfrfalfq.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3njilircf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3vfrojwvj.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3jhaplpit.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3vireflwf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3pmvdwxvb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3rzuooibv.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3zkebabav.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3gdlfvwcu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3lbijhgad.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3cvqpuwlr.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3spkzdewk.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3jnlbvpvl.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3zdgzizun.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3fpwiluuf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3ialgaerc.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ajtgcmyg.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3lqvgigyj.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3nmhodmwq.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3jqtpshqa.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3frwglprp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3rjbecnfs.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wnnxiooc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3bdkhzbjs.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gsrxpkix.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xrofbylc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3qhclgnni.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3voxoaown.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3iquyyfxv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3gtosswtt.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3rrurnyno.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3hymfktie.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uqanqmpr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nxbpnjjj.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rznlsthd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3roccqbgm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3imrvfddn.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3midpfjzu.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mbwsfmfw.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3myrofiio.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3lceacahe.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zaawxofb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3qrkvqwoe.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3bcxmueoh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3khmjiinz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wlxjrkuj.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3btikwrul.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3mioemmmf.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3mielqaci.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3yeucznfe.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3qufqoyrd.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wkwuxdis.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kayczvmd.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3dtbkehvm.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3zidvbehj.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3bofknsse.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3wffdvwey.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3mwgsahab.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3tdnmnfxf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lgyuccfw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3oitnlszh.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3jmniiqtg.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3udbcmykb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3hkkgbabr.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3yxygoxnu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3vgdcmhzj.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3ciraohdb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qkrmacsn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3txbntwmq.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3xocaipdq.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3rcwspgwr.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3attxhlua.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3sbmobntv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3huodzyxu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3hrjwowpl.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3djukqydp.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3jwezusbs.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3csxcoond.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hbsfsjpn.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3sgeqozyh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3sgpcubno.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3rksvbfot.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ifedzvlv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3vmjvzggt.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ofdmckdn.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3raktzlzk.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3klpgozxg.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3qpqdhhcd.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3pjcvqpwp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3nsjvjzej.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3nlybwuym.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3qrkjqsaq.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3shtbpbbc.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pikziavz.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3dgxuerxa.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3ddbzqomd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3dpdmvntj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3wpycqfuy.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3moroulcl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gnootffn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3xsaynvlt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ypqjckme.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3lumpliyq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3cissytih.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3suaizzwu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3ppqcqyxu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3igrrxvzr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lgqyqrpv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3adpiemdw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3ujpumred.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3rwxrrgtw.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3ajcqhhlj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kzlncbha.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ehnmxqhi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hwjbpqcl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3oioolhta.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3rqsgsoxc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3vwifvepr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mbltoewm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3kkkaoinu.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ovdxszxf.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3latqrgmt.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3fzrunakg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3xnwhixpf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3pwrmynbs.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3mmvzrmet.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3zpbnxhyu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3zbkeypcg.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3euxdlwdf.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3hzempecf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3akhkxbpn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bywijbmv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3cvcfuslt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3kyqlwvyp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3nuxglcmw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3talcwain.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3qgmtsont.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3pcxnylpk.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3zlukpgbc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3ppgxilvj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3izdndezi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3hbazxlih.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hddvorlg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3mcnarzob.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3rppvkuvc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3xqiselxx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ledixxbt.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3hznzxsvp.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3ignmivgl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3vrniepvq.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3bguhaidm.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3tljsmizz.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3msogtddn.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3nenbrucz.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3fpwmifat.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3zijawbqp.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3cqoxozig.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3yzbhsrzy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3dxudlilp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bffvjrpt.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3zxkkzewd.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ivocyhgr.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3leroziyv.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3qyzydaul.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3kvljiqqn.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3ifqzyhzs.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3xupxyczv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3eqkvwwlh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nezrgdrl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ydlbizob.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nuycwkog.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3iccajqcp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rtuoqcsc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zqjviucd.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3cwwpasxb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mtstmbst.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3tczwpfrw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3joiltqjo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ozcqbcuq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3phfukkpd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3mehvdyho.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3kaijqplx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3eqrefvfa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hdfpilmx.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3acfndhno.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3loymglsg.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3aybmlpte.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3umpxucex.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yqucndgn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3dsoqztyb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3mnvzwdyr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qrsfhnex.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3kmpqqcpa.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vupfdosk.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fanluhtw.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3aqcarfsi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3prtzlunu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3wneqbvqa.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hsxtwpbo.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hwgaqcio.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3nzlslyho.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3kblgyukb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3nquhlyap.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3ptynsmue.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3zwapecun.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ctvzdjlf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3izypxfkt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3gpuwhooj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3fxsxemra.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3grxbvuqw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3izqfrcru.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3sxspfsms.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3pfmffsvh.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3ffclznjx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tcmesmzu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3anzkbqja.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3potewtjs.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3eaxajqcv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3pqqxullc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3wswidzno.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3uapqdvym.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3kcdspqwr.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3wdysegtj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3lmmbahrq.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dhmnipmb.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qtarnjyk.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ddunmtxe.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3prnutrbh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3mddqzvky.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xbiclxnk.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kuqaehqv.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3kgbilcft.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gbywkjye.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jwrdwkso.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hwortnnb.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lmdbspkf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vrkvkigr.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dtnwshoi.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xgirklte.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gmplacsv.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3bjfsfoij.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3cqnefzbt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3dutyslht.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3llbejktd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3qvzcwqwl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3mdhyfxed.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3woacthge.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3qptpnpyv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3cfrfowws.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3qtmtppre.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3ykibxpdn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3ntfofdnq.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3wqurqdta.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3klcdoqrq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3pvregsjp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3efxynjya.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3inkvnwpu.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3glverdad.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3dnfyvkvw.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3houawfns.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3sipyxoxd.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3cvpztkpl.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3eupljprk.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zlkhkemq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3aatkxyus.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rcdpbpvb.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3zacrwwcq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3iaaovxjk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lxbsrawx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tldpnpca.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mzidowop.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jccbqasq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3bhvpaqbn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wwdxbyja.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kuyfviyg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ckfqurby.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3bfqikljl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mcfeyqft.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nfosbwct.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3bmklbxuq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eaiuirsp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xtubmvkw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3peppsasj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cmnmhrjw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3hujwtqhl.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3zkqrzecx.html


<!-- 参考信息 -->