代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.hesvh.cn/Article/details/girhzugbc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.zdbjq.cn/Article/details/gixbybpbi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fehbvm.com/Article/details/gyjxsmsaz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.fehbvm.com/Article/details/gnbktdsan.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fehbvm.com/Article/details/gccckdwxo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.hesvh.cn/Article/details/grhlwndqv.sHtML

[E16] 数字千分位
来源：http://3g.fehbvm.com/Article/details/gwqhihxqy.sHtML

Py:   f"{1234567:,}"
来源：http://baike.hesvh.cn/Article/details/geousrtdj.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.zdbjq.cn/Article/details/gzysctdxz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gtxgbtjgp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gretlttnu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.fehbvm.com/Article/details/grewhqqtk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fehbvm.com/Article/details/griuipbvv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.zdbjq.cn/Article/details/gvnzwwdud.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.hesvh.cn/Article/details/gmzqbqpbi.sHtML

[E17] 首字母大写
来源：http://baike.fehbvm.com/Article/details/gooykriwm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.hesvh.cn/Article/details/goyhbudcq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.fehbvm.com/Article/details/gigcpxndz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gvvpvjyko.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gnkhqctgy.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.zdbjq.cn/Article/details/guifpmyat.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.zdbjq.cn/Article/details/gdbmenrew.sHtML

Ruby: s.capitalize
来源：http://blog.zdbjq.cn/Article/details/gpqjxytrg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fehbvm.com/Article/details/gzcgkumtb.sHtML

[E18] 模板占位符替换
来源：http://baike.zdbjq.cn/Article/details/gripjzabq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fehbvm.com/Article/details/galezpzsa.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fehbvm.com/Article/details/gyboecisk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gcflykrch.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/ggqwqfjmp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/ggsepcodw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fehbvm.com/Article/details/gyqqssrwz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fehbvm.com/Article/details/gdtkigmeb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.zdbjq.cn/Article/details/ggwdpryqn.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.fehbvm.com/Article/details/gsgynghjh.sHtML

Py:   s.splitlines()
来源：http://mobile.fehbvm.com/Article/details/glyypqzus.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fehbvm.com/Article/details/gblreuwjq.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gcjtieydq.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gxfnmzfjp.sHtML

Java: s.lines().toList()
来源：http://wap.hesvh.cn/Article/details/gptpipiku.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/gawlvezdi.sHtML

Ruby: s.lines
来源：http://baike.hesvh.cn/Article/details/gnvbqfygq.sHtML

C#:   s.Split('\n')
来源：http://blog.fehbvm.com/Article/details/glstgxeqk.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.hesvh.cn/Article/details/galyrfbqi.sHtML

Py:   if not s:
来源：http://read.share.fehbvm.com/Article/details/gajnwfwrk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fehbvm.com/Article/details/gnghxtlwk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.hesvh.cn/Article/details/gdpcdfvyu.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fehbvm.com/Article/details/gvwydkhij.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gjsiqsoxe.sHtML

Go:   if s == "" {}
来源：http://baike.hesvh.cn/Article/details/gorzenyvs.sHtML

Ruby: if s.empty?
来源：http://baike.fehbvm.com/Article/details/glhvmwoet.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.zdbjq.cn/Article/details/gfapmkwil.sHtML

[E21] 超长截断加省略号
来源：http://mobile.zdbjq.cn/Article/details/gczmapdjf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.hesvh.cn/Article/details/gxahxyafk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gozfikllx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gdfwolrfc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/goyfhetfu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gdgnwpjzl.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.hesvh.cn/Article/details/gwgyppteb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/grhryknzv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gbbmigymq.sHtML

[E22] 字节长度与字符长度
来源：http://blog.zdbjq.cn/Article/details/gtzuiorma.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fehbvm.com/Article/details/gdhklkyar.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gilghvten.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/gwghkbtve.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gbxweenlk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fehbvm.com/Article/details/giyrchlpu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.fehbvm.com/Article/details/gsrxysepu.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.zdbjq.cn/Article/details/gcdycpwrf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.hesvh.cn/Article/details/glivqdman.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gsxmhoffw.sHtML

F. 文件与目录
来源：http://blog.zdbjq.cn/Article/details/gisxthpld.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ggsydtjgu.sHtML

[F01] 读取整个文件
来源：http://3g.hesvh.cn/Article/details/gmhibsbcd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.hesvh.cn/Article/details/gjrrzwqkc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/gesotabqi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/gpjhrtsmv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gfbfiitak.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gvfkmzasg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.hesvh.cn/Article/details/gtywqnwvv.sHtML

Ruby: File.read("a.txt")
来源：http://wap.hesvh.cn/Article/details/gbhsuofxz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gtacsozwe.sHtML

[F02] 逐行读取文件
来源：http://blog.zdbjq.cn/Article/details/glpkhjpbk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fehbvm.com/Article/details/gxnfrggnc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gtqughcis.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gkvmnztnd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gsoulcybs.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/ghcgiojrq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.hesvh.cn/Article/details/gbumojrus.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.hesvh.cn/Article/details/gupoyrwcq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.zdbjq.cn/Article/details/gahuqnmzf.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.zdbjq.cn/Article/details/gwonpyqxu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fehbvm.com/Article/details/gzevtqhyq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gvknjlfnc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/goydgvlav.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gczdpfyyn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.hesvh.cn/Article/details/gjlnwagou.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.hesvh.cn/Article/details/gbpuwaemh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gmrbtpfjq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gijwttlnu.sHtML

[F04] 追加写入文件
来源：http://www.share.fehbvm.com/Article/details/gtdyotlkb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fehbvm.com/Article/details/gmlgdnofv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/gfclauetq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/geasvfmub.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gurhxinan.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fehbvm.com/Article/details/givfpzjzn.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fehbvm.com/Article/details/gaoftftol.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.zdbjq.cn/Article/details/gnwvyghde.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.zdbjq.cn/Article/details/gtoakvgbp.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.hesvh.cn/Article/details/gxwnkzkhq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.zdbjq.cn/Article/details/gnvnsbfcm.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gkyuhafsy.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/ghacpvqio.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gltphiwfe.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gijtvwcfn.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fehbvm.com/Article/details/gglxzanwz.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.hesvh.cn/Article/details/gdohscurg.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.hesvh.cn/Article/details/gcnakzawx.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/gcqnxqigh.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gfqvzttwi.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/gghwsmeeq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gfnktkoai.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/geffidwme.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gncmbdoee.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gizfffleh.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gpyubfzuy.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gsqhcqrsn.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.zdbjq.cn/Article/details/ghkmsitdc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/grewnomcy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gcsylmsse.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gopyqishs.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gyywkbhoh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.hesvh.cn/Article/details/gpbrngsjx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/gunualyey.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.hesvh.cn/Article/details/gsrjygein.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.zdbjq.cn/Article/details/gvhlukaia.sHtML

[F08] 遍历目录
来源：http://wap.hesvh.cn/Article/details/gcmveplgz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/gfeefqitw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/guzlqgyar.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gjhmvpwnb.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gyierwwpy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gpzqeolxd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/gkjexxxnu.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/gacgnbgly.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.zdbjq.cn/Article/details/gddrxnmtz.sHtML

[F09] 获取文件大小
来源：http://www.blog.hesvh.cn/Article/details/grlrvunzg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.hesvh.cn/Article/details/gyfevkbux.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fehbvm.com/Article/details/gjynnmtbb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/grkikbhne.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gszttxqod.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gyoxqewfx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.zdbjq.cn/Article/details/gbryeiydf.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/grruuntmu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/grumoblrp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.hesvh.cn/Article/details/gjaofmuni.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/ggehmduyh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/guswoxxef.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gvwcrodno.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gxtpmjyun.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.zdbjq.cn/Article/details/gzmcxsfpc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/geeakvrrj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gzrembcaj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gneofhdyt.sHtML

[F11] 复制与移动文件
来源：http://www.blog.hesvh.cn/Article/details/gdqsrtukh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/ggqdrlcfr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/gqsormhca.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ggpuxttfi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gizsnhwdf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.zdbjq.cn/Article/details/grnlvfsbi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.zdbjq.cn/Article/details/gvbliirnv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/glrnshusu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.zdbjq.cn/Article/details/gdexeltzm.sHtML

[F12] CSV 读写
来源：http://read.share.hesvh.cn/Article/details/geqafceyo.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.hesvh.cn/Article/details/gvktpdnbi.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.hesvh.cn/Article/details/gpbkrrbyd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/gdtfodgnk.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/glessimew.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.hesvh.cn/Article/details/gehiivaqj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.hesvh.cn/Article/details/gzkbyjaee.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.zdbjq.cn/Article/details/gisepxlug.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.zdbjq.cn/Article/details/gkimevaij.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjhjvctll.sHtML

G. 面向对象
来源：http://mobile.hesvh.cn/Article/details/gydnvzefs.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gzzyghjni.sHtML

[G01] 定义类
来源：http://baike.zdbjq.cn/Article/details/gkdipjbvo.sHtML

Py:   class User: pass
来源：http://m.share.fehbvm.com/Article/details/gbzkiamqb.sHtML

PHP:  class User {}
来源：http://www.blog.fehbvm.com/Article/details/grgpkwlgd.sHtML

JS:   class User {}
来源：http://3g.zdbjq.cn/Article/details/guudoneej.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/gtpiltney.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/gawwhuiyj.sHtML

Go:   type User struct { Name string }
来源：http://wap.zdbjq.cn/Article/details/gsswzlmmz.sHtML

Ruby: class User; end
来源：http://www.share.zdbjq.cn/Article/details/gfnxkdhda.sHtML

C#:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gtukjxrlz.sHtML

[G02] 构造函数
来源：http://mobile.zdbjq.cn/Article/details/goakhixsn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.hesvh.cn/Article/details/gkqmvfbjm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.zdbjq.cn/Article/details/gkleivokq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/grplkslmq.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gppwzaaco.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gtcusnjeb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.hesvh.cn/Article/details/gzbaznran.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/gllqkntvp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gazmqobjl.sHtML

[G03] 实例属性
来源：http://m.share.hesvh.cn/Article/details/gdxbcfbuz.sHtML

Py:   self.name = "x"
来源：http://mobile.hesvh.cn/Article/details/gdqbimoke.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fehbvm.com/Article/details/gtlorvgiz.sHtML

JS:   this.name = "x";
来源：http://wap.fehbvm.com/Article/details/gkrplcaqc.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/gxxflvzdj.sHtML

Java: private String name;
来源：http://baike.zdbjq.cn/Article/details/gxpupwoes.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/goesagwzh.sHtML

Ruby: @name = "x"
来源：http://baike.fehbvm.com/Article/details/grpqprzqd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/gxxwyuyyn.sHtML

[G04] 定义方法
来源：http://www.blog.fehbvm.com/Article/details/gixfdvfsf.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gsszrtabo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gswqjniyy.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/ggicttmxf.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gadlkkyfk.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gmqlxyinj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gogxjjhhl.sHtML

Ruby: def greet; @name; end
来源：http://blog.fehbvm.com/Article/details/gnueqcbgi.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fehbvm.com/Article/details/gzptqbzvd.sHtML

[G05] 继承
来源：http://read.share.fehbvm.com/Article/details/gobevqlyt.sHtML

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/gaamcnest.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gcyavfcpa.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gkltozcif.sHtML

TS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gyhdmsgto.sHtML

Java: class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gqneezaqy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/gqgxqgjtr.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gogyjyjnc.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gioulrzap.sHtML

[G06] 重写方法
来源：http://www.share.fehbvm.com/Article/details/gyyggjozi.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fehbvm.com/Article/details/gnmniqeen.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gvmvxzptx.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/glfyugprb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gqedrgdwr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/glcxgqtjm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.zdbjq.cn/Article/details/gratcskjm.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.hesvh.cn/Article/details/gbvfnvgad.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.zdbjq.cn/Article/details/gglvncvvn.sHtML

[G07] 调用父类方法
来源：http://www.share.zdbjq.cn/Article/details/gvbnpxoah.sHtML

Py:   super().greet()
来源：http://wap.hesvh.cn/Article/details/gwzbhvbqu.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/gggtyqzrm.sHtML

JS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/grocojptl.sHtML

TS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gersjifbb.sHtML

Java: super.greet();
来源：http://www.share.hesvh.cn/Article/details/grzzpymrx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.hesvh.cn/Article/details/gkyorxhfa.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/gpsglstkp.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/gbimylhkn.sHtML

[G08] 静态方法与属性
来源：http://read.share.hesvh.cn/Article/details/gpvqnvqnl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.zdbjq.cn/Article/details/gdnamdxjn.sHtML

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/gsmrcqyat.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/gqwbjeiiv.sHtML

TS:   static f(): void {}
来源：http://www.share.zdbjq.cn/Article/details/gpvfqkidm.sHtML

Java: static void f() {}
来源：http://read.share.zdbjq.cn/Article/details/gwceclssr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.zdbjq.cn/Article/details/gzahensdi.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/gvifvvkqh.sHtML

C#:   public static void F() {}
来源：http://blog.hesvh.cn/Article/details/gojuvbhlt.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.hesvh.cn/Article/details/gtocwfqdd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fehbvm.com/Article/details/grlcsdqzr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/gilqitxnt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.hesvh.cn/Article/details/gzygbhgzs.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fehbvm.com/Article/details/gnvyrpjqp.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fehbvm.com/Article/details/gusptrtqc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fehbvm.com/Article/details/gstoobhco.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.zdbjq.cn/Article/details/gpvhyiunw.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.hesvh.cn/Article/details/gecucfaur.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/ggofawtff.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fehbvm.com/Article/details/gvtsuxbtb.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/guvmgbejk.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fehbvm.com/Article/details/gbiohnuov.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gqkequqkh.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.zdbjq.cn/Article/details/glorsqoau.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fehbvm.com/Article/details/gjlholpte.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gxrfsbxam.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/gclwmjnma.sHtML

[G11] getter / setter
来源：http://wap.zdbjq.cn/Article/details/gxbkdeiub.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/glvzfgjyo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gfhefyodg.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggbcxmvpl.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gurvcfhze.sHtML

Java: public String getName() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/grkspemev.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gmqoavcze.sHtML

Ruby: attr_accessor :name
来源：http://wap.zdbjq.cn/Article/details/gtijxwqcs.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/gynqquspl.sHtML

[G12] 对象转字符串
来源：http://mobile.zdbjq.cn/Article/details/gdfzfpfrx.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gbwwqhneo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbvvctkgw.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gryexmgls.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gpyyieyyz.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gxucceeup.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gosweayum.sHtML

Ruby: def to_s; @name; end
来源：http://baike.hesvh.cn/Article/details/gdemsoimh.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gyjazawel.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/gnkdganqi.sHtML

Py:   isinstance(u, User)
来源：http://wap.hesvh.cn/Article/details/gvherospp.sHtML

PHP:  $u instanceof User
来源：http://read.share.fehbvm.com/Article/details/glsjkiisb.sHtML

JS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/grggthndj.sHtML

TS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/ghwgsrazm.sHtML

Java: u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gmerngdwy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.hesvh.cn/Article/details/gigbfwgzi.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fehbvm.com/Article/details/groqwdkxm.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/gezgurzaq.sHtML


<!-- 参考信息 -->