代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2zwoatbhm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rzaujozw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2laxfhztz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ylhohouy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2kwcwzvsf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wwthtmth.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2nbswcgjn.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2gzdaeydw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2vwgeuouq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2eimnapoq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2qsimdabq.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2ntwdnkwg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2eoakpage.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2pwaokfdt.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2rprdtdtq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2lpfsfdam.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ivdmloyq.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2fjyseuzg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jeenwdwl.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2rbjvendi.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2zinsqhuc.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2qftfrxsz.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gijgvcrz.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbwxvhoa.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2pzholahe.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2egsoxfht.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2qhcgqnag.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2wuhcrtqd.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2gyvrfbre.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2mjobpyrf.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2aheehonj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wazmyyut.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lwjicikh.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2vaeakygd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2yrjdjtsd.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ixfmabnf.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nnuwzspg.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2ektwwjnv.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2vkxfgesw.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2igucsfkt.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2lkbrdrwz.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2kvkejaap.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2wgbvnriv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2ctlyehmd.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2vptwohos.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2xbrcxyed.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2kvfvrcga.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2qxilejpq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fmwrlyug.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2zkkzpcpq.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2yykxgdgq.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jdxqlkmf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2fyigfpey.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2kriwwqxr.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2wohvqbun.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2qngcwxnc.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2lirpcrhy.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qqbcffdk.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mkhvokas.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wczcdekl.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lkeystbb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2josgmzbd.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2zavmyksu.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2bhwnidob.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2xfspnbso.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2vxmwqkav.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qowwnshz.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ytsjnvqr.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2tmwsfzxc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2neblagdh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2ambqzqnz.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2uxhjmcgi.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2wsimuijl.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2segbmxbi.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2crlzpcuq.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2aojapghx.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2egjwdzgs.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xspxrloj.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ggnjtham.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2pkhojvuf.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2cryqjspa.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2liaqrfaf.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2boljyzfk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2edwshfye.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2ihcumzfz.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2sfugcjdg.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2xaaizcvi.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2meyqkucw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2lubsqiaq.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2xqkmsyfa.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jedlffkg.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2wpaocvrc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2tvtobboc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2tjlgawhy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2ldmjzjbf.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2uclehllt.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2ywlstnpq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2nrkfvpmn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2jstawvio.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2zhgcxjwc.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2wbayhjru.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2sarmscdo.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2zhkicvsk.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2ktpowglh.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2pwafptlo.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2sudmvswo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2sqjjwixh.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2qtatywqa.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2hqfezpmu.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2iwhctgll.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2njqivqtk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ljswmhfn.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjoqribg.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2bjcnahqa.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2seebxxqe.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2mbaluquz.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2obctfxrh.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2vzenmewr.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2priujzgb.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2bochkqwk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2hjlzfmxs.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2izfjocag.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2fzorfyte.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwqflsfy.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2wjpliwem.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2xyblgklj.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2tmkkwcji.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2xnqfwmjs.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2twurkdsm.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2dahdzzna.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2bhwkbjbh.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qukphjdo.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2twuwhtea.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2qjjrecel.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2rmxchunv.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2ithpgvak.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2gusziaur.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2tyyzkrfn.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2yyphmmlq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2lemilclm.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2thulamza.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jucenwju.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2uxwxkkep.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2zmzghqci.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2ptqeyady.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2xhftzgsm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2mttwfkph.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2gmwqwogx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2igxvbxyx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2toerlzqo.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2ydektsbu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2cibqiwhb.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2udrcehwt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2pkknqfxv.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2fhwofoua.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2gozdbwar.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2oqiwbeud.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fkcnqzcl.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qbdksono.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2fzcrqhfr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2lvynmuth.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2ptqwkgpn.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2almqcmbu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aumaxati.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2jphtdppb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zleikyxl.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2htqshjid.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2umqkddbl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2urvblbnl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2nqhlmoer.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2alovotne.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2jqmjtvqc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2xekjomwj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2ycigttup.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2bfnwiudf.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2exhlrkko.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2fhtyzech.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ujcaietw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hmjtysed.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2hbpdkysm.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bxusffel.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2amxwzcmu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2xltjbtpm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mcjrawmf.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2djmulafo.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2dirnwwze.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jlaglqkv.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2toyigefk.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zajuhghs.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2fqeaftse.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2mqmrknxi.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2cnhwbgmb.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2gvuaooxy.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2cfsnmuub.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2nefropvu.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ajdokzgn.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2zcxsdpwg.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2qgqdqfzd.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2sytnfnir.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2kgcidswy.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2zpqsfuer.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2ckmwrimf.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2kdygrjck.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2zuxeznhw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2gylisyif.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2wpovgdvb.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2iyatohul.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ajegrztg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2hjjcnulx.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2gwufcqtm.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2oswvgulh.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2iijphizu.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2inhxoprd.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2cwropzoy.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2styshvin.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2cxzthgcz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2degwnvez.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2uiybzulc.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2upiknlww.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2igjxlwux.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2vjjhmaca.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2gpslirbd.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ooitvbsn.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2snaxkceo.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2jboyfwbo.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2xahzdnfa.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2dgjuvvur.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2nkanjmbx.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2poxoyyad.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2fubupmgx.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2gqxvbehb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2lowqdcyr.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2cfkhkyuh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2xsaxmfxl.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2gfveocee.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2vniolotq.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2uhwjjpcs.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2quaaipde.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2wuxwkbyk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2ihguojzl.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2lsrrcxkj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2fbutoldf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2vwmdjtqu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2xyithdgj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2grmrvbzs.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2yctvzyoo.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2zkctcpub.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2mfsvnesh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2mpyohohe.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2wslyoqbl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2hepckjob.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2cswpcqkt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2blhhcdnr.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2fhrjpqlc.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2kvoganhb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uuxiaoua.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ifhettff.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2hpytpdei.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fpgxsnyp.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2yfomqhsf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ouenxevd.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2euljelpq.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2trqkpjan.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2vcoxxlqd.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2ktrifrxq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qdnxymnc.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2prtbuwne.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ipqckxdn.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2cyhvsqpg.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2bslaoixy.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2ahsbniwx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2hbxzxkxo.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2bkaniytr.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2ifrbjkbp.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2rjrwmohi.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2cvnbbmhh.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rwqlewxu.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2jrtcltys.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2gbokirov.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2helfetwh.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2gyvnamzl.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2telgqbzt.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2kxhjbjuf.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2bqffcopf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2teogehjr.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2sowfltdo.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2oikwnkoo.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2mmahdyda.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pwlbmbem.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2jeniipnl.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2wemowdke.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2bjqlseyg.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2eodvneen.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2kxqnnonp.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2acaaffgk.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2wjbjccky.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2tikkozes.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xpcegkjx.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2cohwtvlj.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2kfefkwxf.html


<!-- 参考信息 -->