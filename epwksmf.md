代发 wailian999

PHP:  substr_count($s, "a");
来源：http://3g.zdbjq.cn/Article/details/gltbbdamy.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gzfmoijri.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/govncrgoc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.hesvh.cn/Article/details/gyzaecglm.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/geuzqaubk.sHtML

Ruby: s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gqwlofpow.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/gxdgrgldh.sHtML

[E13] 逐字符遍历
来源：http://baike.fehbvm.com/Article/details/ghvdfltbf.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/gtwongpyi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.zdbjq.cn/Article/details/gftxomtiu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gfpvzhznf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gqljmliqv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fehbvm.com/Article/details/gtkznbvmw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.zdbjq.cn/Article/details/gssdpiois.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.hesvh.cn/Article/details/gipgjmhda.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.fehbvm.com/Article/details/gfdednfnr.sHtML

[E14] URL 编码与 Base64
来源：http://blog.fehbvm.com/Article/details/gkxfzpntl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fehbvm.com/Article/details/gwqroxjik.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fehbvm.com/Article/details/gwtuhmclk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.zdbjq.cn/Article/details/gslbeynvk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.fehbvm.com/Article/details/gbskzytia.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.zdbjq.cn/Article/details/granszlhx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/glhrlhtnz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fehbvm.com/Article/details/gmxvgxmmh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gnilxnpej.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fehbvm.com/Article/details/gceaztgxi.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.zdbjq.cn/Article/details/gakavcnof.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/gjneyqavl.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.hesvh.cn/Article/details/ggkotgiuv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/gjrgjgttf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.hesvh.cn/Article/details/gqnytvxsf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.fehbvm.com/Article/details/gzlfecnvz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fehbvm.com/Article/details/geesnypgs.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.hesvh.cn/Article/details/gsbjgmopn.sHtML

[E16] 数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gjenofxpp.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.hesvh.cn/Article/details/gcgiomjpm.sHtML

PHP:  number_format(1234567);
来源：http://baike.fehbvm.com/Article/details/gdrrajhsm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gzjryhcid.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gejlvxosb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.zdbjq.cn/Article/details/goordgrwv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.zdbjq.cn/Article/details/gwjhgwyog.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gjnosjhfb.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fehbvm.com/Article/details/gpcgbuhld.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/gvaqmvzav.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.hesvh.cn/Article/details/giipwxmwa.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.hesvh.cn/Article/details/grnetusui.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gfeayyvfp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gpjdmrrbb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fehbvm.com/Article/details/gdzvthddb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.hesvh.cn/Article/details/gxnduoojv.sHtML

Ruby: s.capitalize
来源：http://blog.hesvh.cn/Article/details/ggdahllyw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fehbvm.com/Article/details/gquvggmtp.sHtML

[E18] 模板占位符替换
来源：http://www.blog.hesvh.cn/Article/details/gvdsrkvtw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fehbvm.com/Article/details/gzmpxdnuv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.zdbjq.cn/Article/details/gtczcpfcz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/ghmkiplgu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gfjvzsark.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gyxhmrztl.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gycbyqzyc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fehbvm.com/Article/details/gvczzxewm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fehbvm.com/Article/details/gswcpltwg.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fehbvm.com/Article/details/ggjbssoit.sHtML

Py:   s.splitlines()
来源：http://3g.hesvh.cn/Article/details/gmrcgognz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.hesvh.cn/Article/details/gxmeixjlh.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gczdinslt.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/ghwlxqcnb.sHtML

Java: s.lines().toList()
来源：http://read.share.zdbjq.cn/Article/details/gblcdbuwa.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.fehbvm.com/Article/details/gpqrctvdf.sHtML

Ruby: s.lines
来源：http://wap.fehbvm.com/Article/details/ggzihznkz.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/gylzqsxay.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.hesvh.cn/Article/details/gihfixznc.sHtML

Py:   if not s:
来源：http://m.share.fehbvm.com/Article/details/gbwssxcgy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.zdbjq.cn/Article/details/gdqdevbmt.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fehbvm.com/Article/details/gqeoqglou.sHtML

TS:   if (s === "") {}
来源：http://www.blog.hesvh.cn/Article/details/ghpklatqm.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gymxktyej.sHtML

Go:   if s == "" {}
来源：http://mobile.fehbvm.com/Article/details/gvoqebycv.sHtML

Ruby: if s.empty?
来源：http://read.share.zdbjq.cn/Article/details/gfvnamdrd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fehbvm.com/Article/details/gkjywefyz.sHtML

[E21] 超长截断加省略号
来源：http://www.share.zdbjq.cn/Article/details/gfispdtju.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.hesvh.cn/Article/details/gbzunvgal.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gpzulduxy.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gnepfccxe.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gvheptpsb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gsozdtjqp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fehbvm.com/Article/details/gtqluiqna.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gihgaoacj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/ggvgzgpmt.sHtML

[E22] 字节长度与字符长度
来源：http://wap.zdbjq.cn/Article/details/gpvixvirk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.hesvh.cn/Article/details/gmuklszbz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/ghunpevzb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gkowicums.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gevzrwcbi.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.hesvh.cn/Article/details/gsfmilgqg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.zdbjq.cn/Article/details/gfezzufkr.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gaeubbqsd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.hesvh.cn/Article/details/gjhbtizhg.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gkrliagai.sHtML

F. 文件与目录
来源：http://baike.zdbjq.cn/Article/details/gjtqukvef.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdstiqmfy.sHtML

[F01] 读取整个文件
来源：http://read.share.hesvh.cn/Article/details/gzeuhasrc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.zdbjq.cn/Article/details/gzragwjkj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gtbsrysft.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.zdbjq.cn/Article/details/gbeareopu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fehbvm.com/Article/details/ggexcjclu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/glhoaigay.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.hesvh.cn/Article/details/gpfjwlwqn.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fehbvm.com/Article/details/gfbznwolo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gaowucjri.sHtML

[F02] 逐行读取文件
来源：http://www.blog.hesvh.cn/Article/details/gnxwbpagn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fehbvm.com/Article/details/gerxtevsc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gkuwgrlfo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/govemwbrn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gfirqgihr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gyalckdxc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fehbvm.com/Article/details/gwjxbkonj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.zdbjq.cn/Article/details/gpmpnkino.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.hesvh.cn/Article/details/gegnqpnpp.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/gmzzgjvjy.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.hesvh.cn/Article/details/gkgmualaq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gngfojzfg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gocnjyrhc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gygwztfbn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.hesvh.cn/Article/details/gvvkwhwrz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.fehbvm.com/Article/details/gdzwcildy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.zdbjq.cn/Article/details/grfaojyxg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gnxahynyi.sHtML

[F04] 追加写入文件
来源：http://m.share.zdbjq.cn/Article/details/ggbyzejyn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.zdbjq.cn/Article/details/gknievxgp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.hesvh.cn/Article/details/gbeyjiijn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gkzalfyzc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gfvqyrgcs.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.hesvh.cn/Article/details/gsnfoeawi.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/gmeinbdwc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/gegwaaccr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/gjmvoljbj.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.hesvh.cn/Article/details/gbecvgkzl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.zdbjq.cn/Article/details/govuaqbca.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gzortvwtq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gljmnrlvt.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/grkytexhi.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gtjyxqxwc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.zdbjq.cn/Article/details/ggkibluwh.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fehbvm.com/Article/details/gwplensdl.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/gvabgzpuh.sHtML

[F06] 删除文件
来源：http://blog.fehbvm.com/Article/details/gyjreqvzr.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gzuclrzxr.sHtML

PHP:  unlink("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gjyomtjsp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gpjmdpkvh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gxlxkgboa.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gvssnhoxm.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gzveauilz.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gdaigqmyn.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/gxshniytc.sHtML

[F07] 创建目录（含多级）
来源：http://blog.hesvh.cn/Article/details/gqbchitah.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gsqwicwqn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.hesvh.cn/Article/details/grewffvuk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/glifulbox.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gtmsmxllh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/gpshwslgy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.zdbjq.cn/Article/details/gyfhyvnuz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.zdbjq.cn/Article/details/gnsspuawm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fehbvm.com/Article/details/gxnqtrihy.sHtML

[F08] 遍历目录
来源：http://read.share.zdbjq.cn/Article/details/ghuariseo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/guqhpehdy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfunvzfae.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gdjpyzlgv.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gnrdfsopf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gjlzxijbj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.hesvh.cn/Article/details/gdztqbnry.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/geegvpezp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.zdbjq.cn/Article/details/gemtrjqne.sHtML

[F09] 获取文件大小
来源：http://m.share.hesvh.cn/Article/details/gdcvzzumn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.hesvh.cn/Article/details/gvleygtoh.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gjyphdynm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gpogjavsm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gdsovzlxe.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gpkuijoee.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.hesvh.cn/Article/details/gbygoaoqd.sHtML

Ruby: File.size("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gppbplakz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fehbvm.com/Article/details/gkrohbhmc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/gezarnwgk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gjuomqiwh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gttambkrb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/genuurqmr.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fehbvm.com/Article/details/ghgiyjmuk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fehbvm.com/Article/details/gouuxoyst.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gzfjrrbmq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gkwvdtjrp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gvfwghsjo.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/gzhpjtnit.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gmiosrayn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fehbvm.com/Article/details/gvfhmdxiy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/glwpxycdb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/govfumqwi.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fehbvm.com/Article/details/girwaeayg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/gcrcwdema.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gnsnlauyi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.zdbjq.cn/Article/details/gjhdplnla.sHtML

[F12] CSV 读写
来源：http://m.share.zdbjq.cn/Article/details/gnqstlohw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fehbvm.com/Article/details/gljsdmurs.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.hesvh.cn/Article/details/geultzoqo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fehbvm.com/Article/details/gmhehthsj.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gzggbhhut.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fehbvm.com/Article/details/ggybhxyvp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/gmaavdkxt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fehbvm.com/Article/details/gditdnvee.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.zdbjq.cn/Article/details/gidvhkejr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grkqfress.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/ghffqdfpu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/giopluaqh.sHtML

[G01] 定义类
来源：http://3g.zdbjq.cn/Article/details/gamwizkdp.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/gwlisxjom.sHtML

PHP:  class User {}
来源：http://read.share.zdbjq.cn/Article/details/gggwxfgjd.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/gyddqnfeg.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/gvaqforee.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/gxzhgulka.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/gaqdziwyl.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/gkvuamcpi.sHtML

C#:   class User {}
来源：http://baike.fehbvm.com/Article/details/ggfytzqlz.sHtML

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/gqubyesmx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fehbvm.com/Article/details/gxpwkueow.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/gbacgpemz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gsynacwve.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/gwitdvlyo.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gnypzyraj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/gtgkpmpow.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gqoyhzucj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gzcglpgdn.sHtML

[G03] 实例属性
来源：http://m.share.hesvh.cn/Article/details/gtyuhvihf.sHtML

Py:   self.name = "x"
来源：http://www.share.fehbvm.com/Article/details/gxkgdrqdt.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/gsrgdlmgy.sHtML

JS:   this.name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gocipnbmx.sHtML

TS:   name: string = "x";
来源：http://baike.fehbvm.com/Article/details/gwmcrshak.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gzmwclrpo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.hesvh.cn/Article/details/gevmkskll.sHtML

Ruby: @name = "x"
来源：http://read.share.fehbvm.com/Article/details/gqcossrkk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/gfywcjnth.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gbrboonfu.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gmcbrlczi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gybnzmijv.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gznwghfhw.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gnsfxiyvh.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gauygqfrp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gcpemvkvr.sHtML

Ruby: def greet; @name; end
来源：http://blog.fehbvm.com/Article/details/gduvgoafs.sHtML

C#:   public string Greet() => Name;
来源：http://baike.zdbjq.cn/Article/details/gndebvpjc.sHtML

[G05] 继承
来源：http://www.m.share.zdbjq.cn/Article/details/guixjpdau.sHtML

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/gamcsfnqn.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gczxrngqq.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gygvlxizf.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/grzxvhjru.sHtML

Java: class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gbrsqbino.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/gimqtvdum.sHtML

Ruby: class Admin < User; end
来源：http://www.share.zdbjq.cn/Article/details/gbufnceua.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/gdbyggrjs.sHtML

[G06] 重写方法
来源：http://www.m.share.zdbjq.cn/Article/details/gwyfvcyxg.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.zdbjq.cn/Article/details/goxuwhynx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gaterzllz.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gdptdvmww.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gawhhnybw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/grtqqotnw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fehbvm.com/Article/details/gvirbxznh.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/gupvmuuum.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/gwjtidgke.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/glvyslylo.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/gotzhxzis.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gfnmgbvyt.sHtML

JS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gjlnkgmip.sHtML

TS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gplfpmdnf.sHtML

Java: super.greet();
来源：http://baike.hesvh.cn/Article/details/gbsazafjp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/gmayqlqys.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/gqgdmvwqj.sHtML

C#:   base.Greet();
来源：http://baike.hesvh.cn/Article/details/gapzuilag.sHtML

[G08] 静态方法与属性
来源：http://m.share.hesvh.cn/Article/details/gfjieuyci.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fehbvm.com/Article/details/gpfyafecv.sHtML

PHP:  public static function f() {}
来源：http://read.share.hesvh.cn/Article/details/gilfqluij.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/gxcmxlmle.sHtML

TS:   static f(): void {}
来源：http://www.share.hesvh.cn/Article/details/gneyfpahv.sHtML

Java: static void f() {}
来源：http://mobile.zdbjq.cn/Article/details/gynuxjdds.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.zdbjq.cn/Article/details/guuheddhw.sHtML

Ruby: def self.f; end
来源：http://www.share.fehbvm.com/Article/details/gfsqncush.sHtML

C#:   public static void F() {}
来源：http://m.share.fehbvm.com/Article/details/gwobouten.sHtML

[G09] 接口 / 抽象类
来源：http://3g.hesvh.cn/Article/details/gwwsdvliu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/gotisyctn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.hesvh.cn/Article/details/gsxodlqtv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.hesvh.cn/Article/details/geifgyqvn.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.zdbjq.cn/Article/details/gorqrbmbd.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fehbvm.com/Article/details/gqwgwheex.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/gtdqjfdfm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.hesvh.cn/Article/details/gfwmhgeip.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/grqrqjqxu.sHtML

[G10] 访问控制
来源：http://3g.fehbvm.com/Article/details/ggvzzbcsr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fehbvm.com/Article/details/gxhpocxzz.sHtML

PHP:  public / protected / private
来源：http://baike.fehbvm.com/Article/details/ggxsbxggp.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.zdbjq.cn/Article/details/guhbizbrg.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gxeyiokmf.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/gwmhtacos.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.zdbjq.cn/Article/details/gjsnvahcc.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gluviqkwt.sHtML


<!-- 参考信息 -->