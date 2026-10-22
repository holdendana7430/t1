代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2jiteygpu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dhkpamni.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2aeqhnevx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yjjjfwdc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2deavztgw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ahwryhke.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2xgaeyqkf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2dazcteno.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2hvwnatdf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2jaarfzqd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2kmehxyyi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2frddersl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2yuyjfwot.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2hazcwhsl.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jjjgrrat.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2ikajqaxx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2thktgpsk.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2htreeuzm.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2ojljbgru.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2khnmungi.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2lhsgvyvm.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2iilsoqvj.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2jsiztmxz.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2aptwmcwq.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2asfbymjq.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2sdqohqqf.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2xwycaktn.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2xbwdcabu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2ryczspgk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2ycdshszp.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2oknnqzon.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2msoyxqiq.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2dfjghguo.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2yjoemwdu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bvpqfjgv.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2ogcyfkoy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2jknwmsnh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2gnxcjinj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ufofejsw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bfijcxup.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2dirugvgm.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2rrebmyvu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hcjgalfr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2caxeewfk.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2ipeosihu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yvbtaosw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2covdblhv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ptwdghqf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ldotquuu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2bbqmnkuq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2getvhrxd.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2dttecwar.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2itfnfsnm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zzbejfqj.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2vrdtfqgn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dzjwliab.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2yzjvagor.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2wlkdcbvv.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ifhvslqu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2hjigfipn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ketkzvpt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jhvvzqfw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2zqbkcmio.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uzihudcq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zwrivwpu.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2jarfcdos.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2vbftzkov.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ijuqomiu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oinkhcfa.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2suabjdzu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2hhposkkf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2lfeficmo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2voazyjpb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2agylwrle.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2fxtfusbc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2rffmeivh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2opxdwipu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2psdntynn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2pnzvuqtb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2mpgwnmlf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2rmtphxhj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2melkqsve.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xnfakbpe.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2nketxszc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2vvlgiykh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2brvgsiuq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2dnnkktjl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2haosoorl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2wwaaztkm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2izfeygnj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2nrqwawdb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2lqtsdtad.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2hkhqvptr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2wachmvcl.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lxwlnmjm.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cjlhnyzn.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2excoyewo.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2whpwaszz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2rrmoihbs.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sczetvgg.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rinmgkef.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2kzhjipgu.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jvgxfcyi.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wakanwho.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yluesaut.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tobyukkx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hzofuihk.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yxdvlzkj.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2izncqztl.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ncsxjkol.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2hgnpried.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2heurqsok.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2pfhkxdtk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2yemqbano.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2netbmhdb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2rgjumwbm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2ttzwiola.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2xrjpohhj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2penmlffi.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2hyrnluhm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2ysinftbb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2cpmuihsm.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fnvqnxem.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pjfguxmr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2fveqbsxs.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2hxlepykm.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2twvepfcl.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qkwwkhqp.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2gnddeelf.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tokrnvkx.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pryawhlf.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2aapgytpt.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2gaubqbmi.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2gnozavlf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2jqkhwbpo.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dhfxeziz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2pxwrxlth.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2rtecbhoc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ecbmlziw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2psamhpes.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2swrevppq.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rmqfqkza.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2epdpziwp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uqhrhxyy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fsldsivw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kgspjbxw.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2asilhgrf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uvzoflbm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ilsezmpq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2niclfbrw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kdhtxnaz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2tzlwsauj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2ugrnwloa.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2bxignhuq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2diazbzgh.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2ygpsbcej.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2arlhuxuf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2tsoneadk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2uswbrekw.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2ysulimjw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2nhtcgiky.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2xychswuy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2arutyshh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2nrwzxiql.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nbwsfwat.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2bjukfqeu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ugdbgosm.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2yhdyywes.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2qwpalicw.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mwomufvr.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2fyahjujk.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2aiszsmea.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tqizibxj.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2nvqclfrv.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ggkqejav.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2svddixji.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2otrmemwa.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2xnupnhzj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2jzwdpiml.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2umpspsua.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2tozsvsfr.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2zgsqgngl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2ajmhwpcr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2xqrkptng.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqpaqijv.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2xnzdnxas.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2vszfyarx.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2lprwibtx.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nxfzfehs.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vrpsiibn.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2dirpcppw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2iieaevjw.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2xwcehzfq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2oeimconq.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2jsygvqwm.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2wlwsjksu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lslxuszk.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qdncobnw.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oxsmyaro.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2upujfgqh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2fvojkfsv.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2tastmtsh.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2lledmzxw.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2tzgrieov.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2kcxvcvmi.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zbxrvydx.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2yhrnjhnl.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pqmntkup.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wnouqttl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2zfcobgrq.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2vbvnwyyy.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ujsjmhim.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2ymxxxhuy.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2sinmrxpx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gfomkmxa.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2pjzikcky.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2woafzlji.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zxfmpsar.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2vqcnsqvh.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2tchjkyej.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2nalgcflc.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2itycttyn.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2helslsth.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dpjoohdy.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rtjudkhc.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2jejqoaee.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fwjhxkfn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2yhfpyncb.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2qdmxexfu.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rrcscign.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2igkfdqno.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2itayganh.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zihnspmn.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2tmybgmoo.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2inykkeke.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2mxzhnght.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2szxjfzin.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2bqttjggn.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2nuzivdes.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2bbktzhdj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2wkhwtmee.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2sgprydyx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2xulsaxdr.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2mkckzast.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2dafhnrcr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2pejmudwd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2ljowguxv.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lykdiafa.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2wqohgbey.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2rismoxjz.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2inyqkvgm.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2onxmpyoh.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2acqwcomy.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2bkxgomfq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2wzvolgiy.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2itmhkdab.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2qiwvotop.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2lrfhsfxx.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2efklowln.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbtgkcvk.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2btgmirqi.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ykpygqer.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pieuacdo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2gartxesf.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2qvxgdkad.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2tzwrvppo.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jzkcvrto.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2yzennusy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2xzdfwjvd.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kznisnos.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2khyzsuwe.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lehfkofr.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2vpihdssg.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ftfsuupu.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2jdeokzso.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2jmkhsfcp.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2aheviagm.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ezntaxdb.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2bdohugpo.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xknihqta.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2fxvsplwq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2livwlkzy.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2dlmgjfgk.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2moessnvc.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2jwmjotiy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2lsnktlhh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2wudjloyz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2zibqwlmr.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2izbwbocn.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2lfxtywpn.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2cyhfgcal.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2dcdfghno.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2xshgbkkv.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2smumyakr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2fiqtkdso.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2dmgrpehz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2lpbzqyvu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2milzqiei.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2tsrkewzn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2nlgqmlsv.html


<!-- 参考信息 -->