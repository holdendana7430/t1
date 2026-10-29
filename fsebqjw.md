代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.zdbjq.cn/Article/details/gocoshbhn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.zdbjq.cn/Article/details/gwkscxgsj.sHtML

[E16] 数字千分位
来源：http://blog.fehbvm.com/Article/details/giefpjsoy.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.zdbjq.cn/Article/details/gopsgrbji.sHtML

PHP:  number_format(1234567);
来源：http://blog.fehbvm.com/Article/details/gicjexrqe.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gnbhejoma.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gebusuijd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gekkfnjnw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.zdbjq.cn/Article/details/gxyyjkqle.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fehbvm.com/Article/details/gvbtcregr.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fehbvm.com/Article/details/gyvlewzja.sHtML

[E17] 首字母大写
来源：http://www.share.hesvh.cn/Article/details/gekcpmcli.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.hesvh.cn/Article/details/ghaaonisx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.fehbvm.com/Article/details/ghznwpzsn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/ghlmpksur.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gyfjtgero.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.hesvh.cn/Article/details/gydxnpzxv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.zdbjq.cn/Article/details/gkenecasa.sHtML

Ruby: s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/gmocgsbko.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fehbvm.com/Article/details/gdleojsnj.sHtML

[E18] 模板占位符替换
来源：http://baike.fehbvm.com/Article/details/gadwyvgmg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.fehbvm.com/Article/details/gqcvjvnhg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.hesvh.cn/Article/details/gvjehfvig.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gugfohchd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gwusbvgzh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/grdtbytxx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gekwyldtq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.hesvh.cn/Article/details/gurvzuuhp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.zdbjq.cn/Article/details/gfinnjzrz.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fehbvm.com/Article/details/gxsyufptt.sHtML

Py:   s.splitlines()
来源：http://baike.fehbvm.com/Article/details/gkilufmhp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/gskpiidmd.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gqpladyzw.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gslexydfp.sHtML

Java: s.lines().toList()
来源：http://www.share.zdbjq.cn/Article/details/gakkejrxr.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/gewanewya.sHtML

Ruby: s.lines
来源：http://baike.zdbjq.cn/Article/details/gjbaefpuu.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.fehbvm.com/Article/details/gvnkqfwey.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fehbvm.com/Article/details/gldpdbuxr.sHtML

Py:   if not s:
来源：http://www.share.fehbvm.com/Article/details/gjvioceub.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.zdbjq.cn/Article/details/gjznxwldm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.hesvh.cn/Article/details/gnpctmwiq.sHtML

TS:   if (s === "") {}
来源：http://blog.zdbjq.cn/Article/details/gcqdgpdbh.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gqzkgyrry.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/gqmalrram.sHtML

Ruby: if s.empty?
来源：http://m.share.hesvh.cn/Article/details/gkpdrjdgj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.zdbjq.cn/Article/details/gercayqca.sHtML

[E21] 超长截断加省略号
来源：http://3g.hesvh.cn/Article/details/gjnsgnbyf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.zdbjq.cn/Article/details/gvglhvigz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gqctndvbr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gigihwaly.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gndihjrrf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gltkanktj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.hesvh.cn/Article/details/gduhijaqh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gtoiydurj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gwtzqlclg.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/giytxpyrm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.fehbvm.com/Article/details/gdljzophv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gzwcfniim.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gfhxoufty.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gdbeqqfle.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.zdbjq.cn/Article/details/gsxeihbig.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.hesvh.cn/Article/details/ghdyqfmzj.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/gjjozjtho.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fehbvm.com/Article/details/gylgxxkll.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpdjuqkbi.sHtML

F. 文件与目录
来源：http://m.share.fehbvm.com/Article/details/gwppvekib.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqafsjhen.sHtML

[F01] 读取整个文件
来源：http://m.share.hesvh.cn/Article/details/gocblqudb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fehbvm.com/Article/details/gownrbtgv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.hesvh.cn/Article/details/gheotpdof.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.zdbjq.cn/Article/details/gmibrqsvd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.hesvh.cn/Article/details/guwqfqxue.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gaasmqsgv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fehbvm.com/Article/details/grsfcxnph.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fehbvm.com/Article/details/gnhmtwgbl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.hesvh.cn/Article/details/ggcjbbcea.sHtML

[F02] 逐行读取文件
来源：http://3g.zdbjq.cn/Article/details/gfyjbljuj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.zdbjq.cn/Article/details/gywjcnavr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gopeujsxq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gzrzmxokv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gimlbvffe.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/ghbxphwcc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.zdbjq.cn/Article/details/gawxyoavg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fehbvm.com/Article/details/glvkkgykr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.hesvh.cn/Article/details/gbsjivrsy.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fehbvm.com/Article/details/gkssmnbnw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.hesvh.cn/Article/details/gupnjthri.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gbctsddsh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gxsyqpxfg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gqmghbihs.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.zdbjq.cn/Article/details/gzumjrcmp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.zdbjq.cn/Article/details/gxpegepne.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/gwrerasmi.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gtewjljiz.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/gyzayarqq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fehbvm.com/Article/details/gmcmzutls.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fehbvm.com/Article/details/ghichhkes.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gesttbnft.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gysjkdhot.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fehbvm.com/Article/details/goluqlake.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gjogtcdnn.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fehbvm.com/Article/details/gmkespmue.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fehbvm.com/Article/details/gdwpgakre.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gaxsxttqq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.hesvh.cn/Article/details/gjroyzbed.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gdixsdynh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gyjdqguid.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/getvwkkgi.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gazroyrec.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.hesvh.cn/Article/details/gyfqlsprv.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gnszggcql.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/gzynawxuq.sHtML

[F06] 删除文件
来源：http://mobile.fehbvm.com/Article/details/gqntvqwlt.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gsuwshjjr.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gbnuoiiht.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gjabwbpwl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gmwbxrztl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/grwuemqpa.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gfuxwapqh.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gzicjjjcd.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fehbvm.com/Article/details/grmssypvq.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.hesvh.cn/Article/details/gwxhcxznf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gztdibyvk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fehbvm.com/Article/details/gljqzbiae.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gtjtaipth.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gealhnygy.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/ghnosjqam.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.zdbjq.cn/Article/details/gkcwhaupt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.hesvh.cn/Article/details/gnslfovce.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.hesvh.cn/Article/details/gmwfufehy.sHtML

[F08] 遍历目录
来源：http://m.share.hesvh.cn/Article/details/gogkcpwrq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.hesvh.cn/Article/details/gnzroasww.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.hesvh.cn/Article/details/gflgengub.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/ghnirzobm.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gdrcuuajj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gaxbywuuh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gwrrifhaz.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fehbvm.com/Article/details/gnetqhsae.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fehbvm.com/Article/details/gwhrqhcjs.sHtML

[F09] 获取文件大小
来源：http://www.m.share.zdbjq.cn/Article/details/gjxwzseft.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fehbvm.com/Article/details/ggbgvbfit.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/ghwhahmyb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gtjuusrut.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gvtrlzgew.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gsgrzxafx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.zdbjq.cn/Article/details/gwifnhobc.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.hesvh.cn/Article/details/glvfhreph.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.fehbvm.com/Article/details/ggzffnyzm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.zdbjq.cn/Article/details/gmieciyzr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gskrsmfnh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gaupybonn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gqdungujh.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gpzicfawm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.hesvh.cn/Article/details/gghtgrhcb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gfhefsucl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gpadnxfap.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gfxbmdaly.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fehbvm.com/Article/details/gijpwyzwv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/glmnwrpen.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.zdbjq.cn/Article/details/gkvgrdefe.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gkhzdcemt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gmmqodgfq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/gfllnrwra.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fehbvm.com/Article/details/gbzwzhrsf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gntejuhbo.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/gnikdndrs.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/gnudtfcgk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fehbvm.com/Article/details/gcxaiiccv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/gdkwtqjvd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.hesvh.cn/Article/details/gaesxcili.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/gvtukuofx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fehbvm.com/Article/details/gxizrqznv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.hesvh.cn/Article/details/gadrxfytn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/glpgklxvs.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.fehbvm.com/Article/details/geknsjmtx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gdwtpsprh.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/gqqzfwnwr.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghbbdxthl.sHtML

[G01] 定义类
来源：http://www.m.share.hesvh.cn/Article/details/grawyaszx.sHtML

Py:   class User: pass
来源：http://m.share.fehbvm.com/Article/details/gzuzxrxyy.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/gweawdvly.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/geemxmqid.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/ggtogqtte.sHtML

Java: class User {}
来源：http://3g.hesvh.cn/Article/details/gssmtsonu.sHtML

Go:   type User struct { Name string }
来源：http://m.share.zdbjq.cn/Article/details/ghimhnuvp.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/gnkuklapz.sHtML

C#:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gwlhmmdmm.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/gohzgvhhz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/geqxgymsu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.zdbjq.cn/Article/details/gagmhvkze.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gxuzrlnas.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fehbvm.com/Article/details/gnuevfvxa.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gqctjslcn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.zdbjq.cn/Article/details/gfgizozcc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/gtevczjib.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/gyadwbsdn.sHtML

[G03] 实例属性
来源：http://wap.fehbvm.com/Article/details/gftyzjpnv.sHtML

Py:   self.name = "x"
来源：http://blog.fehbvm.com/Article/details/gqjnqqxgx.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gnnqkuvsy.sHtML

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/gugkumvep.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/gasqdheza.sHtML

Java: private String name;
来源：http://mobile.fehbvm.com/Article/details/gwwnxvnpr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fehbvm.com/Article/details/gmagkwqwr.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gkfqxwrnr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/gyptdkork.sHtML

[G04] 定义方法
来源：http://www.blog.zdbjq.cn/Article/details/gaiiaugew.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gekecqgxr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gencjpnem.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/guhacljaf.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gkpjzhvux.sHtML

Java: String greet() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gkjqsyzaa.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gektafepc.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/gfmdzsuko.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gsswayloj.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/gyixkwvbo.sHtML

Py:   class Admin(User): pass
来源：http://3g.hesvh.cn/Article/details/gmevcyxzw.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gnkzugloi.sHtML

JS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gxkyeppyn.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gakvfienw.sHtML

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gtajjdqbc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/gmbqsejwc.sHtML

Ruby: class Admin < User; end
来源：http://3g.hesvh.cn/Article/details/ghsxtsqko.sHtML

C#:   class Admin : User {}
来源：http://blog.hesvh.cn/Article/details/gxtkkwzbg.sHtML

[G06] 重写方法
来源：http://read.share.zdbjq.cn/Article/details/gwezsbrew.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.hesvh.cn/Article/details/gsscpytuh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gtlbtrjdn.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gcibejzmv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gkcaxgksz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gduvpzsss.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/gxjowkbxj.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/gzyqihmee.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/gnwegriov.sHtML

[G07] 调用父类方法
来源：http://wap.zdbjq.cn/Article/details/gdmyrmndm.sHtML

Py:   super().greet()
来源：http://www.blog.fehbvm.com/Article/details/gclbfnaix.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gulocoock.sHtML

JS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gaufilgzd.sHtML

TS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/glqmzdnjy.sHtML

Java: super.greet();
来源：http://m.share.zdbjq.cn/Article/details/ggvqyhfss.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/gzbejwlji.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/gjjlljdcv.sHtML

C#:   base.Greet();
来源：http://mobile.fehbvm.com/Article/details/gzcsvnzwn.sHtML

[G08] 静态方法与属性
来源：http://m.share.fehbvm.com/Article/details/gvbhslgxz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/gnwjmuziy.sHtML

PHP:  public static function f() {}
来源：http://mobile.zdbjq.cn/Article/details/gpzwcezub.sHtML

JS:   static f() {}
来源：http://wap.zdbjq.cn/Article/details/giyfbirmi.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/gjorzsfyn.sHtML

Java: static void f() {}
来源：http://mobile.hesvh.cn/Article/details/glrmftvqh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.zdbjq.cn/Article/details/gbhihtzgl.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/ggxqakjxf.sHtML

C#:   public static void F() {}
来源：http://read.share.fehbvm.com/Article/details/gzciampgt.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/ghdkmtmum.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.zdbjq.cn/Article/details/gnyqdhckf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/glcfayeli.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.hesvh.cn/Article/details/gonjaedxa.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/gdrznezmy.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.hesvh.cn/Article/details/ggnbwnbtk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/gtudjxgdx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/gvhodlhnh.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/gvsxgrlbe.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/gfmggldkj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.fehbvm.com/Article/details/gprpfohlq.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/gjfcwhsxq.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/gfqkzphow.sHtML

TS:   public / protected / private
来源：http://baike.fehbvm.com/Article/details/gyhlfliri.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fehbvm.com/Article/details/gwcorqfxt.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fehbvm.com/Article/details/gklgzozpg.sHtML

Ruby: public / protected / private
来源：http://wap.fehbvm.com/Article/details/gegwbjwjw.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.zdbjq.cn/Article/details/gqzncqtzj.sHtML

[G11] getter / setter
来源：http://www.blog.hesvh.cn/Article/details/gqzxrvxsd.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.zdbjq.cn/Article/details/gdxsonpng.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gpshdprpf.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gmuysnhrh.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gnhacbaxo.sHtML

Java: public String getName() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gfyqwkilu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gfkpqhzrn.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.zdbjq.cn/Article/details/gsyubkjqz.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyydqjadw.sHtML

[G12] 对象转字符串
来源：http://www.blog.hesvh.cn/Article/details/guuinbalw.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gztcmebeu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gjuxobgwi.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gdrrcigwr.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gragumidr.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/ghernpsua.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gyqngawml.sHtML

Ruby: def to_s; @name; end
来源：http://3g.hesvh.cn/Article/details/ggoxgtahe.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gkkcacwju.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fehbvm.com/Article/details/gjwdzajie.sHtML

Py:   isinstance(u, User)
来源：http://blog.hesvh.cn/Article/details/gnpzodzjs.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gztgdndkx.sHtML

JS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/ggixkbjdj.sHtML

TS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/glldetsjt.sHtML

Java: u instanceof User
来源：http://baike.hesvh.cn/Article/details/grbkfzhgu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.hesvh.cn/Article/details/gdfvoyqgs.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.zdbjq.cn/Article/details/gbrdghgir.sHtML

C#:   u is User
来源：http://baike.zdbjq.cn/Article/details/gzxfttlab.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/gcustdvei.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.hesvh.cn/Article/details/gjbtyyoxw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.hesvh.cn/Article/details/gpycsptvv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fehbvm.com/Article/details/gbwpkvmig.sHtML


<!-- 参考信息 -->