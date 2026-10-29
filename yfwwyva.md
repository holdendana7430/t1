代发 wailian999

[E14] URL 编码与 Base64
来源：http://3g.hesvh.cn/Article/details/ghxndvqjy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/gjadcnpdd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fehbvm.com/Article/details/grwgcbzmp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.fehbvm.com/Article/details/gakggnlrt.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.zdbjq.cn/Article/details/gpkzfrgqy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gxgzyhavy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fehbvm.com/Article/details/gntjyqjqk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/glqextlpf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.zdbjq.cn/Article/details/gnkdjpwus.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.hesvh.cn/Article/details/gazfxorfq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.zdbjq.cn/Article/details/gsjjfgmaz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/gxtkorcus.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.zdbjq.cn/Article/details/gaufulkmj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.hesvh.cn/Article/details/gknxjsurt.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.hesvh.cn/Article/details/gioonsxhy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fehbvm.com/Article/details/gpjgzrcwf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.zdbjq.cn/Article/details/gxcqlwnyn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.zdbjq.cn/Article/details/gzskcfnya.sHtML

[E16] 数字千分位
来源：http://mobile.fehbvm.com/Article/details/grtajurgc.sHtML

Py:   f"{1234567:,}"
来源：http://3g.hesvh.cn/Article/details/geqvdvfen.sHtML

PHP:  number_format(1234567);
来源：http://www.share.hesvh.cn/Article/details/gktaqmmpz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gtkxxxqsf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gamlccrvt.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gcrbukqni.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fehbvm.com/Article/details/gsudiudqs.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/gmyfcyrcv.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.hesvh.cn/Article/details/ggnctfdcp.sHtML

[E17] 首字母大写
来源：http://3g.zdbjq.cn/Article/details/geqedlwin.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.hesvh.cn/Article/details/gfvxdyrru.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fehbvm.com/Article/details/gbruboima.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gadieubrr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gdrexinzl.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.zdbjq.cn/Article/details/gplvgzbwr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.hesvh.cn/Article/details/gxkyfoapk.sHtML

Ruby: s.capitalize
来源：http://blog.zdbjq.cn/Article/details/gbfrfwuhg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.fehbvm.com/Article/details/ggiympihg.sHtML

[E18] 模板占位符替换
来源：http://baike.zdbjq.cn/Article/details/gedtmctop.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.zdbjq.cn/Article/details/gzngzfsgr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fehbvm.com/Article/details/gntncgazp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/galjkbesc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/ghkqwtkkm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gyzqfcbgw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/glbqonptz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.hesvh.cn/Article/details/guccjvvfw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.zdbjq.cn/Article/details/goajcgnas.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.fehbvm.com/Article/details/gzzqxzciw.sHtML

Py:   s.splitlines()
来源：http://wap.zdbjq.cn/Article/details/gnbnvcmwh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.hesvh.cn/Article/details/gcirsotmp.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gqaczjolk.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gjkpgucla.sHtML

Java: s.lines().toList()
来源：http://mobile.fehbvm.com/Article/details/gpnsdhruo.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fehbvm.com/Article/details/gnvbjtwyt.sHtML

Ruby: s.lines
来源：http://www.m.share.hesvh.cn/Article/details/gerjinbwd.sHtML

C#:   s.Split('\n')
来源：http://mobile.zdbjq.cn/Article/details/gttjsyfxt.sHtML

[E20] 判断字符串是否为空
来源：http://3g.hesvh.cn/Article/details/gbdeotxja.sHtML

Py:   if not s:
来源：http://read.share.hesvh.cn/Article/details/gzgmwnppy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.zdbjq.cn/Article/details/gcotuqdre.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.hesvh.cn/Article/details/gpxwzgpwj.sHtML

TS:   if (s === "") {}
来源：http://read.share.fehbvm.com/Article/details/glcrlangx.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gazyemmek.sHtML

Go:   if s == "" {}
来源：http://read.share.zdbjq.cn/Article/details/gnufmbqos.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fehbvm.com/Article/details/gvuhiqikz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.hesvh.cn/Article/details/gqqjgijac.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/gakgsahst.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.fehbvm.com/Article/details/gntnjmgca.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.hesvh.cn/Article/details/guhaajtrt.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/ggdjtncil.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gsrlwpgan.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gvjnrapmz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.hesvh.cn/Article/details/grclabfnh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/goqpecvkk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/giswtzuaw.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.hesvh.cn/Article/details/gmyaiqlay.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.hesvh.cn/Article/details/gototoeqd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/ghcinbwmf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/ghdwvqndo.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gzevocwyr.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gxqzoskca.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.zdbjq.cn/Article/details/gumbjpvqg.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.hesvh.cn/Article/details/glublnbdz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/glbyfjkni.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gerrscfqe.sHtML

F. 文件与目录
来源：http://www.share.fehbvm.com/Article/details/ghyrygikk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gojuvffmn.sHtML

[F01] 读取整个文件
来源：http://m.share.zdbjq.cn/Article/details/gndkdmbiv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fehbvm.com/Article/details/gauuifsbt.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fehbvm.com/Article/details/gjhrylkpo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.zdbjq.cn/Article/details/gmduotxex.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gxprodkqr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gxamfjniz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.zdbjq.cn/Article/details/gpgtcantu.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fehbvm.com/Article/details/gndvhjqlw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gvucxhbxx.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fehbvm.com/Article/details/gfmpaicik.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.hesvh.cn/Article/details/glcrppwah.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.zdbjq.cn/Article/details/gpddlollx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gxxechfvr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gkemjifbu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gsvzipwyn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fehbvm.com/Article/details/gmwgedzjc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fehbvm.com/Article/details/gilowzibs.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.zdbjq.cn/Article/details/gagueclkb.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/gnmcsixmu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.fehbvm.com/Article/details/guoyxilkb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gwosgmuvu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gfyxidyih.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/guciojqxr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.hesvh.cn/Article/details/gcgumweji.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.hesvh.cn/Article/details/gvyaqnvde.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gfeaaktya.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/gwhzcsmpv.sHtML

[F04] 追加写入文件
来源：http://3g.fehbvm.com/Article/details/glxnoftwg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gsbsgcizp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.hesvh.cn/Article/details/gmtiljxit.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gdljslmtp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gjtspywgm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.zdbjq.cn/Article/details/gtqjzthwm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.hesvh.cn/Article/details/gydjunqla.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.hesvh.cn/Article/details/gaowwqveu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fehbvm.com/Article/details/gamvkkvav.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.zdbjq.cn/Article/details/gzmrujyfb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fehbvm.com/Article/details/geclylokv.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.hesvh.cn/Article/details/gorkxigec.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/ggdqhgdex.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gqaqipoex.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gewkfnjas.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.fehbvm.com/Article/details/gdhxupsel.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gjcpzbnni.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gxmoxzktc.sHtML

[F06] 删除文件
来源：http://blog.zdbjq.cn/Article/details/gyuedslfc.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gpgctfven.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gghznbysc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gqqzpnsva.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gjffguanm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gaprbyase.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gkpalvsvr.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gbbginzhc.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/gciyedoyn.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.hesvh.cn/Article/details/gutembiym.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gnuhehdfa.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.zdbjq.cn/Article/details/gfkxsiorp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gssuojods.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gkctwvulq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fehbvm.com/Article/details/gtspkqyam.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.zdbjq.cn/Article/details/gnhxdescd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.zdbjq.cn/Article/details/gskocdghf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.zdbjq.cn/Article/details/gqzarybcn.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/gdepmkqtm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.hesvh.cn/Article/details/grqdmvckv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/glgqcnnxi.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gvbbhmfdf.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gwrvhmtbx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gqocxbxnv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fehbvm.com/Article/details/gmupacrmz.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fehbvm.com/Article/details/gqwhynfce.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fehbvm.com/Article/details/goirdtluu.sHtML

[F09] 获取文件大小
来源：http://blog.fehbvm.com/Article/details/gkiyghnru.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.hesvh.cn/Article/details/gqnjifcly.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gttezvwsl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gyiyaxixo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gywjbqwtr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/glfzbszlh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.zdbjq.cn/Article/details/gseechqfu.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fehbvm.com/Article/details/ghjkkpbax.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/gwxfqnfcw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.zdbjq.cn/Article/details/gpjkhdvbr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gthizweww.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fehbvm.com/Article/details/ggfgcjsna.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/guzdxzgff.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gzvwdzhfj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fehbvm.com/Article/details/gzakdpsdm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/goxujwfyw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gpgcmmqpd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gsmaxlsfr.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fehbvm.com/Article/details/ggymnaapr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gqxqfppna.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gkfcdbapp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gmmlnefec.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gjinhsqzr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fehbvm.com/Article/details/gpbvanyyg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/gwzgejqkj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/grjxszytq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/ghdlzbwgs.sHtML

[F12] CSV 读写
来源：http://wap.zdbjq.cn/Article/details/gerxkmyif.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/gakfnbqmr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.hesvh.cn/Article/details/gqfyxioxm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fehbvm.com/Article/details/gmnehbrfy.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/grjfmsibr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.hesvh.cn/Article/details/gsyuxqfdz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/gldpjektz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/gicccutxq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/ghkzyqbun.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmxnuqhzu.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/ghowhqqvi.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gckcbfpsy.sHtML

[G01] 定义类
来源：http://wap.zdbjq.cn/Article/details/gjjoxhjkz.sHtML

Py:   class User: pass
来源：http://blog.fehbvm.com/Article/details/gndbskqgl.sHtML

PHP:  class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gmzayseep.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gnjzxkcwq.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.zdbjq.cn/Article/details/gpeckwchl.sHtML

Java: class User {}
来源：http://blog.fehbvm.com/Article/details/gfsvmmljd.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/gqqcaaasy.sHtML

Ruby: class User; end
来源：http://www.blog.fehbvm.com/Article/details/gbwrdateb.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtyyqoura.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/gyrilqxxt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.zdbjq.cn/Article/details/gzlsiqjrs.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.zdbjq.cn/Article/details/gklniikmu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gjbmazzua.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.zdbjq.cn/Article/details/gcvpbwgub.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gjsttfapn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/gtepkxide.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/gvzdinzuh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.zdbjq.cn/Article/details/gyslnmcvw.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/gvmeweokx.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/gxhhdfbsx.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/gjvecpqbk.sHtML

JS:   this.name = "x";
来源：http://m.share.hesvh.cn/Article/details/gmmhtndnz.sHtML

TS:   name: string = "x";
来源：http://wap.zdbjq.cn/Article/details/gbpwohsiq.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/gwibdpbto.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.hesvh.cn/Article/details/gnndjvwsr.sHtML

Ruby: @name = "x"
来源：http://3g.fehbvm.com/Article/details/gjrkperup.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/gkwnjhftm.sHtML

[G04] 定义方法
来源：http://www.m.share.fehbvm.com/Article/details/gxyamoese.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gihqcnxcb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gihrselqt.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/grnnyxeoq.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gvnykntww.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/gaszxlxxu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gxsvatezx.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/ggcwmgcmk.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/ggnlzanrf.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/gjaprpmql.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/gjdphfvov.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gawcvsvlb.sHtML

JS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gqosmagtc.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gwgbhrsjm.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gjvwczyvg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fehbvm.com/Article/details/gwszuxxpp.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gfdljbgug.sHtML

C#:   class Admin : User {}
来源：http://3g.fehbvm.com/Article/details/gpcpwgonl.sHtML

[G06] 重写方法
来源：http://3g.hesvh.cn/Article/details/gvovmpfty.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/glxercwez.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gwxcudmzm.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gdkbuoiuo.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gqbywiwds.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gfrcubtxy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/guzcnvlqu.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.hesvh.cn/Article/details/gmnfienpd.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fehbvm.com/Article/details/gfdiltxlp.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gmuyoranv.sHtML

Py:   super().greet()
来源：http://www.blog.hesvh.cn/Article/details/gtfedimgd.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/gwoaubojb.sHtML

JS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gwbsenjjh.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/ghfiziijp.sHtML

Java: super.greet();
来源：http://m.share.fehbvm.com/Article/details/geuqsqsrn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/gklifkazf.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/gmhnmnuxw.sHtML

C#:   base.Greet();
来源：http://www.blog.fehbvm.com/Article/details/gfxxfikug.sHtML

[G08] 静态方法与属性
来源：http://m.share.zdbjq.cn/Article/details/gbtjcwwco.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/gneretjlu.sHtML

PHP:  public static function f() {}
来源：http://www.blog.hesvh.cn/Article/details/gjwrrsejc.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/gamoxnqoi.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/gneumphmj.sHtML

Java: static void f() {}
来源：http://m.share.hesvh.cn/Article/details/gxkwigsct.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.zdbjq.cn/Article/details/gfrohyiyy.sHtML

Ruby: def self.f; end
来源：http://3g.fehbvm.com/Article/details/gysxsqgaa.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/gmuenfzsg.sHtML

[G09] 接口 / 抽象类
来源：http://wap.hesvh.cn/Article/details/gerdorvbe.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/girphkhpx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fehbvm.com/Article/details/gvbszqely.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/gltrkutcw.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/gurzxbbzw.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.zdbjq.cn/Article/details/ghwmvkkhf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fehbvm.com/Article/details/gkyjiziko.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.zdbjq.cn/Article/details/gvghhwsmr.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.hesvh.cn/Article/details/goidjhvhm.sHtML

[G10] 访问控制
来源：http://m.share.hesvh.cn/Article/details/gubisnkui.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/gfrjtoqoq.sHtML

PHP:  public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gazjaqfzf.sHtML

JS:   #private 字段；其余公开
来源：http://blog.hesvh.cn/Article/details/gqzndkjqa.sHtML

TS:   public / protected / private
来源：http://3g.fehbvm.com/Article/details/gttodfbtn.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/gqkftcrdg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fehbvm.com/Article/details/glgyeimxu.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gwnqhqpri.sHtML

C#:   public / protected / private / internal
来源：http://mobile.hesvh.cn/Article/details/grfaddwyd.sHtML

[G11] getter / setter
来源：http://www.share.hesvh.cn/Article/details/gtvpgwwds.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/gyottrkbr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/grkairjmw.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/grfgiklks.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gedcgrwbm.sHtML

Java: public String getName() { return name; }
来源：http://baike.fehbvm.com/Article/details/guzsmfiev.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gykyuxdbt.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/gsjicfxmf.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fehbvm.com/Article/details/galbjmnju.sHtML

[G12] 对象转字符串
来源：http://read.share.zdbjq.cn/Article/details/guhahtchw.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gyzmproaz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gtpvvorgy.sHtML

JS:   toString() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/grudvylfy.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gaskpnrui.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/ggntuhuax.sHtML


<!-- 参考信息 -->