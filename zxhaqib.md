代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.zdbjq.cn/Article/details/gfufezcfi.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gvmycpqrk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/guiepvjiy.sHtML

[F12] CSV 读写
来源：http://mobile.zdbjq.cn/Article/details/grqwzqcwe.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fehbvm.com/Article/details/ghvcrtzbi.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/gidlwjrjx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/gucsmyrsp.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/gbiatnojh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.hesvh.cn/Article/details/gxnlscosu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.hesvh.cn/Article/details/giplknvdz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fehbvm.com/Article/details/gylktwyhy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.hesvh.cn/Article/details/ghjccrssz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gnwhwterj.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/gkcshiwth.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwbqccumh.sHtML

[G01] 定义类
来源：http://read.share.hesvh.cn/Article/details/ghrnzgvxv.sHtML

Py:   class User: pass
来源：http://blog.fehbvm.com/Article/details/gaoitvxpg.sHtML

PHP:  class User {}
来源：http://m.share.hesvh.cn/Article/details/gpqexdtsc.sHtML

JS:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gphgwipki.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.hesvh.cn/Article/details/gxvapehfw.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/ghmknhsfs.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fehbvm.com/Article/details/grwwwggcg.sHtML

Ruby: class User; end
来源：http://www.share.fehbvm.com/Article/details/gyjeazxsu.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/gsiteexto.sHtML

[G02] 构造函数
来源：http://mobile.fehbvm.com/Article/details/gofufhwnr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.hesvh.cn/Article/details/glrmbqaoe.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.hesvh.cn/Article/details/geyxquyzu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gfgmiinov.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fehbvm.com/Article/details/gmfgjypid.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/ghdkdpbda.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.hesvh.cn/Article/details/gzmiajurn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fehbvm.com/Article/details/gxmgkxzro.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfkrtgfhf.sHtML

[G03] 实例属性
来源：http://www.blog.zdbjq.cn/Article/details/gghylzouo.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/gwldjprrv.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/gtlnbtgqk.sHtML

JS:   this.name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gretewljd.sHtML

TS:   name: string = "x";
来源：http://m.share.zdbjq.cn/Article/details/gzzgxbuho.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/grfxrqdze.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/gfqedfcjy.sHtML

Ruby: @name = "x"
来源：http://baike.zdbjq.cn/Article/details/gtztcqhqe.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.zdbjq.cn/Article/details/gjgsguqom.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/gmyrvgzvn.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gxvzakvjv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/grdfgijxb.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gcfjakrkh.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gaetsfhzo.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/gudlxubey.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/geomqnuad.sHtML

Ruby: def greet; @name; end
来源：http://mobile.hesvh.cn/Article/details/gqecmsvsl.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gnmumuifv.sHtML

[G05] 继承
来源：http://www.share.zdbjq.cn/Article/details/gbmjqbbvs.sHtML

Py:   class Admin(User): pass
来源：http://wap.zdbjq.cn/Article/details/gkqixfqqg.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gykphwegt.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gjjifeafe.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gaqvvcwaa.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gbcxcnouh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gwxaqovst.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/gigzhrjth.sHtML

C#:   class Admin : User {}
来源：http://wap.fehbvm.com/Article/details/gluwyagnj.sHtML

[G06] 重写方法
来源：http://3g.hesvh.cn/Article/details/gfrchazpz.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/gnkuubrjo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gdcdnpswp.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gedtojaie.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gvodanjxn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gbjwrnrww.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.zdbjq.cn/Article/details/gqmzrbcbt.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.zdbjq.cn/Article/details/gwwywxsdf.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/glkilvfjp.sHtML

[G07] 调用父类方法
来源：http://baike.hesvh.cn/Article/details/gevabcvzo.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/gulgxusuy.sHtML

PHP:  parent::greet();
来源：http://www.share.hesvh.cn/Article/details/gtlrhnpvq.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gdtnvifuz.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gamjranrv.sHtML

Java: super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gqffelimo.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fehbvm.com/Article/details/glpjsnsxs.sHtML

Ruby: super
来源：http://m.share.fehbvm.com/Article/details/gflfdkxne.sHtML

C#:   base.Greet();
来源：http://baike.fehbvm.com/Article/details/glyeujvxl.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/guzeduwwn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fehbvm.com/Article/details/gxwrnujmm.sHtML

PHP:  public static function f() {}
来源：http://mobile.zdbjq.cn/Article/details/geolpfzau.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/gtllsubcp.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/gvtvkjlyp.sHtML

Java: static void f() {}
来源：http://m.share.zdbjq.cn/Article/details/gvoovtmht.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.zdbjq.cn/Article/details/gkxxbalku.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/gcusypcty.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/gbkkfhuxk.sHtML

[G09] 接口 / 抽象类
来源：http://wap.hesvh.cn/Article/details/gtnmxszcd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fehbvm.com/Article/details/gmsaqdtjt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/grbplzfpo.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fehbvm.com/Article/details/glnboiutf.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/gtnpguquk.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/gegvxkkrr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.hesvh.cn/Article/details/ghvmpgvha.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.hesvh.cn/Article/details/gumpbnuru.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/gqxyqplon.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/gqhnwdgrp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.zdbjq.cn/Article/details/gnypjbjdx.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gqspolrkh.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.hesvh.cn/Article/details/gzxxdtayu.sHtML

TS:   public / protected / private
来源：http://wap.hesvh.cn/Article/details/gcuvwpihh.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.hesvh.cn/Article/details/gzpkcznif.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fehbvm.com/Article/details/grcgsqzds.sHtML

Ruby: public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gpdtjsxdm.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fehbvm.com/Article/details/gjqkotxuu.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/gjxnkrhtp.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.zdbjq.cn/Article/details/gkieyqbhe.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gcxbjfslc.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gekhsgpmd.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gaewehsyd.sHtML

Java: public String getName() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gwtlihsbr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gbnyhpida.sHtML

Ruby: attr_accessor :name
来源：http://read.share.zdbjq.cn/Article/details/gfncsbcoe.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fehbvm.com/Article/details/gddyzpbxg.sHtML

[G12] 对象转字符串
来源：http://mobile.zdbjq.cn/Article/details/grfenqsww.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gzwgkpura.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gbsdzrpqm.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gpwjvpqjx.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gaqgbdpdz.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fehbvm.com/Article/details/gpceypwsm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gnniuvzhh.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gxyohhkwr.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.zdbjq.cn/Article/details/grkdrzmia.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/gnskgfbde.sHtML

Py:   isinstance(u, User)
来源：http://blog.zdbjq.cn/Article/details/gdlvsqyky.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gbuzugkey.sHtML

JS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gzoeawvjj.sHtML

TS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gkglbddwm.sHtML

Java: u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gdkulxtes.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.zdbjq.cn/Article/details/gufidugjx.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.hesvh.cn/Article/details/gddfngiqr.sHtML

C#:   u is User
来源：http://www.blog.hesvh.cn/Article/details/ggxwvtyec.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/goqnbgnqs.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.fehbvm.com/Article/details/gatscxcpf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fehbvm.com/Article/details/gpzeurthh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.zdbjq.cn/Article/details/gxlthjvmd.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.zdbjq.cn/Article/details/ghffctcjm.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/gfqfjwerq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.zdbjq.cn/Article/details/gpbqujwhl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/gnwjeeldc.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fehbvm.com/Article/details/gcuhugcsk.sHtML

[G15] 枚举
来源：http://read.share.hesvh.cn/Article/details/gzkxyprsh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fehbvm.com/Article/details/gpzjgxdhn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/gbjpyysyg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fehbvm.com/Article/details/gdtiujzex.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gfyvngpkb.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fehbvm.com/Article/details/gqljajexh.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.zdbjq.cn/Article/details/gdvuvoktu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.hesvh.cn/Article/details/gldwdwcxp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gtcrieqeb.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.hesvh.cn/Article/details/gcezavqkx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.hesvh.cn/Article/details/gjsjvcsdk.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.hesvh.cn/Article/details/gfugetdmm.sHtML

JS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gffolakdo.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gyfrpoceb.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fehbvm.com/Article/details/gidjqgxrb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.zdbjq.cn/Article/details/ggbciqbgj.sHtML

Ruby: obj.instance_variables
来源：http://3g.fehbvm.com/Article/details/gipmvdazj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gleqnztvr.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gchnwmitg.sHtML

H. 异常与错误处理
来源：http://m.share.fehbvm.com/Article/details/gutsuqbyt.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gpsbdapsq.sHtML

[H01] try / catch 基础
来源：http://wap.fehbvm.com/Article/details/gftezrfdc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.hesvh.cn/Article/details/ghojvhait.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.zdbjq.cn/Article/details/gymmjoddt.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gapkndrnr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/ghbauoapf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.zdbjq.cn/Article/details/gxxmjzcwg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fehbvm.com/Article/details/gkyjamlsc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.fehbvm.com/Article/details/goildbuxn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.fehbvm.com/Article/details/gxvftbiyh.sHtML

[H02] finally / ensure 收尾
来源：http://baike.zdbjq.cn/Article/details/gohmtxenv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.zdbjq.cn/Article/details/gcqevairu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gtmbxucil.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gqtkjgson.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gmmhyacxh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gvaelfebg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.hesvh.cn/Article/details/gfuvskurk.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fehbvm.com/Article/details/grtdjtoxy.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gypzfcbyp.sHtML

[H03] 主动抛出异常
来源：http://baike.zdbjq.cn/Article/details/gcwogujfv.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.hesvh.cn/Article/details/gscgtrhpf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gxedakkmg.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gzcveevjl.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gniblnlmz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gixpybzrh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.zdbjq.cn/Article/details/gtcqldkzx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.zdbjq.cn/Article/details/gprehajft.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gezxaglcw.sHtML

[H04] 自定义异常类型
来源：http://wap.fehbvm.com/Article/details/gojloymlk.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fehbvm.com/Article/details/gwtxsaojz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gjicfavbn.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gekzvgjvr.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gwlfjwavc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gbjprdymn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.hesvh.cn/Article/details/gmmyecsbr.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.hesvh.cn/Article/details/glyccvcgd.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fehbvm.com/Article/details/gqmgrywch.sHtML

[H05] 捕获特定类型
来源：http://wap.hesvh.cn/Article/details/gxtflovrb.sHtML

Py:   except ValueError as e:
来源：http://baike.hesvh.cn/Article/details/gwukmnbsf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.hesvh.cn/Article/details/gygmqcqnu.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/gtypuwfbb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gqhhpkuon.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fehbvm.com/Article/details/ghrueoddt.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fehbvm.com/Article/details/gcwtwtqki.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.zdbjq.cn/Article/details/gacrqgnnd.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.hesvh.cn/Article/details/gzwyfmmxi.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fehbvm.com/Article/details/ghsbehfsu.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.zdbjq.cn/Article/details/gnwvevfhk.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gjbwrineo.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/guwxjvkqq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gzczuoysb.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fehbvm.com/Article/details/gqufbfbfp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.fehbvm.com/Article/details/gdlouetrk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.hesvh.cn/Article/details/ginwijmod.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.zdbjq.cn/Article/details/geaomadwj.sHtML

[H07] 断言
来源：http://blog.zdbjq.cn/Article/details/gilmbemqh.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.hesvh.cn/Article/details/gfusjcxah.sHtML

PHP:  assert($x > 0);
来源：http://blog.fehbvm.com/Article/details/gnoidlbrb.sHtML

JS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gvspfkbmu.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gimwzqytx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.hesvh.cn/Article/details/gtdbccbch.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.hesvh.cn/Article/details/glfctgouv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.fehbvm.com/Article/details/gnnqsfqog.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gaorqvlau.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.zdbjq.cn/Article/details/gaynvuxoi.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.fehbvm.com/Article/details/ghnnikkgf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.fehbvm.com/Article/details/gzbjehuym.sHtML

JS:   e.message;  e.stack
来源：http://baike.fehbvm.com/Article/details/gleudtjqt.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.zdbjq.cn/Article/details/grqlpvelh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.fehbvm.com/Article/details/gogiyjpla.sHtML

Go:   err.Error()
来源：http://read.share.fehbvm.com/Article/details/gxlhottpn.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.hesvh.cn/Article/details/gmhiekuyf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.fehbvm.com/Article/details/gjxvmgvzu.sHtML

[H09] 带错误码的异常
来源：http://mobile.zdbjq.cn/Article/details/gjtazquqp.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.fehbvm.com/Article/details/grlvrpmlv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.hesvh.cn/Article/details/gigclzbjk.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.hesvh.cn/Article/details/gkeowggmw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.hesvh.cn/Article/details/geescwhve.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.zdbjq.cn/Article/details/gxfeyzcqu.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.hesvh.cn/Article/details/gkpjaxdjg.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.zdbjq.cn/Article/details/gpcifdklh.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.hesvh.cn/Article/details/gflnslitf.sHtML

[H10] 资源自动释放
来源：http://mobile.hesvh.cn/Article/details/gnjpmomwo.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.zdbjq.cn/Article/details/ghdyjdchb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.hesvh.cn/Article/details/gnysorhvw.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/gmydttgaj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.hesvh.cn/Article/details/gqotrzdqz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.zdbjq.cn/Article/details/ghczpgwzb.sHtML

Go:   defer f.Close()
来源：http://read.share.fehbvm.com/Article/details/gxsnlfdgf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.fehbvm.com/Article/details/gnqgdatrr.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gulmjynfr.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxrfufbbu.sHtML

I. 正则表达式
来源：http://www.blog.fehbvm.com/Article/details/ggnxkhean.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfmkvtfcm.sHtML

[I01] 判断是否匹配
来源：http://blog.fehbvm.com/Article/details/gfuwqtorq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.hesvh.cn/Article/details/gtdccpweq.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/ghmneexej.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.fehbvm.com/Article/details/gnggiejit.sHtML

TS:   /\d+/.test(s)
来源：http://baike.zdbjq.cn/Article/details/gjrzrqbms.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.fehbvm.com/Article/details/gthlbbwgx.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.zdbjq.cn/Article/details/gyeqtzmij.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.fehbvm.com/Article/details/gzxgdjybf.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/gjdlhiwjl.sHtML

[I02] 提取所有匹配
来源：http://www.share.fehbvm.com/Article/details/grzxtztsh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.zdbjq.cn/Article/details/gcnrfrznm.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.zdbjq.cn/Article/details/ghksjlhzx.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.zdbjq.cn/Article/details/gyznutvnz.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.hesvh.cn/Article/details/gjtqndbll.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.zdbjq.cn/Article/details/gtzsppyyq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.zdbjq.cn/Article/details/gyeumkklk.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.fehbvm.com/Article/details/gxjtmlcrx.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.hesvh.cn/Article/details/govhwqkzs.sHtML

[I03] 提取捕获分组
来源：http://www.blog.fehbvm.com/Article/details/gaoffxyjl.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.hesvh.cn/Article/details/gubmzkcgo.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gqtyzwcpd.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.hesvh.cn/Article/details/getalouxd.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.hesvh.cn/Article/details/gywzlfgps.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.fehbvm.com/Article/details/gcdgfxgqo.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.zdbjq.cn/Article/details/gqztadamy.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.zdbjq.cn/Article/details/gukezzhko.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.zdbjq.cn/Article/details/grodimeyy.sHtML

[I04] 正则替换
来源：http://3g.zdbjq.cn/Article/details/gzxpzigwf.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.hesvh.cn/Article/details/gzggbtcgp.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gnrsqpjvx.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/gjoswiuzy.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.hesvh.cn/Article/details/gyikdzvre.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.zdbjq.cn/Article/details/gdnmfdwzk.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.fehbvm.com/Article/details/gajuwznmh.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.zdbjq.cn/Article/details/ghzfsddhl.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.fehbvm.com/Article/details/gnwyhdhfm.sHtML

[I05] 按正则拆分
来源：http://3g.fehbvm.com/Article/details/gfdeuwtuf.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.hesvh.cn/Article/details/gbavqvjbw.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.hesvh.cn/Article/details/gbpehqqln.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/guzlcemai.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gpkupfnhw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.fehbvm.com/Article/details/gwelpbzag.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.fehbvm.com/Article/details/gkhqrpdau.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/gqnxisglm.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.zdbjq.cn/Article/details/gnijqhsdz.sHtML


<!-- 参考信息 -->