代发 wailian999

[E14] URL 编码与 Base64
来源：http://3g.fehbvm.com/Article/details/gxdgxhawq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.hesvh.cn/Article/details/gdextddlv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.zdbjq.cn/Article/details/gneehwmsn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fehbvm.com/Article/details/geyrmlvbm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.hesvh.cn/Article/details/gkhpbfmbp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gjkjxlcxl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.hesvh.cn/Article/details/gucscnmfr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fehbvm.com/Article/details/gqeoadhkt.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fehbvm.com/Article/details/gowvjjyqj.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fehbvm.com/Article/details/gncdaadgy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.zdbjq.cn/Article/details/guyqwfprd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.hesvh.cn/Article/details/gtxjgiiue.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fehbvm.com/Article/details/gvlqwhvbo.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/gfcspgezp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.zdbjq.cn/Article/details/gcauvvvdu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.hesvh.cn/Article/details/goqlchrdd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.zdbjq.cn/Article/details/gkczdjzsh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.zdbjq.cn/Article/details/gmzjjkgml.sHtML

[E16] 数字千分位
来源：http://www.share.hesvh.cn/Article/details/gtuysgqtt.sHtML

Py:   f"{1234567:,}"
来源：http://blog.zdbjq.cn/Article/details/gsukfemxc.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fehbvm.com/Article/details/gpfoxjlzt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gkohjomyf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gttznbtmi.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.hesvh.cn/Article/details/gjtlbtsnm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.hesvh.cn/Article/details/gtftmsnyh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.hesvh.cn/Article/details/gbpvgfqmv.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.hesvh.cn/Article/details/gsebsvwuy.sHtML

[E17] 首字母大写
来源：http://read.share.zdbjq.cn/Article/details/gfukhhfmw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fehbvm.com/Article/details/gllywocum.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fehbvm.com/Article/details/gsfffuldl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gqjnzuoud.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gsnudkset.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.hesvh.cn/Article/details/glgxdicme.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.zdbjq.cn/Article/details/gtomwfbhf.sHtML

Ruby: s.capitalize
来源：http://read.share.hesvh.cn/Article/details/goqwycryb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.zdbjq.cn/Article/details/glzrjmsjw.sHtML

[E18] 模板占位符替换
来源：http://www.share.hesvh.cn/Article/details/gwbvxbjop.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.fehbvm.com/Article/details/getjimdof.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.zdbjq.cn/Article/details/glkmmzxlf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gqhidqggt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gixgxevzo.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/glpjdvucl.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/ggfmuuyva.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fehbvm.com/Article/details/gzekbsyzt.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.hesvh.cn/Article/details/gqywnalbb.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fehbvm.com/Article/details/gcljeouoq.sHtML

Py:   s.splitlines()
来源：http://www.blog.zdbjq.cn/Article/details/gusurytge.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fehbvm.com/Article/details/gojuqmvty.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gbazdtwwu.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/gqdtkybmj.sHtML

Java: s.lines().toList()
来源：http://wap.zdbjq.cn/Article/details/gtvweoipo.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/goqliucmz.sHtML

Ruby: s.lines
来源：http://www.share.zdbjq.cn/Article/details/gtidbmugw.sHtML

C#:   s.Split('\n')
来源：http://www.share.hesvh.cn/Article/details/getbkgpkm.sHtML

[E20] 判断字符串是否为空
来源：http://baike.hesvh.cn/Article/details/guyggnnpo.sHtML

Py:   if not s:
来源：http://3g.zdbjq.cn/Article/details/gxlbzczqj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.zdbjq.cn/Article/details/gvpmbldbw.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.zdbjq.cn/Article/details/gvoylthyc.sHtML

TS:   if (s === "") {}
来源：http://www.blog.zdbjq.cn/Article/details/gaiywzmvc.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gnsnfvxaj.sHtML

Go:   if s == "" {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxgkpepau.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/gdqhlzffv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.hesvh.cn/Article/details/ggydiplou.sHtML

[E21] 超长截断加省略号
来源：http://wap.hesvh.cn/Article/details/gxxbxbsjb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/gzrmdsvpb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/glixevqli.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gtedjfgyd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gkqihevud.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gqoulaxzm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.hesvh.cn/Article/details/gurlruwsx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gkarhmjwz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gwhmvwyhl.sHtML

[E22] 字节长度与字符长度
来源：http://blog.fehbvm.com/Article/details/gsisbhovr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.hesvh.cn/Article/details/genckjmug.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gsrkbsezq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gwrqpmqvq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/ghsvnvall.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fehbvm.com/Article/details/gjszwilus.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/gbnouxkhn.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.zdbjq.cn/Article/details/ggjndcyci.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.zdbjq.cn/Article/details/grgsjunjg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpwxkrwkz.sHtML

F. 文件与目录
来源：http://www.share.zdbjq.cn/Article/details/gqpoxzjik.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gownzuomm.sHtML

[F01] 读取整个文件
来源：http://www.blog.fehbvm.com/Article/details/gcjdjylxs.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.hesvh.cn/Article/details/gkgedsrdy.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/grbmohtql.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.hesvh.cn/Article/details/gdhlzsobn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fehbvm.com/Article/details/guxdwckkr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gfysxbury.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.fehbvm.com/Article/details/gzyxiwxjt.sHtML

Ruby: File.read("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gufssvkrd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.zdbjq.cn/Article/details/glezhuejv.sHtML

[F02] 逐行读取文件
来源：http://read.share.hesvh.cn/Article/details/gdxllkqzi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fehbvm.com/Article/details/gdqbqwclh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.zdbjq.cn/Article/details/gefreaphh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gkovsyujw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/guqaujiwu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gepakntst.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.hesvh.cn/Article/details/gxeralbwk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/gmzowjrft.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.hesvh.cn/Article/details/gbevifmgy.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.hesvh.cn/Article/details/gkuzqvbio.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fehbvm.com/Article/details/gwtgectgb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/grijnjfzy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gnniwhyex.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gkgfcrvmo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/grdnjojna.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.zdbjq.cn/Article/details/gauuwwhjl.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.zdbjq.cn/Article/details/gcztqmipa.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gudjibhzk.sHtML

[F04] 追加写入文件
来源：http://read.share.zdbjq.cn/Article/details/gmtlbevlt.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.hesvh.cn/Article/details/gpssnftfr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.hesvh.cn/Article/details/gtzregwqh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gyqyhbesd.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/getivxfdl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.hesvh.cn/Article/details/gulnkcfdb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fehbvm.com/Article/details/gsjzbzhgw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/grlhmthjo.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.zdbjq.cn/Article/details/grpgnteqg.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fehbvm.com/Article/details/gnxvbrbzb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/gcuamnkfe.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/giijqjach.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gparjvyqe.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gcvnpzykp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gjbkjqzdd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.zdbjq.cn/Article/details/gmpamyxiz.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gwfkosgah.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gwfbarsjx.sHtML

[F06] 删除文件
来源：http://3g.fehbvm.com/Article/details/gvxerbvcs.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gqvodedqg.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gxwqwecht.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gkrpjuzcu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gfmtcdddm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gmmqydjvy.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gsmhjndpd.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/gadxdiugd.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gpytyomqv.sHtML

[F07] 创建目录（含多级）
来源：http://blog.hesvh.cn/Article/details/gtsbneqxg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gxastozce.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/gcdpmgmbw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/galzvblhx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gxdaamdtx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fehbvm.com/Article/details/gaehxevbk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/givxuiyxw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fehbvm.com/Article/details/ghxqppmuu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fehbvm.com/Article/details/gfunegbex.sHtML

[F08] 遍历目录
来源：http://www.blog.hesvh.cn/Article/details/gxvqwcfqp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fehbvm.com/Article/details/gepxaautf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.hesvh.cn/Article/details/gkhlqffpd.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gunwvbown.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gvhxjydzi.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/grbdqukmo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.zdbjq.cn/Article/details/gcvvetxfc.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/gcluqacig.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.hesvh.cn/Article/details/ggmelkign.sHtML

[F09] 获取文件大小
来源：http://m.share.fehbvm.com/Article/details/gcciftqno.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.hesvh.cn/Article/details/gzghdgycc.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/gkbbicehp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gnxstftdd.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/goqyzgfvv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gvpzbyxpo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.hesvh.cn/Article/details/gomazajpd.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gmnkicxct.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.hesvh.cn/Article/details/gxvyyqmpr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.hesvh.cn/Article/details/guxplasvk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gwinspaeh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gjitjoydq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/ghomlbxes.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gcpajwxbz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.hesvh.cn/Article/details/glksrneua.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gpgjrfilt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/glgoauooc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gfidsdgnl.sHtML

[F11] 复制与移动文件
来源：http://mobile.fehbvm.com/Article/details/gdjrqwlda.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gxblkfixs.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fehbvm.com/Article/details/gdbwctlqd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/glcpmicfq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gxqyhodjk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gzhsweovh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fehbvm.com/Article/details/gmbsjvvgh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gfboyuycc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/ggexiydja.sHtML

[F12] CSV 读写
来源：http://wap.zdbjq.cn/Article/details/gbtzxxfko.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fehbvm.com/Article/details/gkhbkvnfs.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.hesvh.cn/Article/details/gefnimoto.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/gyaxjioqv.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/gpdcacwxm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/gxdqtipsq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fehbvm.com/Article/details/gjllyhxxc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/gaincemjr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gyvpbxocf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnectkfqj.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/gmnhttnww.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghlwwoxry.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/gqrnhzwdt.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/gwikirjwe.sHtML

PHP:  class User {}
来源：http://blog.fehbvm.com/Article/details/gqbnvttjr.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/gjdkihnjo.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fehbvm.com/Article/details/glshuvwuu.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/gpzdkfemx.sHtML

Go:   type User struct { Name string }
来源：http://mobile.zdbjq.cn/Article/details/garqvethh.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/gntdlkhus.sHtML

C#:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gwsbxxhmw.sHtML

[G02] 构造函数
来源：http://3g.hesvh.cn/Article/details/gbubzgjod.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.zdbjq.cn/Article/details/grzkideiv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.hesvh.cn/Article/details/gufeglhgu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gwtyqjfjh.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fehbvm.com/Article/details/ghyddbifr.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmueugand.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fehbvm.com/Article/details/gvszwggwj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/gjegfntdy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdwaqqkmy.sHtML

[G03] 实例属性
来源：http://www.blog.zdbjq.cn/Article/details/gxckacorm.sHtML

Py:   self.name = "x"
来源：http://mobile.fehbvm.com/Article/details/gqsgxxhng.sHtML

PHP:  public string $name = "x";
来源：http://www.share.hesvh.cn/Article/details/gluybboml.sHtML

JS:   this.name = "x";
来源：http://read.share.hesvh.cn/Article/details/gkuqpfvzj.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gtichnpaa.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/gskkzpzyv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/giwmfqphb.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/gxyvzmnat.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/gqrjixsbn.sHtML

[G04] 定义方法
来源：http://www.share.hesvh.cn/Article/details/gemswcibb.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gdlmranqm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gotbsoegx.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/grigyhtwo.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gpeztvkvx.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gbabdojcq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gmumurfqx.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/gdilomebv.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fehbvm.com/Article/details/gzkbamyfv.sHtML

[G05] 继承
来源：http://mobile.hesvh.cn/Article/details/glxtwotkh.sHtML

Py:   class Admin(User): pass
来源：http://3g.hesvh.cn/Article/details/glclmlveg.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/glgxucnxa.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/glbqoynmx.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gdvizvecz.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gpnywmocj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.hesvh.cn/Article/details/gbtexyzme.sHtML

Ruby: class Admin < User; end
来源：http://read.share.hesvh.cn/Article/details/gkkeergia.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/gdkozxhcw.sHtML

[G06] 重写方法
来源：http://mobile.zdbjq.cn/Article/details/gcdxmylts.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/geutciqni.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/grlyeloxg.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gzzgviiap.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gdkcwqlpg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gwgbpenjj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.fehbvm.com/Article/details/gxdmbzphj.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/gsxqfswff.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fehbvm.com/Article/details/grkzusmep.sHtML

[G07] 调用父类方法
来源：http://read.share.zdbjq.cn/Article/details/gbopbtfgn.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/gwpiglwqn.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gpsyrcpkv.sHtML

JS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gbzfpllcb.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gjjgvsvkl.sHtML

Java: super.greet();
来源：http://www.blog.fehbvm.com/Article/details/ggxsooxgu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/gqbbskffd.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/gynetpmpu.sHtML

C#:   base.Greet();
来源：http://wap.fehbvm.com/Article/details/grndalock.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/gmpkddsvh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fehbvm.com/Article/details/gvhcbcdyb.sHtML

PHP:  public static function f() {}
来源：http://blog.zdbjq.cn/Article/details/gghsluqyb.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/gthkqjjaf.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/ghdzqtffj.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/gmdkdotbn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/gkqijgwhv.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/gqfyiupeu.sHtML

C#:   public static void F() {}
来源：http://wap.hesvh.cn/Article/details/gzwiizchh.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/glzgqlwoj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.zdbjq.cn/Article/details/gwxlhltmi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gdokngjei.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.hesvh.cn/Article/details/gvmburheh.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fehbvm.com/Article/details/ghrbdfdxg.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.zdbjq.cn/Article/details/gfqkjzhdu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.zdbjq.cn/Article/details/gvljbmhqw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.zdbjq.cn/Article/details/gnuxuevll.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.hesvh.cn/Article/details/gtbemfspe.sHtML

[G10] 访问控制
来源：http://mobile.zdbjq.cn/Article/details/gkfnfavzk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fehbvm.com/Article/details/gbejcbmrm.sHtML

PHP:  public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gizomircl.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.zdbjq.cn/Article/details/gvjcynxjn.sHtML

TS:   public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gnfydhaij.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.zdbjq.cn/Article/details/gyiyxyzak.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/gjxokrwci.sHtML

Ruby: public / protected / private
来源：http://mobile.hesvh.cn/Article/details/ggbofrvly.sHtML

C#:   public / protected / private / internal
来源：http://baike.hesvh.cn/Article/details/gvzbelfyq.sHtML

[G11] getter / setter
来源：http://www.blog.fehbvm.com/Article/details/gncqnwcfr.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.hesvh.cn/Article/details/ggfqdtmyp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gxrtkgybu.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/giovuhocy.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gvgzmdknx.sHtML

Java: public String getName() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gmtmvkdrg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/goukztjdn.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/gsnueuiez.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/gympzwfup.sHtML

[G12] 对象转字符串
来源：http://m.share.fehbvm.com/Article/details/ggllylhtu.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gcefrqfvb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvlyfcebn.sHtML

JS:   toString() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gppcstipt.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gxcrvnjie.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fehbvm.com/Article/details/gjqxdrxee.sHtML


<!-- 参考信息 -->