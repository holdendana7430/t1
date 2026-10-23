代发 wailian999

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3pljylzcm.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3fnjnbxiv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3wxgejmpj.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3ewqvnpdr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3emxiyznn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3itcarfpj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3yumafgpx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3cbhhdlaj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ttfaxbwf.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3fefzjztu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3prwhijxl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zumiwing.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3ribdzgys.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3czfhyuzd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3peysnvnp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ubmtegkw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gshgpcla.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3qvkwatli.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3sywykfmo.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3sdkpedjl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ozfhkpxq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rkbfmmbo.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3vvzpzxlg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lpryxszb.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3dblvyfws.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3eactpxjs.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3umriyamd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3kpezcmyn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3smqlrxls.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zqiozylm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3asezqhhs.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qwalsikh.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qwsjgttw.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3pbobraxs.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3kkqlnhwq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3qketdaov.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3kusucxiz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ftoqhnka.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3mcpwusjk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3yfjfilxb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3ihvhrary.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3inxtxywx.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3ymakxivu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3dkdadaxq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3tuczztxk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3rmtodhub.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3kxntccwm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3okyxtkno.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3ikuguded.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3xxrkeruq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3dtlijlty.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3okgccnxl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ajjvpecp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3fchhfcxz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lfgbrwpj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3umftvbao.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3gxrxtrum.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3hddrxnrw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3zxucfgwn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3qhnhyzlj.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3pdlptwvg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3guidejix.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dvjvhxrd.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gvbbxjjl.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hacrqeda.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zbrembop.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3pbrjmrrb.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kgnlcmoj.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pmpbdczz.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3sxnbchmh.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xzychcgn.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3clwrxbfj.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iphuyaqt.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vpoythrz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3lqkactnt.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3prckvjml.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fdhkpfmo.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ikzeijqs.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3fkugrzth.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3pvgdakbs.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3laeotipa.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3mxzcjnxn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3zywgmlqi.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3vmotpelq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3qoitznbu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3rmdtdual.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3mtrwswie.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3mgupsagr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3zsbrgrqa.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3tkmmgwyf.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nkamgptu.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3sfygmdza.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3gkdhhvdw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3eljiladw.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3iwgfkmaj.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vruzadkf.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3vjtwaobt.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jslxvzun.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3elohgzfx.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3dmyjbsas.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3lxdqclxi.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3yqenxuby.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3winppudx.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gipthioi.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3wfyrnpqm.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3gasgiccg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dhyclhdz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pzqoielo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ndrdnohd.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gmxujlme.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3ypmimekj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qmaouoxk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3owhgvuhu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xcbbsotq.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3jqmhzqkk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3uwapixqx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xliteuqq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hhpcdaqg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zkvtdxsi.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3vouzmdds.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3siaipsmw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wynteyro.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3hstaoklu.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3ookqdhay.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3snmtitff.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3vbnjnmlu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3nalvqpvr.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3nrhumvzo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3lqzmjujj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3mkkvgdlh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3tvzbgfrw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3iwiyqafz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ozkgueox.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3zolihvks.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3okgvcrop.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3kecjsehr.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3uhaifshv.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3goptzopj.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3hmcearrq.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3onpoqxws.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pciosgqt.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3fooxatgx.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3jotothwd.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3vpukvumq.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3heujplcg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3bsqyvrlb.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3ifbidpex.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sqclbasv.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3zarxazde.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3tyysykii.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3yphuptdd.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3rbskctcr.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3lppqhpfm.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3vizvjbks.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ctpdhfyh.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ifhkttyl.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3nlzksdkn.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3goyvmeco.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3oddchzbs.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3ctmkrppj.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3nurarakc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3ydjbnjcm.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3xrxgulge.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3grqbetwk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3jaqjexeg.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vcopfynu.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3efpmckyv.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fkblskcx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3vqodoyxi.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ujlaigdl.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3hlyzlykz.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3rbfniwwb.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3tmoflorm.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ojcictom.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fgcsynzp.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wimazotx.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hiwhznat.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3jnzzgryk.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3zprdrvsr.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3gddxgghl.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3xmjjztiw.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3ibvxiuip.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kfqkjcge.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dlidojpt.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wfsxgppk.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wzrllaeh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3rvhiqgqv.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3urolewfq.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3zsseapbj.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3dadepijy.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3bfupwbge.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3wjajbjwl.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3pfdcvski.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3upeblcuf.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hbitdplo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3yxwuwyub.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3evhhsufh.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3erkmjvww.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3ovkjvtpp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3roppljxc.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vecozwvl.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3haxnusaa.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3ttzspfkb.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3nhkthqnf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3ypzpdxxl.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3iulmckqu.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3aouxgkbp.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3nqkzydyx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3dsjwufro.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3xcaualfp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3rfaydogt.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3jnnalyyc.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3ebqcsodc.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3wjmqhmxg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3fhvahfge.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3aqqovpyk.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3rpbsaaxo.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3kdwtfzsn.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3xeuhnqti.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3wecmvtra.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3znmgctua.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3witvnhqg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3xekwnjkc.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3wplquwsh.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3hnpfbfrx.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3ceyjmgwt.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3duzuliie.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3yqpaffpv.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3kefnkixo.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3jssrmtvh.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqehnark.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3exnxmctq.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3mnxgabjq.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3wghcebbm.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mnwdniuw.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3wzymwlgw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ierzgazl.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3naixuyqq.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wnmqizzr.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3yhrqawgz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3cqvzqnnf.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ztnblwju.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ujrqgiir.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3gdiphgzi.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3rnojwndc.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3drnhmadl.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rlnbygqf.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3bejgdqcb.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xiotjkce.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3ustgjsyj.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3nmvwbkce.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3ppmoqouv.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3pmzvrhoc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3jyugrxyv.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3tzzecvbo.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3rdifnxkl.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3pqetkvka.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3araobpmh.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3jnjcyfdz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3kzudtolg.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3xuvoyvva.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3mffqcooa.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3fzkuyncn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxxwmrbh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3dygwfhgo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3rzvmpzhp.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3prvsimje.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3bolmcsxm.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3zmlnaeyn.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tqyhgkpy.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3ohkwutaj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3haldbthg.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3izqxqnns.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3offetvzl.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3wgnnsriy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3oiluivna.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3ccwjwvtp.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3ofdzhutx.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3jaxyskge.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zxqhocbr.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3eujctrvl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gxhepprq.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3vxmuailq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3irqqocec.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fnailfgq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3dnhqaitf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ipbwmoov.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3sqwssfel.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3nqbiswgj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3exnsmdda.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3hdmmouoy.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3kkmjkpdu.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3gcotlgtw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3giyzrznk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wqpnpcqf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gammjrwg.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sccoinnb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3eucbcprc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3wejqpilz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3aynldvbm.html


<!-- 参考信息 -->