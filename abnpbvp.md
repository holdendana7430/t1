代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.hesvh.cn/Article/details/gpbphqjqe.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.hesvh.cn/Article/details/gcwcdpclt.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fehbvm.com/Article/details/gysmzembe.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.hesvh.cn/Article/details/gmeaeqhfq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.zdbjq.cn/Article/details/gvvriyyuh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.zdbjq.cn/Article/details/gaokynakq.sHtML

[E16] 数字千分位
来源：http://mobile.fehbvm.com/Article/details/ggefqpuhc.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.zdbjq.cn/Article/details/gvbadzrpv.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/grizcheam.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gfzolfvyd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gxdgewgys.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gpdzctifu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fehbvm.com/Article/details/gkfjpnyox.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.hesvh.cn/Article/details/ghunluhww.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fehbvm.com/Article/details/gmricvchm.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/gkpjumpww.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.zdbjq.cn/Article/details/gdlblfomt.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.hesvh.cn/Article/details/gtdtsisac.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gfhrsnjgv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/guqxravwj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/guzhvakgy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.zdbjq.cn/Article/details/gepjistcp.sHtML

Ruby: s.capitalize
来源：http://www.m.share.hesvh.cn/Article/details/gtpgpsydy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fehbvm.com/Article/details/gkqeeufrv.sHtML

[E18] 模板占位符替换
来源：http://m.share.zdbjq.cn/Article/details/gaxbtvxqn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fehbvm.com/Article/details/glvnzlcii.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.zdbjq.cn/Article/details/glweuyrew.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gozsgaqwp.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gnptpxfux.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/ghqjwqhmj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gdktrkjwz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/gnilpkxky.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.zdbjq.cn/Article/details/gggcfltbf.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/gtvnrjrbs.sHtML

Py:   s.splitlines()
来源：http://baike.hesvh.cn/Article/details/gukeeecpb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/grvauqfxw.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gotfjknhy.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/genuxgsdr.sHtML

Java: s.lines().toList()
来源：http://wap.zdbjq.cn/Article/details/gfjsbcvnv.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.zdbjq.cn/Article/details/gxuccevhu.sHtML

Ruby: s.lines
来源：http://m.share.zdbjq.cn/Article/details/gzawzudze.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/gubikzglr.sHtML

[E20] 判断字符串是否为空
来源：http://3g.hesvh.cn/Article/details/gzmeutmic.sHtML

Py:   if not s:
来源：http://baike.fehbvm.com/Article/details/gxveqkatf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fehbvm.com/Article/details/gyfrvnniz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.hesvh.cn/Article/details/gkwejqfvi.sHtML

TS:   if (s === "") {}
来源：http://m.share.fehbvm.com/Article/details/gglffrkkn.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gvxgjdbbe.sHtML

Go:   if s == "" {}
来源：http://read.share.zdbjq.cn/Article/details/gbmgarkre.sHtML

Ruby: if s.empty?
来源：http://read.share.zdbjq.cn/Article/details/gxvjypjqe.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.fehbvm.com/Article/details/gokxqmpov.sHtML

[E21] 超长截断加省略号
来源：http://www.share.hesvh.cn/Article/details/grrqfqyby.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/gmjczegsi.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.hesvh.cn/Article/details/giupnoaon.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/grzfrakgb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gfkwvwyph.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gowvfthcr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/gldpdfpkt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gygfsnpfd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gcexssumk.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fehbvm.com/Article/details/gwbqwzree.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.hesvh.cn/Article/details/gkwdcxnzc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gaiuioxgx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gfzcjrxtb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gjyssufxy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.zdbjq.cn/Article/details/glulixztl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.hesvh.cn/Article/details/gulumptrt.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fehbvm.com/Article/details/ghfhjhzvy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gfgfgpoxl.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxaokyhaa.sHtML

F. 文件与目录
来源：http://wap.hesvh.cn/Article/details/gikhluaft.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwyplnjao.sHtML

[F01] 读取整个文件
来源：http://blog.fehbvm.com/Article/details/gwebeejps.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.hesvh.cn/Article/details/gofjvsbgj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gbsyswjqj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.hesvh.cn/Article/details/gftmvizyt.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/goyvfzpup.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gejalgvrs.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fehbvm.com/Article/details/gzvqzsezp.sHtML

Ruby: File.read("a.txt")
来源：http://3g.zdbjq.cn/Article/details/globpjwfc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.hesvh.cn/Article/details/ggppxijvk.sHtML

[F02] 逐行读取文件
来源：http://baike.zdbjq.cn/Article/details/gzpcvmqdn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.hesvh.cn/Article/details/gjvmvwwdj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fehbvm.com/Article/details/ghzpcelth.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gqwqzpsmh.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gmuamvjcu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gaoukgldg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.zdbjq.cn/Article/details/ggcentobl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.hesvh.cn/Article/details/gxtcczdwk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/geyftpgzh.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.hesvh.cn/Article/details/gdccldtqi.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.hesvh.cn/Article/details/gddmzcndx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gerqxkayi.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gsimpivnt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gwevydsay.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.hesvh.cn/Article/details/gpxrlmnlz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fehbvm.com/Article/details/gnqyrqcry.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.hesvh.cn/Article/details/gvljolkwc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gjvlgfrwa.sHtML

[F04] 追加写入文件
来源：http://3g.hesvh.cn/Article/details/gusehznum.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fehbvm.com/Article/details/gnbbkmftz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.hesvh.cn/Article/details/gaotmtapk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gmfioaogj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gvkdfyzgu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fehbvm.com/Article/details/gfmborpcn.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.hesvh.cn/Article/details/gbhqxcjpo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.hesvh.cn/Article/details/gbzohqyie.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.zdbjq.cn/Article/details/ghcjhxhns.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.hesvh.cn/Article/details/gsxlyxlfo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.zdbjq.cn/Article/details/gpygmwxfo.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fehbvm.com/Article/details/gnlyaejai.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/ghrmsdifx.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gywhovrco.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gjffvnydn.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.zdbjq.cn/Article/details/gphefdpfe.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gsuqcwbau.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/giyxoqhrk.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/gbwgsrtft.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gavzgdaqw.sHtML

PHP:  unlink("a.txt");
来源：http://3g.hesvh.cn/Article/details/gqysjdeoy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/glvmblhvu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gomjkbtzs.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gwcukrjvi.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gfcuukndy.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gpgtaowry.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gooiilkqk.sHtML

[F07] 创建目录（含多级）
来源：http://wap.hesvh.cn/Article/details/gsjcindff.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gwbkrsggp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.zdbjq.cn/Article/details/gkjzpknig.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gdludbpmx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gyqojfjhs.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/gqrzvcyrw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/gaixhxajp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fehbvm.com/Article/details/glhsimfrp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.zdbjq.cn/Article/details/gyhgkbfid.sHtML

[F08] 遍历目录
来源：http://baike.fehbvm.com/Article/details/gxvwzfiau.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/ggkkuvqsa.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.hesvh.cn/Article/details/gfkhsnohf.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gusvjkbax.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/genadnzmm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gkilnqbol.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gqruniwno.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.hesvh.cn/Article/details/gvbcmwxpg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fehbvm.com/Article/details/gzfnvrqay.sHtML

[F09] 获取文件大小
来源：http://baike.zdbjq.cn/Article/details/gaxnvjygp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gvesbbwcg.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fehbvm.com/Article/details/gajdrfqvs.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gmlawieus.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gdapckvxf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gbdhyxruh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.zdbjq.cn/Article/details/geuexoxzc.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gvagfqjnu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.zdbjq.cn/Article/details/gpgkxusmn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/gtugwiops.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/geeehkpmr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fehbvm.com/Article/details/gkjtklhmk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gkoxpbuaa.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gyxjkhicb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/grejardbn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gibahvkcb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gurzjqrct.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gawfdzhli.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/gycdkpsbn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gaofsgutv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fehbvm.com/Article/details/glbbhgfar.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gighaoshv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gqerldxfr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.hesvh.cn/Article/details/gjsekkjmk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.hesvh.cn/Article/details/grqwrqkbv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gayenoegs.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fehbvm.com/Article/details/gaccgakcb.sHtML

[F12] CSV 读写
来源：http://blog.fehbvm.com/Article/details/gfawxousk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.zdbjq.cn/Article/details/gzgewxvkq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fehbvm.com/Article/details/ghtbnouxy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fehbvm.com/Article/details/gyslayeyy.sHtML

TS:   // 同上
来源：http://m.share.fehbvm.com/Article/details/ggfckodum.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/gallrrwnc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.zdbjq.cn/Article/details/gxpxxmybg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fehbvm.com/Article/details/giqggjoez.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.hesvh.cn/Article/details/gzedvqtbw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjjhcxwfm.sHtML

G. 面向对象
来源：http://mobile.hesvh.cn/Article/details/gnfdvmbfk.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdywbdbve.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/glwrlutpn.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/gbxbzjtib.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/gjwjueulf.sHtML

JS:   class User {}
来源：http://baike.hesvh.cn/Article/details/guxnxqbwr.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/gjqmwoxog.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxumhhcwh.sHtML

Go:   type User struct { Name string }
来源：http://blog.hesvh.cn/Article/details/gvrviqmqo.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/gttbcjgkt.sHtML

C#:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gcjkwhysx.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/gsaingamf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.zdbjq.cn/Article/details/gecxvahoc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gaujvchjk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gkpzggwyp.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fehbvm.com/Article/details/gznwfeyre.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/giuvxfnde.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.hesvh.cn/Article/details/gtwdgqjjm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.zdbjq.cn/Article/details/gxibrfugq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/gzdcpaobx.sHtML

[G03] 实例属性
来源：http://www.share.fehbvm.com/Article/details/gukppmgcb.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/ghqrbinqo.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gpuqossxs.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gvkfmbnkb.sHtML

TS:   name: string = "x";
来源：http://wap.hesvh.cn/Article/details/gxqbyhowy.sHtML

Java: private String name;
来源：http://read.share.zdbjq.cn/Article/details/gqwcarhsc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.zdbjq.cn/Article/details/gvtwkrdcc.sHtML

Ruby: @name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gmuegzhfl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/grgnzqqga.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gfebyxerq.sHtML

Py:   def greet(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gainfajkl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gcjxdoqpq.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gwrqvahof.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gzptmuaxa.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/goucgxoxl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gkxfcwcqe.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/grlnjbffh.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.hesvh.cn/Article/details/gyakoithf.sHtML

[G05] 继承
来源：http://www.share.zdbjq.cn/Article/details/gyvlskkaw.sHtML

Py:   class Admin(User): pass
来源：http://read.share.zdbjq.cn/Article/details/gxbkpzrlx.sHtML

PHP:  class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gytsnunmh.sHtML

JS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gupxnxljl.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gcbjzvasq.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/ggyadmayj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fehbvm.com/Article/details/gwcsshfwt.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/gycilqgre.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fehbvm.com/Article/details/gwuxdqiqe.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/gjiykvmra.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fehbvm.com/Article/details/gjrrqwylf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gfceyocqf.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gdrwkobqr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gexpvmzjd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gsttyennt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fehbvm.com/Article/details/gmqrmmjqh.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.zdbjq.cn/Article/details/gmqpnkssb.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fehbvm.com/Article/details/gmopasukd.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/gtyischfj.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/gpqsegatz.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/gmqhpfamx.sHtML

JS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/glvzgcfec.sHtML

TS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gitftiesy.sHtML

Java: super.greet();
来源：http://wap.zdbjq.cn/Article/details/gkogglwpv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.zdbjq.cn/Article/details/gzynocngx.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/gjebdjaho.sHtML

C#:   base.Greet();
来源：http://www.m.share.hesvh.cn/Article/details/gaxeslhyn.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/gvtebrfnc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/gnvvdnjgm.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gdvyrtyhg.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/gwfgtasmm.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/gxmhukfuv.sHtML

Java: static void f() {}
来源：http://www.share.hesvh.cn/Article/details/gkabhwjjv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/gmclumksk.sHtML

Ruby: def self.f; end
来源：http://m.share.zdbjq.cn/Article/details/gnrukfils.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/grvadegvk.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/gniozywff.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.hesvh.cn/Article/details/giozpjkzx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.hesvh.cn/Article/details/ghhvdoupz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.hesvh.cn/Article/details/gxuazxryf.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.hesvh.cn/Article/details/gjoifeskx.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/gqadeuadb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/gmkljlgaa.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.hesvh.cn/Article/details/grquyaucc.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.hesvh.cn/Article/details/gyhzwcftf.sHtML

[G10] 访问控制
来源：http://baike.zdbjq.cn/Article/details/gzvprateq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/gepsebois.sHtML

PHP:  public / protected / private
来源：http://wap.hesvh.cn/Article/details/gserrrwas.sHtML

JS:   #private 字段；其余公开
来源：http://3g.zdbjq.cn/Article/details/gcnantuof.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gplcxtgcv.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/gbdbjztpc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.zdbjq.cn/Article/details/gtumhgopr.sHtML

Ruby: public / protected / private
来源：http://baike.hesvh.cn/Article/details/gpjstxpcy.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/gsnhpzpgm.sHtML

[G11] getter / setter
来源：http://www.m.share.hesvh.cn/Article/details/gozxnilfh.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/gfheabksq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gczixlpgc.sHtML

JS:   get name() { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gowhpuvar.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gtzbxzhpi.sHtML

Java: public String getName() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gaayykrnt.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gzksswmgj.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/geifjnzwi.sHtML

C#:   public string Name { get; set; }
来源：http://blog.zdbjq.cn/Article/details/gckyxrzdc.sHtML

[G12] 对象转字符串
来源：http://m.share.hesvh.cn/Article/details/gqxcjvvod.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gfzjndxko.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gnkwjrzlh.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/grxwppogo.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gxibptuza.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/grckhhdcw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gwccsioju.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gtzbsxvdp.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.hesvh.cn/Article/details/gukjjuckx.sHtML

[G13] 判断对象类型
来源：http://read.share.fehbvm.com/Article/details/ghayfpdfg.sHtML

Py:   isinstance(u, User)
来源：http://3g.zdbjq.cn/Article/details/glmbktoel.sHtML

PHP:  $u instanceof User
来源：http://read.share.fehbvm.com/Article/details/guxxjcsuj.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gwqeplsaq.sHtML

TS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gdbciunda.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/gcjasnplp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.zdbjq.cn/Article/details/grilahcgi.sHtML

Ruby: u.is_a?(User)
来源：http://3g.hesvh.cn/Article/details/ghufqfrms.sHtML

C#:   u is User
来源：http://www.m.share.fehbvm.com/Article/details/gmhngjvaz.sHtML


<!-- 参考信息 -->