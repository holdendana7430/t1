代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gfzgyprnb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.zdbjq.cn/Article/details/gmsvibtri.sHtML

Ruby: s.capitalize
来源：http://blog.fehbvm.com/Article/details/gxzklafji.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.fehbvm.com/Article/details/gjdfcwjqn.sHtML

[E18] 模板占位符替换
来源：http://mobile.zdbjq.cn/Article/details/gbcrzgkpj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.zdbjq.cn/Article/details/gzfcwbljc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fehbvm.com/Article/details/gpxduebwm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gtamkhypx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gjslamsfj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gjwtelzyc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gwxrgwebb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fehbvm.com/Article/details/gitzogozv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fehbvm.com/Article/details/gpawweukb.sHtML

[E19] 多行文本按行拆分
来源：http://3g.zdbjq.cn/Article/details/grykuviqv.sHtML

Py:   s.splitlines()
来源：http://3g.hesvh.cn/Article/details/glsvlaakm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gvdjvllga.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gcsxawlwf.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gvfmsgezn.sHtML

Java: s.lines().toList()
来源：http://www.share.zdbjq.cn/Article/details/gnjxxcsur.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.hesvh.cn/Article/details/grsdwrfnf.sHtML

Ruby: s.lines
来源：http://www.blog.fehbvm.com/Article/details/gimnvrzhs.sHtML

C#:   s.Split('\n')
来源：http://wap.zdbjq.cn/Article/details/gxhjiscsy.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.fehbvm.com/Article/details/ghqzdopgo.sHtML

Py:   if not s:
来源：http://wap.fehbvm.com/Article/details/glnortzzc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.fehbvm.com/Article/details/geuftlfcf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/gnokqprbb.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/geqtithkc.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gazjyukay.sHtML

Go:   if s == "" {}
来源：http://www.blog.zdbjq.cn/Article/details/gltppotdc.sHtML

Ruby: if s.empty?
来源：http://baike.hesvh.cn/Article/details/glnjcufhx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gzqbqwcur.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fehbvm.com/Article/details/glabpyabi.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fehbvm.com/Article/details/gwznmbnec.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gxwxwcutv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gajsrbahz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gllzdfpmc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/ggpadhsvn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/gkmwctklc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/glquvpvch.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/guncjmeyc.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/gwzysgbac.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.hesvh.cn/Article/details/gdwzmtewf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gcsoafmso.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/guoxjmmjg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gdcgpxvyy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fehbvm.com/Article/details/gfwpcnewu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fehbvm.com/Article/details/gajhhegkr.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.zdbjq.cn/Article/details/glrxkrmrw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.hesvh.cn/Article/details/geblgyses.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmmaoayjd.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/gomnqxyqt.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gcpvwktqw.sHtML

[F01] 读取整个文件
来源：http://wap.fehbvm.com/Article/details/glfwavaao.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.hesvh.cn/Article/details/gygjnprul.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.hesvh.cn/Article/details/gemgyjazf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.hesvh.cn/Article/details/gexbpomla.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/gdjjhdykm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gcudrawvu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.hesvh.cn/Article/details/gtmeixwwv.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gtlkpktqx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gzrqewkhj.sHtML

[F02] 逐行读取文件
来源：http://blog.hesvh.cn/Article/details/gmgszehxg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fehbvm.com/Article/details/gyxnggwca.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fehbvm.com/Article/details/gblnyoyur.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gmbthjtqk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/glwxycqqe.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gtpuixmai.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.hesvh.cn/Article/details/gwrkpmely.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.hesvh.cn/Article/details/gkrrqmjtf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.hesvh.cn/Article/details/gzruwkldo.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.hesvh.cn/Article/details/getrqdaii.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.zdbjq.cn/Article/details/gnnzrgnnt.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gkxktakeb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/geiktynzd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gmsrvliuj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fehbvm.com/Article/details/gzgzbikiw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.zdbjq.cn/Article/details/grejzdryx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.hesvh.cn/Article/details/gbetzivjh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gexjambgi.sHtML

[F04] 追加写入文件
来源：http://m.share.fehbvm.com/Article/details/ghgypftcq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.hesvh.cn/Article/details/gydchcald.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.zdbjq.cn/Article/details/gvcjofkxy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gjxjvqqic.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/guwyldigk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.zdbjq.cn/Article/details/gpevlekow.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gqqikmtwi.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/gxpixhbad.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fehbvm.com/Article/details/gqpgenngn.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fehbvm.com/Article/details/glupiklwt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fehbvm.com/Article/details/gwekbebdl.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gtswlfoax.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/guzcnaqsb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gclzizxen.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gvqcxxgng.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fehbvm.com/Article/details/gctpucwyw.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gpxzaqwec.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.zdbjq.cn/Article/details/glfkiifwm.sHtML

[F06] 删除文件
来源：http://mobile.hesvh.cn/Article/details/gzhotpwsj.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gwwepigmm.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gfmhwazvu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/glrnjsxsi.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gufpktcki.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gwnqxkxnh.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/giwmdxdnb.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fehbvm.com/Article/details/gymyjqlwg.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fehbvm.com/Article/details/gayphpivg.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fehbvm.com/Article/details/gudbfybjf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gxsnjnwlu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fehbvm.com/Article/details/gamydguet.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gblqoyspz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gupglkoxf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fehbvm.com/Article/details/ghdcqzwgy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/gbedfczyy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fehbvm.com/Article/details/gnbraynop.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.hesvh.cn/Article/details/grxyiskpa.sHtML

[F08] 遍历目录
来源：http://wap.hesvh.cn/Article/details/gpdsvgxnz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fehbvm.com/Article/details/gollzhedd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/gfdrdghim.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gpbdgywnz.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gdhvfqkzt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gbvrfawza.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.zdbjq.cn/Article/details/gwrbiiiqn.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fehbvm.com/Article/details/ghnkmsqxx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.hesvh.cn/Article/details/gfdkpfvaf.sHtML

[F09] 获取文件大小
来源：http://3g.hesvh.cn/Article/details/gjnllkyjj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gsrndzhru.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fehbvm.com/Article/details/gapegpkha.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gqamdlmfw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gevijqnjg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gkzrewruj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.hesvh.cn/Article/details/ggelthedf.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gffmltrly.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fehbvm.com/Article/details/ggtgmfvnj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fehbvm.com/Article/details/girvszhak.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gyqpudzid.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gajecbkpd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gjprgkiie.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gwolpcbut.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/gyanjnrdr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gwczltjco.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gjfjxypgy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gpmlfnzpn.sHtML

[F11] 复制与移动文件
来源：http://blog.hesvh.cn/Article/details/gghsiglsu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gumyywrfc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fehbvm.com/Article/details/gpaypzmcz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gsdewbgmn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gzgtbblbs.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gmvrmnlvh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/gcklpxmzu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gbvhctrsq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/gxqiajghe.sHtML

[F12] CSV 读写
来源：http://www.blog.hesvh.cn/Article/details/gwxukajxv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.zdbjq.cn/Article/details/gtfziqmpm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fehbvm.com/Article/details/gjsgksbjc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.zdbjq.cn/Article/details/gdvatepdu.sHtML

TS:   // 同上
来源：http://wap.zdbjq.cn/Article/details/ggekvukgi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.zdbjq.cn/Article/details/ghdjzxikk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fehbvm.com/Article/details/gwnuyxpgk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/gupupnwxh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.fehbvm.com/Article/details/gqfjurskt.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwgruvlsz.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/gbchiqxcj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghjmnlesg.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/gdhcxxfxf.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/guikrymxk.sHtML

PHP:  class User {}
来源：http://mobile.hesvh.cn/Article/details/getaqcqie.sHtML

JS:   class User {}
来源：http://baike.fehbvm.com/Article/details/gkatuvmzs.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.zdbjq.cn/Article/details/gylkhdkne.sHtML

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/grpklvefl.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/ghquofwbi.sHtML

Ruby: class User; end
来源：http://3g.hesvh.cn/Article/details/grtbddkzc.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbixuhfhe.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/gyjrlrtaw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.zdbjq.cn/Article/details/guxjuqbla.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fehbvm.com/Article/details/gpjbugoox.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/guljmxyzh.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/gyanutcpx.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gunsdxidf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.zdbjq.cn/Article/details/gjoptkusg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/gmcvuxdrv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/gnckechnm.sHtML

[G03] 实例属性
来源：http://3g.fehbvm.com/Article/details/gjksvkpko.sHtML

Py:   self.name = "x"
来源：http://3g.hesvh.cn/Article/details/gzamekiur.sHtML

PHP:  public string $name = "x";
来源：http://3g.hesvh.cn/Article/details/gfrclflje.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/gfkcoxkuq.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/gfvdehams.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/gfivodlwu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/geaqafopt.sHtML

Ruby: @name = "x"
来源：http://baike.fehbvm.com/Article/details/gnfgqpdge.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gcwmpdopd.sHtML

[G04] 定义方法
来源：http://www.m.share.fehbvm.com/Article/details/gjomdoxwl.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gegvkbwnc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gbqjubuem.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gkpmedxuo.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gjmvnaujx.sHtML

Java: String greet() { return name; }
来源：http://blog.hesvh.cn/Article/details/ggckiifli.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gxmptkbjt.sHtML

Ruby: def greet; @name; end
来源：http://read.share.hesvh.cn/Article/details/giuivbauc.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.hesvh.cn/Article/details/gqfaflpli.sHtML

[G05] 继承
来源：http://www.blog.fehbvm.com/Article/details/gpndrgkxr.sHtML

Py:   class Admin(User): pass
来源：http://baike.zdbjq.cn/Article/details/gdkveudqp.sHtML

PHP:  class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gqvljxrio.sHtML

JS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gtwbwgqdt.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gommuhqkd.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gcoeslnzl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fehbvm.com/Article/details/gznhwrhhd.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.hesvh.cn/Article/details/gznomcjfs.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/gmoherupi.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/gceucfcme.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/ghcoodczl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/getnuogjz.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/goputcnww.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/giohifhab.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gszoitxqo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/ghfokdnhi.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/gxtecwiqo.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/grgyosqch.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/gzrrxishn.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/gqhjbdnxx.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/gkkrnfpuj.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/ghyoxujwf.sHtML

TS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gbzzggysp.sHtML

Java: super.greet();
来源：http://blog.fehbvm.com/Article/details/gseuxdylw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fehbvm.com/Article/details/giewwmekv.sHtML

Ruby: super
来源：http://m.share.fehbvm.com/Article/details/grmueaalu.sHtML

C#:   base.Greet();
来源：http://wap.zdbjq.cn/Article/details/gnmiliuof.sHtML

[G08] 静态方法与属性
来源：http://3g.fehbvm.com/Article/details/gpeoccdnc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fehbvm.com/Article/details/gdckcfxjt.sHtML

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/gmgrbkuod.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/gbcudlhsc.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/gxpmonvzs.sHtML

Java: static void f() {}
来源：http://www.share.hesvh.cn/Article/details/gjiuqtugi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/grfeejtgv.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/giesvbtro.sHtML

C#:   public static void F() {}
来源：http://m.share.fehbvm.com/Article/details/gubzeanwd.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/gghzmowav.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/gsenusmmt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.hesvh.cn/Article/details/gyaanpmgh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/gdjgjcukt.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fehbvm.com/Article/details/gdpcahudr.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fehbvm.com/Article/details/giedqjsjp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fehbvm.com/Article/details/glkwchimg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/gpdoxglyw.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/gzmstgpoc.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/grlxjbsam.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fehbvm.com/Article/details/gudvcjhfz.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gwiqmqjxa.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fehbvm.com/Article/details/gqhjvoatz.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gqhbhfumf.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/gtejfcipy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/ghufmnznp.sHtML

Ruby: public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/ghpohmzas.sHtML

C#:   public / protected / private / internal
来源：http://baike.hesvh.cn/Article/details/gzzdkmvhf.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/gzvuriiit.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.zdbjq.cn/Article/details/ggazsusoz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gycpjhmum.sHtML

JS:   get name() { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/grlpkspnc.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/ggmmroroo.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gzwclywav.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/goyefocxm.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fehbvm.com/Article/details/ggnpgrcmh.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/gobwhthfp.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/gqkaqnjxa.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gwdryirqn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/ghpqgsybq.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gqpzrnbqf.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gzpbksqyz.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fehbvm.com/Article/details/gckjmuybe.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gclqawqvg.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gwfwlonar.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fehbvm.com/Article/details/gqntthtfa.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/gimotiscf.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/glrelggaj.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gstpdgcxh.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/ggxuzziwd.sHtML

TS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gxattmvsq.sHtML

Java: u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gsqhfgjgs.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fehbvm.com/Article/details/ggxbbeyok.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/gnjpbwfeq.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/gbwgmmenk.sHtML

[G14] 数据类 / record
来源：http://blog.hesvh.cn/Article/details/gkngylhnu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.hesvh.cn/Article/details/goyijqtqs.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.hesvh.cn/Article/details/gyunjkmdx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.fehbvm.com/Article/details/gepetbjmp.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.zdbjq.cn/Article/details/gbzmnhgcx.sHtML

Java: record User(String name, int age) {}
来源：http://blog.hesvh.cn/Article/details/goencgcqy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.hesvh.cn/Article/details/gnkuwokrl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/gmajfmboh.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fehbvm.com/Article/details/gmeehzfyt.sHtML

[G15] 枚举
来源：http://blog.zdbjq.cn/Article/details/ghxzeokpe.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.hesvh.cn/Article/details/glumrmksl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/gtjjmszon.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.zdbjq.cn/Article/details/gexthbooy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gbuznwhqb.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.zdbjq.cn/Article/details/gafdoydjz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/ggtwtxgqw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fehbvm.com/Article/details/gngmzutum.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gguzdzcvb.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fehbvm.com/Article/details/ghtqvdfwa.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.hesvh.cn/Article/details/gefzylzln.sHtML


<!-- 参考信息 -->