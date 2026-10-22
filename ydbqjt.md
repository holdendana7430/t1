代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2hcgybfoh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2uukorzsc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2hipyauqq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2kfjeiwog.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2fegazlyp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2syzoumpo.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vwebkjmj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lkouxfij.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gzpsjqoa.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2czcaeivx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2jkvolmkk.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zkfljgaw.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gtxxnrpy.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2vjruevtl.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2zgzpytot.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2kuqciznl.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ayqxbogz.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2dymjesak.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2xaabxhml.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2gwddntzp.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2ssddkggv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2kpfoupxl.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2qbhaicvb.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2sfwlytbg.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2qfsuutah.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2owigrequ.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2bfovhsnd.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2pajszeaa.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2gxmqqroj.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2kfmdookt.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2bpknuuyg.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2vizcotoj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2tgfqpgfy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vfrchiza.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2jqqruzxu.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2opufwhir.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2gmbacrqa.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2ouaullcf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2geqxhhsm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2jdrwtdtf.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2mpwprsle.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2qjhequqy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2zkjligot.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ewhiusdz.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ajlzhhnf.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2izwlurxf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2sgceqpmm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2lrhfprqu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2fkhhycys.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nwqegfhf.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2xbjdweof.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ixxvaqsj.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2aueuzbuq.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2squuuqmh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2osucvsul.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2uohnzuyc.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zharbehf.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2pcpmzplx.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2mdphladi.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2fihlotsl.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2rcfaesfy.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2nxwmjvnk.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2rsjrgwsi.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2qmbssijn.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2wddzlpqk.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2qnzfauqa.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2gcksnrem.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2iifzwfwa.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2wtfhwkbj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2tqysojgi.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ijnktimg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ivitvuaf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2cxchipwa.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2pgcmvzkl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2gfuamezj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2dyfqcovf.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2sidjsdnr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2tyjanzaf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lrgdtjad.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2niayfszv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2faapyemj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2jushthif.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2vukmnfhp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2rhqwykmj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2lshmnxru.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2ddmymfzn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2pjzfgwlu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2uudgrzlx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bpwcpnsl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2rkokfqfl.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2pgmeakmn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2xlbnolrp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hoimntzd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iynlmnch.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2qjqooixe.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ggrkahas.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2ihuowqzj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2fkatvspg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2mrlwiqvx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ocbnyliy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2nhgdosgm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2hpafeshb.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2grxkwlls.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2pkfbhuib.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2rnobhinp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gbtmscsx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2uydyagqr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2tqakbkfa.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2lrgmildu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2gtohqzcd.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2pacwhqup.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2tzdcuknp.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2cxwbcwla.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2ixmrehny.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2cqbthsqi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dhiicqsd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2laapkjdc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2blouudsx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vniuzimk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ocngwotv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2obtjkrui.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2joucvqvy.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2iilwqnyd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2lxwxbwnx.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2lfjjvotu.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2qfwxdpjr.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xyouqhje.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2menonhxp.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2pgrlcjwq.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2lqsnomso.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2jmuezuue.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2kggtciwu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2xxrjhrpu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2toznmnnp.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2xtemuatw.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wdtpmepd.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2ohqudjio.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2ytxwdtxf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2nyxniszs.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2spcuaxaj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2lbupmeql.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ozqpofim.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2sbsarcnq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pmwpyshk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qvtiuozh.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2fnqpuaox.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wsklxfgc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ryqcakot.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2wgocwqkr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2unfazdqt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2gkgrospg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2tjxwgptg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2azqzuuac.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2jaiiebxo.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2snhnvseu.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2udbksehe.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2jhbekmsj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ujrnidem.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2mscfwcwg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dnemdxij.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2kgbguije.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2wsytyrsy.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gpbhzlob.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2rbxijdtv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2gznphkvh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qfmvfjzt.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2auupewbd.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lbuuzywf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2isfxdjdu.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2xdgklrwd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2ehmyxbfd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2orszwyqs.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2rvconwzw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2nqtmvuoj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2jmumisbw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2hedrckbm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2noptnfge.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2eguzktba.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2dgvlxztr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2jzjiksxz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2eexgwlke.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2utpbzvjp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xhzqhdmd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2brhdrnnu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2uykarrfk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2kmuvyjih.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2wlpdtray.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2aaajuqri.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nfymazvv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2sdahthej.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wuofttbk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jyacplcu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2jmfyifse.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2bkproykz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2hptaneyo.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2mnfwkyeq.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2wmjtcdsa.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2rffcfjdo.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2csxszwga.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2annskgrw.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xvsrzehl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2nllwravq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2xzgoebtt.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tfofzlbd.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xdsmhtrw.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2tmbyyhtf.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2czyecpef.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ytycjylu.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sbldvrkh.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wcihpnsc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wxegjvsa.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lskcydyi.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tlhjcxom.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tsruanre.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2ugilggdb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ddgegyjf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hjaixeii.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2aaltqvay.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2uubwbuhe.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2wtukvqcn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2gvfrrynp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2kitdukpf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2zsjdgbfi.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2ctvagxif.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2qqeafwrv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2ziouuvvt.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2syrdxlkh.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2wyqsulpt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2tjbeewwh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2itjhnkew.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2oxxyhoik.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2cgwsjvxy.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2fjqhrzgp.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2okyydmpq.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2aoingoah.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2zpwkqzlj.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2hsjvitdo.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2eexzglgi.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2ptbxjlgf.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zcnxbmlm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2rudhhbob.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2oujvwzey.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hfolbeja.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qovbbkol.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yesdlclg.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mlyeitto.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2ryajxhrb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vrceydoo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cbnecwer.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kyqnwneh.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2wicbzwlp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dkcxhuzz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2srmdqaiz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ckmxybas.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xwhapnki.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2bddtdvhz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2qbsgjqri.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xoqmyktk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2maicakwi.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2armopadj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2pdorsbsw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2rzggoewr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2cafzqxap.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2nkmczqks.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2wfnmubxn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2vbftlrhr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2ukvuxwcf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2oejpwaze.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ackpfolh.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2afusjkli.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jfvaefws.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2tzuslxvf.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2cbvnipmv.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2wqypsowj.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ucnpplqp.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzxbkeye.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2accofdfh.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2maknfigl.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2htoxbfve.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ypyayfdm.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2yrkgqims.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2tyjxcgzm.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2apehsuqe.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2rfqogrfn.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xznpicwm.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fbfsstdu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2cqloezha.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2hgamomkl.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2dtfjphnd.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2kwskwdgm.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2kmnczlzb.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2envmocsj.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ejrsuejr.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2bkperqou.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2wnejwohq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2glktdlxl.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2brokdxef.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2zhwvwzim.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2wfbcittd.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2lnitksbf.html


<!-- 参考信息 -->