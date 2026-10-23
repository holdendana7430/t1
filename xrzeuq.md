代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3twhfywnw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3xhajzonz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3grmkjuzy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3bcgbsvrf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3sudlxfth.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3yeqgsjqd.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3bfhsyknr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3bwbykiat.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ucxrxbeh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3uwyvfbmf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3hvoosvrn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vfkdejmu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3huhqsipy.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3aqhpmbtn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3seakjiiy.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3esrwuqis.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3aunipetj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3zdzgdtol.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3klxnrxla.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3csofpwgj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3jrbcftvv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3cehzqays.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3wademyxh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3ieeewlqw.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3jbuasbmx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3edjsuetu.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qljtthdc.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eisqcuoo.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jjuaaavh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vqjvzvyp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3owwocznb.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mysseovp.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hqdihbyo.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3citvtzuw.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ypuuqnfk.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wrobegzt.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3itbenfxo.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vyjiodch.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3sgnjcujb.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hdskyzsz.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wqhykcsn.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rytzrfai.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3rnsiuihs.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vgxophmq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3bsluxclk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3bsbcfqxq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3gmnnhjjj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3bcaupwmy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3lycbdsrc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3qocnrbzw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3nehwsuhw.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3yjzmlbrh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3qrghzwwh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3ioopueqr.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xqklmahg.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3juqqwczu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ykqlyvou.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3duwuxrvp.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3bwjdxubv.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3ubjljibg.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3zvmqewaz.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xvcjaupl.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tgsjbfoh.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3bysofwbi.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3mnemejcu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3daxhtgdu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3uswgtxmf.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3glmpnrah.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3soshpcby.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3bvbjzjdx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qrvmnamb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gzedlivq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yryutbsa.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nbeizcok.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3sbknfvbz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ufdzjmmh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ckyeessx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pibhsofo.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3yspplreh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cpjybsbs.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3lggkuvjq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3szupgbnx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mnhwnchx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3nyiezaas.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3urybptvl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kjvdwrov.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3hzoecrmn.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3amlmdjcb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3uabmefbw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3zcxdfzer.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3uxlavqgh.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3trfeahbz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3nhlldnmp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3pzmcmibz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3lyyarwoj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3tvxxbamd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3warmqrur.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3fctcznqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xgdoquma.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3cubjytyx.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3rljmiqff.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3acgrmukb.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3uumznrlo.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3cmuqqrhr.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3tufpcmhf.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3sjdpxrhx.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3ecezynbc.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pojmzpjw.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3urbpaici.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3htiyrozj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3gxwjoznq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3karuefen.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kypzvqkw.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3zeszwxcm.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3khqbnwob.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3fqhlfyxy.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lavorxko.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3vjqkijiv.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3vicwmnbo.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bgqpqztg.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3remruyjv.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3yvztpozl.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3twzwwhmm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3chasvajg.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3hobmmqlu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bwylhnbx.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3izcmfjfe.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3bkuqrurb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtzfzten.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3eigdikel.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sybpjfyx.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kxwoenxm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3nuaybbpb.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3iplaiktl.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3sxyqzaak.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3jlrioxgd.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3rvegqtsw.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3otmngwnr.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3nodzmibv.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qxxakalc.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jjfhgsox.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3kponnlfr.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3aerisfck.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dhgjbiuo.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3awlxhtmx.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3kicmnxvr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3dtlbqtku.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yfaelyew.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dajtixtw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uhusvatq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3swicxklr.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3jqvtgxgy.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3oogwvoqf.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3vqqabfol.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3djieabox.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3gmeyoohc.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3puelweog.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3xkzwoyxa.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3uvxmolnz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3obofmzkv.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3kolqbdjx.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3demxczow.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3lwasxasy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3yefysbqk.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3tcmgcsqz.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3oftksvfd.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3pcvtjhom.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3pezvxxuq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3iedtuphz.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3obdxcdlt.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ybcohixd.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3xnvjsbtb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3dpgintbg.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3ylrnujln.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3wlmadmhl.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3lylskqbn.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3wcfankhz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3ksvicjlx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3yqqgrgbk.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bamthfvq.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3rnsuhcxf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3sdkqxiqn.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3mszbayje.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3sybqysth.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ywcggbgk.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3lpxezsco.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3ojbqeeof.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3rlejlszr.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3tpmdzgpz.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3cnngxdgp.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3vvclcwbl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3cgwachkb.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3stwfwwnq.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tcegsosx.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xaleuzgu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ldefucwo.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3qoaurvls.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3hjaixzpk.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3sqdcyjks.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3nsdhdzcw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ehrqmnwa.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3higlwwvh.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3elichmyl.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fuadzvrk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3egqvqyur.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3pepabtck.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3gefoyzzs.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3bartacgh.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3fhlawjwh.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wrgegdmd.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3yzhxirya.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ygalgahy.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3aoccuhjp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3axxdlmzv.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3clituhiv.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3wgmyschp.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3ggqupxza.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3hisywbny.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3aslkgkwj.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3vvsmxkkk.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3uhxhevmw.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3vnffvlho.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3shnerqlf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3qdyhkgsl.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3syvvjqmo.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3aujymsxi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3uqkasgmw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3asuzvqcr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3ndougxxj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3rffwcdzg.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3aplzfmun.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3ehczphxc.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3mowkxvyu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fadeshid.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3quzrkaff.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3tfpasbnf.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3wkziiufc.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3rnojdbnh.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3xwyptlcr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3mpwxvwlk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3txpozwlb.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3rgdtcfft.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3uqehgnzx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ndgcrmgt.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3hnbxiobi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nxsjnrph.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3yfzqyvdk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3wqppwufm.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3mcodgbqj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3nfhoapvd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ajlnheab.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3zpikjint.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3skhxssrl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3bpowmkdj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3hgbvqigg.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3avasjqyz.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3kdyejfyi.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kigydpin.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bccprjjw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wzfebzle.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nhaocrpa.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3sfmszeky.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3rkdczeos.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kavxayzv.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3sneljnnu.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3tcxujcaf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3kigbpnta.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3osgafpwg.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3quciycmy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qfaknzbr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3nmpfyawx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3xfybbcbb.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3oemldnel.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3hpmmcwkv.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3fzqvqarf.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3doqewuvx.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3kyagwtfq.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ihtneksc.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3nimsbdub.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3bgjncqrg.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3fffvfnyg.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3kuajrpii.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3dnfursnc.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3frvzxdgb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3wyenbpsc.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3sluczmyn.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jqqxqruw.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3midndrwa.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3mdpdoosa.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3tqctmgwa.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3hdqyigcj.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3slotumkw.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3avvmhpib.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3amccrsem.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3mchjfbjo.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3yehiotpk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3runefvhq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3caeatqom.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3rbcarhxj.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3xzjvhexh.html


<!-- 参考信息 -->