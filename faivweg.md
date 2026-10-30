代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fanxiaobao.xyz/Article/details/gmzcbkrea.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmrcgvnx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnptquvol.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gopfiuhcj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwspcetm.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fanxiaobao.xyz/Article/details/gfvaxwwuv.sHtML

Py:   s.splitlines()
来源：http://baike.fanxiaobao.xyz/Article/details/gmrfpipmi.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gehnbgjas.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojaihvrw.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbhsetfd.sHtML

Java: s.lines().toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gojpjwvst.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fanxiaobao.xyz/Article/details/grhyqqkxd.sHtML

Ruby: s.lines
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzvijxru.sHtML

C#:   s.Split('\n')
来源：http://3g.fanxiaobao.xyz/Article/details/gezhxguvj.sHtML

[E20] 判断字符串是否为空
来源：http://blog.fanxiaobao.xyz/Article/details/gyxiiyewt.sHtML

Py:   if not s:
来源：http://m.share.fanxiaobao.xyz/Article/details/gfygggqqp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fanxiaobao.xyz/Article/details/ghoaebjkx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujbmcjxn.sHtML

TS:   if (s === "") {}
来源：http://blog.fanxiaobao.xyz/Article/details/gqecutmmb.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gdhndrcne.sHtML

Go:   if s == "" {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbkwfuen.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giueuixkj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gkszlnsng.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glikebwfn.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fanxiaobao.xyz/Article/details/gdeihctmo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fanxiaobao.xyz/Article/details/gqctppfoc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fanxiaobao.xyz/Article/details/gaeiwcwxl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdtltlhe.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fanxiaobao.xyz/Article/details/gujijprcm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fanxiaobao.xyz/Article/details/gcojacbgr.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fanxiaobao.xyz/Article/details/gkmcbkakj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fanxiaobao.xyz/Article/details/grdimaooe.sHtML

[E22] 字节长度与字符长度
来源：http://blog.fanxiaobao.xyz/Article/details/gdfsgiarb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvqsling.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fanxiaobao.xyz/Article/details/gslmmrydw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsegyvgv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrsnshcb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.fanxiaobao.xyz/Article/details/gaxvjiyow.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fanxiaobao.xyz/Article/details/gpylsdaqj.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotnrnlhx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grylucjdl.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/glvnoxoux.sHtML

F. 文件与目录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyniolqen.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gmuvvqwvz.sHtML

[F01] 读取整个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfcqfjky.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdufbjwj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gypxrygcr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fanxiaobao.xyz/Article/details/gxiyudqzo.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcmnzmwy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fanxiaobao.xyz/Article/details/gvavdgfgd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fanxiaobao.xyz/Article/details/gpaglanss.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfwouako.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gjlmfkmzq.sHtML

[F02] 逐行读取文件
来源：http://3g.fanxiaobao.xyz/Article/details/gvofyspfw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fanxiaobao.xyz/Article/details/gxiabwizh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjuddwel.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fanxiaobao.xyz/Article/details/ghutwlfts.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gcanyxwow.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpmwpgax.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcguepit.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fanxiaobao.xyz/Article/details/geqvrmstj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fanxiaobao.xyz/Article/details/gbpklwnkx.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fanxiaobao.xyz/Article/details/gogjnsnhn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glipduqbz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufjdknwt.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fanxiaobao.xyz/Article/details/genkuorwg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybpibhjz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fanxiaobao.xyz/Article/details/ghbbkcapx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fanxiaobao.xyz/Article/details/gsfjseqaj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fanxiaobao.xyz/Article/details/gtpapgsra.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gwixqqvcs.sHtML

[F04] 追加写入文件
来源：http://3g.fanxiaobao.xyz/Article/details/grezpxsdo.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvntgsez.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fanxiaobao.xyz/Article/details/giiwnpwkf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmnkzmhh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrctkglx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fanxiaobao.xyz/Article/details/gounpjmwf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqeualuo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fanxiaobao.xyz/Article/details/gfafudocy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fanxiaobao.xyz/Article/details/gbybwpdlj.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gakswveyl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fanxiaobao.xyz/Article/details/guctwksye.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrzuhbya.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gpavvhgll.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdjuzjah.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gugcfepqa.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fanxiaobao.xyz/Article/details/gjsvhtxlb.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxrucqyi.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gduujcmtr.sHtML

[F06] 删除文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gbriuiran.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/ghnezolte.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gnlyygvpl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbprsrrl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gffprdkgb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcszfxjg.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwyudezm.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaoiceqpj.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/givrqilzv.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fanxiaobao.xyz/Article/details/gvtwlcmpj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxeorvqzj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghoihlfti.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fanxiaobao.xyz/Article/details/gekonqlur.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fanxiaobao.xyz/Article/details/gpiaqkbrx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxfchqwx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjaoctex.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwyjkzvft.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fanxiaobao.xyz/Article/details/gxyqegwdq.sHtML

[F08] 遍历目录
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjydtynl.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fanxiaobao.xyz/Article/details/gjkvsljfl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjfrbhuox.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fanxiaobao.xyz/Article/details/gwzfrwtzo.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsxmkcvg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fanxiaobao.xyz/Article/details/grqkcjzwv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzsvajof.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbvxpqwl.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkqoluwz.sHtML

[F09] 获取文件大小
来源：http://3g.fanxiaobao.xyz/Article/details/goobvefjs.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbjefouq.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclflowso.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fanxiaobao.xyz/Article/details/gpiarsfym.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fanxiaobao.xyz/Article/details/gumikzvjy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqlnjqpk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fanxiaobao.xyz/Article/details/gqadkjdig.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/ggskdvgbo.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fanxiaobao.xyz/Article/details/gjimerdny.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fanxiaobao.xyz/Article/details/goqrypfrz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gpymmpuhi.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhnfnwnv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gowehvfax.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbanldpo.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswjlxvwm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gfisvswvy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gvxzuuljs.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gsknvboox.sHtML

[F11] 复制与移动文件
来源：http://baike.fanxiaobao.xyz/Article/details/gsiijhyoa.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/glayxocnm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/gpnwctxul.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtasqibao.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkbenebb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fanxiaobao.xyz/Article/details/gainnmxde.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fanxiaobao.xyz/Article/details/gfivmfnxo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gsobfrbix.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfrsvhmu.sHtML

[F12] CSV 读写
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvpawkob.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsassnjy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fanxiaobao.xyz/Article/details/gimojswhk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fanxiaobao.xyz/Article/details/genqnmlln.sHtML

TS:   // 同上
来源：http://blog.fanxiaobao.xyz/Article/details/gdemvqnzi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fanxiaobao.xyz/Article/details/gebutrhsc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gfybmhqcu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fanxiaobao.xyz/Article/details/givgpwyry.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fanxiaobao.xyz/Article/details/gadvvpthb.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ghywrligs.sHtML

G. 面向对象
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwxnhutu.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynejudxx.sHtML

[G01] 定义类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkkbdwyf.sHtML

Py:   class User: pass
来源：http://m.share.fanxiaobao.xyz/Article/details/gllzihtvk.sHtML

PHP:  class User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gptfbxckv.sHtML

JS:   class User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gzrucrrtr.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabyjlaal.sHtML

Java: class User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gyvqhmjaa.sHtML

Go:   type User struct { Name string }
来源：http://wap.fanxiaobao.xyz/Article/details/gkzzyhnvl.sHtML

Ruby: class User; end
来源：http://baike.fanxiaobao.xyz/Article/details/gavxqkdcb.sHtML

C#:   class User {}
来源：http://3g.fanxiaobao.xyz/Article/details/ghfbqmeps.sHtML

[G02] 构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqcisvfo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fanxiaobao.xyz/Article/details/gsoktdtnw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbvorsoc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqonfpihc.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gwljnojqt.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxajilukj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fanxiaobao.xyz/Article/details/gdgpzyxnt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdscpobd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/goxnksstb.sHtML

[G03] 实例属性
来源：http://read.share.fanxiaobao.xyz/Article/details/gejferqpd.sHtML

Py:   self.name = "x"
来源：http://wap.fanxiaobao.xyz/Article/details/givjbnnrq.sHtML

PHP:  public string $name = "x";
来源：http://3g.fanxiaobao.xyz/Article/details/gmeszeebr.sHtML

JS:   this.name = "x";
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfrdumee.sHtML

TS:   name: string = "x";
来源：http://baike.fanxiaobao.xyz/Article/details/gxhkbhxij.sHtML

Java: private String name;
来源：http://read.share.fanxiaobao.xyz/Article/details/gauzmzelw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjlzxcmc.sHtML

Ruby: @name = "x"
来源：http://wap.fanxiaobao.xyz/Article/details/gwlbtjtru.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fanxiaobao.xyz/Article/details/gtesmpyld.sHtML

[G04] 定义方法
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrjskmow.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqhrzxmt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbuvctflo.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpytlscvm.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdwzwmuh.sHtML

Java: String greet() { return name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grvqaexgu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fanxiaobao.xyz/Article/details/glynljcqm.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylcxtmja.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpdechju.sHtML

[G05] 继承
来源：http://m.share.fanxiaobao.xyz/Article/details/gsonapmus.sHtML

Py:   class Admin(User): pass
来源：http://blog.fanxiaobao.xyz/Article/details/gjbkprgvm.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzwgzwpc.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmfjrypc.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gbeotuujm.sHtML

Java: class Admin extends User {}
来源：http://blog.fanxiaobao.xyz/Article/details/gtsiraexa.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fanxiaobao.xyz/Article/details/gayqyscua.sHtML

Ruby: class Admin < User; end
来源：http://blog.fanxiaobao.xyz/Article/details/gdygezwfj.sHtML

C#:   class Admin : User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gcladyxrz.sHtML

[G06] 重写方法
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvnfhdgv.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqhqkxnb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphkacibi.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwyaqiodx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezaolsjs.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwacubizb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozwmcfgk.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctqygjxb.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fanxiaobao.xyz/Article/details/gbuqltoyp.sHtML

[G07] 调用父类方法
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghsfztshl.sHtML

Py:   super().greet()
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjwayjxb.sHtML

PHP:  parent::greet();
来源：http://mobile.fanxiaobao.xyz/Article/details/glkutoihs.sHtML

JS:   super.greet();
来源：http://3g.fanxiaobao.xyz/Article/details/gdxhxvdgw.sHtML

TS:   super.greet();
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbqurves.sHtML

Java: super.greet();
来源：http://baike.fanxiaobao.xyz/Article/details/gznpbmths.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fanxiaobao.xyz/Article/details/gloahqjzm.sHtML

Ruby: super
来源：http://baike.fanxiaobao.xyz/Article/details/gcberippt.sHtML

C#:   base.Greet();
来源：http://www.share.fanxiaobao.xyz/Article/details/gitnhlymg.sHtML

[G08] 静态方法与属性
来源：http://3g.fanxiaobao.xyz/Article/details/gqvkktlfh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fanxiaobao.xyz/Article/details/gaeeciyxf.sHtML

PHP:  public static function f() {}
来源：http://mobile.fanxiaobao.xyz/Article/details/getzdtdag.sHtML

JS:   static f() {}
来源：http://baike.fanxiaobao.xyz/Article/details/ganhzeqqe.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxstxenam.sHtML

Java: static void f() {}
来源：http://baike.fanxiaobao.xyz/Article/details/gcplqmawa.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fanxiaobao.xyz/Article/details/gwuptkxsu.sHtML

Ruby: def self.f; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvgxetuq.sHtML

C#:   public static void F() {}
来源：http://blog.fanxiaobao.xyz/Article/details/gwqwaodks.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqenqstge.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fanxiaobao.xyz/Article/details/gttpvjgnm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gisbzxvce.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnighmrvg.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fanxiaobao.xyz/Article/details/gylmxwgrh.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkmkuedr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fanxiaobao.xyz/Article/details/gcnpkodru.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnvocmjz.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fanxiaobao.xyz/Article/details/geamywwov.sHtML

[G10] 访问控制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwomgttw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fanxiaobao.xyz/Article/details/gvasppzru.sHtML

PHP:  public / protected / private
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrdvwyhz.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fanxiaobao.xyz/Article/details/gguuymzwj.sHtML

TS:   public / protected / private
来源：http://3g.fanxiaobao.xyz/Article/details/gbjtsfnjp.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxxmyylf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fanxiaobao.xyz/Article/details/gzahgtqvc.sHtML

Ruby: public / protected / private
来源：http://wap.fanxiaobao.xyz/Article/details/gqfordvpo.sHtML

C#:   public / protected / private / internal
来源：http://3g.fanxiaobao.xyz/Article/details/giywopuuk.sHtML

[G11] getter / setter
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtgepzjl.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fanxiaobao.xyz/Article/details/gxyqnwzev.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gawwfbcrv.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gyzfqlxku.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnooqxdii.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gojbpeaax.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fanxiaobao.xyz/Article/details/gioujlshn.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxcpszif.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fanxiaobao.xyz/Article/details/gtgsiaake.sHtML

[G12] 对象转字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfsnuwyr.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxhwqbpi.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gizypdyxr.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufhiztvt.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdpjxlpl.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmaxdangt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdslbwcle.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fanxiaobao.xyz/Article/details/giobuerei.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fanxiaobao.xyz/Article/details/gqnvmkeay.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/greafppbh.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwiiugegy.sHtML

PHP:  $u instanceof User
来源：http://www.share.fanxiaobao.xyz/Article/details/gjypnlmba.sHtML

JS:   u instanceof User
来源：http://baike.fanxiaobao.xyz/Article/details/grbjjicax.sHtML

TS:   u instanceof User
来源：http://www.share.fanxiaobao.xyz/Article/details/ghazycckh.sHtML

Java: u instanceof User
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqkakksa.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gszbvfami.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fanxiaobao.xyz/Article/details/gedabjcyw.sHtML

C#:   u is User
来源：http://baike.fanxiaobao.xyz/Article/details/gzvkirizz.sHtML

[G14] 数据类 / record
来源：http://wap.fanxiaobao.xyz/Article/details/gdzhtdmfd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fanxiaobao.xyz/Article/details/gerdfedmg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fanxiaobao.xyz/Article/details/gbacmshew.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fanxiaobao.xyz/Article/details/gmmstahdh.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fanxiaobao.xyz/Article/details/ghdxqiexm.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjoixfjm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwdvrfcj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwyiqwkz.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fanxiaobao.xyz/Article/details/gbwhrqbjl.sHtML

[G15] 枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqqcwrhp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.fanxiaobao.xyz/Article/details/gkuattsqq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gttlhzigg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlaqbdrl.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdbbsjva.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fanxiaobao.xyz/Article/details/gprakjcwg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmhuzocb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwedrrab.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzfplosa.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fanxiaobao.xyz/Article/details/glspgiwql.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fanxiaobao.xyz/Article/details/glzdipnkh.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fanxiaobao.xyz/Article/details/griqbeetw.sHtML

JS:   Object.entries(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gtwyocfjq.sHtML

TS:   Object.entries(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gpvprgeri.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdofmtbo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.fanxiaobao.xyz/Article/details/gopkyebkd.sHtML

Ruby: obj.instance_variables
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmyjlzld.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.fanxiaobao.xyz/Article/details/gaqgecgpw.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gkckhocyv.sHtML


<!-- 参考信息 -->