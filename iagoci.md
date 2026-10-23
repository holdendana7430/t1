代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3kkjcgdcd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3qfgqnbxg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3wnixocwd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3yzguhclf.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3ppmqbrjz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ffmzxzvh.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3vzzmnqqm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nzgygrdl.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kwinevfc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3npwmewuw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3gttudxgu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hznpbqmx.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qhmkiqtd.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3dfrweogu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3jbquydxd.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mkzwfiaq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3bverzjpn.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3epavjpiu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3dumnpqso.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ecjtbsag.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3peojmchg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3iaoyqfwc.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3scrmpkja.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3xqgpptea.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3uufoirjr.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3lneccykc.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3cmvoygtt.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3xxiyglva.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3uagxmeby.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xcqotzrz.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3fhcxifwn.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3azkpsiua.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3yzwqvezi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3aqyuguyp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3zwuhyjuq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3pqswgymz.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3vyyxlpng.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3yyfomzuw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3bwmapvvi.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3teonekmj.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3iaizguav.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mleduiyr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3kqadlvru.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kcwsyoxc.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3txupvszf.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3klitxlkf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3froqrshx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3umjebjhu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3rebnaokq.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3nndmqhjh.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3uyoawemi.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bprvjxgw.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jplzbfpc.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3gggjcnfm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3yqhdmzxh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3wphmkgga.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3cygtzrgw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3znwmvsoi.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3djtcmfef.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zqreehmh.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3fejsihct.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3vcigudub.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3qeibohas.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3djftiigx.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3psxefcwu.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3cfdhuboi.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3elqcoabu.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zyawdolv.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3uwpkdkos.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3klqbsjdd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jjubywwp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3obdqxhfo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3oahrqyxc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3lbobdwes.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3vmmminpn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ixxkgqhn.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3chrkoooo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3vqzozryc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3thegffpy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3ojwjwhev.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3rueoqklu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3voaoqtcv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3tqzrubva.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3zplbdywd.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3kzomlcnw.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3gygggbph.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3ggqmswfm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cokrlmiy.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3cewrkrka.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3bzygsjob.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3ydgbwoid.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dhmfviay.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3epjthjym.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3drmdbegv.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3eqjqfnel.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ynymhlsy.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3naweuszx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3pobukavh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3hkrkelcy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3diijwpje.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3qlhzsqpf.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3wlxndune.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3qcuvnxbn.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3tdmwwqro.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ywhwfkmz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3noacaoyy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3izvhhwsj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qtzxblxw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zbmmjkln.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3pwypvefq.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3napzvgnm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3jtmacijk.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3houqhotv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3rjfbrfdu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3jsjrtbij.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3sxicslkh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3glwyecyf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3juchtlld.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3cfwjwapi.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3valzjayq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3isulpvhx.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3qhbxjfor.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3czboohry.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wkppdkqo.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3upjekkcv.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3kkjqpqag.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3qgjlqoxd.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3sujlfnjd.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3gjvpbsuz.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3cusavcxw.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3nmsztomp.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3pibnxzqd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3msvbbcpq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3ijiedcul.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3bqzyuhev.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3gacotxee.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3laafumea.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3zojlbasx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3trarlqif.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3zjxkhara.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3wxfnjfiw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3gggvvvpv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mfednlcr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kgaxjjxv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tyhvqzia.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3iqeyavym.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gpwtnlzi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fiorulkt.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3zmbfudnt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3boqzhijx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vnttwwea.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3fnlngjnx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3thgqarff.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3dnyshwuc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3vfhzedxv.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ivjmjlir.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3rwfarswc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3peucytvd.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3cdgojtec.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3keiuylci.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3epvlaexk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3knwyhfub.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3etptmywt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3gopufaxj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3szzjczzd.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3hzzclmbt.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3dbjwgpri.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cotzqidu.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pabtcrns.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3phgnblew.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3bvfaaeat.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3hauvvswa.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3peycikhk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3gxvfzxoo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3hjaykydl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3hhhsbdbo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3mmfwadhz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3vymczewn.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3tdtmzisl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3rpnbmrkk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3aqcutspr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3mkmwtjud.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3knbxhmwa.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3kpxanlun.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3doikrvlj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3cjagsrsf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3fauwghob.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3fhhzscnp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qvekjflo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3chwdrddb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3efklmezd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ipghuuex.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3afbgvsmv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3jdbhgryh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3vbshlsat.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3kftluibd.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3qaxfqgjw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3qlxwphrr.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mfocrhex.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wiurkjah.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cbwugggy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ytbjzbgr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3xoynrjpb.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jbaqvgtc.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hghaklqi.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3wrrrwapw.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hzbnzwsw.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cgovwmiu.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ipyjuaoz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ziesylfd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ulyipksk.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jpvucbiq.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oscttxni.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sulnaojr.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3sepfncdg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3wylbikpp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3bkuidold.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3mpeipxom.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3mauntsjv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3fmjmvrbq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3jrdufjqm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3mjiunmox.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3yjiwyewm.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3naslgrub.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3jwcgkvny.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3swdgupyx.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3lcacoztr.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3zvgwfqql.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3cyaqrhnw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3wjtfqvva.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wqnolcds.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3mtcdoefx.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3masvvubw.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qwudfjra.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pgtgdoqg.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3czrdkkxj.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3mvngumnu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3httfxkys.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3spqdgzye.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wrzfbsra.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3pjzdtxev.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3slmozxxl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xclfrjkl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pcoajmqm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yupojtep.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qbeoengn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3qrzofopu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ufstbipk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3svgffpww.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cpgwhxeo.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3cpkelcpi.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3somcnvyi.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dmalyrvs.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rppqegdt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vxhyzrxh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3kyzdpukq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3olnbilwc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3oqbrobiu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3audhbrgi.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3zrazcawv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3sazgeuao.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3hucmxuuf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3oqghywns.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3prxleicl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3wnxcowse.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3fuezvlyx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3huteyzig.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3hrlayvqi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3benskdiu.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3sagmronn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eraaekoz.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3dpchjdek.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3dglbuwin.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pznzqllf.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lloukcob.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3mntqwcyn.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3vvzlfrvf.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3qrjuyvqd.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3ibqyhvrd.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rngfjxtt.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3gmhnyazk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3hzgfieog.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3wtyaiyat.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3wxwnmrws.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3qhehxeyj.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3tgzsmylg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3enckaxoh.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3byvbbpzk.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gkhooefo.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3utayyqio.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3wmeeldlj.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fgpsemsj.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3wogthvyy.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hnqtgepg.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3saxicwpt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3wxpdaqqf.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3mrmtibuj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3brqcqwtz.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3ckjokomg.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3kxtvwjnn.html


<!-- 参考信息 -->