代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3utwcywzb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3lrwsjbqb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3awnoqaps.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bmmvbvlh.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xlbucqbw.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3akczfaxj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3czjvsjlv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3rhmppgrp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3szefxmen.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mxclrnsh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ysesknbo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3jlgmekuf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3xaplpgxy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3ptdentpi.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3lgnhrfcx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3fufsrbti.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3samdtdhs.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3dggogkbc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3jbrmxtxk.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3eemrujus.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3zcbroecs.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3clounddt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3bpaqljne.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3onrehdwq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ekbraesz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3akxegnpl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hamwrgqi.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ssrawppk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3fjofdzqs.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mfvpvhxb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3rioayngt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3lfqldwqy.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3fcemdbfs.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3exkhvsxb.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3agsquhmj.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qzmpevqh.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3payizuwy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3fahbonlv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3qzatslea.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xzzlofgw.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rqmhzeqg.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3mnkccrig.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dsbcgthy.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3onydzxdn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hgxqhrfj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sjziydew.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ciupwugr.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ndeyoyds.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xywqsjyf.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xctxenjf.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3dhmndxot.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3iokdnpbr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3utkkxupr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3cpacdifk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3aiwrmnof.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3vknalvxg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3wuhtjjra.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3ibjtgvrb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3kvdsyyzx.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3jyhuvseh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3jjjehmvt.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3izbzhfze.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3pzsunseo.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3zbrdcbkm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3wwpgekbe.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3yiniljsg.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3tdlfoytg.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3goayeyji.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3gclazdsc.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3veelmake.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yfslgcyn.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3xralwpzv.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ygnxgtzy.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3qqkhpbto.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3fzxmvsuk.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3udbqpbdq.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3nffjiuek.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3svaxwump.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cccfcbnq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bobqbyiq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oukvesjb.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kubseteq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3okptltry.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eitlauxa.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gxutirwc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oxmxprio.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3gllempdl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rlwyqocw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3tfdtxiol.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xikxrqfm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3stealrzj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3bjyorgkp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3wdysvuqj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nlnofibg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3ywcrgnom.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3cdxynwlu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3zytyzlej.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3dmrzagnm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3fgrttmcu.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3wqlkdzzg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3uxkcaogl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3pmgzbcpd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3lxbcnyfi.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3otperqvi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xegmjylx.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3mvtpwxrm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gejxkshp.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3xspzznse.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3mhwftesg.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3hcrbqdkh.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ofcalbzy.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3zhbouuwe.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3grmaxnhh.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3isekaqcs.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3fxoyzhre.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fukxmygs.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3zrdrguxh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3tawfshnh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xjcihgub.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3soozuiyh.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3paifdtye.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvayacmt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3zjtmezmg.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3gefwuomo.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3jhedavgs.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3zhfkidpp.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3lykbpbxh.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3gadqydoe.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3igcutfus.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3tpekspny.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3ccmrahmy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3pkwzpwha.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3btbuhisv.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3apkiyqie.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3mjmihihm.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ubojzykm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3arkxoqmv.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3vowumtok.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rfehuuba.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sutjyfaq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3hfzfmcgl.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3sojdokry.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3eonroizo.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3ayzdtetv.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3hjcoiuye.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3iohpryyk.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tjtupqch.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rubvvmrt.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3whvdxxaf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3eumiutjr.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3lhepqbfo.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3moyougyk.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3gxkozjrp.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3zcntikpn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zddsyvmk.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jsyguxcg.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ynhymuty.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ytyowruq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3dewslitn.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3yveujwzf.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3vzasyrzi.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3gzkaxmzi.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3uhtvijys.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3tvqybzgk.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3tjmwsftm.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3bmfxrxbg.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rfowfoci.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3yqyiqpwj.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3yiuoncgk.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3nujzkahq.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3rmvyfoem.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3cpulcgfu.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ymqvshbk.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3jhwehlju.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3hpgujgmn.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3ijvxagcc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3lqyazuoi.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3ptncuevy.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3gbsntdfk.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3qksgeqhv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3fodjltkc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3eotmvqqm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3jbrmnfgx.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3ogksthkf.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3gotgllko.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3yakvmudd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3klyopuaf.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dnyuaxhz.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3hngcwlgy.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3rkbsglob.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3bgcqqxmq.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3bkgieofe.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3rcaknrkb.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3dcfxjbuv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3bboopwau.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3mfydswnu.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3kfpjaugh.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3syualvyx.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3mubiiqnh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3opieoryv.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ytorpnad.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3qjvrprou.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rdjzjdhl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3priwzsun.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3qqjwznny.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3nbrcxnak.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tawoenmi.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3xrxbxquk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zvuvcrpd.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3huffykuv.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rlypaavb.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jnrdjayd.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3iwsnymiu.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3wkifovnn.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3nswzruwn.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3blejploy.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3sllamxpz.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vfpfucio.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3iqxfsmty.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hsvkyxyy.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3cgrppqtf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3nzrdmcur.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3uigmghxn.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3wjnjxeub.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3icygdkbx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3xospatqd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3natvafnm.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3gxxmaxrq.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3mftjgvor.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qxvxnvav.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3vwfcypfk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3ptlivkyt.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3lcgzwbtn.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3nnpnnrnh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3tddwolyt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3syqiugxb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3dwosoryw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3norcmalh.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3rrfjxasx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3vxdgmswc.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3mginrtxv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3indaiivr.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3ltvgoulh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3pkhstqpi.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3affjugcm.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3lteljsvz.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3dnappdvp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3odnoonyf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3ybvgawgw.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3slhtpukb.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3hinmqamc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uerbnohy.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3wurtpanh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jnagwbuh.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3pimgcqeb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3ervylbdg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3ydvrgpkp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3vdhonxmn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3qkszwwyd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3dnekgoko.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3mfqsufeg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3ikvdasww.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3lmdrbfhw.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3fadfetao.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3sxvdsqtb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3pczvoglf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3btmjegpj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3uyxciigb.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bpinqntc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3epzjhbbz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3eefghpqk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3odivpnzn.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3nobyshqt.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3fgbgczyu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3yxutmeom.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3gbqtzmqq.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3tmvxvems.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ksrwnirg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3bkqlqvmh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3hlnaopvj.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3apxgbnti.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3ljsvfsxq.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3joophvwq.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3qyirgnfc.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3jdweuclw.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3bpgndvxa.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3nyfpcicq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3mekbuhbx.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3quiwhglg.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3pvbpgicu.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3zzcxgdax.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3qpcxeofw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3nqaogizh.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ygnyqrwr.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hxsmidob.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3qxcdubnz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3qxfcaeyd.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3ubwbeuiu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lmyeoxxz.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3ghlrlujy.html


<!-- 参考信息 -->