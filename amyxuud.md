代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.hesvh.cn/Article/details/giefkvrob.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.zdbjq.cn/Article/details/gqctasqwk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.zdbjq.cn/Article/details/giyjhzolx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.hesvh.cn/Article/details/gaoexnlvj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.hesvh.cn/Article/details/gxstzwagb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.zdbjq.cn/Article/details/gdkzcdapt.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.hesvh.cn/Article/details/gfubyfoio.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fehbvm.com/Article/details/ggpqwbaye.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gtdfzgqqz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fehbvm.com/Article/details/glneuiuzs.sHtML

[E16] 数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gobkngkgj.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.zdbjq.cn/Article/details/glstkhzyp.sHtML

PHP:  number_format(1234567);
来源：http://m.share.zdbjq.cn/Article/details/gogcboyhl.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gwkjjqslk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gwdajaujf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gizfogadp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.hesvh.cn/Article/details/gkeqtwfsb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/gxggisffg.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fehbvm.com/Article/details/gzmvgmnmn.sHtML

[E17] 首字母大写
来源：http://read.share.zdbjq.cn/Article/details/guetmulgy.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fehbvm.com/Article/details/gmxtlfesp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.zdbjq.cn/Article/details/gnxhearfk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gzjxggysa.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/ghbpwgabi.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.zdbjq.cn/Article/details/gjisxysik.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fehbvm.com/Article/details/gvqgiygvf.sHtML

Ruby: s.capitalize
来源：http://www.blog.zdbjq.cn/Article/details/gxgwjdupg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.hesvh.cn/Article/details/gwvznrgvd.sHtML

[E18] 模板占位符替换
来源：http://mobile.hesvh.cn/Article/details/gfpouvtpl.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.zdbjq.cn/Article/details/grxwswvmj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.zdbjq.cn/Article/details/gsarjzewt.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gvxvpgehf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gskgfafbc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gcznxyafc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fehbvm.com/Article/details/gksznfeky.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.zdbjq.cn/Article/details/geixgueww.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.fehbvm.com/Article/details/gkevgvtuq.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.zdbjq.cn/Article/details/gbrbiunes.sHtML

Py:   s.splitlines()
来源：http://m.share.fehbvm.com/Article/details/grazlziku.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.hesvh.cn/Article/details/ggpumrdoh.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gilnwtdvl.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gxokznwwe.sHtML

Java: s.lines().toList()
来源：http://baike.fehbvm.com/Article/details/gefhmalvc.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.fehbvm.com/Article/details/gyzorlksr.sHtML

Ruby: s.lines
来源：http://3g.zdbjq.cn/Article/details/grwlmygiy.sHtML

C#:   s.Split('\n')
来源：http://baike.zdbjq.cn/Article/details/gqnfslmce.sHtML

[E20] 判断字符串是否为空
来源：http://blog.fehbvm.com/Article/details/glaljikeq.sHtML

Py:   if not s:
来源：http://baike.hesvh.cn/Article/details/grtmfdyhz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fehbvm.com/Article/details/gqgzihtfs.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fehbvm.com/Article/details/ggdllplrv.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/ggjebejrx.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/guuhfwsky.sHtML

Go:   if s == "" {}
来源：http://www.share.hesvh.cn/Article/details/gklsacofg.sHtML

Ruby: if s.empty?
来源：http://www.blog.zdbjq.cn/Article/details/gzcfmmvdh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.hesvh.cn/Article/details/gdwmtlkyu.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.hesvh.cn/Article/details/gatjdwnfa.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/gknywmhqo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gwzofgnci.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gqwwurcde.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gqecrsisv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gjylcfwun.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.zdbjq.cn/Article/details/gmbgdnbuv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/ghioujirt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gqscbsdhh.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fehbvm.com/Article/details/gnkwmhbpo.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.hesvh.cn/Article/details/gvjpkdzwn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/ggcbiedmi.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gakuvvqtk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/ghuevwtjc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.zdbjq.cn/Article/details/gwqcdkkjo.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.hesvh.cn/Article/details/gqgznpbsp.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/ggneeifup.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/gnmivafnr.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grnmmaqfb.sHtML

F. 文件与目录
来源：http://wap.fehbvm.com/Article/details/gqliriyyg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gnqtxdgmy.sHtML

[F01] 读取整个文件
来源：http://www.blog.zdbjq.cn/Article/details/gohvmbynk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/glcatjzgz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gnzzpcpel.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.zdbjq.cn/Article/details/gsabxojoy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fehbvm.com/Article/details/gvszxxdyq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gooqzzcaf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.zdbjq.cn/Article/details/gjjnmkann.sHtML

Ruby: File.read("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gknzykosg.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.hesvh.cn/Article/details/glizlxfyp.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fehbvm.com/Article/details/gqeezdxbf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.zdbjq.cn/Article/details/grcnnaiiv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.hesvh.cn/Article/details/gdwdzhehr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gjpbuoeqq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gvumnmhir.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gmicpgaey.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.hesvh.cn/Article/details/gvsacmeqn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.zdbjq.cn/Article/details/gqujyqwrh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fehbvm.com/Article/details/gpxlwvupo.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/gswwfjlao.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.zdbjq.cn/Article/details/gzhyhemrx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gdvdjumts.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gokxealfn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gwkeijajp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fehbvm.com/Article/details/grxlaqdor.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.hesvh.cn/Article/details/gsrthrctk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.zdbjq.cn/Article/details/gwqsmfxrw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gehrssnwy.sHtML

[F04] 追加写入文件
来源：http://read.share.zdbjq.cn/Article/details/gyjcurnfi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.hesvh.cn/Article/details/gkkpunrxh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fehbvm.com/Article/details/gfibuxpve.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gqioqiduh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gypmgnlkw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.hesvh.cn/Article/details/gtdqsllzs.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gfkouhuqz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.hesvh.cn/Article/details/gtwjvmhll.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.hesvh.cn/Article/details/gzzvbimmz.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fehbvm.com/Article/details/gwtqlhbbe.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.zdbjq.cn/Article/details/gvqoljanm.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fehbvm.com/Article/details/guheamaqf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/grrqztmul.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gdxhajxpf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/grxljqxib.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fehbvm.com/Article/details/geboenphn.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gcuszpxia.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gdtihikwj.sHtML

[F06] 删除文件
来源：http://wap.zdbjq.cn/Article/details/gkwxyobdw.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gsapcevzx.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fehbvm.com/Article/details/gubrnqpan.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gzoldruit.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gniekuxhy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gpklcnciw.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/guyryacxf.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.zdbjq.cn/Article/details/ggxfjpyvl.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gjhpuxffq.sHtML

[F07] 创建目录（含多级）
来源：http://3g.hesvh.cn/Article/details/gkhbjurti.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gizjkeype.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fehbvm.com/Article/details/gwdxrnhar.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gtqauxxkn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gnetyntck.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.hesvh.cn/Article/details/gmzsredhw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fehbvm.com/Article/details/gxwgvcqbo.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.zdbjq.cn/Article/details/grkxpxhny.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fehbvm.com/Article/details/gqnssqzwh.sHtML

[F08] 遍历目录
来源：http://baike.hesvh.cn/Article/details/gfnhruybw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.zdbjq.cn/Article/details/gshkvgfhc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.zdbjq.cn/Article/details/gkejwwxar.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gxxibobrh.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/ghbqrlpap.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gwzjitrxp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.zdbjq.cn/Article/details/gzxvoqiju.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fehbvm.com/Article/details/gzutgkaid.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fehbvm.com/Article/details/gbevcdlrn.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/gsfaahogu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gzclnjcjq.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gxivlfwdn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gyytasxme.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gynussmil.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gibvbqdah.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/ghuhpaiph.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gxzahbxti.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.zdbjq.cn/Article/details/gdrjoaobh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/gbqhrzdvt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gvuhhrbkd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.hesvh.cn/Article/details/gyekorgyt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gydwmfpqr.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/giojxnwxk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/gzykgodpk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/glllhmuov.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gkelkeitn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gollcktop.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fehbvm.com/Article/details/gvyzkrubb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gmyiacqjm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.hesvh.cn/Article/details/gzyykkhnr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gedrvlnwo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gstsjnmnd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/galukmolu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.zdbjq.cn/Article/details/guluvnovj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gnlkqsdbl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.zdbjq.cn/Article/details/gvirptffl.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/gibmupkuf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/gnhkrifxl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/ggsdpkyem.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.zdbjq.cn/Article/details/grwfsztpx.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/grkneabpr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/gpvrvizof.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fehbvm.com/Article/details/gtnqeatmb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/gkpmpjefv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fehbvm.com/Article/details/grtmouscw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtaaxmzvf.sHtML

G. 面向对象
来源：http://3g.zdbjq.cn/Article/details/ggvgaarkx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvciwwemy.sHtML

[G01] 定义类
来源：http://blog.hesvh.cn/Article/details/gfnovjklg.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/ghtczherx.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/glxyfylsm.sHtML

JS:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gtxlwfsvl.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fehbvm.com/Article/details/gqfbewfwm.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/gpnwwjyyt.sHtML

Go:   type User struct { Name string }
来源：http://baike.fehbvm.com/Article/details/gqzyjeoth.sHtML

Ruby: class User; end
来源：http://wap.fehbvm.com/Article/details/gqbixnorr.sHtML

C#:   class User {}
来源：http://blog.hesvh.cn/Article/details/gkubazhqg.sHtML

[G02] 构造函数
来源：http://mobile.zdbjq.cn/Article/details/gkmmazkew.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fehbvm.com/Article/details/gjliqlune.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.hesvh.cn/Article/details/gpapbjvcc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gjppuphua.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gniatsupg.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gbxrwrhse.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.hesvh.cn/Article/details/gmvedbdwa.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fehbvm.com/Article/details/gytucgeco.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/gwxvigfsw.sHtML

[G03] 实例属性
来源：http://read.share.zdbjq.cn/Article/details/gpgudnvfx.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/gcapdbbwf.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gihpucepw.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gvlejbjfa.sHtML

TS:   name: string = "x";
来源：http://3g.zdbjq.cn/Article/details/gmqaytwtc.sHtML

Java: private String name;
来源：http://3g.zdbjq.cn/Article/details/gtgfaxhhq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/gsllzftgy.sHtML

Ruby: @name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gyulmmguq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/gqgdlghte.sHtML

[G04] 定义方法
来源：http://mobile.hesvh.cn/Article/details/gvpiiiasl.sHtML

Py:   def greet(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gqdhkfwhn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gcgpisabh.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gxrhhxjdx.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gapofsifm.sHtML

Java: String greet() { return name; }
来源：http://wap.fehbvm.com/Article/details/ggsrtnhnd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gdkudllmi.sHtML

Ruby: def greet; @name; end
来源：http://mobile.hesvh.cn/Article/details/gifagxmpi.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/gbnbexaeq.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/gznyxhewn.sHtML

Py:   class Admin(User): pass
来源：http://mobile.zdbjq.cn/Article/details/gvtiinmdu.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gddixyhne.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gffkijhcq.sHtML

TS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gtewagcvl.sHtML

Java: class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gigdveclx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/gseffvbgh.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/grpbnqbtu.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/gdiqizonf.sHtML

[G06] 重写方法
来源：http://3g.hesvh.cn/Article/details/gnvbjzggy.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/gtvdszyii.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gjgcvzxkm.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gqebwpnaf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gqasdvxht.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmepmzzra.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/gffexqyqg.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fehbvm.com/Article/details/gwhzgyyhj.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/gzojfhgev.sHtML

[G07] 调用父类方法
来源：http://wap.zdbjq.cn/Article/details/gucvrigan.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/glojnktfy.sHtML

PHP:  parent::greet();
来源：http://m.share.hesvh.cn/Article/details/gbgnjngee.sHtML

JS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gjfnnjumv.sHtML

TS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/ghukufxoe.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gmcyttedw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/gvmahcbsc.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/gmmrmqgwy.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/gbvtbblfd.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/geghjvuti.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.hesvh.cn/Article/details/gizunbmme.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/gdwkjafyx.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/gfvdpoyzb.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/gqtpaayrw.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gasfgjrlg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.zdbjq.cn/Article/details/gxlqxkjlk.sHtML

Ruby: def self.f; end
来源：http://3g.hesvh.cn/Article/details/gxkolopta.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/gyfldpcmm.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/gpjikqiuk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.hesvh.cn/Article/details/guinzofvn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fehbvm.com/Article/details/gbmzbkuwb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.zdbjq.cn/Article/details/guspxlggn.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/gnclfpsrb.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.zdbjq.cn/Article/details/gvzgnsslq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/gxgeynwyp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.fehbvm.com/Article/details/gceqlliro.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fehbvm.com/Article/details/gvfactjhc.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/gwigwqgxl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/gwuxzlhqi.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/gbcilgzbj.sHtML

JS:   #private 字段；其余公开
来源：http://baike.zdbjq.cn/Article/details/gdktzhpgo.sHtML

TS:   public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gsdkisqpq.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.hesvh.cn/Article/details/ghjunaukb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.zdbjq.cn/Article/details/gzehddmbi.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/ghakggjrr.sHtML

C#:   public / protected / private / internal
来源：http://wap.fehbvm.com/Article/details/giwawqzjz.sHtML

[G11] getter / setter
来源：http://3g.zdbjq.cn/Article/details/gpghoymug.sHtML

Py:   @property 与 @x.setter
来源：http://wap.hesvh.cn/Article/details/gudtjietn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gjngzvzaa.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gleoqgtzp.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gqoaenplk.sHtML

Java: public String getName() { return name; }
来源：http://blog.zdbjq.cn/Article/details/grcpucbas.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gtaactyde.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fehbvm.com/Article/details/gggspomuw.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/gdgwbxleu.sHtML

[G12] 对象转字符串
来源：http://read.share.fehbvm.com/Article/details/gxocyfiag.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gavfccmva.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gdglllezy.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gcmijvbrq.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gycmxlosm.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gpqofjpum.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gigfmazcr.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gmlfyxszg.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/gfvjvywkw.sHtML

[G13] 判断对象类型
来源：http://3g.fehbvm.com/Article/details/gfwinlbsx.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/giwcnoxhp.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gfvvogrlg.sHtML

JS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/goiydgqlb.sHtML

TS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/ghgrjliqq.sHtML


<!-- 参考信息 -->