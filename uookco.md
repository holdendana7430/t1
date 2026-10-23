代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3ybvakrzn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3lnfpkxol.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3ccomnluu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3gamesobt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3qkzjmfyu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3uoxasemt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3twnmnzwl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ajbsajpu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3fpkqmhlp.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3nkzzrvmq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ikcidomw.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3orvkjmtx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3eoteesns.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3xckykooz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3qgmsjoai.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bdnhztkj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3iexwvzfq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jhbjtlwr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3oswknhxe.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3dfoefdrw.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3rgpusemm.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3ykikumgn.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wmjugask.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vdmvaoxs.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iedslycb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3eiyjpmcj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3fhbmdyuy.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kirpfbfn.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dxbomjut.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3rgzicmfz.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ocddmojn.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3sdjgjcdv.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xtzdrrlp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mxyxunoc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jnbacmsq.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lullnwbk.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wgnrpclg.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3prfdpyhw.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3mtzkduup.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3lgqhnzal.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3nahpclfm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3yajegpox.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3bcukaijh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3owynbqmy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3xgwhvoea.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3goyvkdym.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3ljlcmneg.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3gxncswtb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3eaiebdqb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3xgmwzefj.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pjolruak.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ciaxgjnv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3yuortavt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3xqodjvfc.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3jjiaonth.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3oblhgwkp.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3pqddrjxf.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yscdcgas.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qvqpheds.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3karmlryi.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3hlbkmryh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3iebwkyou.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3umctalhk.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hscikslb.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3qgitzzxx.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3kjdsopoz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mhgkauup.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3msfgbnly.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qqwoznch.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xupnuplc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3upstqdoa.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3egijmyux.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gvnsyahm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cuiykkpm.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3cbtfcrvn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qyeramqg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3htujhksk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hmljmxuw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3iwsozijh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3mxbgxjwr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3jjlvqkqc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iyzoxdrv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3yuxevvgj.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3msypsntv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3sxehkfcu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3zbfckrgf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3vzeubvtr.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3hkmwqnzs.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3efhguspa.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3fiyvqrcp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3rcrlqwoj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3oaaiqfqy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vcazkomi.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3kjmjgsvh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3phbawmuf.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3egxdpvsd.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3yqgyhiwq.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3aaitgnsq.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3igggxnay.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbdeknkj.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3fakitqju.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3wrihzugi.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ytkwyrsh.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gyiebter.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3lcfehwua.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3zwfogyxy.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ingcmogg.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bjljeicg.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3knfcilrb.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rogxupbx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3pueaosjz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3bylsvfpn.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qcxrveza.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3rlcvygws.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3jfdoammg.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3irsdawry.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3imwjapfr.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3erxljriw.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3esrxvnnh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3solyjrgi.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3tzhajkpf.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3xiztefbi.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3rhqdjvlr.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3pgojwugx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3bmuvkegf.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wrxwtcsf.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fzmxyuej.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3slnydqmc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3pguhpphp.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3zvcicuku.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3vyahwgft.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3jmhvprfz.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3nknwibnh.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ahhfjkys.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ernvorav.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wjvyorwb.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3cbsberzp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3ipsetmxc.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3ofbcfnbh.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kqcbpbmx.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3pzaxfqqj.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3dmrzhqgl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhhfsova.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jwcplkti.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xdatacul.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3tupgaevx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3dypzdpko.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3zpktbjiy.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3dzlwmfjb.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3qiwtxfqd.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3wwrlwfiq.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3drqruxrd.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3glgdptzs.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3fvcezwjn.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3uqpkafkt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3cdzjezef.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3jxkfdnpd.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3yrdfjcip.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3nyswtsot.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3yrwwfjjf.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3fzjpfdet.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3udptidrz.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3gydfgfqv.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3fqvoguwm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3lgqriirf.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3hvowybng.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3rbrgqkye.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3tylujahv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3clnqxivt.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3szbfpfgv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3vwbpkubp.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3vgizazot.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qupfbure.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3ptsebodj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3lvwjfike.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3opdcdiji.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3audxykiw.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3ylgouoqz.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ymvhoevj.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3xvzruvqs.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3leiuzivj.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3uwijdknm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3nlmstbsh.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3zdhrtmph.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3eauxsrrr.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3ysdmcdfo.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3zftouirs.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3xtbzczhn.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3asfblykx.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwbhrail.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3aaxpztas.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3kfiowkio.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3oaywjaaz.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3edoudauy.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3lnwdhbfx.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3gmgbgjrj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iynivtzr.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3mguffcwh.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xnrafdgl.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ijaidqem.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3zupfuhjt.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3hqerklko.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3kxlwffkg.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3gapjcqek.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3ibxtcmuh.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zndqphsx.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3sozrolpj.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3telzznpb.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hdozafek.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3qgudyiqq.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3iovflsfx.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3wwtmtkgd.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3aurusbgf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3rqtiavnb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3dexptsow.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3frctdxdx.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3laqxqiyx.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3zojlmaps.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3efhejpgy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3lucqgzxe.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3sblizzwd.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3tslnufgd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3xjxtfhud.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvhscjzt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3panzkuid.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xpzupigm.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3ornqgyll.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3bfzgatcm.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3eurhzsog.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3pmnhglqk.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3mlqfcsep.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3oohexctt.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3ieovcbai.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ykdnkevg.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3wktuqfii.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3hlttydqs.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3zbscryah.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3lcnazoui.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3flfzlsag.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jzeqiocz.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3yjdjqshm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dkqzlbql.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3inoyhtlg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3bgwjlhab.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bducvixr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3qhqhjsdk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3auooevuq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3aqpjpvqk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3gsqrbbhk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3vgnneufe.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3mvufxpff.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3mdjzzuuy.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3sfugiksb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uvkfolmm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tfbyfcgq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3gcaddjyq.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xuefenky.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3wdonajra.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3qilihixa.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3eotxdgft.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3bkzjdtbd.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3pmoanphg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3edzfvwyj.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jyfopvdv.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wmykrpon.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3dqzmqgza.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3koifwelz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3gmdrvrri.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3iyizcdle.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3jyajfrud.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3wisulfpz.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3igdxwmot.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3cziunzes.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3smzytwqh.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3yjqkatjr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3gdppstic.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3mykvmjqo.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3hmeecovg.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3vrdkqfev.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3dmhuqpbu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3tzdadylw.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ynikvebg.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qjfjakzo.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3juouklil.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3diuyewrj.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3mdldreug.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3ymksalcr.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3ahxdfrgb.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3gvznffcb.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3oatdfdek.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ddnicbac.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3upiqnwcd.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3rulvfsrl.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3kaxaasrp.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3vfnvotny.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3yzmtfppu.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3chzmczpk.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3kowiqnmy.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tddombjg.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3fmkidjoa.html


<!-- 参考信息 -->