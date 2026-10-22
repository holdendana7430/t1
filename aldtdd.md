代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2mmeqynjo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mbnvocwk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2vgksgfqt.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nddmoaij.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mfzmpfzz.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2eyuyjlfg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2cvhpxnja.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2tbugsqvb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2qmwlgvhm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2vimujlks.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2krikofvy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2pwggbtrr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2tzeksbjd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2dxoebvme.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2pmkbkjsx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2owhcmmnm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2zlgjqywr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2sbtsriew.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2kmgxccgn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2qdpzljyn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2jbfgagvj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2vlkhbzmy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ldacxiyc.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2flcfaexi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2rtcudtvr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2rqcybgef.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jnuikcdo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nltzjuvo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2tivzghzm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lkblqknf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2hejgmsot.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2cvlmhlaf.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jrushltn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2beexigmi.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fihwdutm.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nnldhzui.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tuhqpigc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2zjdvjbsh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2oyrsdytd.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ctfgshws.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wwiqsvuh.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2zngzailv.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zggtrjpi.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nchbqazt.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2clcgeqir.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2skqohijt.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jjtnzygn.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2diowvbhs.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bktyldqs.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gtcqlstj.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2itbiwftj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kwjvbtbu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2aioaigvd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2zyqnneen.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2erpmbtbb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2tmfyioet.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2foybiwyn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2ibtaylxn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2qcahmdrw.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2olsmbrjk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2afgbfwkk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2zkrygvnr.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2nofnnchg.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2evnonehg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2otpnjjyt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2smceitpf.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2yigwhohc.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2xvxtdmni.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2bixbsprg.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fkzbusdh.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xvecjvfh.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2vymzdtcp.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2rnaeswqo.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vabziphz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2hcrfwuqf.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oxybpuvm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2zitdxsmq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2wtwmmqbe.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mgbqqtny.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gvlxqszx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rpporlzo.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2usqfjnkv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2dhmqpizq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nephkcuw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gglmkktv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dokpttor.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2uuqshxei.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vtnhvidb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pmlguvij.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xcxrtwhz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hxvbvtzq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2xfizqyzo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2tiznhfun.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mtjwpcop.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2vlkwrdij.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2fiadppkq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2ygkxpynh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2xxbjxtut.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2xjmmuijn.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2lgpbwxnn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2vjstbwhb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2psrbfweo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2pvetqbre.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2noalubrp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2psjnshxu.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2ytkcvcto.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ztnvypnf.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2wlonwzzc.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2mhtlkscp.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2oivsszej.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2thykdvyw.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2fkxvooqe.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ttcrxuvy.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2mzditjwn.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2pwlzzwob.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2yhjqltqi.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2ppcwuwgu.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2zrjdczfm.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yxcyymte.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2imvjgntm.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2orgfqsth.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ymcoykey.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2nmqmdcaa.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2fdhuzgiq.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2jpnrwzra.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2ywraluma.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2njfiisez.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2znplwxoh.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rccwvdtd.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2qyhvvfby.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2cfsfahtw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2ilyqicut.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2zwcypick.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2eruausqm.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2knfzxmrl.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2vtbtgyka.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2chtaygai.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2avipvtpz.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vntecupv.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yreggxjm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2eulcwoyp.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2aldvjtei.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2qxagapoy.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2krhgpnvp.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2molbvexo.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2secvzqgq.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pyfwlhtm.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2uwgjpmbp.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ukhgorbn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2pfccvsqx.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2ieuxfbai.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2qnhzaiix.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2zalkhwpu.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2mktlcvck.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hapsgpzs.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wbqcvbyl.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2bqzpyxih.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhjxfidv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2qsbrepdj.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2khsrkjco.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2dputzaqf.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2lapdinnb.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2qegekzbh.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2uxaaiqgz.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2vovnztaa.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ogsjjzvw.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mgaquplc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2ageceyrd.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2cxpkugac.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2sbxihocb.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2vrujluxm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2qpymrlxg.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xweccgoz.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2xevjbika.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2ifayyrkj.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2phhpoobt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2ukycrdvg.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2endoqujt.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zotrxvib.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2mbmpekxb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2tygsvqxm.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2nezvlazy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2nwxywbhd.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2imcjrshc.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2jwcewgdv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2zpbbyhaa.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2fvuozheu.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2uqlxflen.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2bfqkjpvr.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2xunzsvwl.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jtvqcxpg.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2yolbfoko.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2fwrlckqb.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2aepslzkg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2cibekxlm.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2dqrmrjpf.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2xjjnvzrf.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2vyhhkbok.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2fpbfyboa.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2gywsjcoy.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hegiyxdu.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tmlxzzqe.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aktxaeng.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2yyacyoyy.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2xyoqsrps.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2euekkjdy.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cwatygun.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ysuzxwva.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjvmjuky.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2smqlcbik.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fqnugkqq.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqdbpues.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2nmgnyumv.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2pbsijrxz.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2pmyvmeio.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2nehiupmg.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2sufteiky.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2fnaskxvk.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2imczhlbq.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wxbsjywa.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2hbgqxgjq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2wfmtsrgb.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2mnslilto.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2nuktpplk.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2eehmaktu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2harojlfy.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2mnnmrknc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2tszvllsp.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2soyoydku.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2hpiflxtp.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2kuqtvrhq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2miemgbkg.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2lphserhu.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2komnbtaz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2gyyjoumy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2emeoqzdf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2nyeylnxy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2tnmuueaj.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2rcekqvjm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2ncscoutj.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2ancdunsg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ptojgrkp.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2hvtudkzg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2nymbofto.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2esqjsoop.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gwzocbgn.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nlcyhbni.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2jxckwwkk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2zrfbymye.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2xlmvtxvd.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ogzahzbx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nuyqmggu.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2cyjjtilz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oioxjfjw.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2wrzqpnxa.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2ndjvsqns.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2flaqrhcc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2pgcjqupt.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ndshocil.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2jtkujpli.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2qvmcwxzk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2yxirxvuf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2cqpqqiww.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2vcqpshhv.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2xosbwhvz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rblmfodj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bhfilglk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oxqtclkx.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2apmosnxp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2kjkhijpf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2wyzztuul.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2nojmegys.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2wnglsrtm.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2kgzbbgum.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2dmpxfqoy.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dnnsxdsm.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2pgkygjob.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2rsykkbgz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2katgdwuk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2vtdmdcwn.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mlyhjpsq.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2tlamophg.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2amxemwca.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2pwqtweuz.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2faqpnqjr.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2lovugyky.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2uiidgtpt.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2fbrdnuxv.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2srojfcnd.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2qcbhvaad.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2jmqmszkb.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2jiarjdaa.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2gacmofru.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2pasfimmg.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vgfopdbd.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2dhbthepb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2oywevcbn.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2hyblivzu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2llfomqyz.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2dckrwknr.html


<!-- 参考信息 -->