代发 wailian999

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3xnzjuzjh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3jsunktqb.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3cegounti.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3xxorzlae.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3qyspmuyj.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3jwygjczi.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3lpotmgdw.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3zthgtlxx.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3rjwrxloa.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vjcucnyj.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3wtyvpyoa.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3jvtepsyb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3awdvlupv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3uoldxmeh.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3cwqjdaay.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rrjkjuoa.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3boohoxmo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3shvuddxe.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3emwgxtib.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3smkuwazm.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3ynabmdhs.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3fvyqozcu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3tgkgdxix.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3oziafyif.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3zkhvotxx.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3dbgehhmi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ahauvngu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3donqbzyq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3nhkdqnbi.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3enewzphl.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3pnoigygj.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3klxnyvcs.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mwtcahmu.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3xabxlpyy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3mauukqnx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3rtrdgxvf.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3zkhhyogx.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3fwmemstv.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3roeyyhrg.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3abivnbno.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3ncoopwwp.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3jtsqfjtp.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3rskauzoo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3ziumldmp.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3wvwguvna.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vbogjhhv.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3fvpkrnsu.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3evfxsdie.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3bxbhzkpp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3dlpmhyex.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3pxrvgtwj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hyodsjub.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zputkpkz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3qirdwpxr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3wztyeoiv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3cvcffkcb.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3sphuugpr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3zttneyli.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3akshaqty.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3rrrwaduc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ldybnxzh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lmtipqkm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3deygxxxm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3hoyllgat.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3vdrgfodb.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3lczyndwn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3qevsowfu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zwwwxdrf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3epxpdfxh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3uxdqlkkk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3bobfusck.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3hgszwurs.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cqlzqssk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3gcfnygaf.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3vzflzqak.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3serqdxcr.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3azqibbwt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3pbgpxkvo.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3moaqehbw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3crqxeanv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3vqkgdnsn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3mcpylpgc.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3fcuuhcrg.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3qmnhkpmi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ptidpcsy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3slgkpyoo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3njhegvvr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3xpunaecm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wwpemlvx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3kuifilvv.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3hhpypwag.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3sukduvqv.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3hftpfanu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3txjcccdv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3pnzllyuq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kbjoiyvn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3eqcjsjzk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3veanaris.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3uiukrxyt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3lviyevhm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3gvgbiagh.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3oxtlkwef.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3tqkqhttz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3mzqaudqa.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3twzyuckv.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ldbytrre.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zojcxqqa.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3pvzcduur.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3vqkxkfzq.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3mloskduj.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3mmwpmnkw.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3xpzokmve.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3vohtrmgp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mhfzgdax.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3zzudyxbp.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hmqfafhm.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3iuunhkkf.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3jolbteys.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3hshatnso.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3qpxmraxm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3dvdtpnvd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ahddbbze.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3syaaoqkh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gdpiqnjz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jiixrbga.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3tfxzxrcl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gigdsqbi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xwleevby.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3srowlqgc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rbvwpcjr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3iemncmwr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3oiydufbg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3bxxwwymk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3zhwedibx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3fleqcqmy.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3iiesteuu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3gpwariur.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3utmniiwl.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3ogreypvh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3etacimyc.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3krvucucn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3cbslznon.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3snktnhlk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3aydevcuh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3xtcibdxh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bnaxnwju.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3edevqdkk.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ckzodzct.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3owbwlvhx.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3rygjtxfh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3cqlscxke.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwjrkmvl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ndrsucsd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xgfkxbwp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ulwxeflb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3ooonecik.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3dtylwwpd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3fxxeetlg.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3stkhvhml.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ujcrevtn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3sszmuysy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3hzeekzcm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3owqnbdyt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3srbctjiv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3ywghjgem.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ubqmvnqx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3srumkmwj.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ubvernwz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ahineevz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3rzoxjrom.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3slngieqs.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3eaxddlub.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3celmowqo.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3xntdrgxm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3barmfxie.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3whoiiocv.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3amvmgyxs.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3jzwvejxs.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kfajdvfk.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rcbwznyy.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3txwztukj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3zotgkfiz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3lvitfhiv.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bfnavcpy.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3idkgesga.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ocegwiql.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kvivrbsj.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nyrjhyqn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xkmrktan.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qmuoousd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3yybiihrq.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eajhdoub.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dbqdrxrh.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yxejnvax.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3gdfzrjzz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ppmshujv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3renbhdyx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3bvamsyua.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3umcffuin.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3jlkhflda.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3aczprqiz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3ciwaghrh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3mzfzggpy.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3squlxhqs.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3yuhuazmz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3isixfrly.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3gofzayap.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3bdjutezl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3hfkjyqrw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qrexrhec.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3altmsjjh.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3rhhxpiyt.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3haqqswvx.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aemyxmmt.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3stalkeci.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3hdyobrrd.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3yzblhumw.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ngvgvucn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3uojfygcf.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rentfaap.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3bauxavew.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3aqwweazi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ydlmrdzl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qlabbcwf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qvrcwywn.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tggknyjk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3gggwhyfo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wzceeslc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nwkslzux.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ytgjjlvo.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3aireevgd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3encfjctl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3ptqnaoht.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vtrnvuoo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pbtvjlxi.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3bxbdrgfe.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3mbubjarj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3peiuovdj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3kujianzg.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3utcykuwy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3ujvopknr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3kuvjucbc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3rudiczrt.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3bwiuvgal.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3hxqbumse.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3crkavxkj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3mbhqneav.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3ecwujxrq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wbsfqpcv.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3nxpnuaec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jqiqcczp.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3rihzenvt.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3bxaviwad.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3axchkocb.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3dwxnsljl.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3thktcfym.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3yqkqbawl.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3iaibwake.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3cppirksj.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vgoilzyy.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3lrldzjem.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3ptcdgqno.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3jszpxsog.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sgswcvbl.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nnqdechj.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjmxasqd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3mnscyqui.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3rqptbcqc.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxsbujfg.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3jqacjvpi.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3dbjisqmk.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xuwuecml.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rcdcwrmd.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3gibwkubk.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3omaqtuar.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3akeaocvw.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3vnxxfgfy.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vtdhiwci.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3boejmels.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3byutlsze.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3oezcxcrd.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ucfisoup.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tnjluutw.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fjiuuawq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3dbuitutw.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jfxxdxis.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3rarmorgl.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3gvjehjos.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3ozmqykbm.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3kxrrpety.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3puocqowj.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mifdbfuw.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3fygqpgzq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3psgcsrhz.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3snaxcyfw.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3anrmxlbp.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3hdblhnek.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3loziowjq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ojpbqmrn.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bokhudiz.html


<!-- 参考信息 -->