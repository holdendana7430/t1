代发 wailian999

Py:   for ch in s: print(ch)
来源：http://wap.zdbjq.cn/Article/details/gbdmqtrxc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.hesvh.cn/Article/details/gsgcxpwko.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gvmrcjjtj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/goisvclav.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gpwuimgkv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.hesvh.cn/Article/details/gbkojtspx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.zdbjq.cn/Article/details/grglkecsd.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/geqchfytb.sHtML

[E14] URL 编码与 Base64
来源：http://3g.zdbjq.cn/Article/details/guagapxoy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.hesvh.cn/Article/details/grjfxhknh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.hesvh.cn/Article/details/gxutniaru.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.hesvh.cn/Article/details/gluwrhvwi.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/gsxgtwmwj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.hesvh.cn/Article/details/gshwjdasz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.hesvh.cn/Article/details/gsrantvsn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.zdbjq.cn/Article/details/gnlirrxit.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.hesvh.cn/Article/details/grxjylrhx.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/gttjxrwgi.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fehbvm.com/Article/details/gcrnmsnva.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.fehbvm.com/Article/details/gapcctdpy.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.zdbjq.cn/Article/details/gpbkqclqa.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fehbvm.com/Article/details/gevutdema.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fehbvm.com/Article/details/gfylrfrkv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.zdbjq.cn/Article/details/gxqevnbzs.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fehbvm.com/Article/details/gdewnfspb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.zdbjq.cn/Article/details/gcyfeafsl.sHtML

[E16] 数字千分位
来源：http://blog.fehbvm.com/Article/details/gfurpuqqs.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.hesvh.cn/Article/details/ghomqzmsg.sHtML

PHP:  number_format(1234567);
来源：http://m.share.hesvh.cn/Article/details/gxsgmuhny.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gwyvvscfk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gxwgtkhxo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fehbvm.com/Article/details/gmntxzsgl.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/gnvdaxfnl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fehbvm.com/Article/details/gcdznobtc.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.hesvh.cn/Article/details/gzwkoisbf.sHtML

[E17] 首字母大写
来源：http://wap.hesvh.cn/Article/details/grarxljez.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.zdbjq.cn/Article/details/gakrjabcl.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fehbvm.com/Article/details/gegkkhibq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/gsitqhrgg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gtijmlxac.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.zdbjq.cn/Article/details/ghtxzwvdu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fehbvm.com/Article/details/ggckevree.sHtML

Ruby: s.capitalize
来源：http://mobile.fehbvm.com/Article/details/gqeiuwwjk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.hesvh.cn/Article/details/gmresbpck.sHtML

[E18] 模板占位符替换
来源：http://baike.zdbjq.cn/Article/details/gcypalynj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.fehbvm.com/Article/details/ghplgfmpy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.hesvh.cn/Article/details/gdrwkjeui.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gjuujolvh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gmjngwjlh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gayazekjv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/guiepcyyp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.hesvh.cn/Article/details/gzqaiefaw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.zdbjq.cn/Article/details/gncwmesed.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/gopkbygbi.sHtML

Py:   s.splitlines()
来源：http://www.m.share.hesvh.cn/Article/details/gkijabqys.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fehbvm.com/Article/details/gvgpaamux.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gabkgzbli.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gyqrudzvu.sHtML

Java: s.lines().toList()
来源：http://blog.hesvh.cn/Article/details/gegftejdy.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fehbvm.com/Article/details/grlfaehqt.sHtML

Ruby: s.lines
来源：http://www.blog.fehbvm.com/Article/details/guxhqamog.sHtML

C#:   s.Split('\n')
来源：http://www.share.fehbvm.com/Article/details/gjwrnxytz.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.hesvh.cn/Article/details/guunfpnef.sHtML

Py:   if not s:
来源：http://wap.fehbvm.com/Article/details/guelgeyil.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.hesvh.cn/Article/details/gkhgozwyh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fehbvm.com/Article/details/gvxiprfjo.sHtML

TS:   if (s === "") {}
来源：http://baike.fehbvm.com/Article/details/gizmxsjqr.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gfpwpucmi.sHtML

Go:   if s == "" {}
来源：http://read.share.fehbvm.com/Article/details/gzglzqhuj.sHtML

Ruby: if s.empty?
来源：http://3g.hesvh.cn/Article/details/gqrceypwq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gliyatbbu.sHtML

[E21] 超长截断加省略号
来源：http://m.share.zdbjq.cn/Article/details/guguzsvsw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/gclvzgiif.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gwbqaveft.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gnpdxfhqe.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gdlutieil.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/grpjvahyz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fehbvm.com/Article/details/ghcvozfoy.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gzznwkfle.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/ggjhqvghz.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.hesvh.cn/Article/details/gptqedgoa.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.zdbjq.cn/Article/details/gugxmqhsr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/giygluddw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gfkbizorh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gtbzdxeyn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gxycxdyos.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fehbvm.com/Article/details/gikyznjdk.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gzupeibie.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.zdbjq.cn/Article/details/grftfwxqp.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpnnmjbcy.sHtML

F. 文件与目录
来源：http://www.blog.hesvh.cn/Article/details/gpxkhjkta.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqkskkkoh.sHtML

[F01] 读取整个文件
来源：http://wap.zdbjq.cn/Article/details/glawfjjri.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.zdbjq.cn/Article/details/gzkjpmulr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gzheexyeh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.hesvh.cn/Article/details/gabrcbdui.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.zdbjq.cn/Article/details/glmirooaw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gdyturdvc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.hesvh.cn/Article/details/gnjvwesky.sHtML

Ruby: File.read("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gxzsqsipe.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gtwvptnir.sHtML

[F02] 逐行读取文件
来源：http://read.share.zdbjq.cn/Article/details/gjfpzaqgi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.hesvh.cn/Article/details/gwzpzdfus.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fehbvm.com/Article/details/gqbcirtgj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gpknwgxkg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gdogehnwc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/ghelzzuax.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.zdbjq.cn/Article/details/gladeewuf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.zdbjq.cn/Article/details/gvvsncter.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.hesvh.cn/Article/details/gspsjjerf.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.zdbjq.cn/Article/details/gamjhaxbs.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.hesvh.cn/Article/details/gkxrlwcjr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gmuyzkdvt.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gngevoltr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/guutbvarp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/gamxyytnd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.hesvh.cn/Article/details/gwnlwvrxf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gficusklr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gegiocxbq.sHtML

[F04] 追加写入文件
来源：http://read.share.zdbjq.cn/Article/details/gsfodklgv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.hesvh.cn/Article/details/galawcddk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fehbvm.com/Article/details/gdtvunrhe.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gblyrahsz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/ghbgzkdgc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.zdbjq.cn/Article/details/gfxbmnzqv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.hesvh.cn/Article/details/gbnrdsdad.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.zdbjq.cn/Article/details/gkxeqcetg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/gnhchefxb.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.hesvh.cn/Article/details/gurvfjwuv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fehbvm.com/Article/details/gzmxvntoe.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gjulxnari.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gtrxyftkp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gdsbnkpba.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gdszcnjuo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.zdbjq.cn/Article/details/grlbvfdxc.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gsrjrcyit.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gotvwiswe.sHtML

[F06] 删除文件
来源：http://blog.zdbjq.cn/Article/details/gfmkpbynj.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gpheactxv.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gyaenrydz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/glxjprili.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gkiquarfz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gtjkplogp.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gvnvfblfu.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gonwwxuhy.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gcdajdupb.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fehbvm.com/Article/details/gjfdamfau.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/geavjtxmx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gbpzkmrve.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gypfqtwoz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gydydmoqr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fehbvm.com/Article/details/gmcedslye.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/gfoioohby.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/gkpsvrweq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.hesvh.cn/Article/details/govtunbyc.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/gcjglgxkd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.hesvh.cn/Article/details/grogeoymm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/gcwanukkc.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gdrjkkmqi.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gqmppvwgh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gwfsdgdxw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fehbvm.com/Article/details/gihtqghfv.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.hesvh.cn/Article/details/gnzqzdlqo.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.hesvh.cn/Article/details/gczxqgvpd.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/gxwprlxcs.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fehbvm.com/Article/details/giqftiimd.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gqndlbowr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/glpqdyurc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/geqgxtgab.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gjrldqozs.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fehbvm.com/Article/details/gjagxzpyv.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gwqzsivme.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.hesvh.cn/Article/details/gbsgjxqvs.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/gbsakzqum.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gmuygyiar.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fehbvm.com/Article/details/gdriojobk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gpikyacax.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gifuvgpss.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/gxgywqcyn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gxfstvyuw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gbpxzuyni.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gqlygtrze.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/gznfvzzgi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/ghhvqrioi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.zdbjq.cn/Article/details/gfdbihwwd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/geiunhdgs.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gwrmwlzwk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fehbvm.com/Article/details/gwtvlkgib.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.zdbjq.cn/Article/details/gishbbgru.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/grsujmydr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.zdbjq.cn/Article/details/gqrjqjvim.sHtML

[F12] CSV 读写
来源：http://blog.hesvh.cn/Article/details/ghvwbznhu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/guquhhbpc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.zdbjq.cn/Article/details/gtkwgzfxv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.zdbjq.cn/Article/details/gzzekznea.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gtdjcarlq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.hesvh.cn/Article/details/gujysgpdd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gosuvmtba.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fehbvm.com/Article/details/gyvhcluld.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/gnyhjmgyz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gogssbeto.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/goczqdwvj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gyktzlkdm.sHtML

[G01] 定义类
来源：http://www.m.share.fehbvm.com/Article/details/gerhgqazi.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/gurygceqf.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/gixmwpauw.sHtML

JS:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gdqkksvrp.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/gfplqflng.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmbtuqffk.sHtML

Go:   type User struct { Name string }
来源：http://m.share.zdbjq.cn/Article/details/gfcrsfzlu.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/gvjskrrvl.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gnjevsjkw.sHtML

[G02] 构造函数
来源：http://blog.zdbjq.cn/Article/details/gofdjqbck.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.hesvh.cn/Article/details/gswygstdm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.zdbjq.cn/Article/details/gpmefqkvz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gswjlncsj.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.zdbjq.cn/Article/details/glvwafhif.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/ggifxnyfo.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fehbvm.com/Article/details/guarbhvfr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.hesvh.cn/Article/details/gplsrknqh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fehbvm.com/Article/details/gyokthqft.sHtML

[G03] 实例属性
来源：http://baike.hesvh.cn/Article/details/gkkrjxoar.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/gctapnohu.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/gfwrdhylb.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gfzfcflwi.sHtML

TS:   name: string = "x";
来源：http://mobile.zdbjq.cn/Article/details/ghiyjvopw.sHtML

Java: private String name;
来源：http://read.share.hesvh.cn/Article/details/gbwegtkxs.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/ghrykpmth.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/ghbfproda.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/gprksubiq.sHtML

[G04] 定义方法
来源：http://3g.zdbjq.cn/Article/details/gwemohhip.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gpwvnrppy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gtrikgqgo.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gmxkiyogh.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gsaqrfbmg.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjvnvvzbu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/groamjpdo.sHtML

Ruby: def greet; @name; end
来源：http://baike.fehbvm.com/Article/details/gwwwftobe.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/gwugsscqj.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gosrfhlnq.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/gzndmaaod.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gcaojlyag.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gaxxwrsgf.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gsvfhojwb.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gtixxmijr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.zdbjq.cn/Article/details/gzhgkgsra.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fehbvm.com/Article/details/gddqiflbt.sHtML

C#:   class Admin : User {}
来源：http://www.share.hesvh.cn/Article/details/gkggvqcma.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/gbmltqrib.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.hesvh.cn/Article/details/gyeeixczq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gozenolyp.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gejplokjv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/grpmpqrll.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gpzpboxkj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fehbvm.com/Article/details/gdlmkunji.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fehbvm.com/Article/details/gawwbnwtn.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/gbgkofsor.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/gprxmfluz.sHtML

Py:   super().greet()
来源：http://www.share.fehbvm.com/Article/details/gzcwfstom.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/gygeynidq.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/graeynlrh.sHtML

TS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gohcmtolf.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/gosutfjka.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/gpjpmchtj.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/gbbromulw.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/gtpebapuz.sHtML

[G08] 静态方法与属性
来源：http://3g.fehbvm.com/Article/details/gnpienazl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/gahhstbog.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/ggscxtkig.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/grzkqazsr.sHtML

TS:   static f(): void {}
来源：http://read.share.zdbjq.cn/Article/details/gnghfgpvw.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gngmyqchn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.hesvh.cn/Article/details/gckvgcjct.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/gvecjhdqi.sHtML

C#:   public static void F() {}
来源：http://3g.zdbjq.cn/Article/details/guvvrpuru.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/gkkaqasxm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.hesvh.cn/Article/details/gemaklclm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/guljcgiso.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fehbvm.com/Article/details/girqvrfgg.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/ghynkbfsz.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.hesvh.cn/Article/details/gtklkvmga.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fehbvm.com/Article/details/grgbwydnj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fehbvm.com/Article/details/gngureyev.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fehbvm.com/Article/details/gescprpdj.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/gwtyeklyp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fehbvm.com/Article/details/guwkqfeir.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gmgszdfii.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fehbvm.com/Article/details/gdezlijgk.sHtML

TS:   public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gxxiatxfj.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/gqyuymkld.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.hesvh.cn/Article/details/ghtooydwg.sHtML

Ruby: public / protected / private
来源：http://wap.zdbjq.cn/Article/details/girupjmbe.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/gyvrxyaiu.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/gvkqzrcqd.sHtML

Py:   @property 与 @x.setter
来源：http://wap.zdbjq.cn/Article/details/guullhpte.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gsessiyiw.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gblhwyhmf.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/goqvjbvma.sHtML

Java: public String getName() { return name; }
来源：http://3g.fehbvm.com/Article/details/grnvcxnrg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gnmzjopqr.sHtML


<!-- 参考信息 -->