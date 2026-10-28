代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.xinyue.icu/gtihwhijbd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.hongshengwenyu.top/gtrcoictuy.html

[F11] 复制与移动文件
来源：http://hz.sysykeji.top/gtxpcajkuo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zhoulong.xyz/gtekkqeowl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zhixingplan.top/gtpbuojitw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.quarkkingdee.top/gtlstyyqlj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sysykeji.top/gtcnoxdmtr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.fengsongda.top/gtjumziqrd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.tian-w.cn/gthprzbzbu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.haohaochexian.top/gtxkdsdzxn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.dashuyun.cn/gtmwxadnzz.html

[F12] CSV 读写
来源：http://hz.jinqigufen.top/gtudfkferr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zycfv.cn/gtnacanrbo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yongpay.top/gtcevkbwsk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yueranfly.top/gteebmsyem.html

TS:   // 同上
来源：http://hz.ydzc1.top/gtrydrxsqj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yueranfly.top/gttyiocxsy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zycfv.cn/gthgppsmdy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.cqqwz.cn/gtoiuiujls.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jinqigfzy.top/gtxzzqbtyq.html

================================================================================
来源：http://hz.zhijiandao.cn/gtgndlrvqk.html

G. 面向对象
来源：http://hz.mhx1999.top/gtklxozljt.html

================================================================================
来源：http://hz.snrcjt.cn/gterzwbypz.html

[G01] 定义类
来源：http://hz.gaohongyu789.top/gtzxidgsgo.html

Py:   class User: pass
来源：http://hz.xuanzx.com/gtoehvjmmi.html

PHP:  class User {}
来源：http://hz.zdqjudy.top/gtfdaebbur.html

JS:   class User {}
来源：http://hz.tian-w.cn/gtdamumepl.html

TS:   class User { name: string = ""; }
来源：http://hz.jinghuilouyu.cn/gtcvjtvgdu.html

Java: class User {}
来源：http://hz.hongshengwenyu.top/gtrsulvanj.html

Go:   type User struct { Name string }
来源：http://hz.jianghu66.top/gtohyonfiv.html

Ruby: class User; end
来源：http://hz.jinqigfzy.top/gtvsjxtfqj.html

C#:   class User {}
来源：http://hz.andypj.xyz/gtropxkxyc.html

[G02] 构造函数
来源：http://hz.andypj.xyz/gtywoaovpz.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.xingfuxueyuan.xyz/gtgoddvxbx.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.mhx1999.top/gtzofmervt.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.0kj1m.cn/gthxgxqhrl.html

TS:   constructor(public name: string) {}
来源：http://hz.zhengqikj.top/gtsjqwywqi.html

Java: User(String name) { this.name = name; }
来源：http://hz.jinyuanbaomall.cn/gthrukwmwi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.gogol.net.cn/gtbkibckmi.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.chenzaomai.com/gtftacqnhd.html

C#:   public User(string name) { Name = name; }
来源：http://hz.hywenlv.cn/gtzofqitiw.html

[G03] 实例属性
来源：http://hz.vqdsnc.cn/gtivzdfrcv.html

Py:   self.name = "x"
来源：http://hz.hnxiangtu.top/gtxhskotmm.html

PHP:  public string $name = "x";
来源：http://hz.aibaodan.cn/gtmdwtjrdn.html

JS:   this.name = "x";
来源：http://hz.ybcxt.top/gtzbirfyeh.html

TS:   name: string = "x";
来源：http://hz.hfpthk.cn/gtqhyftphm.html

Java: private String name;
来源：http://hz.zhongyouzk.top/gtvadfcqvb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hywenlv.cn/gtfoqivohj.html

Ruby: @name = "x"
来源：http://hz.sweek.top/gtmlirluqv.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.snrcjt.cn/gtyfzzvsdt.html

[G04] 定义方法
来源：http://hz.gotoacloud.top/gtehcpywzj.html

Py:   def greet(self): return self.name
来源：http://hz.chenlongwang.top/gtgcunnnqa.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.0kj1m.cn/gtyyrxadak.html

JS:   greet() { return this.name; }
来源：http://hz.gaohongyu789.top/gtlegefwni.html

TS:   greet(): string { return this.name; }
来源：http://hz.yvedp.cn/gtkzoqvoej.html

Java: String greet() { return name; }
来源：http://hz.zdqjudy.top/gtsfppkgvy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.xinyue.icu/gtolaxcpoe.html

Ruby: def greet; @name; end
来源：http://hz.ivvv.top/gtlpgnzkhp.html

C#:   public string Greet() => Name;
来源：http://hz.wangdashe.top/gtjycfovba.html

[G05] 继承
来源：http://hz.chenlongwang.top/gtcqnznain.html

Py:   class Admin(User): pass
来源：http://hz.jinyuanbaomall.cn/gtzqpzbuyu.html

PHP:  class Admin extends User {}
来源：http://hz.chenzaomai.com/gtxndijynk.html

JS:   class Admin extends User {}
来源：http://hz.hammf.cn/gtmtoajcpy.html

TS:   class Admin extends User {}
来源：http://hz.iojbl.cn/gtumzjoupc.html

Java: class Admin extends User {}
来源：http://hz.yj20258888.top/gtrotmclpj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.wangshuangyany.cn/gtfjkueija.html

Ruby: class Admin < User; end
来源：http://hz.shuidangran.top/gtnilxweyc.html

C#:   class Admin : User {}
来源：http://hz.redwolf501.top/gtbrdvgijn.html

[G06] 重写方法
来源：http://hz.chenzaomai.com/gthpmhovbn.html

Py:   def greet(self): return "admin"
来源：http://hz.ydjk.org.cn/gtwdecjiub.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.hfpthk.cn/gtymriwvhv.html

JS:   greet() { return "admin"; }
来源：http://hz.vqdsnc.cn/gtakyorgsh.html

TS:   greet(): string { return "admin"; }
来源：http://hz.ydjk.org.cn/gtdzdwiwps.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.gzhubu.top/gtqpkpzwph.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.wangdashe.top/gtlvmjzfqw.html

Ruby: def greet; "admin"; end
来源：http://hz.yuanzhike.top/gtfikpydaz.html

C#:   public override string Greet() => "admin";
来源：http://hz.yueranfly.top/gtiadqshal.html

[G07] 调用父类方法
来源：http://hz.sxryk.cn/gtzywapxxx.html

Py:   super().greet()
来源：http://hz.yvedp.cn/gtoerhpycy.html

PHP:  parent::greet();
来源：http://hz.hongshengwenyu.top/gtfeotrhpr.html

JS:   super.greet();
来源：http://hz.gaohongyu789.top/gtohsgnhcl.html

TS:   super.greet();
来源：http://hz.ywan-chungtsiang.top/gtovpjegiz.html

Java: super.greet();
来源：http://hz.hnqzz.top/gtafdrgauz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.pengpengdd.cyou/gtcrfmjljj.html

Ruby: super
来源：http://hz.pengpengdd.cyou/gtqfwqdrcz.html

C#:   base.Greet();
来源：http://hz.kuanghao11.cn/gtqpujbvny.html

[G08] 静态方法与属性
来源：http://hz.52xcode.cn/gtrmdersya.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.nwbrower.top/gtapaptcri.html

PHP:  public static function f() {}
来源：http://hz.sysykeji.top/gthwdqzobe.html

JS:   static f() {}
来源：http://hz.sweek.top/gtuydrdqpy.html

TS:   static f(): void {}
来源：http://hz.vqdsnc.cn/gtfpaveqpe.html

Java: static void f() {}
来源：http://hz.yvedp.cn/gtkifuxdam.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zdqjudy.top/gtyisdzhoo.html

Ruby: def self.f; end
来源：http://hz.bjfxy.top/gtvwyngkms.html

C#:   public static void F() {}
来源：http://hz.zhiwuduotai.top/gtvxbfbeqo.html

[G09] 接口 / 抽象类
来源：http://hz.9152youxi.cn/gtlejrhzag.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zhoulong.xyz/gtfpvxggab.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.havefunace.top/gttqqgbwti.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.kuanghao11.cn/gtfnddkltp.html

TS:   interface Shape { area(): number; }
来源：http://hz.dianchejie.cn/gthbgnhisn.html

Java: interface Shape { double area(); }
来源：http://hz.meibo888.top/gtrbvrbciy.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zycfv.cn/gtkuunxted.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jyoumei.cn/gtzvefdjeb.html

C#:   interface IShape { double Area(); }
来源：http://hz.daria6918.cn/gthirqsdyy.html

[G10] 访问控制
来源：http://hz.0kj1m.cn/gtzwacpjks.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hnxiangtu.top/gtacruwxig.html

PHP:  public / protected / private
来源：http://hz.zhengqikj.top/gtahqnbptf.html

JS:   #private 字段；其余公开
来源：http://hz.redwolf501.top/gtezhuyjdc.html

TS:   public / protected / private
来源：http://hz.nwbrower.top/gtusgycrxe.html

Java: public / protected / private / 默认包级
来源：http://hz.yj202588.top/gterfkymoy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.aizwys.cn/gtklmlxwhg.html

Ruby: public / protected / private
来源：http://hz.iojbl.cn/gtfhkxdmsf.html

C#:   public / protected / private / internal
来源：http://hz.zhaomingkeji.xyz/gtgvokwvxb.html

[G11] getter / setter
来源：http://hz.daria6918.cn/gtfksgghry.html

Py:   @property 与 @x.setter
来源：http://hz.bjfxy.top/gtjfszzdht.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.cdnleiting.top/gtwnakadol.html

JS:   get name() { return this._name; }
来源：http://hz.fengsongda.top/gtppehyzcc.html

TS:   get name(): string { return this._name; }
来源：http://hz.hnqzz.top/gtrremujcz.html

Java: public String getName() { return name; }
来源：http://hz.zhongyouzk.top/gthmjuebfj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.daxiang520.top/gtbnqqbcju.html

Ruby: attr_accessor :name
来源：http://hz.xylfe.cn/gtjtqfqwte.html

C#:   public string Name { get; set; }
来源：http://hz.yangfankeji.com/gtnfjvyljf.html

[G12] 对象转字符串
来源：http://hz.zhengqikj.top/gtxvdkhaul.html

Py:   def __str__(self): return self.name
来源：http://hz.jyoumei.cn/gtpgcfkteh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.sufxvd.cn/gtxghfxdav.html

JS:   toString() { return this.name; }
来源：http://hz.yuanzhike.top/gtngxflqwv.html

TS:   toString(): string { return this.name; }
来源：http://hz.sufxvd.cn/gteiucxrex.html

Java: @Override public String toString() { return name; }
来源：http://hz.yuanzhike.top/gtqayvlvgx.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.meibo888.top/gthxvcfolk.html

Ruby: def to_s; @name; end
来源：http://hz.nanxinkj.top/gtnhhmdhlz.html

C#:   public override string ToString() => Name;
来源：http://hz.hongshengwenyu.top/gtbszktfuo.html

[G13] 判断对象类型
来源：http://hz.yangfankeji.com/gtqgvwdbcq.html

Py:   isinstance(u, User)
来源：http://hz.9152youxi.cn/gtzacadvrk.html

PHP:  $u instanceof User
来源：http://hz.aizwys.cn/gtqkjminux.html

JS:   u instanceof User
来源：http://hz.hysaishi.cn/gtackxeien.html

TS:   u instanceof User
来源：http://hz.meibo888.top/gtgpjhhuyl.html

Java: u instanceof User
来源：http://hz.smart0.xyz/gtdhkczveq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.tianlin.xyz/gtxrwhqsfz.html

Ruby: u.is_a?(User)
来源：http://hz.kuanghao11.cn/gtsvzmxdhe.html

C#:   u is User
来源：http://hz.aibaodan.cn/gtyzllgepr.html

[G14] 数据类 / record
来源：http://hz.0kj1m.cn/gtxpgbqvgl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.chenzaomai.com/gtlrmvtmep.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jianghu66.top/gtctpgevyu.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.fengsongda.top/gtfttmwkyp.html

TS:   type User = { name: string; age: number };
来源：http://hz.yj20258.top/gtubfsmdju.html

Java: record User(String name, int age) {}
来源：http://hz.cdnleiting.top/gtiqaacnni.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jqgfzy.top/gtnczzmipy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.sufxvd.cn/gtqpubzpvy.html

C#:   record User(string Name, int Age);
来源：http://hz.jyoumei.cn/gtpbfmvzaj.html

[G15] 枚举
来源：http://hz.havefunace.top/gtrvqnwoup.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.iojbl.cn/gtjihxqvhq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.sweek.top/gtoblsocba.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jinyuanbaomall.cn/gtxtmiampm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhixingplan.top/gtagullcsp.html

Java: enum Color { RED, GREEN }
来源：http://hz.yj20258888.top/gtyemynzyb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.hfpthk.cn/gtgpdqigqb.html

Ruby: Color = %i[red green].freeze
来源：http://hz.andypj.xyz/gtfboqkkkq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.haohaochexian.top/gtyphkwtlz.html

[G16] 对象转数组 / 字典
来源：http://hz.jinqigufen.top/gtgihyvssm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.shanyushiyangtech.top/gtfnfaugcv.html

PHP:  get_object_vars($obj);
来源：http://hz.andypj.xyz/gtltzjcrpt.html

JS:   Object.entries(obj)
来源：http://hz.zhoulong.xyz/gtmfomvfzy.html

TS:   Object.entries(obj)
来源：http://hz.tian-w.cn/gtmsabuint.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.guannengcc.top/gtkovexblp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hammf.cn/gtymgienvd.html

Ruby: obj.instance_variables
来源：http://hz.smart0.xyz/gtrgmppljn.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jinqigfzy.top/gtlolfjoxg.html

================================================================================
来源：http://hz.fengsongda.top/gtbptgwluc.html

H. 异常与错误处理
来源：http://hz.ywan-chungtsiang.top/gtkfpopgty.html

================================================================================
来源：http://hz.dashuyun.cn/gtnheecsrv.html

[H01] try / catch 基础
来源：http://hz.cqqwz.cn/gtfagiekpf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.cashguo.top/gtwzxwhlkt.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.pycfn.com/gtixpvwehy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zhaomingkeji.xyz/gttwstwwja.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.feifeiyinyue.top/gtkihjzyix.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ehwqpu.com/gtpbojyfsj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.andypj.xyz/gtpbzvdlom.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.cucudq.cn/gtistufqzg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.iojbl.cn/gtojmdzihe.html

[H02] finally / ensure 收尾
来源：http://hz.gogol.net.cn/gtwjfxjvwu.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yuanzhike.top/gtqlugkonb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jyoumei.cn/gtkuxtqjib.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yongpay.top/gtciblubmr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ywan-chungtsiang.top/gtulkrjxbq.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.feifeiyinyue.top/gttglbqeck.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.0kj1m.cn/gthfbynpck.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.birdmap.top/gtnevrmgzm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hywenlv.cn/gtqnmjdhyn.html

[H03] 主动抛出异常
来源：http://hz.hfpthk.cn/gtlrcmbner.html

Py:   raise ValueError("错误信息")
来源：http://hz.chenlongwang.top/gtcinikgcm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.gzhubu.top/gtedqgrihb.html

JS:   throw new Error("错误信息");
来源：http://hz.zhengqikj.top/gtgzhohvpm.html

TS:   throw new Error("错误信息");
来源：http://hz.smart0.xyz/gtaloqbjmi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.c1oappe.top/gtvbsdzlnh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.kuanghao11.cn/gtmtkgvmvw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jinqigufen.top/gtkovdwwvb.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.cqqwz.cn/gtaisdxktw.html

[H04] 自定义异常类型
来源：http://hz.xuanzx.com/gtzmldysoa.html

Py:   class MyError(Exception): pass
来源：http://hz.tian-w.cn/gttpnouonj.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.vqdsnc.cn/gtdjxgzsvh.html

JS:   class MyError extends Error {}
来源：http://hz.jqgfzy.top/gtgqwmvxaz.html

TS:   class MyError extends Error {}
来源：http://hz.fengsongda.top/gtfxrwvntd.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jinyuanbaomall.cn/gtlbhtnzaw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jlsjyb.cn/gtbbwfrnrm.html

Ruby: class MyError < StandardError; end
来源：http://hz.shzxlz.cn/gthvwtwnhq.html

C#:   class MyException : Exception {}
来源：http://hz.snrcjt.cn/gtsuwypemx.html

[H05] 捕获特定类型
来源：http://hz.yanxiufei.cn/gtrqnbilju.html

Py:   except ValueError as e:
来源：http://hz.xuanzx.com/gthewjepla.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.redwolf501.top/gthmgdhmwt.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yueranfly.top/gtqhkguzyr.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.sysykeji.top/gtizwebkwk.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.gogol.net.cn/gtejpbxvgq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.shuidangran.top/gtkpgkwscw.html

Ruby: rescue ArgumentError => e
来源：http://hz.9152youxi.cn/gtglygqvlv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.dashuyun.cn/gtyvvymygb.html

[H06] 可选值 / 空值安全访问
来源：http://hz.sxryk.cn/gtjbbtsdli.html

Py:   value = d.get("k") or default
来源：http://hz.chenzaomai.com/gttamxcmhc.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.316326.xyz/gtqkryccoz.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jlsjyb.cn/gtgmxtzpqw.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.daxiang520.top/gtzbfmmali.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.meibo888.top/gtljzrfwrx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jianghu66.top/gthmnodvjt.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yueranfly.top/gtyalfxjje.html

C#:   obj?.A?.B ?? default
来源：http://hz.gotoacloud.top/gtsxqtzdun.html

[H07] 断言
来源：http://hz.zhongyouzk.top/gtxzjajrbr.html

Py:   assert x > 0, "必须为正"
来源：http://hz.gaohongyu789.top/gtvyitdork.html

PHP:  assert($x > 0);
来源：http://hz.hnxiangtu.top/gtafjbzmjj.html

JS:   console.assert(x > 0);
来源：http://hz.zhongyouzk.top/gtelcuzhkg.html

TS:   console.assert(x > 0);
来源：http://hz.shanyushiyangtech.top/gtzibiqjal.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zhoulong.xyz/gtxxqueeyr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.aibaodan.cn/gtevhaphbe.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhijiandao.cn/gtnpyaisav.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jlsjyb.cn/gtetnbrxpz.html

[H08] 获取错误信息与堆栈
来源：http://hz.316326.xyz/gtpydqvjto.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.xinyue.icu/gtycyghtvw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.guowangkeji.top/gtpjszkvje.html

JS:   e.message;  e.stack
来源：http://hz.cqqwz.cn/gtetajouqn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.pycfn.com/gtimennzhg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.kuanghao11.cn/gtsbfslacn.html

Go:   err.Error()
来源：http://hz.kuanghao11.cn/gtikyikqxf.html

Ruby: e.message;  e.backtrace
来源：http://hz.zhongyouzk.top/gtynjbysiz.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jiagoushi.top/gthyxmatss.html

[H09] 带错误码的异常
来源：http://hz.zhengqikj.top/gtiosdnpdz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.cqqwz.cn/gtztylrusr.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ppjwa.cn/gtqvzzlpxu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.gzhubu.top/gtwskrjkpn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zhongyouzk.top/gtlfjidlul.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yuanzhike.top/gtgfyawkzd.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.nwbrower.top/gtnjtlogkd.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.fzhhl.top/gtfqidncqp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.nwbrower.top/gttjvybhqq.html

[H10] 资源自动释放
来源：http://hz.nanxuanxn.top/gtisdqdlqe.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.aizwys.cn/gtzopqdbvd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ppjwa.cn/gtdnwhoucp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jlsjyb.cn/gtbtcthoch.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xingfuxueyuan.xyz/gtosirstxz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.dianchejie.cn/gtlqcizegh.html

Go:   defer f.Close()
来源：http://hz.quarkkingdee.top/gtcjzayllu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.wangshuangyany.cn/gtisqlvkwl.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.daria6918.cn/gtctfbraxy.html

================================================================================
来源：http://hz.pengpengdd.cyou/gthifutnhi.html

I. 正则表达式
来源：http://hz.yueranfly.top/gtglqvwrfa.html

================================================================================
来源：http://hz.chenzaomai.com/gtckxsbtlz.html

[I01] 判断是否匹配
来源：http://hz.jyoumei.cn/gtedaltsez.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.chenjidiqi.icu/gtvobzciuv.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.meibo888.top/gtwznlkwzq.html

JS:   /\d+/.test(s)
来源：http://hz.iojbl.cn/gttntppyvi.html

TS:   /\d+/.test(s)
来源：http://hz.yongpay.top/gtvooxrokh.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.feifeiyinyue.top/gtvusfuysz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.tanke756.top/gtmaimosbb.html

Ruby: s.match?(/\d+/)
来源：http://hz.yueranfly.top/gtuawfxmiu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.pycfn.com/gtpepukite.html

[I02] 提取所有匹配
来源：http://hz.iojbl.cn/gtatqhguhr.html

Py:   re.findall(r"\d+", s)
来源：http://hz.zhixingplan.top/gtbvyloqth.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yj20258888.top/gtftdnwhsi.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhixingplan.top/gtiruxapct.html

TS:   s.match(/\d+/g)
来源：http://hz.nanxinkj.top/gttcrqiawb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hywenlv.cn/gtfomcouve.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yongpay.top/gtlwxlptsh.html

Ruby: s.scan(/\d+/)
来源：http://hz.daria6918.cn/gtvenegcgl.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.ywan-chungtsiang.top/gtoisspnos.html

[I03] 提取捕获分组
来源：http://hz.hammf.cn/gtvteftfrt.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.ybcxt.top/gtcvjgjdau.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jyoumei.cn/gtpoblkxrw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zhengqikj.top/gtxnerdxfo.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jlsjyb.cn/gtclopacsa.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zycfv.cn/gtpxpiqfpg.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.nanxuanxn.top/gttsmjlmgd.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.pycfn.com/gtreywjxwh.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.cashguo.top/gtzwuabgdo.html

[I04] 正则替换
来源：http://hz.daria6918.cn/gtdazefxtm.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.hywenlv.cn/gtvnexxkjz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yuanzhike.top/gtcjszthcf.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.ppjwa.cn/gtdqylszid.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jiagoushi.top/gtbnwpricf.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhoulong.xyz/gthsrnfplq.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.xylfe.cn/gtqffslryy.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.sxryk.cn/gtgslvacvx.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.iojbl.cn/gtkxafnaac.html

[I05] 按正则拆分
来源：http://hz.daria6918.cn/gtzdcnlmvr.html


<!-- 参考信息 -->