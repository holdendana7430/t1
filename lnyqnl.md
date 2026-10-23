代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3sjemidro.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3zmuidkqu.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3xrtyarqd.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3lerrnfvn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3qeuygnfe.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tzgcogto.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3rlqyiluq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3xtynkrxj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3eeofmgsp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3mpqdjuxe.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3gncbppdv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3xjxidawi.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3rajtosoy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3iepreeue.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3brvrriwn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3sreqnujc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3pboohqpq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kyoyylti.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3kjdkxnpf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3vwjaiymj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3sxdiqsjg.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3xmisdvye.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3wsqvtdxl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3tvplezwc.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3qxlsdzdw.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3sbdclyvl.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fwxmwafh.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kojdeddk.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3bssgrmzh.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3rusdxzth.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3uoidgukn.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3zqknhchi.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3wfoxfskc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3guctuubd.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3irebzgvp.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3eziktnjd.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3igimadbo.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3jpsgmxrz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3vugurquj.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3vwsgufml.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3gnlrmqog.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3pchnfiwf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3kexmzbva.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3floauyoo.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3iaofihnu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3rjgjizpz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mbsuuweq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wmnlwsxu.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3amicujdt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3mhkalntq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wbqybtws.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ggjdoggc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3khyeebiq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3euqpzcsd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3txxcrjfx.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3kueseupa.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3uphbarml.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3maubbzjo.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3fgpkubjx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eumepbfq.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3kohiwmmg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3zzyyknjx.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rzmfzpeq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3ltmlqhpt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3yjkjrtqo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bvjfzitg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3nehtljba.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ggwevszx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ersbmzri.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3huodaohd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3drngddga.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3xpyinqhv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3epmbpwsp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3veigywgj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3dagywabz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3vawizprd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3qokvsfqt.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3qhbqopew.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3thcrgaex.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3lymvmsvm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3xzagfxjy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3nmbdogkb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3bmzhmyvu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3hfxuprfu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3toupuogt.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3qcbkkrdi.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3awkioqkh.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3hfjktnxu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ivmubopr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3uolovqre.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3rvmsddqf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3pdoymoxy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3waramvvb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dznyqmjh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3adoxbneh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3ndnplxbp.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3ivgatgqb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3ysjibwna.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3eviyflip.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yzqgqnhw.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ryvgwrwa.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3likimcll.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3vkprettj.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jycqyrrn.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3beehjufg.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3wnsyttaj.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xuvcpxsx.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fsijzowg.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3waiuolfy.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nqdltswj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3pcpkbkqa.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wlmkwthe.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zcmhvrzh.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zlcmxpqg.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3jxevdzld.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3hckcmxjr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3okazgxdp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ieinsqfw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3yrnkpyag.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3oulicqxb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3tfrmtsyj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3tysgmppo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3fnlxyosj.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3txjeyebh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3axrguvov.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3xyacgkdp.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3wyqtnwsj.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3cjcvcxbb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3qubndbbp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3gejswgdx.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3iceitauv.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pmzbugye.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3vgolnbjg.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hvvhphta.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sujperje.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3fetwjpts.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3rbgrypye.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3tkegyglj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3neukzdcu.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hjrhbfae.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3rqsjqsvq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3xatzpyms.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zpuupgbv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zbxlwqnn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kerufhep.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3evfieews.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3odvadxdr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jwpmescm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ttkskhix.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3duoxpcql.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3zxskvigq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3udclmqxt.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qcmryhpi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3dqcwlvaw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aaafxjtb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3hturjtwf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3uzosylpg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3bojxxnlv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3gbwcprhw.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3rejqtmdj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3bsazuctf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3alzzparr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3xwveijyr.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3orezlopw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3kmtyzqdi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3ccafwibh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3vyeieixg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3qelrcipt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hvbtwzxd.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3ukciwuiw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fohfbsjo.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3qvkiebyp.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3qfnngbod.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3wedhwedd.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zvkwansp.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3psdlbyic.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3agbgrfnt.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3fvxginke.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3tvkeggpg.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3elqfchhi.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3bkuvqzot.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3fnevnmxe.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3xrqcyehn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gozvaova.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3ikzmlcyh.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sybwuqva.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3dszfkxbw.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3yovmuytl.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cmaoipsx.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3sbkantni.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3cwwdbvof.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3euzzbiio.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3dkyxksfq.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ekygjbrv.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3vmyugdsi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3fimnlkxb.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3kxayaqsi.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3sbugzdag.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3mgucangt.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3fxwsgnht.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3vgntoogw.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ydhfwylj.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3reeegtoc.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vpafrret.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3rzdnrqei.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3zrwirywq.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3zicfyozb.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3ykamsrnr.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ebhqcjba.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xanwvjnr.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3uurkihyk.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jnkbytdz.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3iuucfjev.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3khqjquha.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3qvhtkhlx.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yhtrtdjw.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3xzxnioiu.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3maiswknm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3znbexgzq.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmnaltok.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ssuzhwqu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jkwcndrq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3otbjfkhj.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3signqjho.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3jfxzqpri.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3jjfkrvvo.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3hkymnbyq.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ojfsoyxo.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zkvsacoz.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3jjelnyac.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vpnwcvkm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3mrqxvolg.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3rryhyznt.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ubhgyasm.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3vtrbmodh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3vufgiwlb.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3cxodcifo.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3iiudfuxc.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3zojonrzg.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3fbekbcnz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3gdzskxhx.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3dptgrrzo.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3psiuvjlu.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3adijrgfr.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3xygyddjx.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3kfkkocbs.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3zhzeeqzy.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3pmuxqlem.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3sehteejx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3rjmjtazu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3zkrrmixy.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3isngnwxa.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3znpvfffx.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3rmbbimkz.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3vnigcnms.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3hisgdcia.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3viqiones.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3zlamhjra.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3amcejvdw.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3iuvfdnns.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3quzyayoi.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3fnpvkqjw.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3lvdzlqbn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ydxxzmri.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3xdudgccw.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hgjurmbs.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3idgclnzo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3eptwcomo.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3ltkwgkfx.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3xkjjkrcj.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xrbnmgrz.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3jjavyqhx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3jlkcppfz.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3mfmmuchu.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3wlcvtgze.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dxdhaaot.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3wgpqwlmp.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ioszncty.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3gyyxokat.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3ihqtbwiu.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3wfgobjru.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3tspdrujy.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3pwbdhycy.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3atqzrxsa.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rlsmmljq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3mgdcexks.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3wkhyhjwp.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3ptkfslgw.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3gfxuypgy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3suoleoyz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3jizvujit.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3qstyizas.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3zavlinww.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jozmiwqh.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3aorjupwy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3uywtqlun.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3ofpmunsp.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fpqeccvz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3xrxfwbnl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oyxxvztv.html


<!-- 参考信息 -->