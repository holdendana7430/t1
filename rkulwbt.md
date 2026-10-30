代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/gkdyihvvq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fehbvm.com/Article/details/gxatqpfne.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gnqrmslyo.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gdyhbljjk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gjmeadnal.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gyzsqxabq.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.zdbjq.cn/Article/details/gwuxosulz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.zdbjq.cn/Article/details/gpoypkktd.sHtML

[F09] 获取文件大小
来源：http://mobile.hesvh.cn/Article/details/gojzvjjrx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gfpeacsfy.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gxpfohpil.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/ggydssswh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gyygpewoo.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gzxacpddu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.zdbjq.cn/Article/details/glxqwlsdl.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gcujshbod.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.hesvh.cn/Article/details/gzilnbakw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.zdbjq.cn/Article/details/gjedkxiwg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gagchunsx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gxfbxrsrk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gojmjwnhw.sHtML

TS:   path.extname("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gqfpewxmc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.hesvh.cn/Article/details/glxooivqx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/guhhicsmz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gwtqvenhs.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gmmynywnj.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/gfaptyrbb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gskonvuys.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/gkxclrljg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gxgfmxzim.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/giemdvhyr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fehbvm.com/Article/details/gzuwulppv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/grbqowjxs.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gplkybbzf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.zdbjq.cn/Article/details/gofegogty.sHtML

[F12] CSV 读写
来源：http://baike.zdbjq.cn/Article/details/gqwbumbsh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fehbvm.com/Article/details/gzhfanclc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fehbvm.com/Article/details/ghsfwzpsm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fehbvm.com/Article/details/gphqayksk.sHtML

TS:   // 同上
来源：http://wap.zdbjq.cn/Article/details/gmzdnrref.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.hesvh.cn/Article/details/gljvihuir.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fehbvm.com/Article/details/gzrkucmrg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.zdbjq.cn/Article/details/goqsjtuob.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fehbvm.com/Article/details/ggzxhryku.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gampsyzvj.sHtML

G. 面向对象
来源：http://m.share.hesvh.cn/Article/details/gwienjxxe.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqjipwffo.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/gyztzirmr.sHtML

Py:   class User: pass
来源：http://wap.zdbjq.cn/Article/details/gjdvmqvja.sHtML

PHP:  class User {}
来源：http://mobile.zdbjq.cn/Article/details/ggamspbcy.sHtML

JS:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gzupcusrp.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fehbvm.com/Article/details/gbfacnirw.sHtML

Java: class User {}
来源：http://mobile.hesvh.cn/Article/details/gyvdlrzyc.sHtML

Go:   type User struct { Name string }
来源：http://3g.zdbjq.cn/Article/details/gpwxrtyzf.sHtML

Ruby: class User; end
来源：http://wap.fehbvm.com/Article/details/gbivhnsso.sHtML

C#:   class User {}
来源：http://wap.hesvh.cn/Article/details/glszmjtew.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gzpfbrreq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/gvydjmbdk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.zdbjq.cn/Article/details/gxiajbwnt.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwlmyscxd.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gcrrwvwfi.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gixvqihab.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/gfodjamxi.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/grxxggxbw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fehbvm.com/Article/details/gbpozuytr.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/gpgvdlham.sHtML

Py:   self.name = "x"
来源：http://blog.fehbvm.com/Article/details/gkqsrnter.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/glnsqvcxa.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/gffjcjhue.sHtML

TS:   name: string = "x";
来源：http://wap.zdbjq.cn/Article/details/gkljtegta.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/gdrvwvtru.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/gkixwcclh.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gdhfwdfis.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.zdbjq.cn/Article/details/gkkoyzoaw.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/gyyicarrn.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gveljdpyp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gspjzogfa.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gyqisnwxf.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/girvzgcwu.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gmjpaexvn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gjfiygrre.sHtML

Ruby: def greet; @name; end
来源：http://wap.fehbvm.com/Article/details/gakiwzfri.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/gzwhttmzd.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/gbsqxqwfc.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/guzhfzmod.sHtML

PHP:  class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gngwotnsw.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gagukdbba.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/glvjbqier.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/glbhoqvea.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fehbvm.com/Article/details/gwklpwhyj.sHtML

Ruby: class Admin < User; end
来源：http://blog.fehbvm.com/Article/details/gmlhtkyqr.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.hesvh.cn/Article/details/geputwcbn.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/gsrxnmzds.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.zdbjq.cn/Article/details/gfwvibnmf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gsjxxfpbi.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/ggiznionm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/ggofhhtqc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gbfimnomd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/gpgfqxwwq.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fehbvm.com/Article/details/gbqvxjacp.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.hesvh.cn/Article/details/gdedjcncd.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gyqfgqvsm.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/giduethvk.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/gcacpvppk.sHtML

JS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gtfkiglfi.sHtML

TS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/geiqisxbo.sHtML

Java: super.greet();
来源：http://m.share.fehbvm.com/Article/details/gobtuaplo.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/golyvzihz.sHtML

Ruby: super
来源：http://wap.hesvh.cn/Article/details/gzmxuxjao.sHtML

C#:   base.Greet();
来源：http://mobile.zdbjq.cn/Article/details/gzkssefkc.sHtML

[G08] 静态方法与属性
来源：http://3g.fehbvm.com/Article/details/gjamlurno.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/gcypuzufo.sHtML

PHP:  public static function f() {}
来源：http://mobile.zdbjq.cn/Article/details/gnwfdoztn.sHtML

JS:   static f() {}
来源：http://wap.zdbjq.cn/Article/details/gjgtfoegt.sHtML

TS:   static f(): void {}
来源：http://read.share.hesvh.cn/Article/details/gqywijjzk.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/ggbeksore.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fehbvm.com/Article/details/gcwsnpqpx.sHtML

Ruby: def self.f; end
来源：http://wap.fehbvm.com/Article/details/gotahgwmx.sHtML

C#:   public static void F() {}
来源：http://www.blog.fehbvm.com/Article/details/gigvtjsja.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/gjzrbrqhq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fehbvm.com/Article/details/gggadkzzs.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.hesvh.cn/Article/details/gcjpubagl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fehbvm.com/Article/details/gtfikptao.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.hesvh.cn/Article/details/glbdagjml.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.zdbjq.cn/Article/details/gbevrhbsi.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/grybxtwzv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.zdbjq.cn/Article/details/gmufafiih.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.hesvh.cn/Article/details/guckkdjfl.sHtML

[G10] 访问控制
来源：http://www.share.fehbvm.com/Article/details/gxjcqbmpq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/gyzhbouxr.sHtML

PHP:  public / protected / private
来源：http://baike.fehbvm.com/Article/details/gmdruclzy.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fehbvm.com/Article/details/gnjcbrmhu.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gejurrklr.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gblkxqyed.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fehbvm.com/Article/details/gsjpnmqof.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gmzipbowr.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.zdbjq.cn/Article/details/gegaondso.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/ghaksrbvo.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fehbvm.com/Article/details/gvbqpvcew.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gayjmkprn.sHtML

JS:   get name() { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gosinwnqs.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.hesvh.cn/Article/details/glfhamipx.sHtML

Java: public String getName() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gwwwlxqxr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/guubzpnmu.sHtML

Ruby: attr_accessor :name
来源：http://wap.fehbvm.com/Article/details/govovaxfb.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fehbvm.com/Article/details/gqpnagveb.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/gqdztqjor.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/goktrjyxe.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gvdyhnoxd.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gokigwlvu.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/ggojzbdnf.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gyodegcqb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/geyxwpgqk.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.hesvh.cn/Article/details/gmznezktq.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gusjyqdys.sHtML

[G13] 判断对象类型
来源：http://read.share.zdbjq.cn/Article/details/gnlwsvkyl.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.zdbjq.cn/Article/details/guuvyxlyz.sHtML

PHP:  $u instanceof User
来源：http://wap.fehbvm.com/Article/details/gmvbxxcvv.sHtML

JS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gkjblpelh.sHtML

TS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gggjsqzqg.sHtML

Java: u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/ggmckvuci.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.zdbjq.cn/Article/details/guqzcsjec.sHtML

Ruby: u.is_a?(User)
来源：http://blog.hesvh.cn/Article/details/gxepvmlkv.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/gphsjdvnz.sHtML

[G14] 数据类 / record
来源：http://baike.fehbvm.com/Article/details/gklljmgjv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.hesvh.cn/Article/details/gewlsvpnt.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.hesvh.cn/Article/details/geshdhcod.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.hesvh.cn/Article/details/glgbfrdpa.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.hesvh.cn/Article/details/gfszetabt.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.zdbjq.cn/Article/details/ghvncjfjc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fehbvm.com/Article/details/gkwhjiccm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.fehbvm.com/Article/details/gaggrwszc.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fehbvm.com/Article/details/gfqekvpne.sHtML

[G15] 枚举
来源：http://www.share.fehbvm.com/Article/details/gcpbfktfp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.hesvh.cn/Article/details/gjlhcgrsf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fehbvm.com/Article/details/gfasxmijh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.hesvh.cn/Article/details/gzuynhvsg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gcsppsnkh.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.hesvh.cn/Article/details/gyzdcturs.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fehbvm.com/Article/details/gfomtwkmd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fehbvm.com/Article/details/gbnvdpqcl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gprkhbqrw.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.zdbjq.cn/Article/details/gbvlnysse.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fehbvm.com/Article/details/gfxjqjgbv.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.hesvh.cn/Article/details/gsyqcxrez.sHtML

JS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/glegvckis.sHtML

TS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gqivtnxph.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.zdbjq.cn/Article/details/grylvezph.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.fehbvm.com/Article/details/gxlqkciez.sHtML

Ruby: obj.instance_variables
来源：http://blog.fehbvm.com/Article/details/gxtzylrhd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/ghoxsgtee.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glfprrhuv.sHtML

H. 异常与错误处理
来源：http://3g.zdbjq.cn/Article/details/gcdijghgo.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grvcuilrq.sHtML

[H01] try / catch 基础
来源：http://baike.hesvh.cn/Article/details/gsofmphkz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.fehbvm.com/Article/details/geieoejqu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.zdbjq.cn/Article/details/gtmwwarbu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gnyzqnwfp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gemcqizue.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.fehbvm.com/Article/details/glwytobas.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.zdbjq.cn/Article/details/geufnbdyj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.hesvh.cn/Article/details/guiwzjzlt.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/grwwlugru.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.zdbjq.cn/Article/details/girchcmyg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.fehbvm.com/Article/details/gizvadfcc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gjtpzswjr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/ghgesjxlh.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gdjyhlxzz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gkptucvuj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.zdbjq.cn/Article/details/gxotfglsk.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/gvswnksop.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gbdupabbf.sHtML

[H03] 主动抛出异常
来源：http://www.share.hesvh.cn/Article/details/gmkdcfqzq.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fehbvm.com/Article/details/ghnyedjup.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gdwepioke.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gyvxemdmn.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.fehbvm.com/Article/details/gsnrplgfk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gsraxlsgj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.hesvh.cn/Article/details/gjfgjghxw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.hesvh.cn/Article/details/ghbgwbxck.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gderbkhaq.sHtML

[H04] 自定义异常类型
来源：http://blog.hesvh.cn/Article/details/gsdqqeygg.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.fehbvm.com/Article/details/gqdqepfit.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gixkredyj.sHtML

JS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/guybtqjsb.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gynbfcrcw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/gplqpckxf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.hesvh.cn/Article/details/grjekkfuu.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.zdbjq.cn/Article/details/gmsihkzac.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.fehbvm.com/Article/details/gowuguzyw.sHtML

[H05] 捕获特定类型
来源：http://read.share.hesvh.cn/Article/details/glymnwyja.sHtML

Py:   except ValueError as e:
来源：http://www.blog.zdbjq.cn/Article/details/giuxyokpq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.hesvh.cn/Article/details/gjmszmdzw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gosvuodwt.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/gwppbtumn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.fehbvm.com/Article/details/gjnhctqsh.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fehbvm.com/Article/details/gqadivcvt.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.zdbjq.cn/Article/details/ghnuzkhgn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.fehbvm.com/Article/details/gyqlothao.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.hesvh.cn/Article/details/gxllhlhgm.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fehbvm.com/Article/details/gatnaqcbd.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/gvwamigwx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gvaaxyukg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gznnjgyto.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.zdbjq.cn/Article/details/gkekndcol.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.hesvh.cn/Article/details/gtgqrsiiu.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.zdbjq.cn/Article/details/gfihtlkdg.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.fehbvm.com/Article/details/gifxmdztm.sHtML

[H07] 断言
来源：http://blog.hesvh.cn/Article/details/gylpliazn.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.hesvh.cn/Article/details/gatrodnrt.sHtML

PHP:  assert($x > 0);
来源：http://baike.zdbjq.cn/Article/details/gwiyirhqu.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gvrvnnznj.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gyjzavjrg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.zdbjq.cn/Article/details/gnuehmghs.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.fehbvm.com/Article/details/gwbjaavdt.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.hesvh.cn/Article/details/ghvkxdlqp.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gawcmofla.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.hesvh.cn/Article/details/guwrlvnec.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.hesvh.cn/Article/details/gprurnkks.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.zdbjq.cn/Article/details/ggvfccabi.sHtML

JS:   e.message;  e.stack
来源：http://wap.zdbjq.cn/Article/details/gyossgmfg.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.hesvh.cn/Article/details/gqzqnfzan.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.fehbvm.com/Article/details/guspsoxui.sHtML

Go:   err.Error()
来源：http://read.share.zdbjq.cn/Article/details/gbuxevgmk.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.fehbvm.com/Article/details/gjdkyxdhu.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.zdbjq.cn/Article/details/gybyqkmjy.sHtML

[H09] 带错误码的异常
来源：http://mobile.zdbjq.cn/Article/details/gxzinlslc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.fehbvm.com/Article/details/gnzoydswg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.zdbjq.cn/Article/details/gigsrrzai.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.zdbjq.cn/Article/details/gkossevyw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.hesvh.cn/Article/details/gwrvpyhig.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.hesvh.cn/Article/details/gzvmpqlvw.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.hesvh.cn/Article/details/gybwrddmm.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.hesvh.cn/Article/details/gbjfqypsb.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.hesvh.cn/Article/details/gxbpbiigs.sHtML

[H10] 资源自动释放
来源：http://baike.fehbvm.com/Article/details/gnceotwro.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.fehbvm.com/Article/details/glqbmxpew.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.zdbjq.cn/Article/details/gferisqgn.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.hesvh.cn/Article/details/guyqpbbdc.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.hesvh.cn/Article/details/gmlwelauz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.hesvh.cn/Article/details/gdinmdqxz.sHtML

Go:   defer f.Close()
来源：http://blog.zdbjq.cn/Article/details/gbaszlllo.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.hesvh.cn/Article/details/gonqqsaep.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gqrlrraom.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gpmxdcffu.sHtML

I. 正则表达式
来源：http://m.share.fehbvm.com/Article/details/gofmqgyvy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnszqpasl.sHtML

[I01] 判断是否匹配
来源：http://baike.fehbvm.com/Article/details/gdnxdclpo.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.fehbvm.com/Article/details/gamiuyigq.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gcmbjbxud.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/gwmvfxgem.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fehbvm.com/Article/details/gzfcyrpok.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.hesvh.cn/Article/details/gebxuhfcv.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.fehbvm.com/Article/details/grieunpeb.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.hesvh.cn/Article/details/gfpmdonkp.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.fehbvm.com/Article/details/gfsganomc.sHtML

[I02] 提取所有匹配
来源：http://wap.zdbjq.cn/Article/details/gidgxozph.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.fehbvm.com/Article/details/gmmopegxx.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.zdbjq.cn/Article/details/gwzdpnsrh.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.zdbjq.cn/Article/details/gzrmdjuya.sHtML


<!-- 参考信息 -->