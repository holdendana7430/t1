代发 wailian999

[E14] URL 编码与 Base64
来源：http://m.share.zdbjq.cn/Article/details/gwvtlzoie.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fehbvm.com/Article/details/geoiiumpt.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fehbvm.com/Article/details/gucjxaxnp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.hesvh.cn/Article/details/glyjtvjyy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.hesvh.cn/Article/details/gfbhhadrh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fehbvm.com/Article/details/gjzigizus.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.hesvh.cn/Article/details/gmllfgisu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.fehbvm.com/Article/details/gcekdjylq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.hesvh.cn/Article/details/grpbilnan.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fehbvm.com/Article/details/gxspwuzji.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.hesvh.cn/Article/details/gmwywqkhe.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.zdbjq.cn/Article/details/gnidemhmn.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fehbvm.com/Article/details/gmdgxmlah.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/gjtqnfuzt.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.hesvh.cn/Article/details/geqyokpiu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.zdbjq.cn/Article/details/gddhfypic.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.hesvh.cn/Article/details/gscxblhpk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.hesvh.cn/Article/details/grdemseon.sHtML

[E16] 数字千分位
来源：http://m.share.fehbvm.com/Article/details/gnbuomfdh.sHtML

Py:   f"{1234567:,}"
来源：http://blog.zdbjq.cn/Article/details/ghqzbbrty.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/gxjihcdcy.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/ghtwazhql.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gxwuavleb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gejdqkoxq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.zdbjq.cn/Article/details/gbhkittdl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fehbvm.com/Article/details/gfvszxtzv.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fehbvm.com/Article/details/gtebvyytn.sHtML

[E17] 首字母大写
来源：http://mobile.fehbvm.com/Article/details/gdwvhsabp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.zdbjq.cn/Article/details/gxmywrofd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.zdbjq.cn/Article/details/gvgkpvowi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/ggvcpvvja.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gudqkvssh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fehbvm.com/Article/details/gupmxmfqv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.hesvh.cn/Article/details/gwowutreb.sHtML

Ruby: s.capitalize
来源：http://3g.fehbvm.com/Article/details/gxkwaeqld.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.zdbjq.cn/Article/details/gopfmidpz.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.hesvh.cn/Article/details/getxtzwsu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/ggxhbriof.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/gkvzfvrkw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gsjmufkgv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gjduxzdvf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.hesvh.cn/Article/details/grvppdhgb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gqgmrzkri.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/gocdxhzqj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fehbvm.com/Article/details/gjelshmxx.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.zdbjq.cn/Article/details/gacqscmrq.sHtML

Py:   s.splitlines()
来源：http://blog.zdbjq.cn/Article/details/gedfnftnh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.hesvh.cn/Article/details/gmwhtsfem.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gvcmkykwo.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gtpvwxypo.sHtML

Java: s.lines().toList()
来源：http://baike.hesvh.cn/Article/details/ghmjgofsj.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fehbvm.com/Article/details/gsjfulpbj.sHtML

Ruby: s.lines
来源：http://www.share.hesvh.cn/Article/details/gntcslsqb.sHtML

C#:   s.Split('\n')
来源：http://wap.zdbjq.cn/Article/details/gbtbhbjwh.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.hesvh.cn/Article/details/gnmqeekoj.sHtML

Py:   if not s:
来源：http://blog.hesvh.cn/Article/details/gzmsmzymr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.hesvh.cn/Article/details/gekhmbzxx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.hesvh.cn/Article/details/gluovmidm.sHtML

TS:   if (s === "") {}
来源：http://blog.hesvh.cn/Article/details/gjotbqavb.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gatghujdo.sHtML

Go:   if s == "" {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcjncrhdi.sHtML

Ruby: if s.empty?
来源：http://baike.zdbjq.cn/Article/details/guaboufqu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fehbvm.com/Article/details/gybnpwipa.sHtML

[E21] 超长截断加省略号
来源：http://m.share.hesvh.cn/Article/details/gudxqzrng.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.hesvh.cn/Article/details/gwkfhkprl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gihorcbzg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gmpmkxjay.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gbhzjdzpr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/ggbptqfvt.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.zdbjq.cn/Article/details/gmiiavsde.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gtczshiye.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gxrpentuz.sHtML

[E22] 字节长度与字符长度
来源：http://baike.zdbjq.cn/Article/details/giayxcxch.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.hesvh.cn/Article/details/gyxkzjvye.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gkhamivfz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gjmoggffk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gtxljvyvj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gizfwhrsl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.hesvh.cn/Article/details/gzamhpjrv.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gurgwfphx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fehbvm.com/Article/details/glipkfdmq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gywajmatm.sHtML

F. 文件与目录
来源：http://read.share.zdbjq.cn/Article/details/guubkezks.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gsfjnkveq.sHtML

[F01] 读取整个文件
来源：http://read.share.fehbvm.com/Article/details/gfhjmruik.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.hesvh.cn/Article/details/gofsejfct.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.hesvh.cn/Article/details/gnxokqeqt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.hesvh.cn/Article/details/giexguhdd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gullczgvy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gxwdqodph.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/gpmacmtvh.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gkxvwyibn.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.hesvh.cn/Article/details/gurqnpjcw.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fehbvm.com/Article/details/gfooziknz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.zdbjq.cn/Article/details/gurlbbaup.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/gvryrnkcp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gqruiwaim.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gcpfacdso.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gjnrwbyfo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fehbvm.com/Article/details/gbdslfntm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.hesvh.cn/Article/details/gtbedjcbt.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/gjwegafmq.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.hesvh.cn/Article/details/gdlenqnki.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.hesvh.cn/Article/details/garqhbmwh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gynvpgkyk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gqaoqlhwk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gohrzmcsn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fehbvm.com/Article/details/gipczxqwe.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fehbvm.com/Article/details/gscdysvmp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.zdbjq.cn/Article/details/gaemcyljl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/ghdggfygz.sHtML

[F04] 追加写入文件
来源：http://baike.fehbvm.com/Article/details/gqvxrooby.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fehbvm.com/Article/details/gafbrwoal.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.zdbjq.cn/Article/details/gnpczvatd.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gggamvvzi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gqewkoyxp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.hesvh.cn/Article/details/gzbgvjags.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fehbvm.com/Article/details/gayhxbkhx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.zdbjq.cn/Article/details/gaadksktu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fehbvm.com/Article/details/gjuwbvwsm.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.zdbjq.cn/Article/details/gzdbyfuun.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/guxsyoprb.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gvoahcifm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gmnfajtpq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gmwgdupnn.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gwsuptkfg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.hesvh.cn/Article/details/gkyfrssqr.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gooqwvexx.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gayhjtdib.sHtML

[F06] 删除文件
来源：http://mobile.fehbvm.com/Article/details/gqqgyaqpc.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gpkivylkt.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gbjlopgho.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gstdsjztx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gadevboqx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/golxauyyd.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gkhgyhcir.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gglcirrrz.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gxzttvblw.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fehbvm.com/Article/details/ghgqqvouw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/goprmscmn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.hesvh.cn/Article/details/gkoqgfael.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gpluxshco.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gymclpgld.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.hesvh.cn/Article/details/gpzslknhw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fehbvm.com/Article/details/gtonggiib.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fehbvm.com/Article/details/gyyfnbcgt.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.zdbjq.cn/Article/details/gyiyhjczv.sHtML

[F08] 遍历目录
来源：http://3g.fehbvm.com/Article/details/gmulprdmt.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/gqhugbxzd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.zdbjq.cn/Article/details/gaifzuuau.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gwwbkjbod.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gnfjcetzy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/ginsrymcd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.zdbjq.cn/Article/details/ggfxemhcg.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.hesvh.cn/Article/details/gxrhiuyck.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.hesvh.cn/Article/details/gobautofd.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/gymgwnhuu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.zdbjq.cn/Article/details/ghhefpgfq.sHtML

PHP:  filesize("a.txt");
来源：http://3g.hesvh.cn/Article/details/gkagtelxm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gzeulicwj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gzergtwal.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gygsnryib.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fehbvm.com/Article/details/gnlbqkpfk.sHtML

Ruby: File.size("a.txt")
来源：http://3g.hesvh.cn/Article/details/glfvxyjij.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.fehbvm.com/Article/details/ggnvlvpgt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.hesvh.cn/Article/details/gojalyaqd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/glgzrcurh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gwfskeovj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gghrtggda.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gbyokdukm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.hesvh.cn/Article/details/gwlqoatya.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gzkdxlrgm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gmrojpepx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gewqagxvh.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/gpidlpxrd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/giusyteqp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fehbvm.com/Article/details/grtjbjsku.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/ggexfvfxc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/golpyhnqb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.zdbjq.cn/Article/details/gfpswpewd.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/glqkikfpi.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gzsoqnyxx.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.hesvh.cn/Article/details/gdcjvmsbq.sHtML

[F12] CSV 读写
来源：http://read.share.hesvh.cn/Article/details/gjbfkggil.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/gfnbngjfa.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/gphtelgpe.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/gmmpfipig.sHtML

TS:   // 同上
来源：http://m.share.zdbjq.cn/Article/details/gevsburla.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.zdbjq.cn/Article/details/grakcfwsd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fehbvm.com/Article/details/gdixojtrr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fehbvm.com/Article/details/gejwssoqx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.zdbjq.cn/Article/details/gzjhwqffn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/glonfozlx.sHtML

G. 面向对象
来源：http://www.share.hesvh.cn/Article/details/gsjivnnqm.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/govwutlzk.sHtML

[G01] 定义类
来源：http://www.m.share.hesvh.cn/Article/details/gmhyulefm.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/gshdeiaif.sHtML

PHP:  class User {}
来源：http://blog.hesvh.cn/Article/details/gfrokzpkc.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/grvmysbyu.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/gjkwdnyvn.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/gvmkmyrfr.sHtML

Go:   type User struct { Name string }
来源：http://baike.zdbjq.cn/Article/details/gbcdfwtbz.sHtML

Ruby: class User; end
来源：http://www.blog.hesvh.cn/Article/details/ghlzzskkr.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gfopeqefh.sHtML

[G02] 构造函数
来源：http://www.share.fehbvm.com/Article/details/gwagyshmp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.zdbjq.cn/Article/details/gulgbzdzi.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/gjcryeeub.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gdcfqlpgv.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/glbcpsart.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gdrynmvck.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/gzwifoikr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.fehbvm.com/Article/details/gnpwwmowd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gediixpwx.sHtML

[G03] 实例属性
来源：http://3g.fehbvm.com/Article/details/ghrychkhf.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gbccattrb.sHtML

PHP:  public string $name = "x";
来源：http://3g.fehbvm.com/Article/details/gyxztxivl.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gwylxyint.sHtML

TS:   name: string = "x";
来源：http://mobile.zdbjq.cn/Article/details/gbpmrmggg.sHtML

Java: private String name;
来源：http://read.share.zdbjq.cn/Article/details/gtkbqkzne.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/glpnszvln.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/gurbjrxcm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fehbvm.com/Article/details/gvhxjenkm.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/gnpznakmz.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gqnyquodq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gtifstrce.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gpynczlri.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/ggnlvgkwv.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gvwbmkwwt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gcznzxqre.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/gksnovvyk.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.hesvh.cn/Article/details/gsxhygjlw.sHtML

[G05] 继承
来源：http://baike.hesvh.cn/Article/details/grayxsjyy.sHtML

Py:   class Admin(User): pass
来源：http://www.share.zdbjq.cn/Article/details/gnxtcdcka.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gdlnnlxme.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/girbsphfd.sHtML

TS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gidmwtajk.sHtML

Java: class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gvitcewlh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/gksbdwddq.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/goyotsaxh.sHtML

C#:   class Admin : User {}
来源：http://read.share.hesvh.cn/Article/details/gynjafpwq.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/gqlvvsxfq.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fehbvm.com/Article/details/gvgyszxtg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gkybpmkli.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gtrvjdwnh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gksfmufeu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gcnetqknh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fehbvm.com/Article/details/gnrmdhirv.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.zdbjq.cn/Article/details/gdwsbrxnw.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fehbvm.com/Article/details/gfwvfufar.sHtML

[G07] 调用父类方法
来源：http://3g.fehbvm.com/Article/details/gtybmrunl.sHtML

Py:   super().greet()
来源：http://mobile.fehbvm.com/Article/details/gbeenlegd.sHtML

PHP:  parent::greet();
来源：http://baike.fehbvm.com/Article/details/gdfscswvf.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/galdsuaso.sHtML

TS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gotbupbdy.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gjxqsjjcj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.zdbjq.cn/Article/details/ghhqyotco.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/gijzbjkrw.sHtML

C#:   base.Greet();
来源：http://www.m.share.hesvh.cn/Article/details/gpsjxhzhm.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fehbvm.com/Article/details/gmbosnaog.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/gktyjzerz.sHtML

PHP:  public static function f() {}
来源：http://baike.zdbjq.cn/Article/details/guyvskzpv.sHtML

JS:   static f() {}
来源：http://mobile.hesvh.cn/Article/details/gwbiguoan.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/grctthohq.sHtML

Java: static void f() {}
来源：http://m.share.zdbjq.cn/Article/details/gwtrhwixt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/gkkxybxtf.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/gptqydpgf.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/gkuriauul.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fehbvm.com/Article/details/gsvodlwta.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.zdbjq.cn/Article/details/gybepamln.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/gawrnzxmx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/grdoiosru.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/glbgqvttv.sHtML

Java: interface Shape { double area(); }
来源：http://blog.hesvh.cn/Article/details/gdysyvrjz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fehbvm.com/Article/details/gotlmikor.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/gfdomnhon.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/gevwtzbmz.sHtML

[G10] 访问控制
来源：http://www.blog.fehbvm.com/Article/details/guobdfqtv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fehbvm.com/Article/details/gsqelntmc.sHtML

PHP:  public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gfjytfane.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.hesvh.cn/Article/details/gdjltsodq.sHtML

TS:   public / protected / private
来源：http://blog.fehbvm.com/Article/details/gibxxcqlo.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fehbvm.com/Article/details/gdhxcgrxv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.zdbjq.cn/Article/details/goawmhyup.sHtML

Ruby: public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/glzxptqon.sHtML

C#:   public / protected / private / internal
来源：http://wap.fehbvm.com/Article/details/gpvzeuyzo.sHtML

[G11] getter / setter
来源：http://mobile.zdbjq.cn/Article/details/gtmzwcrtf.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/ghssmfqhs.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/grdqwkcan.sHtML

JS:   get name() { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gyandvxlc.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.hesvh.cn/Article/details/glcjifkqc.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gzgwnnlip.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gygrjvglo.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/gwlhpapzw.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/gqmpsbmwx.sHtML

[G12] 对象转字符串
来源：http://wap.hesvh.cn/Article/details/gmkohkhhy.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gibzewrjc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gmbxwdlpy.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gqdecfxie.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/grvgwbigw.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/gupvemlgk.sHtML


<!-- 参考信息 -->