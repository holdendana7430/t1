代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yj202588.top/gtpehstblx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.cdnleiting.top/gtorpdradi.html

[F11] 复制与移动文件
来源：http://hz.yongpay.top/gtwytgsjtj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.feifeiyinyue.top/gtqeuqgiaa.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yuxming.cn/gtwblauges.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.havefunace.top/gtuvmhwgdu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhongyouzk.top/gtwudpmcne.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.hammf.cn/gtsouagukm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yj202588.top/gtyxzlrvib.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.0kj1m.cn/gtrkzmqgwv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.snrcjt.cn/gtdrvoiomg.html

[F12] CSV 读写
来源：http://hz.zycfv.cn/gtcdoexfnv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.quarkkingdee.top/gtuadzidhz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.fengsongda.top/gtvotuawxq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.wangshuangyany.cn/gtjhzhcdbk.html

TS:   // 同上
来源：http://hz.haohaochexian.top/gtagslzylm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ppjwa.cn/gtufyztfcs.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yuanzhike.top/gtdepsylhv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.9152youxi.cn/gtyszeyzmo.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yonumen.top/gtqfmnxejv.html

================================================================================
来源：http://hz.chenzaomai.com/gtxykinbeu.html

G. 面向对象
来源：http://hz.gotoacloud.top/gtqggqzbms.html

================================================================================
来源：http://hz.52xcode.cn/gtvwnumnkx.html

[G01] 定义类
来源：http://hz.fengsongda.top/gtdnwaosjp.html

Py:   class User: pass
来源：http://hz.yj20258.top/gtueibwnwx.html

PHP:  class User {}
来源：http://hz.cdnleiting.top/gtstdxnepa.html

JS:   class User {}
来源：http://hz.daxiang520.top/gtplsanqes.html

TS:   class User { name: string = ""; }
来源：http://hz.chenjidiqi.icu/gtdtybqujv.html

Java: class User {}
来源：http://hz.yangfankeji.com/gtxrxbobvt.html

Go:   type User struct { Name string }
来源：http://hz.nwbrower.top/gtqhlrjxbw.html

Ruby: class User; end
来源：http://hz.sysykeji.top/gtpcliqunl.html

C#:   class User {}
来源：http://hz.xingfuxueyuan.xyz/gtzizclsrl.html

[G02] 构造函数
来源：http://hz.redwolf501.top/gtiaqtglik.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.shanyushiyangtech.top/gtgejdpfxx.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.pengpengdd.cyou/gtmshlgqau.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.shuidangran.top/gtqsttdscb.html

TS:   constructor(public name: string) {}
来源：http://hz.jlsjyb.cn/gtlooxkata.html

Java: User(String name) { this.name = name; }
来源：http://hz.zhixingplan.top/gtdghoachu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.ivvv.top/gtlvgabtmc.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jyoumei.cn/gtfrgwmakb.html

C#:   public User(string name) { Name = name; }
来源：http://hz.nanxuanxn.top/gtyibrlyqa.html

[G03] 实例属性
来源：http://hz.fengsongda.top/gtqaloagwd.html

Py:   self.name = "x"
来源：http://hz.yongpay.top/gtszyajpan.html

PHP:  public string $name = "x";
来源：http://hz.hammf.cn/gtgwvwshpm.html

JS:   this.name = "x";
来源：http://hz.ydjk.org.cn/gtdmfmnphz.html

TS:   name: string = "x";
来源：http://hz.tanke756.top/gtpheyibia.html

Java: private String name;
来源：http://hz.jyoumei.cn/gtvcrjlfxb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.52xcode.cn/gtndewiqed.html

Ruby: @name = "x"
来源：http://hz.zhixingplan.top/gtjsdkahdd.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.birdmap.top/gtobxtvldm.html

[G04] 定义方法
来源：http://hz.redwolf501.top/gtukvjcunh.html

Py:   def greet(self): return self.name
来源：http://hz.xziqi.cn/gtmkzekgpn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.cucudq.cn/gtsiuybkzt.html

JS:   greet() { return this.name; }
来源：http://hz.aizwys.cn/gtcvkhlmsr.html

TS:   greet(): string { return this.name; }
来源：http://hz.redwolf501.top/gtuctptxht.html

Java: String greet() { return name; }
来源：http://hz.zhaomingkeji.xyz/gtjbpfkhpp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yanxiufei.cn/gtukiumqwh.html

Ruby: def greet; @name; end
来源：http://hz.chenjidiqi.icu/gtvwtnatyp.html

C#:   public string Greet() => Name;
来源：http://hz.zhongyouzk.top/gtnpnyvdte.html

[G05] 继承
来源：http://hz.birdmap.top/gtxwcfbria.html

Py:   class Admin(User): pass
来源：http://hz.shzxlz.cn/gttssbiteq.html

PHP:  class Admin extends User {}
来源：http://hz.snrcjt.cn/gtcnzyrmvg.html

JS:   class Admin extends User {}
来源：http://hz.svipenyu.cn/gtemkrgcrb.html

TS:   class Admin extends User {}
来源：http://hz.nanxinkj.top/gtnugzkxqe.html

Java: class Admin extends User {}
来源：http://hz.shanyushiyangtech.top/gtvqlbtoow.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.guannengcc.top/gtykyazpcd.html

Ruby: class Admin < User; end
来源：http://hz.chenjidiqi.icu/gteqqonffv.html

C#:   class Admin : User {}
来源：http://hz.hywenlv.cn/gtambvooyq.html

[G06] 重写方法
来源：http://hz.hfpthk.cn/gtpdjvxtkn.html

Py:   def greet(self): return "admin"
来源：http://hz.zhengqikj.top/gtobkelwmc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yongpay.top/gtgijmfstq.html

JS:   greet() { return "admin"; }
来源：http://hz.zhoulong.xyz/gtwidlwhpz.html

TS:   greet(): string { return "admin"; }
来源：http://hz.tian-w.cn/gtrbooxmnt.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.gaohongyu789.top/gtubukayey.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhiwuduotai.top/gtgiizokso.html

Ruby: def greet; "admin"; end
来源：http://hz.tian-w.cn/gtdfjackgu.html

C#:   public override string Greet() => "admin";
来源：http://hz.mhx1999.top/gtmaayrgvb.html

[G07] 调用父类方法
来源：http://hz.ybcxt.top/gtjgxyyyud.html

Py:   super().greet()
来源：http://hz.hammf.cn/gthkriamon.html

PHP:  parent::greet();
来源：http://hz.tanke756.top/gtgwqlqtik.html

JS:   super.greet();
来源：http://hz.aibaodan.cn/gtoxkpuxya.html

TS:   super.greet();
来源：http://hz.xylfe.cn/gtaerihyea.html

Java: super.greet();
来源：http://hz.ivvv.top/gthgvizygu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.pengpengdd.cyou/gtecwpiqwa.html

Ruby: super
来源：http://hz.nwbrower.top/gttdnkhsul.html

C#:   base.Greet();
来源：http://hz.hongshengwenyu.top/gttdjplnyb.html

[G08] 静态方法与属性
来源：http://hz.316326.xyz/gtntzomdor.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.cucudq.cn/gtsrzhbfuj.html

PHP:  public static function f() {}
来源：http://hz.yvedp.cn/gtcnjmvjiq.html

JS:   static f() {}
来源：http://hz.jlsjyb.cn/gtlhrdsjgj.html

TS:   static f(): void {}
来源：http://hz.yj20258888.top/gtnijbprbm.html

Java: static void f() {}
来源：http://hz.ybcxt.top/gtolwkolvt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.andypj.xyz/gtoznxtkbi.html

Ruby: def self.f; end
来源：http://hz.hysaishi.cn/gtwsshjlhz.html

C#:   public static void F() {}
来源：http://hz.zhiwuduotai.top/gtelprkdzg.html

[G09] 接口 / 抽象类
来源：http://hz.xinyue.icu/gtvbkkgika.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.gotoacloud.top/gtouwfqovy.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.shuidangran.top/gtnffpmcfo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.snrcjt.cn/gtrxefuswj.html

TS:   interface Shape { area(): number; }
来源：http://hz.chenlongwang.top/gtyppmqvko.html

Java: interface Shape { double area(); }
来源：http://hz.birdmap.top/gtxqoxxlwv.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zhaomingkeji.xyz/gtwvyzwggk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yueranfly.top/gtihlfkjgx.html

C#:   interface IShape { double Area(); }
来源：http://hz.xingfuxueyuan.xyz/gtbnhrwpzc.html

[G10] 访问控制
来源：http://hz.pengpengdd.cyou/gtajutwqmb.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yueranfly.top/gtmxkkioqm.html

PHP:  public / protected / private
来源：http://hz.ppjwa.cn/gttntekgfg.html

JS:   #private 字段；其余公开
来源：http://hz.shuidangran.top/gtneszrghv.html

TS:   public / protected / private
来源：http://hz.jqgfzy.top/gtbbcgiysg.html

Java: public / protected / private / 默认包级
来源：http://hz.nanxinkj.top/gtixyjvlzn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.redwolf501.top/gtjhokckgd.html

Ruby: public / protected / private
来源：http://hz.zhaomingkeji.xyz/gtunmsurui.html

C#:   public / protected / private / internal
来源：http://hz.nanxuanxn.top/gtqceilgru.html

[G11] getter / setter
来源：http://hz.xuetiantiany.cn/gtvughanhw.html

Py:   @property 与 @x.setter
来源：http://hz.316326.xyz/gtzexztbyv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.hnqzz.top/gtxrfmajil.html

JS:   get name() { return this._name; }
来源：http://hz.nanxuanxn.top/gtypotpkdz.html

TS:   get name(): string { return this._name; }
来源：http://hz.yj202588.top/gtslvsiqlh.html

Java: public String getName() { return name; }
来源：http://hz.aibaodan.cn/gtwtkwnbzd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yongpay.top/gtlonkdikd.html

Ruby: attr_accessor :name
来源：http://hz.jianghu66.top/gtpwhhmrlh.html

C#:   public string Name { get; set; }
来源：http://hz.chenlongwang.top/gtbfihojdi.html

[G12] 对象转字符串
来源：http://hz.jqgfzy.top/gthkhyrvkc.html

Py:   def __str__(self): return self.name
来源：http://hz.feifeiyinyue.top/gtfqwcthiw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jinyuanbaomall.cn/gtzfukdaqc.html

JS:   toString() { return this.name; }
来源：http://hz.xylfe.cn/gtjnewyrdo.html

TS:   toString(): string { return this.name; }
来源：http://hz.fengsongda.top/gtkohldpoi.html

Java: @Override public String toString() { return name; }
来源：http://hz.dashuyun.cn/gtakelobyi.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.xuetiantiany.cn/gtdmzszjoc.html

Ruby: def to_s; @name; end
来源：http://hz.gaohongyu789.top/gtqgkxzvcr.html

C#:   public override string ToString() => Name;
来源：http://hz.vqdsnc.cn/gtvmnytlhi.html

[G13] 判断对象类型
来源：http://hz.shangyingyoupin.top/gtykxecaqw.html

Py:   isinstance(u, User)
来源：http://hz.ppjwa.cn/gtafxkmlmu.html

PHP:  $u instanceof User
来源：http://hz.zhiwuduotai.top/gtjytszukj.html

JS:   u instanceof User
来源：http://hz.sxryk.cn/gtxtzxfclw.html

TS:   u instanceof User
来源：http://hz.0kj1m.cn/gtobmoukcq.html

Java: u instanceof User
来源：http://hz.zhiwuduotai.top/gtbspdrwqz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.sysykeji.top/gtrojmmsvm.html

Ruby: u.is_a?(User)
来源：http://hz.wangshuangyany.cn/gtonrpgljg.html

C#:   u is User
来源：http://hz.zhijiandao.cn/gtvadphwac.html

[G14] 数据类 / record
来源：http://hz.316326.xyz/gtvxthvwpc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jqgufenzy.top/gtmqcqjymr.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.wangdashe.top/gtcdwmpqji.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.shanyushiyangkeji.top/gtznsuatxw.html

TS:   type User = { name: string; age: number };
来源：http://hz.wangdashe.top/gtfacutcgt.html

Java: record User(String name, int age) {}
来源：http://hz.yj20258.top/gtejyiqwbo.html

Go:   type User struct { Name string; Age int }
来源：http://hz.hysaishi.cn/gthlleidch.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.gzhubu.top/gttftwebgx.html

C#:   record User(string Name, int Age);
来源：http://hz.zdqjudy.top/gtfglqvdvt.html

[G15] 枚举
来源：http://hz.daria6918.cn/gtitkmocxv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.sweek.top/gttxesfcrh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.tian-w.cn/gtzfcgcxca.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hammf.cn/gtuwfkxiua.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.9152youxi.cn/gtlacxydwj.html

Java: enum Color { RED, GREEN }
来源：http://hz.sxryk.cn/gtildzbrpd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.cdnleiting.top/gtcpmvbfjj.html

Ruby: Color = %i[red green].freeze
来源：http://hz.chenjidiqi.icu/gthspxwitw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ywan-chungtsiang.top/gtrnlyujym.html

[G16] 对象转数组 / 字典
来源：http://hz.ydjk.org.cn/gtpkqqcjlp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhiwuduotai.top/gtfkgupwjo.html

PHP:  get_object_vars($obj);
来源：http://hz.quarkkingdee.top/gtbiftwqjw.html

JS:   Object.entries(obj)
来源：http://hz.ydzc1.top/gtriucghin.html

TS:   Object.entries(obj)
来源：http://hz.hnxiangtu.top/gtizmukhvp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.xuanzx.com/gtrxvxwwma.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.shuidangran.top/gtbbfnxdwt.html

Ruby: obj.instance_variables
来源：http://hz.jinqigfzy.top/gtynermwab.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.feifeiyinyue.top/gthgjrnine.html

================================================================================
来源：http://hz.mhx1999.top/gtoiptxbiz.html

H. 异常与错误处理
来源：http://hz.gaohongyu789.top/gtyncylaab.html

================================================================================
来源：http://hz.yangfankeji.com/gtdfwqswey.html

[H01] try / catch 基础
来源：http://hz.hfpthk.cn/gtaijwugbw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.vqdsnc.cn/gtgbqolnwb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hammf.cn/gtklmrmulh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.cucudq.cn/gtjauiycsv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jqgufenzy.top/gtfxuzybus.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.cqqwz.cn/gthkcqkcnj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yueranfly.top/gtuagltobo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.xinyue.icu/gtesphqulq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jinyuanbaomall.cn/gtimqrgofv.html

[H02] finally / ensure 收尾
来源：http://hz.gzhubu.top/gtyqiewgfe.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zhaomingkeji.xyz/gtutobgpqd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhoulong.xyz/gtocxhuccq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yuxming.cn/gtcbtiiirc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.kuanghao11.cn/gtadtwewer.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jlsjyb.cn/gtwcolsbqo.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jinqigufen.top/gtaxhahxkn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yuxming.cn/gtifisqpug.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.xylfe.cn/gtskpyjgla.html

[H03] 主动抛出异常
来源：http://hz.xuetiantiany.cn/gtcipdcabm.html

Py:   raise ValueError("错误信息")
来源：http://hz.aibaodan.cn/gthinsiyxp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jinghuilouyu.cn/gtjmgtvdbh.html

JS:   throw new Error("错误信息");
来源：http://hz.pengpengdd.cyou/gtesiqlkva.html

TS:   throw new Error("错误信息");
来源：http://hz.zhiwuduotai.top/gtslucmchk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.dianchejie.cn/gtlkuatsig.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.xuanzx.com/gtjshpeehu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.pengpengdd.cyou/gtzjltsdtm.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.aibaodan.cn/gtagqxyizp.html

[H04] 自定义异常类型
来源：http://hz.ehwqpu.com/gtgqupfixl.html

Py:   class MyError(Exception): pass
来源：http://hz.havefunace.top/gtniawxvfv.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zhaomingkeji.xyz/gtqnhjvmwt.html

JS:   class MyError extends Error {}
来源：http://hz.52xcode.cn/gtltdmbxeg.html

TS:   class MyError extends Error {}
来源：http://hz.shanyushiyangkeji.top/gtaifvnngj.html

Java: class MyException extends RuntimeException {}
来源：http://hz.52xcode.cn/gtkytmrsls.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.snrcjt.cn/gtmxtynlot.html

Ruby: class MyError < StandardError; end
来源：http://hz.chenlongwang.top/gtitkuhdsp.html

C#:   class MyException : Exception {}
来源：http://hz.chenjidiqi.icu/gtbubqvqfc.html

[H05] 捕获特定类型
来源：http://hz.sysykeji.top/gtgmxbpmim.html

Py:   except ValueError as e:
来源：http://hz.shangyingyoupin.top/gtqgknzxiz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.snrcjt.cn/gtmqljcfgw.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jinqigfzy.top/gttfrudfmh.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.daria6918.cn/gtsfxfvzcw.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhongyouzk.top/gtnwwreysn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.cucudq.cn/gtcqqnnggz.html

Ruby: rescue ArgumentError => e
来源：http://hz.wangdashe.top/gtgqnehvzj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yuxming.cn/gtnwwxtqmo.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zhongyouzk.top/gtpkmoawox.html

Py:   value = d.get("k") or default
来源：http://hz.yvedp.cn/gtsnvicecr.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yvedp.cn/gtdigmvhld.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.redwolf501.top/gtdimtmggb.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.xinyue.icu/gtqzvfsfqp.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.shanyushiyangtech.top/gtgpjbdbji.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.chenjidiqi.icu/gtalqkneog.html

Ruby: d&.dig(:a, :b)
来源：http://hz.gzhubu.top/gtrpqatwbl.html

C#:   obj?.A?.B ?? default
来源：http://hz.9152youxi.cn/gtvupirgtl.html

[H07] 断言
来源：http://hz.hywenlv.cn/gtlgohtaaw.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jinqigfzy.top/gtdpsnpqod.html

PHP:  assert($x > 0);
来源：http://hz.pengpengdd.cyou/gtoncizrpy.html

JS:   console.assert(x > 0);
来源：http://hz.c1oappe.top/gtdkvvsexe.html

TS:   console.assert(x > 0);
来源：http://hz.zdqjudy.top/gtkhaeabcf.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zhiwuduotai.top/gtpgphyjlv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.shanyushiyangtech.top/gtomohmmvv.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.gogol.net.cn/gtluttjdfr.html

C#:   Debug.Assert(x > 0);
来源：http://hz.cucudq.cn/gtrmembhpi.html

[H08] 获取错误信息与堆栈
来源：http://hz.jianghu66.top/gtsnbjecnd.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zycfv.cn/gtqrcvalzh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.cdnleiting.top/gthnqoghyi.html

JS:   e.message;  e.stack
来源：http://hz.hysaishi.cn/gtgjcfavxg.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jyoumei.cn/gtpaosckya.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.gzhubu.top/gtmavewwvh.html

Go:   err.Error()
来源：http://hz.shangyingyoupin.top/gtbnbltfbs.html

Ruby: e.message;  e.backtrace
来源：http://hz.xziqi.cn/gtzmgepgmk.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yj20258.top/gtozmvasol.html

[H09] 带错误码的异常
来源：http://hz.jlsjyb.cn/gtcfzbilhs.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.shanyushiyangtech.top/gtipgykpqz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.sweek.top/gtltjqevry.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.sysykeji.top/gtjbqxhtqz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.c1oappe.top/gtxdllspaz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.nwbrower.top/gtsiwenptk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.sxryk.cn/gtxukzhdzm.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.ivvv.top/gthorkouye.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yuxming.cn/gtrijigiqc.html

[H10] 资源自动释放
来源：http://hz.yangfankeji.com/gtfzhmgjww.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.xziqi.cn/gtnptniiqf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.hywenlv.cn/gtofewlvsj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yj20258888.top/gtyuxzactw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shuidangran.top/gtrohakghm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.c1oappe.top/gtkvbuukkg.html

Go:   defer f.Close()
来源：http://hz.chenlongwang.top/gtslevbklf.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.haohaochexian.top/gtbpgmkwxa.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.dianchejie.cn/gttseclioe.html

================================================================================
来源：http://hz.xuetiantiany.cn/gttrmdvlyy.html

I. 正则表达式
来源：http://hz.shanyushiyangkeji.top/gticojmczc.html

================================================================================
来源：http://hz.ivvv.top/gtlwnrtywb.html

[I01] 判断是否匹配
来源：http://hz.gaohongyu789.top/gtkahnptur.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.dashuyun.cn/gtwvpgllsu.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.gogol.net.cn/gtavcmcfsv.html

JS:   /\d+/.test(s)
来源：http://hz.chenlongwang.top/gtggtjuyqw.html

TS:   /\d+/.test(s)
来源：http://hz.gogol.net.cn/gtthrqnoqf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.c1oappe.top/gtuxspserq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yonumen.top/gtvzwvkxil.html

Ruby: s.match?(/\d+/)
来源：http://hz.zhongyouzk.top/gtefmhpxgg.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jinqigufen.top/gtjebtbxhc.html

[I02] 提取所有匹配
来源：http://hz.mhx1999.top/gtfruqmgvn.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ivvv.top/gtnbzkkpis.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.wangdashe.top/gtyliprdmk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.shzxlz.cn/gttqktbqgf.html

TS:   s.match(/\d+/g)
来源：http://hz.52xcode.cn/gtmkfkmwfa.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.xziqi.cn/gtadwzfpud.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zhaomingkeji.xyz/gtckjbxmyn.html

Ruby: s.scan(/\d+/)
来源：http://hz.cdnleiting.top/gtkdbzgowk.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zhongyouzk.top/gtjpcnjhex.html

[I03] 提取捕获分组
来源：http://hz.sufxvd.cn/gtactvfrbf.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.cheryme.top/gtpggwhltz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.chenjidiqi.icu/gtmesbuxqn.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yangfankeji.com/gtnlszsxun.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ppjwa.cn/gtorwnejfa.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.xinyue.icu/gtabiyvzjo.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.dianchejie.cn/gtmfzbzpys.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhongyouzk.top/gtuednozlw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.sxryk.cn/gtgydqggkj.html

[I04] 正则替换
来源：http://hz.yongpay.top/gtthznjlny.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.aibaodan.cn/gttcxpmugk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yanxiufei.cn/gtobfewqdx.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.zhijiandao.cn/gtxirjthae.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.iojbl.cn/gtdfjmrmmy.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yuanzhike.top/gthijbpuse.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jinghuilouyu.cn/gtturbxiif.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.pycfn.com/gthkbskgwr.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.c1oappe.top/gtzclwcapw.html

[I05] 按正则拆分
来源：http://hz.cucudq.cn/gtalqfkexs.html


<!-- 参考信息 -->