代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.zdbjq.cn/Article/details/guvkutauk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.hesvh.cn/Article/details/gskfilsgs.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.zdbjq.cn/Article/details/gxydhkaks.sHtML

[F08] 遍历目录
来源：http://3g.zdbjq.cn/Article/details/gqrejaqmb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.hesvh.cn/Article/details/gffsfkvzl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.zdbjq.cn/Article/details/gubewncrq.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/grqfpkwsb.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gsedtoykt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gjihbruse.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fehbvm.com/Article/details/ghourwvti.sHtML

Ruby: Dir.children("dir")
来源：http://blog.hesvh.cn/Article/details/gdrxhtgpe.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fehbvm.com/Article/details/galgbxgzu.sHtML

[F09] 获取文件大小
来源：http://www.m.share.hesvh.cn/Article/details/gdobsmlac.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gdrwzfpfq.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gsqnsjkhu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gehsvlusr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gakjgaiqm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/ggmfpytek.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.hesvh.cn/Article/details/gjxhnxxsb.sHtML

Ruby: File.size("a.txt")
来源：http://blog.zdbjq.cn/Article/details/ggtxknzmr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fehbvm.com/Article/details/gxepfaizj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/gbxaiwbqd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gzvoktcsy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/gkbnpusnw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gtqqvfxfa.sHtML

TS:   path.extname("a.txt")
来源：http://3g.hesvh.cn/Article/details/gxrjndrjm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fehbvm.com/Article/details/gcjcjtcdg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/geppfetnj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gxkdpyedc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gfsaotrts.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/goacdjroe.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gsxcrmyvh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.hesvh.cn/Article/details/gvkpwjpxr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gqqdjwapy.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gxhyhzhok.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gqnfqroow.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.zdbjq.cn/Article/details/gryhwkuck.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gwvolwhzs.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/gyxguqkwe.sHtML

[F12] CSV 读写
来源：http://m.share.fehbvm.com/Article/details/gnnuikejj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.zdbjq.cn/Article/details/gkttmhajt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/gxrpvtbpl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fehbvm.com/Article/details/gjitnrcpf.sHtML

TS:   // 同上
来源：http://www.share.zdbjq.cn/Article/details/gebtjwmxw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/gzfrdrebv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fehbvm.com/Article/details/gkukmozeb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fehbvm.com/Article/details/gxwhqfcvb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/glturjqpp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grxousktq.sHtML

G. 面向对象
来源：http://3g.hesvh.cn/Article/details/gqkkaanbd.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gappxxdaq.sHtML

[G01] 定义类
来源：http://read.share.fehbvm.com/Article/details/ggwkaxpwf.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/ggnsxvzhk.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/gthcupans.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gctnhuukd.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/gvxzcpmhy.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/gxgxtjfoi.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.hesvh.cn/Article/details/gyfxpupea.sHtML

Ruby: class User; end
来源：http://www.share.zdbjq.cn/Article/details/gjuoakqmf.sHtML

C#:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gjzpjypvq.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/gmvlnfwtd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.hesvh.cn/Article/details/gcsqnxyka.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwtlotcgu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gsojmallg.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/gesdxxqlb.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gradxbzfn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fehbvm.com/Article/details/grscswmcz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fehbvm.com/Article/details/gkubdwbai.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/gldqrvptq.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/gnrmypgcq.sHtML

Py:   self.name = "x"
来源：http://read.share.fehbvm.com/Article/details/gabclhtpb.sHtML

PHP:  public string $name = "x";
来源：http://blog.zdbjq.cn/Article/details/gtculfiro.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gnvxmdkzu.sHtML

TS:   name: string = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gckgjyhlv.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/guvdgfbtg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.hesvh.cn/Article/details/grbhzckmi.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gyjvkdspb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/gndgqffmf.sHtML

[G04] 定义方法
来源：http://baike.hesvh.cn/Article/details/gqxyfloqa.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gcljwnzbw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gposexjfo.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gjyealoca.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gkpwqlwud.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gezmczcac.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gfsizatqd.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fehbvm.com/Article/details/gnxfrxdco.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gadpoqcys.sHtML

[G05] 继承
来源：http://read.share.fehbvm.com/Article/details/gqnsrohwp.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/gnthowhlk.sHtML

PHP:  class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gdkykgnqr.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gmqdvkjsj.sHtML

TS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gddsdhupd.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gbcygadsp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/gxbgbxrgv.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.hesvh.cn/Article/details/gksgbamba.sHtML

C#:   class Admin : User {}
来源：http://3g.zdbjq.cn/Article/details/gmopfjprb.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/gqikplyes.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/gaxkvdwqy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/grlchokhi.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gbusbrolh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/geuktaxjy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gminafkob.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fehbvm.com/Article/details/gzpwgaxcd.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/gmlrxyvhm.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.hesvh.cn/Article/details/gpmtkgniy.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/guoqoviti.sHtML

Py:   super().greet()
来源：http://read.share.zdbjq.cn/Article/details/geqqjwzsh.sHtML

PHP:  parent::greet();
来源：http://3g.hesvh.cn/Article/details/gyziivicp.sHtML

JS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gybawjpvm.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gukfofbzj.sHtML

Java: super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gouwzmeoi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/gqoxhpuvs.sHtML

Ruby: super
来源：http://mobile.fehbvm.com/Article/details/gqvzgtrep.sHtML

C#:   base.Greet();
来源：http://baike.fehbvm.com/Article/details/gplkrpvlv.sHtML

[G08] 静态方法与属性
来源：http://m.share.hesvh.cn/Article/details/gjqjoakhi.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.hesvh.cn/Article/details/gftcfxxpc.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/gtbzqxpph.sHtML

JS:   static f() {}
来源：http://baike.zdbjq.cn/Article/details/gqxapexcj.sHtML

TS:   static f(): void {}
来源：http://read.share.zdbjq.cn/Article/details/gvgbsjkit.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gdbiuiras.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/gczehcfms.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/ghqylbqrq.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/gqhqqbxsb.sHtML

[G09] 接口 / 抽象类
来源：http://3g.hesvh.cn/Article/details/ghmgmlcal.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.zdbjq.cn/Article/details/gjrrwjuie.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/grftonmdo.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fehbvm.com/Article/details/gruayggsa.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fehbvm.com/Article/details/gnwlieqnb.sHtML

Java: interface Shape { double area(); }
来源：http://baike.zdbjq.cn/Article/details/goumzhcbl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.zdbjq.cn/Article/details/gsvvqyklf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.hesvh.cn/Article/details/gcwaqratw.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.hesvh.cn/Article/details/gaoahsfdt.sHtML

[G10] 访问控制
来源：http://www.blog.fehbvm.com/Article/details/gibtgkkas.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fehbvm.com/Article/details/gqkoohude.sHtML

PHP:  public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gldjgzhac.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/gvwdidiaf.sHtML

TS:   public / protected / private
来源：http://wap.fehbvm.com/Article/details/gpmhnortg.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/gtzdfmlzz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.zdbjq.cn/Article/details/grnmbfgrp.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gkcqvdhpy.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/goskkueeg.sHtML

[G11] getter / setter
来源：http://www.blog.hesvh.cn/Article/details/glhdndgem.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.zdbjq.cn/Article/details/gnjgxlpww.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gijlfshhz.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/ghvqsylwd.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/ghqewbayv.sHtML

Java: public String getName() { return name; }
来源：http://3g.hesvh.cn/Article/details/gpfxcpihg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gsnwkyorx.sHtML

Ruby: attr_accessor :name
来源：http://blog.fehbvm.com/Article/details/gcqyoilwd.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.zdbjq.cn/Article/details/gdxgdydmb.sHtML

[G12] 对象转字符串
来源：http://www.share.zdbjq.cn/Article/details/ghjgjuswj.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/grthkpsmr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/ghxoniwfs.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gviipexqq.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gjayrnnjt.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gzzwwuvrz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/goarecvzd.sHtML

Ruby: def to_s; @name; end
来源：http://blog.hesvh.cn/Article/details/gyebmwxqb.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.hesvh.cn/Article/details/gdfzqcbfh.sHtML

[G13] 判断对象类型
来源：http://baike.zdbjq.cn/Article/details/gwkbkloaq.sHtML

Py:   isinstance(u, User)
来源：http://wap.hesvh.cn/Article/details/ggtlpyuhj.sHtML

PHP:  $u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gscbhrvls.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gvrljbmup.sHtML

TS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gomjpxbaf.sHtML

Java: u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gwgnlilbu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.hesvh.cn/Article/details/gmnedetih.sHtML

Ruby: u.is_a?(User)
来源：http://3g.hesvh.cn/Article/details/gzvgdjrlx.sHtML

C#:   u is User
来源：http://www.share.zdbjq.cn/Article/details/gaqbkvhir.sHtML

[G14] 数据类 / record
来源：http://m.share.zdbjq.cn/Article/details/gkxdmcwcg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/glviaiqsn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.zdbjq.cn/Article/details/gveqtfayt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.hesvh.cn/Article/details/gumbfltaz.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.zdbjq.cn/Article/details/guecuysqm.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.zdbjq.cn/Article/details/giecchrna.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fehbvm.com/Article/details/gowzycscz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/gypdhgwmq.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.fehbvm.com/Article/details/gdhvhaldy.sHtML

[G15] 枚举
来源：http://baike.hesvh.cn/Article/details/gswpzhmwx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fehbvm.com/Article/details/gmbgkkilk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fehbvm.com/Article/details/geucrjaxq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.hesvh.cn/Article/details/gdrtdlpua.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gzdudxxia.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/gzuosjrfa.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.hesvh.cn/Article/details/gtcgaaepm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fehbvm.com/Article/details/gfeldrtgx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/ghynkbquj.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.zdbjq.cn/Article/details/ghrflrsjh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fehbvm.com/Article/details/gkytosnkt.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.hesvh.cn/Article/details/gatcedwhd.sHtML

JS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gpedtxfau.sHtML

TS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gdxhxkzdr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.zdbjq.cn/Article/details/gcbdmlxqa.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.zdbjq.cn/Article/details/giscthcfm.sHtML

Ruby: obj.instance_variables
来源：http://www.share.zdbjq.cn/Article/details/gbtblubue.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.fehbvm.com/Article/details/giethrchf.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvqutisgz.sHtML

H. 异常与错误处理
来源：http://www.blog.hesvh.cn/Article/details/gbvgtawik.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/giwuznwgk.sHtML

[H01] try / catch 基础
来源：http://mobile.zdbjq.cn/Article/details/gwydeopvc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.hesvh.cn/Article/details/gqzmjkowi.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fehbvm.com/Article/details/gbiepwpxd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gzrcinomg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gdbgwwynt.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.fehbvm.com/Article/details/gvdhdaftj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.hesvh.cn/Article/details/gqwkwhmpe.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fehbvm.com/Article/details/gycwgtqyp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.fehbvm.com/Article/details/gdsqdctac.sHtML

[H02] finally / ensure 收尾
来源：http://blog.zdbjq.cn/Article/details/gtywaeeff.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.hesvh.cn/Article/details/gzczikhsd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gpuyibanu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gsgvkvrse.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gwccmjgqj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gyjilbcfz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fehbvm.com/Article/details/gqwsfizhh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/gzwvljitg.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gdiimxwif.sHtML

[H03] 主动抛出异常
来源：http://blog.hesvh.cn/Article/details/glgoxliog.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.hesvh.cn/Article/details/gyapntrdi.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gtyjrcsmw.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/guvbgsmbt.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/ggdekmsgr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gnwemozow.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.hesvh.cn/Article/details/gnfbwtrll.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.zdbjq.cn/Article/details/githzuvum.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/ghssqtors.sHtML

[H04] 自定义异常类型
来源：http://3g.hesvh.cn/Article/details/gmaxrghrz.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.zdbjq.cn/Article/details/goooeuscx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gwyhmyfcb.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gfkwiqzpp.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gzetxmqlv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gygitbroa.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.zdbjq.cn/Article/details/gijcjizog.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fehbvm.com/Article/details/gmzvsosyt.sHtML

C#:   class MyException : Exception {}
来源：http://wap.hesvh.cn/Article/details/ghwpjaorx.sHtML

[H05] 捕获特定类型
来源：http://3g.fehbvm.com/Article/details/gkabsvutw.sHtML

Py:   except ValueError as e:
来源：http://www.share.fehbvm.com/Article/details/gqglcqkhv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.hesvh.cn/Article/details/grerpsxei.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gigcuircc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gmifuyyjp.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.hesvh.cn/Article/details/gnmshiggp.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.zdbjq.cn/Article/details/gvuoegafx.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.zdbjq.cn/Article/details/gvvxqszue.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.fehbvm.com/Article/details/gsjsfppzi.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.fehbvm.com/Article/details/gfydlsosy.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.fehbvm.com/Article/details/goixbfxyo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/glhlnmdzr.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/gldzwlnmw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gwspvsnws.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.zdbjq.cn/Article/details/glqribafq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.zdbjq.cn/Article/details/gkffxthfg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.zdbjq.cn/Article/details/gcexcfggd.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gonzoovcg.sHtML

[H07] 断言
来源：http://3g.zdbjq.cn/Article/details/gtdwvqckk.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.fehbvm.com/Article/details/gryersitk.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gfzktfchs.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gqstemeuv.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/glaubcfkt.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.hesvh.cn/Article/details/gqydqzjou.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.zdbjq.cn/Article/details/gwoujbqph.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.hesvh.cn/Article/details/ggffhhdan.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/guzcnknur.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.zdbjq.cn/Article/details/gpzhhqkvs.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.zdbjq.cn/Article/details/gsyprsusf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.zdbjq.cn/Article/details/gxhbqnkhj.sHtML

JS:   e.message;  e.stack
来源：http://3g.zdbjq.cn/Article/details/gtfmfxlec.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fehbvm.com/Article/details/gkotauhgv.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.fehbvm.com/Article/details/gueqgompb.sHtML

Go:   err.Error()
来源：http://wap.zdbjq.cn/Article/details/gwzzrbyzr.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.zdbjq.cn/Article/details/goaddcgwk.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.hesvh.cn/Article/details/guuspjrur.sHtML

[H09] 带错误码的异常
来源：http://mobile.zdbjq.cn/Article/details/gqggmgmpq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.zdbjq.cn/Article/details/gvvjibxox.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.fehbvm.com/Article/details/gbmreidqc.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.zdbjq.cn/Article/details/gvirhxozz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.fehbvm.com/Article/details/gnojcutdp.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.hesvh.cn/Article/details/gmjysqjgi.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.fehbvm.com/Article/details/gkmnzslgv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.fehbvm.com/Article/details/gdlysujbd.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.fehbvm.com/Article/details/grmksbbjk.sHtML

[H10] 资源自动释放
来源：http://3g.fehbvm.com/Article/details/gqzxbskcx.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.fehbvm.com/Article/details/gxgzmqzkd.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.hesvh.cn/Article/details/gbnodlxzz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/gyczrcmtn.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/gfzeketip.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.fehbvm.com/Article/details/gomjpfggi.sHtML

Go:   defer f.Close()
来源：http://blog.fehbvm.com/Article/details/glaxhbwtl.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.zdbjq.cn/Article/details/glwbhofkr.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gmubvthra.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmudkgppn.sHtML

I. 正则表达式
来源：http://mobile.hesvh.cn/Article/details/gkkgtzqws.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gasjzyjzf.sHtML

[I01] 判断是否匹配
来源：http://mobile.zdbjq.cn/Article/details/ghwxckkac.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.hesvh.cn/Article/details/gmevdaras.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.hesvh.cn/Article/details/gyojvwnbp.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.fehbvm.com/Article/details/gzyocdoml.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.hesvh.cn/Article/details/gsmhlpkvh.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.zdbjq.cn/Article/details/gqtohkatm.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.zdbjq.cn/Article/details/gqijupjhj.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.fehbvm.com/Article/details/gcuowpvbs.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.hesvh.cn/Article/details/grvapxvcp.sHtML


<!-- 参考信息 -->