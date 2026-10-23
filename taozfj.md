代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3qkewmwbb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3eglqexqa.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fiioqxls.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3dlyuxhgn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3riqusdwc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3jgwpwmyv.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3wuzlwbzu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3vxyxcxwh.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3waoubfng.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3wvohjugb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3lulvqhpm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kwsiixqt.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zgmtqrud.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3sghylbsa.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3wiynsyxn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3rowmvijt.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3anclhwdb.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3ihjxsoyx.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3irezvpfj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3gttfdnjp.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3rofjiwse.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3baaryhob.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3rhljeaas.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3gciiodfk.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3dvwkasdl.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3wratxpdv.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3cjmaepiy.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3sfsqpxsd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3fwycsjsb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3jaqgcsni.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3ptwdogaa.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lmmelfhr.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3ubnwwzdk.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3lkrubhcc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gzbiwvzd.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3csbppogi.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3inzryzov.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ntwjfesx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xmuhepcz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zdgukswe.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3crowirtn.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3vomtomnh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tbtwssku.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3agiwuaqe.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3hffvzsjy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3rngrfrmd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qbdxbslj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3cofaxuic.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ovwcrjkh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3zvqehmpi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3sgcharqq.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3wbkwfihs.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3knyyyvia.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nsvojdow.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3akxfuxxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3arhecjhx.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3tezxudqv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3cnwmbsrp.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ekqnxldu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3tmhyfgrl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3occppsvp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ariheicd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3brcdrqzb.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dktwqgmb.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zqvpawmr.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3buwygewh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3tcarpdvj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3vrddyhnu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3wgqtssuv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ckxyfksf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3bgpbglbv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3fcgsgnfm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3xidfdrwx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3fwjyffku.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3owwpkpvh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3jsgisxtk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3yntbmrdv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ivwhgmsb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3pcufoije.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3spifhwkr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3spiyslvf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3pvxqytqa.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3egystrru.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3vkwblbuw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3acdlhxuz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3ujcjhmdx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3tbjzdwsl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3bydlkgos.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3vnttlpgk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3isvdnnaf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3vpmfpqnr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3vrqogcmy.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3azzlizip.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3pgmayljo.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qvrnwclu.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3azsncziu.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xudnpzlj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3luscbosi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3bwhymzow.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oguvabed.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wasbrzfa.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3byadomom.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3evghzxrm.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3iwgvpgii.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aahmfjne.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oxyqqaiw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vjpwxbot.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ugrabdnp.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pvimucny.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qdfzqtue.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3oukjighu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zporafmb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wfgqwmqt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3whgedlrr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3mehierhl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ihgzhagj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3tgwronza.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3mdocqbap.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3ogcoaexy.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3tstymewh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3cxbjwdtx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3oqunoctf.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3tzxqgmyn.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3wfgoonld.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3qdgttylf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kycapaxn.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3hpqetozz.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ulvedaov.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3aaenhcwj.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lihcxwpk.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qonvvpcu.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ufuhiufs.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3qfbsdfuc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3yewmldce.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3ldkjjxew.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ffmadpll.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3doqgaboc.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3xfqqjkgm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zojijpjz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nfmmnfbl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rkdrcwzt.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3suglqiqu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3mpbwxwcy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pwzxboju.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rkqxwpeh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3viueyomd.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3yjcmphbn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3lzhlrdhq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3xpwhcpei.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3geqknlsm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3begyzzev.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3tgsavhzw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3cjqthsqk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3jktamhlm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3ahctshjx.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3acotxtqf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3vrbbjacj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3yrrhknbo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3pfjgsoyj.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3cnklzyin.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3drkxdgbt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3gxmtvwko.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3xtnvepfi.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3fpbwkkvc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3edyfssop.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3hmaxxlqx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ddoatqao.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3qyrrctve.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3mtbauztf.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gsonredp.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3edatdyfr.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3qgyfesbe.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3emtiohbo.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3zvakcuoz.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3ccyrfrxz.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3exuglhve.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3kgipszvo.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3ormhsehw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ngdwclew.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqdzcvjs.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mxzfyyrl.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3meazvlwk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3ifmjelbi.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3zpyoihgm.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jnvbfwhq.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3qytwyzls.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3anmwtzjy.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ocfppaqb.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3vtlfuutb.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3yecdmlmv.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3ltfusvmn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3lkaqkdez.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3pguccieg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vaqnmubd.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3atxogayy.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3qxorjwws.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3azogquis.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qncwzvtp.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zbnbmyjy.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dcvfflta.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vyucaauc.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3qeeyoyrp.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ycbftkvz.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3ddnjppgm.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3zbeykevx.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rcyyabel.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zsqqhydx.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rxydwado.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3aguxrmlk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3yypxqvwe.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3sqrohugz.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cjakvibz.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3nhkveyzi.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3ylmprjyp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3nfwsrtsw.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ddgrccrq.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zaqvbvfn.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3bticonqv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3dmcdhydl.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3zpnooylx.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3qzbjlsin.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3xdhzyyej.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3cwfysguq.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dmamzfem.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hyswtaod.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3kgktflrk.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gfakdlal.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3xvwivpyp.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3zsyshzge.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3mtxekioc.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3tqoovlob.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3lovrkxwh.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3hnroxuqm.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3iswmlrcy.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3txtmkhhu.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xjiqlswu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3mzuuekwx.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3hfgscpks.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3opmsnhba.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3wvmwmcfa.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3nbzbtfbx.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3rbfcynjv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3jtdujkaj.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3vpkqadqe.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3xwbwfvtq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3omjgnfwm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3qjfiqfkj.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3ssmhqiqx.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3swbmeqsj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3cczdfiov.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3tixetzlp.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3puehljfz.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3iqigafid.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3csjqtuvg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3xmyugvsf.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3rzegpyfz.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3egskjghk.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3idgojbwh.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3gdlzqkke.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uokbzscm.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3fblzhszd.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3wdjmouqq.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jbwqczfk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3jqpwaduf.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3nedupbex.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3mmaomtro.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3zwbohzqh.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3qthwkxij.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kznjoqks.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kgikoyhr.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zkaaejue.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ziqnxujb.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3zmfeduiu.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3mhtpfuvw.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3zvciytvn.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3anrpvjxe.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3ksgehwiy.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xcrnfqvh.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xkoustlb.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3eaifgbwc.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3aswmhdki.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3ptrspcln.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3qboofnio.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3euqfsczt.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3ptzwpycz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3sumypkcl.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3pjjzrbnm.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3sjorjiqq.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3flrnbgzn.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3dgspyglp.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3jfdzlqkz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3yptpabzb.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3ndrnvitm.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3zvtycbdi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ascfxwvz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3psirtrhj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3bqjubbau.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3xutxewde.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3eannjtzz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3rtfulpgt.html


<!-- 参考信息 -->