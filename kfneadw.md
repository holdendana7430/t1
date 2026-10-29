代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.zdbjq.cn/Article/details/gzvaqevhq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.hesvh.cn/Article/details/gutyaojhm.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.zdbjq.cn/Article/details/gnkzzymmz.sHtML

[E17] 首字母大写
来源：http://wap.zdbjq.cn/Article/details/gtnddtbxj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.hesvh.cn/Article/details/gttazicnj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.zdbjq.cn/Article/details/ggoermyri.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gnschtlsz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gmwpvumrf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/gsgagdanb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gwattbqzi.sHtML

Ruby: s.capitalize
来源：http://3g.fehbvm.com/Article/details/gdtinborw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.zdbjq.cn/Article/details/gvnsulbkw.sHtML

[E18] 模板占位符替换
来源：http://wap.zdbjq.cn/Article/details/gzgdeqdsj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/guxyzungf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.hesvh.cn/Article/details/gxwmvgkyu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gjpfiodsw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gshffhsso.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/grsiqynsk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gxjzcwpyp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fehbvm.com/Article/details/gdwteyvxx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fehbvm.com/Article/details/gbntjsyzy.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.hesvh.cn/Article/details/grnxpekph.sHtML

Py:   s.splitlines()
来源：http://www.share.hesvh.cn/Article/details/gytokpbdz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fehbvm.com/Article/details/gnnxvbrli.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gvevqdjry.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/glpixsdxh.sHtML

Java: s.lines().toList()
来源：http://baike.zdbjq.cn/Article/details/grizvbkaj.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.hesvh.cn/Article/details/gpozfgozj.sHtML

Ruby: s.lines
来源：http://mobile.fehbvm.com/Article/details/grvcydfxc.sHtML

C#:   s.Split('\n')
来源：http://m.share.fehbvm.com/Article/details/gaqkwfdfc.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fehbvm.com/Article/details/gtkjglxxj.sHtML

Py:   if not s:
来源：http://blog.fehbvm.com/Article/details/gezhmwclr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fehbvm.com/Article/details/giwctvvaa.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.zdbjq.cn/Article/details/giwyyrgqd.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/gcaqkffos.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/grventkcf.sHtML

Go:   if s == "" {}
来源：http://read.share.fehbvm.com/Article/details/gbxvggcim.sHtML

Ruby: if s.empty?
来源：http://blog.hesvh.cn/Article/details/gnwjflfzh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.zdbjq.cn/Article/details/gmjltbtkz.sHtML

[E21] 超长截断加省略号
来源：http://blog.zdbjq.cn/Article/details/gqsknftii.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.hesvh.cn/Article/details/gqsvqvrdr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/glsiegoaj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gwrjdshmi.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gzsszqlum.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/ggrkbrctv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.zdbjq.cn/Article/details/guptqhjcp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/genslfgqh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gkdhaxrkv.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.fehbvm.com/Article/details/gshiifewv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.hesvh.cn/Article/details/gvzskbqub.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gnqpwcrwj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gxlwvoeeo.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gteuzozpd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.fehbvm.com/Article/details/ghihbmlia.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.hesvh.cn/Article/details/gznnllafp.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/gughxyjll.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fehbvm.com/Article/details/guzoyumnm.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gryjqurul.sHtML

F. 文件与目录
来源：http://www.share.fehbvm.com/Article/details/gveuzcktd.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/geecernaf.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/germsfioo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fehbvm.com/Article/details/gchorgwwj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gozntqpal.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fehbvm.com/Article/details/gorvowenm.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gaeukzzqa.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gnbonnzrc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.zdbjq.cn/Article/details/gsewteurw.sHtML

Ruby: File.read("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gfvqtwaoi.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gdeusfimh.sHtML

[F02] 逐行读取文件
来源：http://mobile.hesvh.cn/Article/details/gtkrvphcd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fehbvm.com/Article/details/glmoezrhm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/gvjnqljlb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/ghkpomoza.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gjmplqsdn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gahkuzhvc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.zdbjq.cn/Article/details/gvgdkzeip.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.zdbjq.cn/Article/details/gptcakvly.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.hesvh.cn/Article/details/gvvgpvnpe.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.hesvh.cn/Article/details/gcugrlcoz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.hesvh.cn/Article/details/gesdvbdxj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gvtmivopb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gzseqlzfl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gmdaekrjp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gmrxnpubr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.zdbjq.cn/Article/details/ghsffvkye.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fehbvm.com/Article/details/gklzeeijx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gwsnajkci.sHtML

[F04] 追加写入文件
来源：http://read.share.fehbvm.com/Article/details/gopseeuyb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/ggfadytyz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.zdbjq.cn/Article/details/gqwvgedma.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gzblvssah.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/goinzmezy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.zdbjq.cn/Article/details/gknxevgav.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gxtasjgeb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/gonfjomne.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.zdbjq.cn/Article/details/gbhzgxmmy.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fehbvm.com/Article/details/gtbeweodc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.zdbjq.cn/Article/details/gmzhtfvmo.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gbozwffhw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gipeuquml.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gofjtltxz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gydnhrhlh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.hesvh.cn/Article/details/gjdrbyuss.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gedvpxais.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gsnphlghy.sHtML

[F06] 删除文件
来源：http://www.m.share.fehbvm.com/Article/details/gdoqrrbks.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gjcidukfs.sHtML

PHP:  unlink("a.txt");
来源：http://wap.hesvh.cn/Article/details/gciglnasm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gfnlfhzgt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gvsveivrb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gnenrueej.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/grdclrfhn.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gjfyfpbdw.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.hesvh.cn/Article/details/glfhnzypl.sHtML

[F07] 创建目录（含多级）
来源：http://3g.hesvh.cn/Article/details/gzimzpwxh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gbopqfjuo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.hesvh.cn/Article/details/gajeiahvm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/ggeatngmb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gjuxspqrf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/gebvzsfxk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fehbvm.com/Article/details/gjwmykwvn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fehbvm.com/Article/details/getegzvhu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/gnozhurar.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/ghhsapmcd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fehbvm.com/Article/details/gnloldqam.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fehbvm.com/Article/details/gvriywacg.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gcjwnjxjd.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gdlzlehdk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gnioeqgra.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.hesvh.cn/Article/details/gtmdchcbh.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/gmtdlrtil.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.zdbjq.cn/Article/details/gklsjgcpj.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/gvxgyigxr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/ghbhawdvr.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fehbvm.com/Article/details/gucykazzx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/glunzggmn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gexekzwij.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/grzyctdeb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.zdbjq.cn/Article/details/gbtqximtu.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gtylpgdau.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.zdbjq.cn/Article/details/gaiftkrof.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.hesvh.cn/Article/details/gvtuvjids.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gupxixxpw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gkqdyohib.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gduuazudy.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gjwpjngpj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/gaavihrla.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gpllgdnuy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/ghtdlndul.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gpqusuibj.sHtML

[F11] 复制与移动文件
来源：http://wap.fehbvm.com/Article/details/guqsekoeq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gugtgguzq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.hesvh.cn/Article/details/gadmncfhz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/grnmwjlyx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gjaaxisqa.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.hesvh.cn/Article/details/gzexdritv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gyqgmzhxc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gdmlxvmex.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fehbvm.com/Article/details/glrnriuct.sHtML

[F12] CSV 读写
来源：http://baike.zdbjq.cn/Article/details/gsfiusnaj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.hesvh.cn/Article/details/ggivdooha.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.hesvh.cn/Article/details/gbtfehhdm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/gbapnlvyc.sHtML

TS:   // 同上
来源：http://m.share.hesvh.cn/Article/details/gornxcral.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.hesvh.cn/Article/details/gbkztbgqn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/gconchxcw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fehbvm.com/Article/details/gtsvixnnw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/gbydivzoa.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/giptbwowc.sHtML

G. 面向对象
来源：http://www.share.fehbvm.com/Article/details/gmglqdjvn.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gaisuiclu.sHtML

[G01] 定义类
来源：http://3g.fehbvm.com/Article/details/gvqwgbglh.sHtML

Py:   class User: pass
来源：http://blog.fehbvm.com/Article/details/grqebfxoj.sHtML

PHP:  class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjlettxon.sHtML

JS:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gpalylteq.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fehbvm.com/Article/details/grsorooyb.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/gfpowycec.sHtML

Go:   type User struct { Name string }
来源：http://mobile.hesvh.cn/Article/details/gihsmhuof.sHtML

Ruby: class User; end
来源：http://www.share.zdbjq.cn/Article/details/gfbwauhkx.sHtML

C#:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gjnjhvueb.sHtML

[G02] 构造函数
来源：http://3g.zdbjq.cn/Article/details/gfqroisdv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.zdbjq.cn/Article/details/gazmrnajc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/gauzhmbfz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gvvoniiah.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fehbvm.com/Article/details/gmzxpmyvm.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gyuvklwtq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/ghtmskltt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.zdbjq.cn/Article/details/glvhggidk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/gtqnjowkq.sHtML

[G03] 实例属性
来源：http://m.share.fehbvm.com/Article/details/gehmigwdj.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gzfqjzind.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/gdljcptar.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gzwmoroao.sHtML

TS:   name: string = "x";
来源：http://mobile.zdbjq.cn/Article/details/gjmmevetc.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/gowkbtzgc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.hesvh.cn/Article/details/gnvqphsht.sHtML

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gychosrty.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/gchlvxbxj.sHtML

[G04] 定义方法
来源：http://read.share.zdbjq.cn/Article/details/gbmbnfgkt.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/githebtfp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/grjfbmncf.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gigclgbdw.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gjfxvfmkg.sHtML

Java: String greet() { return name; }
来源：http://3g.fehbvm.com/Article/details/gldrpheff.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gkejibdua.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/gxiimhths.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gmtpbygbj.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/gmfxqubus.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fehbvm.com/Article/details/gmefmqlxj.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gjflvwyrg.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/ggrnanajw.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gxvsekzew.sHtML

Java: class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gmerjnuqr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/grktuwuwq.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/gmlrbuejg.sHtML

C#:   class Admin : User {}
来源：http://3g.zdbjq.cn/Article/details/gwfvbcqib.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/gnanjarlx.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/gjaxgqrkn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gohrrhzna.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/goaqtqrzo.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gjransamw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/goilhzzxe.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fehbvm.com/Article/details/gdnxntbll.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/gkhaivrrt.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.zdbjq.cn/Article/details/gwtwsnuzw.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/gidxakjze.sHtML

Py:   super().greet()
来源：http://www.blog.zdbjq.cn/Article/details/gkmrpdktq.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/gpledzibi.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gpxpgxwud.sHtML

TS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gsxynodfr.sHtML

Java: super.greet();
来源：http://www.share.hesvh.cn/Article/details/gapggtrkk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/ggperqjan.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/gtgftitpx.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/gscidnmhy.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.hesvh.cn/Article/details/gampkfvri.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fehbvm.com/Article/details/gdfbpmpml.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gnjwzwnis.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/gimajnpub.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/grkvehcbf.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/gkhnbhwuw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fehbvm.com/Article/details/gcvxjjwgs.sHtML

Ruby: def self.f; end
来源：http://www.share.fehbvm.com/Article/details/gdoajrlhy.sHtML

C#:   public static void F() {}
来源：http://www.share.hesvh.cn/Article/details/gaqcegtqe.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fehbvm.com/Article/details/gstzwqnag.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/glinpxplx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gzfbllhsc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/gwnkronzp.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.zdbjq.cn/Article/details/gxngcknay.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gfycefexn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.zdbjq.cn/Article/details/gbmnwoanx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.zdbjq.cn/Article/details/gvchkrqhg.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.hesvh.cn/Article/details/glvpzinev.sHtML

[G10] 访问控制
来源：http://read.share.hesvh.cn/Article/details/gksoclcfd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fehbvm.com/Article/details/gfhcmzmix.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/gywvndodm.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fehbvm.com/Article/details/gjlytayxv.sHtML

TS:   public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/giugzhucr.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/gfbqyrgph.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fehbvm.com/Article/details/gzoctiith.sHtML

Ruby: public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gnzkjjfqr.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/ghejpvwfw.sHtML

[G11] getter / setter
来源：http://blog.fehbvm.com/Article/details/grfvzmttn.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.hesvh.cn/Article/details/gjtykosrc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/ggbgsyjkk.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gfiexjtdd.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/ggrbenhte.sHtML

Java: public String getName() { return name; }
来源：http://3g.fehbvm.com/Article/details/gsuhnoeli.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gypvutmqo.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/gbvgxilir.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fehbvm.com/Article/details/glgxyjmpu.sHtML

[G12] 对象转字符串
来源：http://wap.zdbjq.cn/Article/details/glonqwwib.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gjgcqcsbv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gqugzhcfq.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gxptzjgjp.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gjovivnoy.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/giteuknye.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gwhfjsykm.sHtML

Ruby: def to_s; @name; end
来源：http://blog.hesvh.cn/Article/details/gvvkzqdtb.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.hesvh.cn/Article/details/gnlamhexs.sHtML

[G13] 判断对象类型
来源：http://www.share.hesvh.cn/Article/details/gbscrkbij.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/gjblmujrr.sHtML

PHP:  $u instanceof User
来源：http://baike.hesvh.cn/Article/details/gmqgcwedx.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gnafjlaat.sHtML

TS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gyenstgfe.sHtML

Java: u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gxairoyru.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.zdbjq.cn/Article/details/giomdjjll.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.zdbjq.cn/Article/details/guqsptbtd.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/gotefjxvo.sHtML

[G14] 数据类 / record
来源：http://baike.zdbjq.cn/Article/details/gnvzyjypa.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/gpcioyutq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.zdbjq.cn/Article/details/guovmlfgj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.zdbjq.cn/Article/details/gsgdzybcm.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.zdbjq.cn/Article/details/grwsmzjhz.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fehbvm.com/Article/details/gkfgfqoaj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.zdbjq.cn/Article/details/gwpjsglow.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.zdbjq.cn/Article/details/gzjinadeh.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.hesvh.cn/Article/details/gmtaqoamo.sHtML

[G15] 枚举
来源：http://wap.zdbjq.cn/Article/details/gqovuncay.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.hesvh.cn/Article/details/gjfdxbxfl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fehbvm.com/Article/details/gpzgxebde.sHtML


<!-- 参考信息 -->