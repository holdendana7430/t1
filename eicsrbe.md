代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fehbvm.com/Article/details/gckkttypd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/geelxutgn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/gqithizlk.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/gvrhautmc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/gunnwuyob.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fehbvm.com/Article/details/gwywaluib.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/gydmgzzkx.sHtML

TS:   // 同上
来源：http://wap.zdbjq.cn/Article/details/gwhhltdnu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fehbvm.com/Article/details/gbjzdzuib.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/giuoqqtyx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.hesvh.cn/Article/details/ghufyjlip.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.zdbjq.cn/Article/details/grzhdatha.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkjfblapx.sHtML

G. 面向对象
来源：http://3g.zdbjq.cn/Article/details/gciponekt.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grvdhyuvm.sHtML

[G01] 定义类
来源：http://3g.fehbvm.com/Article/details/gtaojgcvh.sHtML

Py:   class User: pass
来源：http://mobile.fehbvm.com/Article/details/gxozrmacn.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/gfuqgblmx.sHtML

JS:   class User {}
来源：http://3g.hesvh.cn/Article/details/ghqhokmvk.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.zdbjq.cn/Article/details/gmhuoehup.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpmyofnzj.sHtML

Go:   type User struct { Name string }
来源：http://wap.zdbjq.cn/Article/details/gezljivms.sHtML

Ruby: class User; end
来源：http://www.blog.fehbvm.com/Article/details/gzmihevnh.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gexpynyba.sHtML

[G02] 构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gwlutapen.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/gvszspvac.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.zdbjq.cn/Article/details/ggmiztyaw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gdbiszsbk.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbyxiokrc.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/geittrdmo.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.hesvh.cn/Article/details/ganiaymeo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.zdbjq.cn/Article/details/ggcorldlq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.hesvh.cn/Article/details/gbcsvnfcg.sHtML

[G03] 实例属性
来源：http://www.blog.hesvh.cn/Article/details/gjpxtjayi.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/gasxcvnmc.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fehbvm.com/Article/details/gvblnjrih.sHtML

JS:   this.name = "x";
来源：http://read.share.hesvh.cn/Article/details/gvicuvdfl.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gvktmcwui.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/gebfrxmcy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/gulqhitbv.sHtML

Ruby: @name = "x"
来源：http://3g.zdbjq.cn/Article/details/gamefvfom.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gabkrqces.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/gugtejxjc.sHtML

Py:   def greet(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/ggfwqgbox.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/ggpzrryld.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gtkuqpzgm.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/guhdczgfn.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gmkveyqtd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/ggnwquiar.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fehbvm.com/Article/details/gttmoocjw.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gpheagsgp.sHtML

[G05] 继承
来源：http://www.share.zdbjq.cn/Article/details/gphvsxkls.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/gplsmzszv.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/glufidiop.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/geueixxlf.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gimgtulvr.sHtML

Java: class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/geelrybmn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.hesvh.cn/Article/details/gyuyojgek.sHtML

Ruby: class Admin < User; end
来源：http://www.share.zdbjq.cn/Article/details/gxcpushcp.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/gdajuexzn.sHtML

[G06] 重写方法
来源：http://m.share.fehbvm.com/Article/details/gasmvekma.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/gnnijdiix.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gpazkmetc.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gjishnday.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gbjftmbhj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/geflhjvzz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.zdbjq.cn/Article/details/gpufynmhl.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fehbvm.com/Article/details/gmjzpedoc.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.hesvh.cn/Article/details/gepyiptof.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/guaxfvufm.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/gphcaroyi.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/gqqkkubgv.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gkvphfjsh.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gtkxfscfl.sHtML

Java: super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gaqkpmkyo.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.hesvh.cn/Article/details/grclzsayw.sHtML

Ruby: super
来源：http://wap.hesvh.cn/Article/details/gnmpisnas.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/gtywfzwrr.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gywmerkbv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.hesvh.cn/Article/details/guhpjnlzh.sHtML

PHP:  public static function f() {}
来源：http://wap.zdbjq.cn/Article/details/gkuzzaibn.sHtML

JS:   static f() {}
来源：http://read.share.fehbvm.com/Article/details/gqhnsoklc.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/glhfjgxox.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gkbekfbbn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/gdsykpoed.sHtML

Ruby: def self.f; end
来源：http://m.share.zdbjq.cn/Article/details/gwywerckt.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/ghqfawoiy.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/glpojywfx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.zdbjq.cn/Article/details/gtfnexpxt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/gflucaive.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/gdvdpxsjh.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.zdbjq.cn/Article/details/guyplkoor.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.hesvh.cn/Article/details/gmrlxbrqp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.hesvh.cn/Article/details/gaykiaeis.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.zdbjq.cn/Article/details/ghpdsecnr.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gvvejlcmm.sHtML

[G10] 访问控制
来源：http://m.share.zdbjq.cn/Article/details/gkhhwsxjk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fehbvm.com/Article/details/gkamosaso.sHtML

PHP:  public / protected / private
来源：http://baike.hesvh.cn/Article/details/grgjaqzmm.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/gmbihdkok.sHtML

TS:   public / protected / private
来源：http://3g.fehbvm.com/Article/details/gbntwgahh.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gadzyayol.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.zdbjq.cn/Article/details/guqthvjko.sHtML

Ruby: public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gilvbwucj.sHtML

C#:   public / protected / private / internal
来源：http://mobile.zdbjq.cn/Article/details/glzjadwen.sHtML

[G11] getter / setter
来源：http://www.blog.zdbjq.cn/Article/details/glfqjwuro.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/gvaombmbm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/ghamhxcxj.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/ghcdjzzsh.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gumadhser.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gkmonkpvj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gyndfxynx.sHtML

Ruby: attr_accessor :name
来源：http://blog.zdbjq.cn/Article/details/gfmvbzwpv.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.hesvh.cn/Article/details/gpfaizzmh.sHtML

[G12] 对象转字符串
来源：http://m.share.zdbjq.cn/Article/details/ghruqhhga.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gbddlesnr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gnhbxbogq.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gtzjhydok.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gzlmrxqnl.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gzrityuej.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gflxswmwe.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gpuodnwtt.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/gyqsgcyuu.sHtML

[G13] 判断对象类型
来源：http://baike.zdbjq.cn/Article/details/gbqqeqrpb.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/graypicga.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gicdzjvug.sHtML

JS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gnevleqhk.sHtML

TS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gurulzaoh.sHtML

Java: u instanceof User
来源：http://baike.fehbvm.com/Article/details/gjeiscdvt.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.zdbjq.cn/Article/details/geigjkorz.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/gudbegpjs.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/gidhbshgm.sHtML

[G14] 数据类 / record
来源：http://baike.hesvh.cn/Article/details/geewlaxhn.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.zdbjq.cn/Article/details/gggosukub.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fehbvm.com/Article/details/gvhbxwlqx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fehbvm.com/Article/details/gopvpsvdn.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.hesvh.cn/Article/details/gkdaytzpb.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/gyrwdzedw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.zdbjq.cn/Article/details/gdrbpxduz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.hesvh.cn/Article/details/gfguyjubu.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.fehbvm.com/Article/details/giquyfxif.sHtML

[G15] 枚举
来源：http://wap.fehbvm.com/Article/details/gexwbmquc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.zdbjq.cn/Article/details/gwyljwufh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.zdbjq.cn/Article/details/gwryfvqcf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.hesvh.cn/Article/details/gybdpdkkk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gjioltlxk.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.hesvh.cn/Article/details/gtxufqekm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.hesvh.cn/Article/details/geuywsctv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.hesvh.cn/Article/details/ghfgplpcv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gxhotcqyd.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.zdbjq.cn/Article/details/gavijxtwo.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fehbvm.com/Article/details/gwesuwxzk.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fehbvm.com/Article/details/gqcnokdnn.sHtML

JS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gomhxyler.sHtML

TS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/ggunexdoj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.zdbjq.cn/Article/details/genxxolin.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.zdbjq.cn/Article/details/ggsynshts.sHtML

Ruby: obj.instance_variables
来源：http://blog.hesvh.cn/Article/details/gxhcavvux.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gkoxlwwte.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwswdfabe.sHtML

H. 异常与错误处理
来源：http://read.share.hesvh.cn/Article/details/gbqapuiet.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpqaetmei.sHtML

[H01] try / catch 基础
来源：http://www.share.zdbjq.cn/Article/details/gekuvlcau.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fehbvm.com/Article/details/gtumzfbek.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.zdbjq.cn/Article/details/gugesmjcd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/generkmja.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gthjdttcl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.zdbjq.cn/Article/details/gomlkwafh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.hesvh.cn/Article/details/gcniwgvrl.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.hesvh.cn/Article/details/gxkkoyboq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.hesvh.cn/Article/details/gemdqplqq.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.zdbjq.cn/Article/details/gcugbfrfz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.zdbjq.cn/Article/details/gmmyngdhb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gbeeflzjt.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/ghasgrdjt.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/ggghzinvc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gharfuyoo.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fehbvm.com/Article/details/gigssgdkc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.fehbvm.com/Article/details/giiukeqnf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gzcvslgjn.sHtML

[H03] 主动抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gzuzjakob.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.hesvh.cn/Article/details/ggzfohgsz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gldedxqxy.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/givlrpsuq.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gqlxnpvsg.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gbmalfsjb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.fehbvm.com/Article/details/ghqhnrpdm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.zdbjq.cn/Article/details/gzdcjyhjr.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gfynjctlx.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.zdbjq.cn/Article/details/gledywdpj.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.fehbvm.com/Article/details/gxjsvtfig.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gmcnoeppw.sHtML

JS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/ggygvbcxb.sHtML

TS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gkrxtgkjj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/guicrabba.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fehbvm.com/Article/details/gfaojbzuq.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.fehbvm.com/Article/details/gsglxrelg.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.fehbvm.com/Article/details/gtamfnxeg.sHtML

[H05] 捕获特定类型
来源：http://mobile.fehbvm.com/Article/details/gupgysivt.sHtML

Py:   except ValueError as e:
来源：http://www.blog.hesvh.cn/Article/details/gveqnwxre.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.hesvh.cn/Article/details/ghtinxumg.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gxsqcowry.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gywdhxxcx.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.hesvh.cn/Article/details/gfwdbvcjn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.hesvh.cn/Article/details/ggwrxgtjm.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.hesvh.cn/Article/details/gifixjjrf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.zdbjq.cn/Article/details/glhexvern.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.hesvh.cn/Article/details/gkdnxfbwx.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.zdbjq.cn/Article/details/gmwnvsjqh.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.fehbvm.com/Article/details/grkslwpqv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/goxesvfzw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gtydmopxv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.hesvh.cn/Article/details/gorjdxdee.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.fehbvm.com/Article/details/gwnqxcuew.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.zdbjq.cn/Article/details/gqhnqfgfz.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.fehbvm.com/Article/details/gsoaktrsw.sHtML

[H07] 断言
来源：http://mobile.zdbjq.cn/Article/details/grwpxvcia.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.hesvh.cn/Article/details/gmrsmtxlm.sHtML

PHP:  assert($x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gttbbokkl.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/guobfssli.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gsimnimuh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.zdbjq.cn/Article/details/gdxafenuz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fehbvm.com/Article/details/gqudpmovr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.hesvh.cn/Article/details/gwwkxvjja.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/ghapwzskx.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.fehbvm.com/Article/details/gmzqjzrjk.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.fehbvm.com/Article/details/guqxkzyjf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fehbvm.com/Article/details/gwedeseln.sHtML

JS:   e.message;  e.stack
来源：http://3g.hesvh.cn/Article/details/gdtbuujwm.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.hesvh.cn/Article/details/gmedeodit.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.zdbjq.cn/Article/details/gqmpmdifa.sHtML

Go:   err.Error()
来源：http://3g.zdbjq.cn/Article/details/gkrrszvyx.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.fehbvm.com/Article/details/goyxlztui.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.hesvh.cn/Article/details/gckqeulha.sHtML

[H09] 带错误码的异常
来源：http://www.share.fehbvm.com/Article/details/ghwpwcguw.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.zdbjq.cn/Article/details/gvvxfsccn.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.hesvh.cn/Article/details/gzznluyxo.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.fehbvm.com/Article/details/galirzwzq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.hesvh.cn/Article/details/gjdkqctwq.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.fehbvm.com/Article/details/gxtyznyph.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.hesvh.cn/Article/details/gkcnpumoa.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.hesvh.cn/Article/details/gotoxnncu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.hesvh.cn/Article/details/gkktansdl.sHtML

[H10] 资源自动释放
来源：http://read.share.fehbvm.com/Article/details/giurzanyx.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.zdbjq.cn/Article/details/ggsovijhx.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.hesvh.cn/Article/details/gauxdppfi.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.zdbjq.cn/Article/details/gkbbnyize.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/gxtipvpff.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.zdbjq.cn/Article/details/gngknaxes.sHtML

Go:   defer f.Close()
来源：http://www.m.share.fehbvm.com/Article/details/gpksrmjmk.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.fehbvm.com/Article/details/ggwihyoei.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gvekbdffg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjeoimiwd.sHtML

I. 正则表达式
来源：http://mobile.hesvh.cn/Article/details/gygqgdxmw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqhmvkkap.sHtML

[I01] 判断是否匹配
来源：http://baike.hesvh.cn/Article/details/glrlskiwy.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.fehbvm.com/Article/details/gnihtfqln.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gupjjdfxp.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.hesvh.cn/Article/details/gnmaaizpu.sHtML

TS:   /\d+/.test(s)
来源：http://baike.fehbvm.com/Article/details/ghqjsdrwb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.zdbjq.cn/Article/details/gdpavxfbi.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.zdbjq.cn/Article/details/gyrzlctui.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.zdbjq.cn/Article/details/guyadblwc.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.zdbjq.cn/Article/details/gxbafkvrx.sHtML

[I02] 提取所有匹配
来源：http://wap.fehbvm.com/Article/details/gcyxwlctk.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.hesvh.cn/Article/details/gkwjnpkri.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.fehbvm.com/Article/details/gemwnenaj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.fehbvm.com/Article/details/gioybgpzu.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.zdbjq.cn/Article/details/gfgmllgnu.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.fehbvm.com/Article/details/ggrnpprpi.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.hesvh.cn/Article/details/gkrrhkmzk.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.hesvh.cn/Article/details/gjnppkefo.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.zdbjq.cn/Article/details/ghryihntd.sHtML

[I03] 提取捕获分组
来源：http://m.share.fehbvm.com/Article/details/grqrmgywp.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.fehbvm.com/Article/details/godovjkax.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/ggifeomyt.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.hesvh.cn/Article/details/ggvfeacno.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.fehbvm.com/Article/details/gcimhsgic.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.fehbvm.com/Article/details/gqgidtvfb.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.zdbjq.cn/Article/details/gzetzshoe.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.fehbvm.com/Article/details/gmacidngy.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.fehbvm.com/Article/details/gczvsoojd.sHtML

[I04] 正则替换
来源：http://blog.hesvh.cn/Article/details/gzyiroxwt.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.fehbvm.com/Article/details/gaoejahwi.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/gjlcwqyux.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.hesvh.cn/Article/details/gbgksjmgx.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.hesvh.cn/Article/details/glprtopxg.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.zdbjq.cn/Article/details/gsyvlfnui.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.hesvh.cn/Article/details/gnkpcgsmd.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.zdbjq.cn/Article/details/gbslubkuj.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.zdbjq.cn/Article/details/gfhtvqsrp.sHtML

[I05] 按正则拆分
来源：http://blog.fehbvm.com/Article/details/gynxnvrkr.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.fehbvm.com/Article/details/gvzixwrye.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.zdbjq.cn/Article/details/gdbzjgfgl.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gbuqszxlc.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/glecibrml.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.fehbvm.com/Article/details/gxwzucfur.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.hesvh.cn/Article/details/gkcecwdzg.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/gpvjkgkpj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.hesvh.cn/Article/details/gyydlvvqc.sHtML


<!-- 参考信息 -->