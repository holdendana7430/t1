代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2noiihbgm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2miwbwmfr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2onothiwi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ugiaabws.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hgnndtzr.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2teurgxfq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2uycwjxya.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2boosrtyf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2ahyzaple.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ajpciqir.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2bozpmwgz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2dchqjdkt.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2bjmptiex.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2hlnjxxed.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2lkeedzuk.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2dqljbbtj.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2pykdoyug.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2vfrsnahb.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2xcyyevgn.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2donebdvt.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2goembwxf.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2pstuwwxh.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ewxyvszv.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2afhnyikv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2fuifevnt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2laoeqouf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2soiikecj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2phaoafqu.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2akcyfhxy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2xmiuwjad.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2uqtdugsx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2xowvvvkj.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2vfcrsnlm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2yrvhrsts.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2fzlhmdmr.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ilxcuxkz.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qoqqikhq.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2cwufjbcs.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2henljwup.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2igufskgf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2tgdkvanx.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rvtfrfax.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2irmzxiun.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2muozjcsa.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mnvjgulz.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2rbdisjdj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hqdlziyb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ferftrdn.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ekefmzbz.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2hyevkbcc.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2gshpfocr.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ueydspfx.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2dgofcgsl.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2tcajarmt.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ynwrqzoc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2tucuoldy.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2qepyzzpp.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2zpcbibav.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2oojwsjtz.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kxwvfhkt.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2qzyutiuh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2mdfjhhdp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fcnplvfr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2yltdjjbp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ebpjudot.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2cmriknhj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2nxzcwyxl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qltygwyl.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2xtsyoaxf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2yrypvfwg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2afsafigq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2htwgvtxg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2crhjqcdv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2okoyhyvc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2phdpqggb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2wzufwwjp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xshgdwai.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2xzejrmue.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2kzvlahpt.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2quhatvic.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gffmybzh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dnldoppf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2rmsfjbaa.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xmscidzl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2oecnlcal.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2szfkvdxi.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2mqhnnllr.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2zecftzmy.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2tatorzqv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2zdjyzgih.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2cdthrrdp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2dcqzrkys.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2gmztkhya.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2ctpjvesc.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2fzmbpunr.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2hnpuuwqn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2qimhovgx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xsmgkkje.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ixhfmezv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2nuiexxri.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2nujedloj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2tvhsfnuy.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2dsiqxnxq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2cnfmbdgh.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2dngqeaix.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2cqoegftu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2jnhuqksp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zxkdnlyn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2nxwmcqnj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2fyibvqam.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xsaebxhq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2gbiozsiv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2irvmxgnn.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2zsablsbu.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2glbudgbs.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2icpoakot.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2hulmdjbp.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2dirdkjgx.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2naxxmyue.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tquynsbq.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2xjdxygjb.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2qqtoqlxl.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2xyxlqrrz.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2elnfsiyi.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2vewxftme.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cspvydcz.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2eaweqhnr.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cypeagfq.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2igrddyao.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2xdjttplk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2ekleawnc.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2noevwble.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2gyrumfev.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2gycoyodw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2agkgfufu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qglljmpn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2izglyrdu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2jnmkzjat.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2cwhqbbtj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2uwbetqqj.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2mztrlryh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2vqrqrbwk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2twhvtqyh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2fukvhgxg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lsmgmxmu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2wwtcfero.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2hosrrrkk.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2bnjrgxgt.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2dapeuliq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kkqcmgcj.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2idynvbdv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kgmhqyet.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2dhcozvtz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2reevwoft.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tumhrnev.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2xslmjrei.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2drloladr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jfkzcbqh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2ydyyowjk.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fpkbvtxq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ulfjvpxs.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2ylekaarj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2rtxjiupp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2rqfbgtjw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2psdcaouj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2qqstusxg.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2jkgkerje.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2nlzmdvbp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2elptdwqt.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2wfswemuu.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2ggvjnnen.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2kcvpxovn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2gjoggxrb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2fuisqbhw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2fbjryyyr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2qkbytlaf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2pkjwbzmr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2lcoxgsvd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2aiqjmprt.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2hphywjsp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2igmeqxxm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2obkfeoka.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2squncysg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2aabbzsys.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2wslfqspv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qaauioqe.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2tyjkhpvm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2siqanxck.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2irnryvwi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2rsgpysjn.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ckkxupso.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2opzhgsss.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ebdtdvyc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hmflddxi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2iiuijpzm.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wrtbsjdz.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bfkfzjoc.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2cjhakwcl.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nrvqqetn.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2iejtisco.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wmhdkqpf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xmvtfrxf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ptrszgzy.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vodbxylp.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tatqpbbn.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rhmaggyz.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2mzcqyphp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ttosyqbo.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2spnktmoz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ieaovwyd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2nrwzdztr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2spatohgd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2hfnwqknv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2iybuvqxe.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2vfocezzb.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2kixlkefy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2alcuudfo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2cqcblgso.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2lektrwbh.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2thgdbwvk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2dhyjionu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ejnynqbj.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zzrzocsy.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vqkqiugn.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2ongyvcxa.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2makhjfcu.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ebyhgkjo.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2fcptdjnz.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2fmpdbahc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2fmymrtge.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2fjzfsixl.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cfcpyvzr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2ruldeygh.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2oisgqyog.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rdfafmww.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zaxwnubh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lmruaezv.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kjxdbntn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2gaxinieg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2flbdxwpl.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vncjsoyk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tncaxaxu.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2hxcofcoe.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2llqhipni.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2tulcpevs.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rcazzlom.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zswjncua.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2byfnavuv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2txeejfkz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gwtzcdqy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2ouqmkcuv.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2kahpouyr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2fwxlpyuo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2uajfykex.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2nfkfcqmm.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2rycwkwyp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2ndairahm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2volvhync.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2dasonzhc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2zatxzgdh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ucegfana.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2dgsajily.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cgoycwpu.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2kdecfvfj.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2btyowlpe.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2uvosgedy.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2qotzusxl.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2yrjtwojv.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vhoowpht.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2kjowyyxm.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2cehgghof.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2wpppnthe.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2dntpcrkt.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2bauiazfe.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2brmyklti.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvgapvuh.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2waddcgcf.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvoxsjfy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2pqsawsei.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2dyqeechm.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2wgnzlmia.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2caspucxr.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2deaeujtn.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2tlqxekup.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2meizrwlz.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2byflfowk.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2swhjsknt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2vipiqohu.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2zfxsolws.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2nsdizyfn.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2dpczsisp.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2zballzcj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ofxoytrx.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lvrapckb.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qirbvged.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvysujuf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2rtzpcruy.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2yzypthpl.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2hkjzibuy.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2wyfygdys.html


<!-- 参考信息 -->