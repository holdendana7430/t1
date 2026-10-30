代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gegxvwjii.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.zdbjq.cn/Article/details/gvxcybtjg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.hesvh.cn/Article/details/gqpfvoxbd.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fehbvm.com/Article/details/gxaiwyfqt.sHtML

[E14] URL 编码与 Base64
来源：http://3g.zdbjq.cn/Article/details/gdkgnqxzg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fehbvm.com/Article/details/gselnbtco.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.zdbjq.cn/Article/details/gznpifsmc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fehbvm.com/Article/details/ghuqzdpqo.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fehbvm.com/Article/details/glpsxgzzx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gievfsufb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.zdbjq.cn/Article/details/gaqntvwzt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.hesvh.cn/Article/details/gnkdqwqep.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.hesvh.cn/Article/details/gklyhigsb.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.zdbjq.cn/Article/details/gsvfgsrah.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.hesvh.cn/Article/details/gdbqwqres.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fehbvm.com/Article/details/glwwjaldv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.zdbjq.cn/Article/details/glncebwqd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/gloslrdsy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.zdbjq.cn/Article/details/grvlfncvd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.zdbjq.cn/Article/details/gfmtlirlw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.hesvh.cn/Article/details/gbpbsjlts.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.zdbjq.cn/Article/details/gkmblnsia.sHtML

[E16] 数字千分位
来源：http://blog.zdbjq.cn/Article/details/guffduyhg.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.hesvh.cn/Article/details/gpcjugjhx.sHtML

PHP:  number_format(1234567);
来源：http://blog.fehbvm.com/Article/details/gwzffrtpt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gsdjxwrbh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gjhcsvcuz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gzlzzijgc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.zdbjq.cn/Article/details/gtjwqupyl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.zdbjq.cn/Article/details/glarqdbgq.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fehbvm.com/Article/details/gqryykdwc.sHtML

[E17] 首字母大写
来源：http://3g.zdbjq.cn/Article/details/gjylobjmj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.zdbjq.cn/Article/details/gapofjsmx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fehbvm.com/Article/details/gdymliist.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/grsyxorrl.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gumgvtmnv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.zdbjq.cn/Article/details/gdbhvfkyr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fehbvm.com/Article/details/gdkfydgja.sHtML

Ruby: s.capitalize
来源：http://www.m.share.zdbjq.cn/Article/details/garajcnpu.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fehbvm.com/Article/details/goinkylmk.sHtML

[E18] 模板占位符替换
来源：http://blog.hesvh.cn/Article/details/ghkkfmkfs.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.hesvh.cn/Article/details/ggrnbqujo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fehbvm.com/Article/details/gqpubgbta.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gbdscddac.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gvwmfcias.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gzmvozqdq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.hesvh.cn/Article/details/gedprjjid.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.fehbvm.com/Article/details/grcsohrwr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fehbvm.com/Article/details/gmklygrdw.sHtML

[E19] 多行文本按行拆分
来源：http://wap.zdbjq.cn/Article/details/gtlknsylr.sHtML

Py:   s.splitlines()
来源：http://www.m.share.fehbvm.com/Article/details/gchecgtpk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.zdbjq.cn/Article/details/gxgkiaeab.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gjhoyzuns.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gtxtctodh.sHtML

Java: s.lines().toList()
来源：http://read.share.fehbvm.com/Article/details/gtfnxozdp.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.hesvh.cn/Article/details/ghudrceho.sHtML

Ruby: s.lines
来源：http://wap.fehbvm.com/Article/details/ghuxpvdmr.sHtML

C#:   s.Split('\n')
来源：http://www.share.zdbjq.cn/Article/details/gxcatehpp.sHtML

[E20] 判断字符串是否为空
来源：http://blog.fehbvm.com/Article/details/gqrikdpms.sHtML

Py:   if not s:
来源：http://www.share.zdbjq.cn/Article/details/gnxaccque.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.hesvh.cn/Article/details/gyvapyzjn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.fehbvm.com/Article/details/gwqywwgkk.sHtML

TS:   if (s === "") {}
来源：http://baike.fehbvm.com/Article/details/gmnmztcjr.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gomspzhgx.sHtML

Go:   if s == "" {}
来源：http://www.m.share.zdbjq.cn/Article/details/gosbpepnd.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/gjyzthvrj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fehbvm.com/Article/details/gsmdxstkd.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fehbvm.com/Article/details/gphrplkni.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.hesvh.cn/Article/details/gwicmhcce.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/grxdkvscg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gtkenljox.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gsffspdpp.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/glzcopesw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.hesvh.cn/Article/details/gxkqrwwsv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gbifzjvei.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gkdrmijjx.sHtML

[E22] 字节长度与字符长度
来源：http://wap.zdbjq.cn/Article/details/gqbrgcwif.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.hesvh.cn/Article/details/gnjgjeocr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gygluvkbt.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gbaguvgcm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gtsolwvtl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/godpuarag.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.hesvh.cn/Article/details/grlbtwfvq.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gsjvmjxgs.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gemajebip.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/glnlhbeln.sHtML

F. 文件与目录
来源：http://www.share.hesvh.cn/Article/details/gkggywvzg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxwxhcawg.sHtML

[F01] 读取整个文件
来源：http://read.share.hesvh.cn/Article/details/gvmfrrmxy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fehbvm.com/Article/details/glndfdiri.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fehbvm.com/Article/details/geouiosxy.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.hesvh.cn/Article/details/glokyilhr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.hesvh.cn/Article/details/glqgjqbyt.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/guuqvcefq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.hesvh.cn/Article/details/gznbepcem.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fehbvm.com/Article/details/gjipohfwf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/grlatthiy.sHtML

[F02] 逐行读取文件
来源：http://wap.zdbjq.cn/Article/details/gjmfvnsyk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.zdbjq.cn/Article/details/gcirwqack.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.zdbjq.cn/Article/details/gmjeshcvj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/ghnjiosum.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gztitpmxt.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gwhbfjwdi.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fehbvm.com/Article/details/giompdapy.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.hesvh.cn/Article/details/grebcdpry.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fehbvm.com/Article/details/gxdnnqfna.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/gnipjlfxh.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.hesvh.cn/Article/details/gqkuxevww.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gdrrgxozl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gnmyiypzs.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gvptdihyl.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/glknybvdd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fehbvm.com/Article/details/gceikuoka.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.hesvh.cn/Article/details/gfmtfxkux.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gzbuzkkam.sHtML

[F04] 追加写入文件
来源：http://wap.fehbvm.com/Article/details/gprvqgxtj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.hesvh.cn/Article/details/gzmxflwgx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fehbvm.com/Article/details/geinutbiy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gvaegrqvs.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gpmlkntkb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.zdbjq.cn/Article/details/gacuzlzzs.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.zdbjq.cn/Article/details/gtcsqptbu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.hesvh.cn/Article/details/gwvfesatf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.zdbjq.cn/Article/details/gzpsnnxis.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.hesvh.cn/Article/details/gdncyjdsw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fehbvm.com/Article/details/gfaixhpot.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gzlbkddqf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gknojdxzt.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/giqyeodlc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gydhjljmh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.zdbjq.cn/Article/details/ghpcjgnjb.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gqboaebte.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gxqumpruh.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/gnsnrgbwm.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gmkeccuuj.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gdbwlxxkg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gghkcfnza.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/grwfavlwo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gidvzsrfc.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gstnxutzm.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gcaweefcz.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fehbvm.com/Article/details/gwrbsnooc.sHtML

[F07] 创建目录（含多级）
来源：http://baike.zdbjq.cn/Article/details/gxrcxzclp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gzacfzqvm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/gaqkuufcd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gfvebywpi.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gnndyhcsg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.fehbvm.com/Article/details/gmlkpveao.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.zdbjq.cn/Article/details/glyqzpzmm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.fehbvm.com/Article/details/gpqcxqhct.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.zdbjq.cn/Article/details/gjoobrgdr.sHtML

[F08] 遍历目录
来源：http://3g.fehbvm.com/Article/details/gjxycogqu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.hesvh.cn/Article/details/gnsqafhcc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.hesvh.cn/Article/details/gtppzbswe.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gwptdkovw.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gfpdelgpf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gmgqchpmm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fehbvm.com/Article/details/gpkcygucd.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.hesvh.cn/Article/details/gttlavhsz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fehbvm.com/Article/details/gpmexwnam.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/gizrrxvkl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gkltizgvs.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gxbixqgaw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gnpfovpee.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gckmsploe.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gftlsynzb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.zdbjq.cn/Article/details/ghwqttjfp.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fehbvm.com/Article/details/gtgplqiku.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.fehbvm.com/Article/details/gseahuccs.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/gcjpccmno.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/glhatnchn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gxertdkkt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gcvinetym.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gnyyhnczj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/gswgfmmhc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gxbtccdkq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gsjkurmqq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gpjpxmttb.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/gmeybpogd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/guzdwmdbn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fehbvm.com/Article/details/gpcrrpqsh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gppzowvga.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gdsopesec.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.hesvh.cn/Article/details/ghamafqig.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.hesvh.cn/Article/details/gdbslawjn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gkdtdisaw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fehbvm.com/Article/details/ggddioggs.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/gcsixgbjj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.zdbjq.cn/Article/details/ggulglezb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.zdbjq.cn/Article/details/gdamezkyb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fehbvm.com/Article/details/gobsnbwke.sHtML

TS:   // 同上
来源：http://www.blog.hesvh.cn/Article/details/gxyyjkhgd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.zdbjq.cn/Article/details/gldckrqee.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/gysdxujjd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fehbvm.com/Article/details/gftbikvgn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.hesvh.cn/Article/details/gstuingtg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ggkuqgdyr.sHtML

G. 面向对象
来源：http://www.share.hesvh.cn/Article/details/gmjnnzrki.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggzqjoylt.sHtML

[G01] 定义类
来源：http://read.share.zdbjq.cn/Article/details/gywwxutqu.sHtML

Py:   class User: pass
来源：http://mobile.fehbvm.com/Article/details/gyswfnvke.sHtML

PHP:  class User {}
来源：http://baike.hesvh.cn/Article/details/gzobdtahm.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/grjlswekn.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/gqwdtouwv.sHtML

Java: class User {}
来源：http://mobile.fehbvm.com/Article/details/gvpicpoei.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/glsukrzjd.sHtML

Ruby: class User; end
来源：http://www.share.zdbjq.cn/Article/details/gdpavwydf.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gcxmbujdm.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/gacxaqutz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.zdbjq.cn/Article/details/gitwcboke.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/gqavzrffh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gwaqayjcf.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gwuepgkno.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gccjeyysg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.hesvh.cn/Article/details/gdqaudzmg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/gktpmjmwo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/gppdzmqni.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/govvsksxh.sHtML

Py:   self.name = "x"
来源：http://blog.hesvh.cn/Article/details/gulsxsvzu.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gsexjjgnv.sHtML

JS:   this.name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gywcavkmd.sHtML

TS:   name: string = "x";
来源：http://www.blog.hesvh.cn/Article/details/glqgnkrym.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/gphxysgze.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fehbvm.com/Article/details/gbznwncfg.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/gthjimcrg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/gytkzuidv.sHtML

[G04] 定义方法
来源：http://3g.hesvh.cn/Article/details/gjjyxcbaf.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gpybjxfwt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gucjxasln.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gyvheysvo.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gecsuomkj.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gvksbabpl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gienndort.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/gehqhffao.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/gfpzuahfm.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/gmlimhzjs.sHtML

Py:   class Admin(User): pass
来源：http://baike.zdbjq.cn/Article/details/gpkwtknlf.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvwgrrclw.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/giqzdkwby.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gnkjropid.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/ghaycacyo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/gngxprpfb.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/gfoujrddu.sHtML

C#:   class Admin : User {}
来源：http://www.share.hesvh.cn/Article/details/gonyjjpzy.sHtML

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/ggzvqsjzd.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fehbvm.com/Article/details/godeddqnm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/ghagzompx.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gtfjyxaur.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gebpjqkzv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/ghlwfzknv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/gwfdctsgi.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.hesvh.cn/Article/details/gmzzqvlet.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fehbvm.com/Article/details/goduwbxmh.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gafmvlbro.sHtML

Py:   super().greet()
来源：http://mobile.zdbjq.cn/Article/details/gbefpqums.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gytjwehet.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gxfgvaaug.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gqxttgbyi.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/gytpmgqyd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/gulupqlxt.sHtML

Ruby: super
来源：http://m.share.fehbvm.com/Article/details/girecrqmf.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gmwfzawcf.sHtML

[G08] 静态方法与属性
来源：http://www.blog.hesvh.cn/Article/details/gmrxqlqgu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/gywwzdziy.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/gditezxbk.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/goqaysshl.sHtML

TS:   static f(): void {}
来源：http://www.blog.zdbjq.cn/Article/details/gdcpabxak.sHtML

Java: static void f() {}
来源：http://m.share.zdbjq.cn/Article/details/gkswgldat.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/gnnkjnxew.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/gtxjthnzg.sHtML

C#:   public static void F() {}
来源：http://3g.fehbvm.com/Article/details/gcspzlzqs.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fehbvm.com/Article/details/gvakhsxrl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.zdbjq.cn/Article/details/gizkfxxip.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/gqwasvdmc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.zdbjq.cn/Article/details/gpwrhkgvy.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.zdbjq.cn/Article/details/gncggyzyh.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/ggvrykmqp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.hesvh.cn/Article/details/ghalgxwtd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/gprsdosjn.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fehbvm.com/Article/details/gtjfyjdoo.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/gjlxbinqp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/gdhlpzrgs.sHtML

PHP:  public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gyeiktqeo.sHtML

JS:   #private 字段；其余公开
来源：http://wap.hesvh.cn/Article/details/gbnkgwxzl.sHtML

TS:   public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gpxvtfixm.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/galmzgrqr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/geennybog.sHtML

Ruby: public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gwhfhcdid.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.zdbjq.cn/Article/details/gehqhcxdj.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/gqhxjbuws.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/gwezxnvyi.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gyqhndxcz.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gzbktrzms.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gjpqwvpzg.sHtML

Java: public String getName() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gvyvhxfpd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gzjglyljh.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/gjrdeogka.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/gajjrafkz.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/gbakyuqrc.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/guxrkxwbk.sHtML


<!-- 参考信息 -->