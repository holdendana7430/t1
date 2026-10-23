代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3vwqpqvet.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3brgprfbb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pbhhowpq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3rrbxnnhk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3sjdybygg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3pofjonnc.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3mvuvsvhb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3imhtjzyz.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3zscglouy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3xidlijnn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3aqeautms.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3tgywalsy.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fdhkcxjg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3elchgvli.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3assvwsmn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3shiwzcqm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3qfmwatfn.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3rpykifuy.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3lcvcunqi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3skiqctyo.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3hahchtaw.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3gzcllkzq.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3drffyzcf.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3fobyvjqh.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3lvbmqkin.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3zvtlynuu.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3igxdiqdt.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3dembmszt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3whojpwht.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3rjhsewir.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3mswfonil.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gwrkbphi.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3decffhdh.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3rluenlvk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3cndipcfx.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3nolftmbm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3etxvzqrt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3mhwextva.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ysrcelat.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fwxmauic.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cqebohzm.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3owvegvtj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3upojrwhs.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xigkkzaz.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3rzdfanor.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fupnytvp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3szzyuvhd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3foytvlfs.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3dzqqzzkl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ciutluun.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3eonqmnmk.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3vyrnqawd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3rqisyyts.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ayknbnsl.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3bdqhlrcj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rcwdcafi.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3atawuwnj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3sifkghkg.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3prhdhjvm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3kpdvyspo.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3uivznise.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mwalxewj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3isideate.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uuwqteiw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hqoikkbr.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3wviiefig.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3uzbnyaqy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3foyihqcv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bhgnmged.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qhvwpjbv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3pqoynpgs.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3yzphknpw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3huvgeivs.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3xwwcfegd.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3eukboqfe.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3nykprxmc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ltqvtlgc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3iuysdzbh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3pkomhxku.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3emtsyqeg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3qgiqqqra.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3caykvfzi.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3flpriqil.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3adiweabs.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3riozmzuf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3pbisgzfe.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3quakiyqd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3stjpdgvk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3bsdpkwpt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3nrbziiab.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3glbluied.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3jjvlwmql.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3ndzssqnz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3kfrjufqg.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3edzfqigs.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mqzuviuh.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fzhoavox.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3cenydsiu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3kqozbkbx.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jywpwxzh.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ikeaujqp.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3gtuxonnm.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cycduzjo.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3euqgwodj.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ndqfsckf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rmawlzwx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xjdrnzdw.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3moqssmzv.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uhhybulh.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xrrvbmce.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3btpzehcf.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3iqwkmxfo.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3chysbwhu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3thrjpxme.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3dtmctagj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3qdmodbyq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3uovbsqzl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3fcvsnuty.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3vfjehllp.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3rzzosdxp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3eldlwuaz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3wsjcqvnj.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mqaxurmc.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xwdhrnph.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3gjwugjez.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3iyiyjcbu.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3hmwtwint.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3pasjbipg.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3sjezhgpj.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tirsleoh.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pyhutfrg.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3plvirfjj.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3rlwspxhj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3lrfysjno.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3anjfovkq.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zxafydgj.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3tbioolhz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3lsvdbfow.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fuoettox.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kjsfwwpz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3abiisldl.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3doemrjii.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3cqcnhwrq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ytcrkene.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bvgpsarl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ugkhbzhx.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3aacoisno.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3nuvxatzn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3zontxhrz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3auekgjok.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3kytlnaeq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3hkzacoof.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3frhgugdm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3eczdashu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3hpbuogkk.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3bjsrzxlh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3wplfbdsc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3biynrkha.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3aypzwnpa.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3smxmyxjw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3jzgbrnzv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3bxspfblw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3skcnzeee.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3ckklgstk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3suyolrqo.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3zqgwvkox.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3peydvyfi.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3vmjynzba.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3slgqygah.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3jdrstggm.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ezdjmbps.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3sjsbilxf.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hujvhvvr.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3gisqcvmr.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3dplkesxu.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3limrnzpq.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3zrrbpqnj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3zfmrimvr.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3spcecclw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ydcolcez.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3uxfripmu.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3lidjccra.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3hdbesasu.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3rlavodvh.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zmojacej.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3xyvnwkvx.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3tnfgecfu.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3pxypncka.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3otikydtn.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3mvhyimee.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3qoeqsbww.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3lzkwikmj.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3oxqxnjwq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rwetlsxn.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3xioatwda.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3nujpvvfu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3wxnhkhmz.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqmfvavm.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3onbjennj.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fgkwetyh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3gsciklkx.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3rqdlljmm.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3aqsunzll.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3kwfpmptr.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3rsclegwo.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vvxruvzh.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3juvkkcin.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3csskhjjm.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wiffgnhj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3sdbavtvb.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3kbcegpzu.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bgyfdtpv.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3wwsncukr.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3nhldfenk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3yscmlvre.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3coigydid.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3edntcwev.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wyrohsqz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3hhabbiap.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3qveltcsa.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3panbjfrp.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3iciqvcgi.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3ltgkuquv.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3vlzubjho.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3nhujtiid.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hmefvwwm.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3imkizfne.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3jzlfgxun.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3jeoorisi.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3uagqwldv.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3mwgiikgm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3bzichtwz.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ltacdnqi.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3acqfgrfm.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3slboiybq.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3qxndivee.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3pjxcwfih.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3kskflpzx.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3snbozyly.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3ngidveco.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3zgxulrxw.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3crvfbtrx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3ielexftj.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3ajhbinif.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3fdpanhsu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3xozglybk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3hqnvxvcu.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3waghsjff.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3asybsjcz.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3feheilcl.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ddixhawq.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3aizpwpsh.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3kbhrepuj.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3srtxmjil.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3rtalfigk.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3mlhprrev.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3ayivucbf.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3ooxtlrhf.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3xmlwgiqe.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mfzcelvr.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3jrqrpzhu.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3wljotitk.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xezlfzjo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3kdaqrsql.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3qnjlrldc.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3xcfriwml.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jpakdupx.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3oxkdgkoy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3xyaguhbc.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3vadglkrh.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zuujhego.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lrrbxwjw.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3bylcgyxa.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3xodbghji.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3bdwmhktp.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3gbdwgbkx.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3eoadczpc.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3uvbmmrgg.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3gsrfennx.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qzwxvuqc.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kbgkjggi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3raznpuit.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3rbhkugww.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3lecjrvxx.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3hrzjbjnu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3pwbljbjd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3eyvygoof.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3etbdvsdy.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3cptkjpkp.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3bfhljqyb.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3xhfkdwfn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3oldtbtyg.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3kjvrtwqd.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3zilibiaa.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3wlxqalee.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3vqdtnqoz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3mvwyvniu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3elhdihht.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3kfejojew.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3uwznmbyv.html


<!-- 参考信息 -->