代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3tbzmqfzk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3eyftlybz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3dxnljbpn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3pmxtsxvq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3cotsgqfh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3kihmzsmm.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3xrhbirra.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3xpgxippk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3smlngbkv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3sxbblgqg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ryfziatv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3esiwyyqk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3nnaqesad.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3rzjgelyi.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3fksencea.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3xmkueuke.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3djcdcpza.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3kgnuwusm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3mhofctnd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rumltqex.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3qftgfmly.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3anqiqhdm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3lxszrvvi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3jmjafrpb.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3wdqnpplo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3jucccwpf.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xuxiknaw.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dqgwwpuj.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aqagvvqy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3csoxusod.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3ddtnqenn.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iejerblt.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jufepvcq.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3xzarenro.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3narpnfih.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nhloxuwv.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rfqfbltt.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qvcivobt.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3lsrcqxzk.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lxjmhcpz.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wbdlclux.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tddkvwvc.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3ncwcflcg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3yfrbfgmt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3gmzqikaz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3xomhaikk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3yxjfvthk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3dklevfuj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3lrzsphvg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3yrnykpxi.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3opszwlcv.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3cjxbginy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3nrcvhlij.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3pmlcxwmf.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3drdjxztl.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ulsmmrbv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3uqgoxuuo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3duklphle.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3jvdlnhqt.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wsegmyxo.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3yqngnfqo.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xfjfgpow.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hffzmjpk.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ygjijdrb.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3aevegkzf.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ojuddnga.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3muoyxjxd.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oxufliwt.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3tjxhwzyb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3oeizemps.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3brlyjkcm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hhofndaw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cucudfac.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zzossrui.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3vuipcgmk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qjqgpdug.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lxzooasp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3papgrzhe.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3iullgqnm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3juqthwsa.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wsyhjhml.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hddcodgb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3icimarre.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3zmcxeyta.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3dbhtdxfy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3nlvxrqld.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3zrnracdm.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3mbishpjf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3nuiifyvn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3dmvqtaug.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3cleybgrw.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3naeygnfs.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3xnxauren.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3sbkepplq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3plwcysut.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3utazolma.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sbrthvly.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3zphrrchw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ckjlvksk.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3vrssxzrg.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3zglasflu.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zmuhlnow.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3brqwgtom.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3twotjgsk.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3jfahkgrp.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3hytmryoj.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3aeozemtr.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qybuqtvk.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3rjyfdcql.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3kqhdyjbw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hnggbihx.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxufikmk.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3kureepnc.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ehoygobc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3uclkteod.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3siwhlcfj.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3hpaxuvwh.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3nbmvvbim.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3tjlsrdra.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3itawbhdb.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3obpgkjrl.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bwdvlwwc.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3ydgqneao.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3qovlrrcp.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3xjdteppy.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3peoiuume.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3ghcdreis.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3sokwwxsf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rshbzgqb.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qslqsavp.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xmenfgnr.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgawmxdz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3rfohqjcg.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3axuskofc.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3qpsjabko.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3sxvayjmh.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3iktbinhw.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jhtznxmz.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qawouvae.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3yfruujwo.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mkjqmarr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3johkjzic.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3gnpsrsao.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3eerokhry.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3bcpgiuev.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3fufpwndy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3auddfsxp.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zxsremnr.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovgkpuew.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3coqbkyvy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3gmdqkejo.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3tesovgic.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3nbggjtbn.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3jlltxwxs.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3vxcqhzbz.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3ohpplrbw.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hhakcusd.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mdeqqaai.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3iyubcwwx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3vgdsxolf.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3uipyfqqn.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vtaquxsc.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3nhyokqpw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3npiassvn.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jmdrggqz.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jjgkokpy.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3hodzvhrx.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3axclajtt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3idiwptfb.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3zypfeawe.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3nyhljkcs.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3bpzslsxb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3cmxfoiuy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3bpfqhpon.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3ijewopdr.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3yromlexo.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3kzaehdju.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3vwgvrfvl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3ncekwduo.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3qcmtdhoe.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3umdbypgj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3qplqazdg.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xrlkkdrq.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3yytwrjco.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3pdogfeok.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3qioozzps.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3mtkfllxn.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3sjjdkdkx.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3wihjjpgz.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3rcsjurvx.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3jujhvfiz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3zfjqexom.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rqaoiumk.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvgyizhz.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3prmdbfyw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3bmmtovcq.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3zcveigaa.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3vubxfjwu.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lyekbjgy.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3kgkaxevn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3axdxxzem.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3phjterdv.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tuluczkh.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dfvdbuox.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3fddptiyn.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3aplqumtj.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3kgaegrie.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3tzzscqee.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3xlnngdqq.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qstrszme.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3arjkpdry.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ifqksdwo.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wkdujyof.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3mjizwrwh.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3hdijzemp.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3ltoafqpc.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3hytcpccu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3ovrfqhkh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3vnjmmwus.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3ndyoeubr.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3bbdwfoay.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mjvrudqj.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3hxfhztof.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3knfkfiyt.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3tbvjdark.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3jnnuacfj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3cmcphciy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3yohpziga.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3mzuxnuvo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tsvqzyca.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3pjhwebqr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3weltklji.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3dzrukbjn.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uiixfmdr.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3pgsgjhme.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3bikvocux.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3ftlybbkf.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3fuehqwuz.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3degoxwxr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3jdzsdxic.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3xsizdkdj.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3cynlulml.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3lyatwuoc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iodxnvsp.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3vvwgdlnx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3huauotfe.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3enlxwitq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3oydsbkil.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cayycywz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3vutmfajc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3xmliyfzv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3wyqahdeh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3tgyeklzh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3zssqbjpb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3ttfxjvye.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3bejfrvjv.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3inlgypkf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xyvnlwtm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3izfypqqr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3isncvtuu.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3byhxfidx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3nwtzqvhl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3rllrqgxh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3sfgitqvj.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3wmxrxnnu.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3tyikvnuk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xbyxwand.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xyxzqodd.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hfzkqeqm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xmqmfhpt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3zkadpihn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3zqtqvhdj.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ueywsnyv.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3kekbgwnf.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3pzeoleid.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3oyinqoiq.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3fswojums.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3hhaulied.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3uyhksprv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3xuuslsvs.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3fevvhneq.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3roodumke.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3vhhvjduo.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3prdjhedu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3fmveavwa.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bwullslx.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ruxbiwym.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rputjvds.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3vtxdchct.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3jrphjphn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ydrrmtxr.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3kzcspnlt.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3cgkpunxt.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3obxfhikb.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3unbltmvg.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3rdpcfwsh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3rmpgjmch.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3ooebipqx.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3tmziyqxm.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3fllefmwe.html


<!-- 参考信息 -->