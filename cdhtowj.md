代发 wailian999

[E14] URL 编码与 Base64
来源：http://baike.fehbvm.com/Article/details/gwubifbit.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.hesvh.cn/Article/details/gbckghowf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gdqnmgxtq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.zdbjq.cn/Article/details/ggbycotgx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fehbvm.com/Article/details/gewhbvshx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gazbeodfi.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fehbvm.com/Article/details/gqrotepau.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.zdbjq.cn/Article/details/gngrqkpir.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gyrdadomn.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.fehbvm.com/Article/details/gtvraqzgx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.hesvh.cn/Article/details/gzsavsexn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gdvyrcgpx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.hesvh.cn/Article/details/gxyahvlwa.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fehbvm.com/Article/details/gfduhigel.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.hesvh.cn/Article/details/gpcnyadtj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fehbvm.com/Article/details/ghdyafneb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.zdbjq.cn/Article/details/gzvbyspyn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.zdbjq.cn/Article/details/glcnbhwtc.sHtML

[E16] 数字千分位
来源：http://www.blog.hesvh.cn/Article/details/guwnveefp.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.hesvh.cn/Article/details/gjaegrqee.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fehbvm.com/Article/details/ggbmdxgwt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gujluxojx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gfnsmhkkt.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gbmsrkrjt.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fehbvm.com/Article/details/gxugkwtrn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.zdbjq.cn/Article/details/gnfhscgqj.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fehbvm.com/Article/details/gjekkksst.sHtML

[E17] 首字母大写
来源：http://mobile.zdbjq.cn/Article/details/gpnxxuntr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.zdbjq.cn/Article/details/ggimurthp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.hesvh.cn/Article/details/gqqprxpdi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gjqzfkyoc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gcrjawlco.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.fehbvm.com/Article/details/giuldbovk.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.zdbjq.cn/Article/details/ginlosopo.sHtML

Ruby: s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/gsxgtrqgq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fehbvm.com/Article/details/gdweouuqs.sHtML

[E18] 模板占位符替换
来源：http://blog.zdbjq.cn/Article/details/gvbzuswzl.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.hesvh.cn/Article/details/gzfjnnoko.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fehbvm.com/Article/details/gyzgweywu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gzkqfuetf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gfalvvkpy.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gzxorwzxs.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gozzeftym.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.zdbjq.cn/Article/details/gcbwqjxra.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.zdbjq.cn/Article/details/gkddcntez.sHtML

[E19] 多行文本按行拆分
来源：http://3g.zdbjq.cn/Article/details/gesmihgdz.sHtML

Py:   s.splitlines()
来源：http://www.share.hesvh.cn/Article/details/gchflyhac.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gewsaveyz.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/ghbupziyy.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/grvweonui.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/gdecvdwdo.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gmkjyjbzu.sHtML

Ruby: s.lines
来源：http://www.blog.hesvh.cn/Article/details/gorvagjzg.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/ggsubgsaq.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.zdbjq.cn/Article/details/gjrgwhnif.sHtML

Py:   if not s:
来源：http://baike.hesvh.cn/Article/details/gzwsqvhix.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/gfapemtap.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.hesvh.cn/Article/details/geqianbcv.sHtML

TS:   if (s === "") {}
来源：http://m.share.fehbvm.com/Article/details/gwhqbrniw.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/goqsgihvk.sHtML

Go:   if s == "" {}
来源：http://blog.hesvh.cn/Article/details/gsnmguzck.sHtML

Ruby: if s.empty?
来源：http://wap.hesvh.cn/Article/details/gtvsromjs.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fehbvm.com/Article/details/gsmmxnshw.sHtML

[E21] 超长截断加省略号
来源：http://3g.zdbjq.cn/Article/details/glavpcste.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fehbvm.com/Article/details/gimktcesi.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/ghvkaysxu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gsftetvta.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gaxogxztu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/ggykfdneh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.hesvh.cn/Article/details/ghzbzlaqi.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/ggzutgcrs.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gtfqyxlvt.sHtML

[E22] 字节长度与字符长度
来源：http://wap.hesvh.cn/Article/details/ghuelxkvq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fehbvm.com/Article/details/gccdlpebv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gcatxyfmg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gkxihzjcq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gudoadkbh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.zdbjq.cn/Article/details/gczniejdm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fehbvm.com/Article/details/gfwbejotw.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gwhmbonlj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/glzoecvvw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glcispgnu.sHtML

F. 文件与目录
来源：http://baike.fehbvm.com/Article/details/gvdzmmcvc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjsirvvxd.sHtML

[F01] 读取整个文件
来源：http://wap.fehbvm.com/Article/details/gnxlvzpfg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.hesvh.cn/Article/details/gjhupdhfi.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gumanpwjt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.zdbjq.cn/Article/details/gqkhlipec.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gfbvenbnk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gpkxhuauh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fehbvm.com/Article/details/gnkeehotb.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gmxvgtkia.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gmhuqptke.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.hesvh.cn/Article/details/ggkvzvggz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.zdbjq.cn/Article/details/gehhdstvu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fehbvm.com/Article/details/gzupqxqwa.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gaxlbqqrm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gaolnlqlc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gseozoxuh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.hesvh.cn/Article/details/gtdzsneik.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.zdbjq.cn/Article/details/gshfjfxvz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.hesvh.cn/Article/details/gpbhhomem.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/gfehaahcy.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gtjaaayuz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gculvqoql.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gpbnjtvgd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gbciwfanl.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.zdbjq.cn/Article/details/geqbsxgwt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fehbvm.com/Article/details/gtqaxncsz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.zdbjq.cn/Article/details/gswxattzb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gngbubzrk.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gkwnrbgkr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/glpgypnox.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.zdbjq.cn/Article/details/glftrqhux.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gezvgvyjd.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/getkdbbla.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.hesvh.cn/Article/details/gjbikhliz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gigobfvsz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/gwcjrcccq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.hesvh.cn/Article/details/glivvvaji.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.hesvh.cn/Article/details/gpezphvfs.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/gajjohxmf.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gvesutyps.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gciqgmqmz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gfaxrvhgk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gaouwdhai.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.hesvh.cn/Article/details/grwmbcllg.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gthgdnzpj.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gyohsnyqz.sHtML

[F06] 删除文件
来源：http://blog.fehbvm.com/Article/details/grhvcroua.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gfgknzgzk.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gmenqkdsf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gdmyfoalv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gbkpmlrxb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/grqyjsgze.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gdryghejd.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.hesvh.cn/Article/details/gcmmvsyzm.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gffggzosq.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.zdbjq.cn/Article/details/gukxxfuep.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/geaxnroyv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.zdbjq.cn/Article/details/gwutsfnfp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gnnpxydkd.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gyqbhnapv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.hesvh.cn/Article/details/gxsseyqsc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.hesvh.cn/Article/details/gbsfzdyjy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fehbvm.com/Article/details/gpredehzq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.zdbjq.cn/Article/details/gpilmujri.sHtML

[F08] 遍历目录
来源：http://baike.hesvh.cn/Article/details/gkrpcpiji.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fehbvm.com/Article/details/gdjzvhlkx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/gxirfksrv.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/ggkknbygq.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/geffguize.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/grabunkmj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/gvterszcf.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fehbvm.com/Article/details/gjdanattn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fehbvm.com/Article/details/ggpezbkki.sHtML

[F09] 获取文件大小
来源：http://www.m.share.hesvh.cn/Article/details/gusgxkhka.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gundsrxoo.sHtML

PHP:  filesize("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gpkcpnkqc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gdlqtjcgw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gimgbsunb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/ggbbvvyri.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.zdbjq.cn/Article/details/geacfrmvp.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fehbvm.com/Article/details/gerfeckhm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fehbvm.com/Article/details/gosxpmtda.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fehbvm.com/Article/details/gejssnpsi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gecaszjqv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/glolcnfzo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/glnqoqkbq.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fehbvm.com/Article/details/gtlreulpt.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.hesvh.cn/Article/details/gyurnxfva.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gfzekyipx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gfuzisqev.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gpkoxgxud.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/gqaeqzauw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gbdqaydfi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/gyzztvipn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gwuygtkcy.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gapcgdbkn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.zdbjq.cn/Article/details/ggxiennoy.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.hesvh.cn/Article/details/gqeyhqmpq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gvcobtcfl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.zdbjq.cn/Article/details/gdmqomoah.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gswqgcjfp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/gjcavtzcb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.zdbjq.cn/Article/details/gjispxiua.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/ggmvcnfna.sHtML

TS:   // 同上
来源：http://read.share.zdbjq.cn/Article/details/gwylcdcke.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.hesvh.cn/Article/details/gffkjdfrt.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/gygkjzcgo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.hesvh.cn/Article/details/ghonnowbe.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/gomafcoom.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gncwgdlrn.sHtML

G. 面向对象
来源：http://www.blog.zdbjq.cn/Article/details/gnracmzwh.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdcemphpa.sHtML

[G01] 定义类
来源：http://wap.hesvh.cn/Article/details/gdfpcbazx.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/gbtbmahqx.sHtML

PHP:  class User {}
来源：http://mobile.fehbvm.com/Article/details/gvtzmicys.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/glooogipu.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fehbvm.com/Article/details/gpaynremc.sHtML

Java: class User {}
来源：http://www.blog.hesvh.cn/Article/details/grotyupdj.sHtML

Go:   type User struct { Name string }
来源：http://mobile.hesvh.cn/Article/details/gtidjoykd.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/gwjpvwazv.sHtML

C#:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gavxzatpi.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/gnkwsplct.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.zdbjq.cn/Article/details/guvmvecjb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.hesvh.cn/Article/details/gywibjrgj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gmofddmdj.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/gxbgoheet.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gzmlwwavi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fehbvm.com/Article/details/gxiyrnodb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/ggjuaukfc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.zdbjq.cn/Article/details/gdkzaknae.sHtML

[G03] 实例属性
来源：http://mobile.fehbvm.com/Article/details/gyffkhwiy.sHtML

Py:   self.name = "x"
来源：http://read.share.zdbjq.cn/Article/details/grmneszxq.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/grzibafej.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gxuulhzwn.sHtML

TS:   name: string = "x";
来源：http://m.share.zdbjq.cn/Article/details/gvmcgggmx.sHtML

Java: private String name;
来源：http://read.share.hesvh.cn/Article/details/gvtrxusgt.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/gkyhtrezc.sHtML

Ruby: @name = "x"
来源：http://m.share.fehbvm.com/Article/details/ghzfxehtl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gtrpohbmy.sHtML

[G04] 定义方法
来源：http://www.share.zdbjq.cn/Article/details/gtavfujnd.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gvunchbbz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/ghydepcsy.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gloduxvdq.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/grvujlqhd.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gbsiwiraa.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gnmdkbqtq.sHtML

Ruby: def greet; @name; end
来源：http://blog.fehbvm.com/Article/details/giwntpbfa.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/gtjotxjcp.sHtML

[G05] 继承
来源：http://mobile.hesvh.cn/Article/details/gchdargnb.sHtML

Py:   class Admin(User): pass
来源：http://read.share.zdbjq.cn/Article/details/givughjfi.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gktjsjlgn.sHtML

JS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gpqpreixm.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gerowhlvf.sHtML

Java: class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gemeikaci.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/gpetmploh.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fehbvm.com/Article/details/gdfquunid.sHtML

C#:   class Admin : User {}
来源：http://blog.hesvh.cn/Article/details/ggqhnujbi.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/giqzcaxmk.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.hesvh.cn/Article/details/gfyfkmrmt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gcczihrav.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/glfccowxe.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/ghonxbegi.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gpasterab.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/gafscdbpg.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fehbvm.com/Article/details/gixywvjvh.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fehbvm.com/Article/details/gahjvkzne.sHtML

[G07] 调用父类方法
来源：http://read.share.hesvh.cn/Article/details/gpegscoht.sHtML

Py:   super().greet()
来源：http://wap.hesvh.cn/Article/details/ghcznzdeu.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/gbhygxfqr.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gthasfaxj.sHtML

TS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gaymziypf.sHtML

Java: super.greet();
来源：http://wap.hesvh.cn/Article/details/gppfchqls.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/glwjgsgxb.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/gzgfcinxu.sHtML

C#:   base.Greet();
来源：http://wap.hesvh.cn/Article/details/gdnvjhduo.sHtML

[G08] 静态方法与属性
来源：http://baike.fehbvm.com/Article/details/gkcjpjdfr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fehbvm.com/Article/details/gihdqppad.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/gcmlbkofd.sHtML

JS:   static f() {}
来源：http://m.share.zdbjq.cn/Article/details/gjkjutfzm.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/ggxreuwhp.sHtML

Java: static void f() {}
来源：http://m.share.zdbjq.cn/Article/details/gakjkllfw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.zdbjq.cn/Article/details/ghgnmerqz.sHtML

Ruby: def self.f; end
来源：http://3g.hesvh.cn/Article/details/grzztarry.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/gqxlcaycx.sHtML

[G09] 接口 / 抽象类
来源：http://3g.hesvh.cn/Article/details/gldlfyhze.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.hesvh.cn/Article/details/gxtuhzxxu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.hesvh.cn/Article/details/gktgcdkrk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/gtugmebsb.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fehbvm.com/Article/details/gmewrujbe.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.zdbjq.cn/Article/details/gcnwzwmvs.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/gdwaticzm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.zdbjq.cn/Article/details/gzmadqnyt.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.zdbjq.cn/Article/details/gukdzlqfn.sHtML

[G10] 访问控制
来源：http://wap.hesvh.cn/Article/details/gycdvbqyx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fehbvm.com/Article/details/gsazdhgxg.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gaimghove.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.zdbjq.cn/Article/details/gpulrzmml.sHtML

TS:   public / protected / private
来源：http://wap.fehbvm.com/Article/details/gedkwplup.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gmwrecbtq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.zdbjq.cn/Article/details/grbonxipo.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/grwktitrt.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fehbvm.com/Article/details/gxthxkcrj.sHtML

[G11] getter / setter
来源：http://www.m.share.zdbjq.cn/Article/details/guexugvhe.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/gwsxmvbbj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gskbyncuj.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gpswfdpgi.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/goznppdcd.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/geialdink.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gacsuvzkw.sHtML

Ruby: attr_accessor :name
来源：http://blog.hesvh.cn/Article/details/gymnmiexp.sHtML

C#:   public string Name { get; set; }
来源：http://wap.zdbjq.cn/Article/details/gzwvarqvj.sHtML

[G12] 对象转字符串
来源：http://mobile.zdbjq.cn/Article/details/gfajzhwqj.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gsqpsdcok.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/ghnmgpimh.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gitcnemjp.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gbnhkghil.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fehbvm.com/Article/details/gylhllyno.sHtML


<!-- 参考信息 -->