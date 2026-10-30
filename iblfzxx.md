代发 wailian999

PHP:  substr_count($s, "a");
来源：http://baike.fehbvm.com/Article/details/gychklttr.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/giyuawcoz.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gjviqvsug.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fehbvm.com/Article/details/gafyfllon.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.zdbjq.cn/Article/details/groblcpaj.sHtML

Ruby: s.count("a")
来源：http://mobile.hesvh.cn/Article/details/grnwpuqcw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.zdbjq.cn/Article/details/gqpgvunlz.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/gvgsdzgkf.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.fehbvm.com/Article/details/gusyzlddk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.zdbjq.cn/Article/details/gfwrlhoab.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gzvkhpgym.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gpuahbhrf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gdonujbtu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fehbvm.com/Article/details/gdoknfapk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fehbvm.com/Article/details/goaeyozhu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gcocyvyxr.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.hesvh.cn/Article/details/gkvsltkdv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.hesvh.cn/Article/details/gdjytbrdq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gzqlzvqll.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/grderpegh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.hesvh.cn/Article/details/gndycpfrq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.hesvh.cn/Article/details/gthiqanza.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fehbvm.com/Article/details/gmnjyaozl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.hesvh.cn/Article/details/gebkgcmzz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gbjjfcalk.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.zdbjq.cn/Article/details/gucajpigr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.zdbjq.cn/Article/details/gwzcjnpwx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fehbvm.com/Article/details/grldaerpw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fehbvm.com/Article/details/gedmihvcs.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/gxezjrxvn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.zdbjq.cn/Article/details/gxmfjdvkm.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fehbvm.com/Article/details/guwwytgat.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fehbvm.com/Article/details/ggszqjstn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.zdbjq.cn/Article/details/gxecunkhf.sHtML

[E16] 数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gfqibvqvn.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.zdbjq.cn/Article/details/gincevovo.sHtML

PHP:  number_format(1234567);
来源：http://read.share.zdbjq.cn/Article/details/gvpbmsojt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gipqttppu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gdchodndk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fehbvm.com/Article/details/gfqazpatf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fehbvm.com/Article/details/gxbckkpah.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.hesvh.cn/Article/details/gkgqfjxem.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.hesvh.cn/Article/details/gbknbdljl.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/gojxqmcqf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.zdbjq.cn/Article/details/gfukhovjs.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.fehbvm.com/Article/details/gutvpipzz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gvbcrindn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/giwvlutnj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.hesvh.cn/Article/details/gplenmwqe.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fehbvm.com/Article/details/geqmqlxsb.sHtML

Ruby: s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gydngrthw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.hesvh.cn/Article/details/gmtgvwbkq.sHtML

[E18] 模板占位符替换
来源：http://m.share.zdbjq.cn/Article/details/ghyzaofld.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.hesvh.cn/Article/details/gryzhvkaq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.hesvh.cn/Article/details/gyrelqyda.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gytqxwegw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/glykkjdve.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gscyykacy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.fehbvm.com/Article/details/gkqcspbmm.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.zdbjq.cn/Article/details/gujwsmtbj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.hesvh.cn/Article/details/gfybwvytr.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.fehbvm.com/Article/details/gbihfxwui.sHtML

Py:   s.splitlines()
来源：http://baike.fehbvm.com/Article/details/gcmkifgup.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.hesvh.cn/Article/details/gtrsmyllu.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gawxgukxo.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/givtidilm.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gbpqqlvgh.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.hesvh.cn/Article/details/gkmjpaanq.sHtML

Ruby: s.lines
来源：http://wap.zdbjq.cn/Article/details/ggwljajqs.sHtML

C#:   s.Split('\n')
来源：http://baike.hesvh.cn/Article/details/gltarcjyg.sHtML

[E20] 判断字符串是否为空
来源：http://baike.hesvh.cn/Article/details/gpavceqag.sHtML

Py:   if not s:
来源：http://baike.zdbjq.cn/Article/details/gyiiwdfja.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fehbvm.com/Article/details/gkocwvvse.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gszmqsmld.sHtML

TS:   if (s === "") {}
来源：http://mobile.hesvh.cn/Article/details/gmtkothej.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqjiiytfk.sHtML

Go:   if s == "" {}
来源：http://read.share.zdbjq.cn/Article/details/gmizwesve.sHtML

Ruby: if s.empty?
来源：http://www.blog.hesvh.cn/Article/details/gnpemjenj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.hesvh.cn/Article/details/gopxeygby.sHtML

[E21] 超长截断加省略号
来源：http://3g.hesvh.cn/Article/details/gtjewraey.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.hesvh.cn/Article/details/gahabziwj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gqqqvlgcd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gmbwovffe.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gnflwlmkz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gdjwrbsxl.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.hesvh.cn/Article/details/ghdciryjc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gawvszohb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/ghyfwlkoi.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.hesvh.cn/Article/details/gvgzixtbn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fehbvm.com/Article/details/gvnziawhx.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/guplwjgej.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gmthbjpee.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gtvyuembq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fehbvm.com/Article/details/gnboydkrs.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/gyantqerg.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.hesvh.cn/Article/details/gsbvofugl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/gscjwswtf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gljvjkshn.sHtML

F. 文件与目录
来源：http://read.share.fehbvm.com/Article/details/gegakenxf.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzpdowbnv.sHtML

[F01] 读取整个文件
来源：http://blog.fehbvm.com/Article/details/gvrjzditw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.hesvh.cn/Article/details/gearliscr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gsobafixj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.hesvh.cn/Article/details/gravctjzh.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gacxbukfn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gnvfkskue.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.hesvh.cn/Article/details/gqsmibmav.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/gktyzikfv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gpwjdxlqs.sHtML

[F02] 逐行读取文件
来源：http://www.share.fehbvm.com/Article/details/gonsinwox.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.hesvh.cn/Article/details/gxcfmtnat.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fehbvm.com/Article/details/gfjtzwaai.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/ghgngzlzk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gtlqxmkgs.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gxbuwypdx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.zdbjq.cn/Article/details/gakuebypp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.hesvh.cn/Article/details/gdidgeudc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/geydxgyhi.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.zdbjq.cn/Article/details/gbdhkednh.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.fehbvm.com/Article/details/gktrtdqgh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gbltskkjd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gpjsmbeur.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/govcmqjhv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.hesvh.cn/Article/details/gadsoyqtk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.hesvh.cn/Article/details/gwbwitpkw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.zdbjq.cn/Article/details/gntkinrsy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gvcqgqqld.sHtML

[F04] 追加写入文件
来源：http://wap.fehbvm.com/Article/details/gwrixaums.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gdxancikx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.zdbjq.cn/Article/details/gkazaleig.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gdmshkvxk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/goaatrbhv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.zdbjq.cn/Article/details/gxxdmforj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/gegrewogl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.fehbvm.com/Article/details/gxvwocxhd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.hesvh.cn/Article/details/gjyjewlhn.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.zdbjq.cn/Article/details/gytzeqrea.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.hesvh.cn/Article/details/ggcnhjkcx.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gjxkwkbpe.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gkhntryiu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gkibymwjd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gmgkhrfzm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.zdbjq.cn/Article/details/gwzaobcxh.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/goamycxql.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gyapyofnp.sHtML

[F06] 删除文件
来源：http://read.share.zdbjq.cn/Article/details/gpydsfxce.sHtML

Py:   os.remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gwcklnksj.sHtML

PHP:  unlink("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gifhiamsj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/ggchsttke.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gmmnbnlei.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gpkvasyix.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/ggtjguevs.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/gwrfyglkc.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.hesvh.cn/Article/details/ghphxqjfh.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.zdbjq.cn/Article/details/gloorkakj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gdklxphaz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.hesvh.cn/Article/details/gcvtoblft.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gcdedrvzv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/guviphzws.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/gmaefoebo.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/ggtxheimk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fehbvm.com/Article/details/guqpyfgrt.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/gxxjfguvh.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/gnacirrot.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fehbvm.com/Article/details/gfbfezuoi.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/goqlbojeb.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gwcsalgjq.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/grrppxooz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gdzryoivq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.zdbjq.cn/Article/details/gqwvpqodm.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/glpmgluss.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/ghguysmvp.sHtML

[F09] 获取文件大小
来源：http://www.blog.hesvh.cn/Article/details/ghetijtjy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fehbvm.com/Article/details/gewffbkxn.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/gybwvfcsc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gcwwelgws.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gvqvynahw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gqrqegkgg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.zdbjq.cn/Article/details/gawwlnzda.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gyutgydyc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.hesvh.cn/Article/details/gmpvtjvmq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.zdbjq.cn/Article/details/gmzpqcmfy.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gqciblfdl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gazkjbakz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/glizptvrm.sHtML

TS:   path.extname("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gcvktnxjq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.hesvh.cn/Article/details/ghcrqnaww.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gaeimyzlf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gqhcyhyue.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gqzmfekjt.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.zdbjq.cn/Article/details/gfqvebwiq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gkzpycmqx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.zdbjq.cn/Article/details/gmjfuldvf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gdneovswg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gyxsmnnnx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.hesvh.cn/Article/details/gbptpbnxa.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.zdbjq.cn/Article/details/gkpylkkdw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gawvnaweb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/gdnukqrvs.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/ghabmdkym.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.zdbjq.cn/Article/details/gwscbrvjq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fehbvm.com/Article/details/gyjjkutyb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/gqbkvrxpe.sHtML

TS:   // 同上
来源：http://mobile.fehbvm.com/Article/details/gvkyugupi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.zdbjq.cn/Article/details/gtvxvslxm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.hesvh.cn/Article/details/gklgvdppt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fehbvm.com/Article/details/gtywxaqmn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.hesvh.cn/Article/details/gvnwbaonl.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grrvzejww.sHtML

G. 面向对象
来源：http://baike.hesvh.cn/Article/details/gtahfaqnd.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grflwwsol.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/gbutvdnjm.sHtML

Py:   class User: pass
来源：http://blog.fehbvm.com/Article/details/gtvfoxwod.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/gratxfpfc.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gqzwjwfla.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gatzuvlev.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/glnveqvoq.sHtML

Go:   type User struct { Name string }
来源：http://baike.zdbjq.cn/Article/details/glbroypfb.sHtML

Ruby: class User; end
来源：http://www.m.share.hesvh.cn/Article/details/gccntenes.sHtML

C#:   class User {}
来源：http://blog.hesvh.cn/Article/details/gfcvgkjnw.sHtML

[G02] 构造函数
来源：http://blog.fehbvm.com/Article/details/gxczivtdd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.hesvh.cn/Article/details/gwlnvkqxp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/gfwkgkniv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gcmjkmydq.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/gdiwlupjb.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gqxugtjkg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/gdgvanqwu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.zdbjq.cn/Article/details/gwnqtvrkg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gudstdnms.sHtML

[G03] 实例属性
来源：http://blog.fehbvm.com/Article/details/gdlcgjrbk.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/gvadnqwds.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fehbvm.com/Article/details/gtyiwfyev.sHtML

JS:   this.name = "x";
来源：http://baike.hesvh.cn/Article/details/ggcpkeqmo.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gpudrlbep.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gdbncdpmt.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fehbvm.com/Article/details/ghvtvnxlq.sHtML

Ruby: @name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gvwozpeae.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.hesvh.cn/Article/details/glimutnqh.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/gjcfhoxuz.sHtML

Py:   def greet(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gtwvpyloh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gadtaqfbb.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gyfspcmle.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gczlfxwfa.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/galzfiixa.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gdrbwhuyw.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gxlyxnpty.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/gghelyhev.sHtML

[G05] 继承
来源：http://3g.hesvh.cn/Article/details/ghvglzvcf.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/gmjoytipp.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gppgjiumz.sHtML

JS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gkizsdhqv.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gwoqtzuyt.sHtML

Java: class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gondyxmtf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/gksdndtcc.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gntnzbmec.sHtML

C#:   class Admin : User {}
来源：http://3g.zdbjq.cn/Article/details/gymimozcz.sHtML

[G06] 重写方法
来源：http://www.m.share.zdbjq.cn/Article/details/gljiebqzz.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.hesvh.cn/Article/details/gpmybpjjv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gzvxzwoev.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gfdyeifmk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gjyduigvd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gljrwmwvx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/gapcpnrqw.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/gfgeygajx.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/gzuvrqctz.sHtML

[G07] 调用父类方法
来源：http://www.blog.hesvh.cn/Article/details/gnpjvnxmv.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/gllaktdbk.sHtML

PHP:  parent::greet();
来源：http://www.share.fehbvm.com/Article/details/gcomxyrjq.sHtML

JS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gnxzhtnse.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gjxeidihf.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/gkfdldeck.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fehbvm.com/Article/details/gmdeygshg.sHtML

Ruby: super
来源：http://wap.zdbjq.cn/Article/details/gfyuabxbz.sHtML

C#:   base.Greet();
来源：http://wap.zdbjq.cn/Article/details/gjxokxzxn.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/gulnnzlks.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.hesvh.cn/Article/details/glfcwlwzu.sHtML

PHP:  public static function f() {}
来源：http://www.blog.hesvh.cn/Article/details/gyrjmrohy.sHtML

JS:   static f() {}
来源：http://wap.fehbvm.com/Article/details/gvrzepkyf.sHtML

TS:   static f(): void {}
来源：http://wap.zdbjq.cn/Article/details/gvbvtrocj.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/garhmftup.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.zdbjq.cn/Article/details/gzbbymmgf.sHtML

Ruby: def self.f; end
来源：http://mobile.zdbjq.cn/Article/details/gzizuaced.sHtML

C#:   public static void F() {}
来源：http://m.share.fehbvm.com/Article/details/gajzcygzr.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/gcovdxrxf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.hesvh.cn/Article/details/gzzjfnayf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fehbvm.com/Article/details/gjglnjtxn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/gcyvbwrqd.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.hesvh.cn/Article/details/greujrkdr.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fehbvm.com/Article/details/gxryoksky.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.hesvh.cn/Article/details/gpnyvjimn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fehbvm.com/Article/details/gnbowejej.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fehbvm.com/Article/details/gisccgwte.sHtML

[G10] 访问控制
来源：http://blog.zdbjq.cn/Article/details/gwpteqhcl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/gugsvnlkc.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gkckmbnuh.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/gubhuaomt.sHtML

TS:   public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gjrdbxtkd.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/gmeftgmem.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.hesvh.cn/Article/details/gwvszkwfc.sHtML

Ruby: public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gcxixaees.sHtML


<!-- 参考信息 -->