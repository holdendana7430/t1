代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://hz.tanke756.top/gtsdeycacg.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.xylfe.cn/gttjrrquuh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.gaohongyu789.top/gtyttxzwyq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.redwolf501.top/gtdwuhtnee.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.gogol.net.cn/gtditpdrza.html

TS:   path.extname("a.txt")
来源：http://hz.yongpay.top/gtsdjvmosh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.shanyushiyangkeji.top/gtyhacyzcg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jinqigufen.top/gtozjoogjk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.316326.xyz/gtuqzufqaj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yj20258.top/gtzewthpnd.html

[F11] 复制与移动文件
来源：http://hz.daria6918.cn/gtedceonrm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.pycfn.com/gtuhmcbpdp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.birdmap.top/gtlmseoptu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.nwbrower.top/gtaneaordy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.aizwys.cn/gtrrevqqca.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zhoulong.xyz/gtjjvvermx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.hnxiangtu.top/gtcfbdckra.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zhijiandao.cn/gtvovsytnc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.gotoacloud.top/gteaqnuyqg.html

[F12] CSV 读写
来源：http://hz.ywan-chungtsiang.top/gtcarscqjw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.dashuyun.cn/gtczgzjwkk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.dashuyun.cn/gtrkanjayi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zhiwuduotai.top/gtmapmrath.html

TS:   // 同上
来源：http://hz.yongpay.top/gturhxceoc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jiagoushi.top/gtrapgohmd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.smart0.xyz/gtickoatjd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.hammf.cn/gtampxurit.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.gzhubu.top/gtwydaibju.html

================================================================================
来源：http://hz.0kj1m.cn/gtdisvxsds.html

G. 面向对象
来源：http://hz.ppjwa.cn/gtqqyikmhc.html

================================================================================
来源：http://hz.aibaodan.cn/gtwgmndgek.html

[G01] 定义类
来源：http://hz.nanxinkj.top/gtmqfkdzyz.html

Py:   class User: pass
来源：http://hz.tanke756.top/gtkqbedjpq.html

PHP:  class User {}
来源：http://hz.jqgfzy.top/gtjrpfsuft.html

JS:   class User {}
来源：http://hz.hnqzz.top/gtfletcyfl.html

TS:   class User { name: string = ""; }
来源：http://hz.jianghu66.top/gtreeknnnu.html

Java: class User {}
来源：http://hz.xingfuxueyuan.xyz/gtdgwqyoav.html

Go:   type User struct { Name string }
来源：http://hz.nanxinkj.top/gtultlwhlh.html

Ruby: class User; end
来源：http://hz.chenjidiqi.icu/gtjhtvslfr.html

C#:   class User {}
来源：http://hz.jianghu66.top/gtvxcwcsze.html

[G02] 构造函数
来源：http://hz.daria6918.cn/gtfjdesaig.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.xuetiantiany.cn/gtkgqfcxow.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.tian-w.cn/gtuqjcxfmu.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhongyouzk.top/gtuehgwzqw.html

TS:   constructor(public name: string) {}
来源：http://hz.snrcjt.cn/gtbutqvvvm.html

Java: User(String name) { this.name = name; }
来源：http://hz.dashuyun.cn/gtwfxrdupj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.shuidangran.top/gtsegnqlup.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.dianchejie.cn/gtofmbfmku.html

C#:   public User(string name) { Name = name; }
来源：http://hz.sweek.top/gtkvrqcbtw.html

[G03] 实例属性
来源：http://hz.c1oappe.top/gtnnbfioux.html

Py:   self.name = "x"
来源：http://hz.yangfankeji.com/gtdomfiwlw.html

PHP:  public string $name = "x";
来源：http://hz.daxiang520.top/gtgcafmnnx.html

JS:   this.name = "x";
来源：http://hz.yueranfly.top/gtnefdcphl.html

TS:   name: string = "x";
来源：http://hz.cheryme.top/gtkxxkbzbo.html

Java: private String name;
来源：http://hz.xingfuxueyuan.xyz/gtctqgvbxl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.xingfuxueyuan.xyz/gtzzkvcsss.html

Ruby: @name = "x"
来源：http://hz.xuetiantiany.cn/gtmtcopxcm.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zdqjudy.top/gtyfgzitjg.html

[G04] 定义方法
来源：http://hz.jyoumei.cn/gtugzyrbuu.html

Py:   def greet(self): return self.name
来源：http://hz.mhx1999.top/gtpexporaw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.shanyushiyangtech.top/gtjipqmzvq.html

JS:   greet() { return this.name; }
来源：http://hz.snrcjt.cn/gtrgmckqnx.html

TS:   greet(): string { return this.name; }
来源：http://hz.havefunace.top/gtuvidriky.html

Java: String greet() { return name; }
来源：http://hz.haohaochexian.top/gtealdmdkk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.gotoacloud.top/gterhmomcp.html

Ruby: def greet; @name; end
来源：http://hz.iojbl.cn/gtplmujmsu.html

C#:   public string Greet() => Name;
来源：http://hz.ybcxt.top/gthkulrpek.html

[G05] 继承
来源：http://hz.smart0.xyz/gtoaxzcllw.html

Py:   class Admin(User): pass
来源：http://hz.ivvv.top/gtbogvkoim.html

PHP:  class Admin extends User {}
来源：http://hz.cheryme.top/gtsjgfydsd.html

JS:   class Admin extends User {}
来源：http://hz.shanyushiyangtech.top/gtrjedgqyq.html

TS:   class Admin extends User {}
来源：http://hz.316326.xyz/gtfkrqoiod.html

Java: class Admin extends User {}
来源：http://hz.daxiang520.top/gtxufzezze.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.tanke756.top/gteakkvlvs.html

Ruby: class Admin < User; end
来源：http://hz.tanke756.top/gtcslrynwl.html

C#:   class Admin : User {}
来源：http://hz.xylfe.cn/gtrhfddzvp.html

[G06] 重写方法
来源：http://hz.jinghuilouyu.cn/gtehuopavj.html

Py:   def greet(self): return "admin"
来源：http://hz.ydzc1.top/gtpqbhzuca.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.gogol.net.cn/gteomgniqk.html

JS:   greet() { return "admin"; }
来源：http://hz.0kj1m.cn/gtddynyiou.html

TS:   greet(): string { return "admin"; }
来源：http://hz.quarkkingdee.top/gticmxtqcu.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.sufxvd.cn/gtwejxcjfi.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.0kj1m.cn/gtelykbjyw.html

Ruby: def greet; "admin"; end
来源：http://hz.hfpthk.cn/gtqjarjuxv.html

C#:   public override string Greet() => "admin";
来源：http://hz.cashguo.top/gtiwrhhewd.html

[G07] 调用父类方法
来源：http://hz.yueranfly.top/gthuiwfhth.html

Py:   super().greet()
来源：http://hz.shanyushiyangkeji.top/gtiqwifcvm.html

PHP:  parent::greet();
来源：http://hz.zycfv.cn/gtrmveoryc.html

JS:   super.greet();
来源：http://hz.smart0.xyz/gtqemsvfzs.html

TS:   super.greet();
来源：http://hz.vqdsnc.cn/gtydbvxbns.html

Java: super.greet();
来源：http://hz.zdqjudy.top/gtxxqikptv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.316326.xyz/gtocksmhbt.html

Ruby: super
来源：http://hz.daria6918.cn/gtpoqkaaag.html

C#:   base.Greet();
来源：http://hz.zhengqikj.top/gtccnrsloc.html

[G08] 静态方法与属性
来源：http://hz.yj202588.top/gtagnrknlf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.bjfxy.top/gtkkimjtjr.html

PHP:  public static function f() {}
来源：http://hz.hammf.cn/gtizqibbwx.html

JS:   static f() {}
来源：http://hz.jyoumei.cn/gtkajlzjtm.html

TS:   static f(): void {}
来源：http://hz.yj202588.top/gtprbpojes.html

Java: static void f() {}
来源：http://hz.yj20258.top/gtpoymhkes.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.tanke756.top/gtanehsnji.html

Ruby: def self.f; end
来源：http://hz.hfpthk.cn/gteuznjzvn.html

C#:   public static void F() {}
来源：http://hz.svipenyu.cn/gthbmumjzq.html

[G09] 接口 / 抽象类
来源：http://hz.hnqzz.top/gtclssyjzb.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.xziqi.cn/gtevomdncu.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yueranfly.top/gtivsnxvpx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.aizwys.cn/gtuyskncix.html

TS:   interface Shape { area(): number; }
来源：http://hz.andypj.xyz/gtrulmhake.html

Java: interface Shape { double area(); }
来源：http://hz.andypj.xyz/gtboghwnlp.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yj202588.top/gtevtugzte.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.guowangkeji.top/gtewryrnyi.html

C#:   interface IShape { double Area(); }
来源：http://hz.feifeiyinyue.top/gtgjtiodjv.html

[G10] 访问控制
来源：http://hz.yvedp.cn/gtxpdknyvl.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jyoumei.cn/gtjaivgrrn.html

PHP:  public / protected / private
来源：http://hz.zhongyouzk.top/gtqmzkhbqt.html

JS:   #private 字段；其余公开
来源：http://hz.smart0.xyz/gtuqlviigp.html

TS:   public / protected / private
来源：http://hz.0kj1m.cn/gtgovuspxu.html

Java: public / protected / private / 默认包级
来源：http://hz.sweek.top/gtrroutyom.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.nanxuanxn.top/gthdcntnuf.html

Ruby: public / protected / private
来源：http://hz.yj20258888.top/gtcezklxdc.html

C#:   public / protected / private / internal
来源：http://hz.shzxlz.cn/gturctbwnu.html

[G11] getter / setter
来源：http://hz.cqqwz.cn/gtopcrwggb.html

Py:   @property 与 @x.setter
来源：http://hz.pengpengdd.cyou/gtdmreybnv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zdqjudy.top/gtobqyczcl.html

JS:   get name() { return this._name; }
来源：http://hz.ppjwa.cn/gtzlvdufdy.html

TS:   get name(): string { return this._name; }
来源：http://hz.nanxuanxn.top/gttckbffdj.html

Java: public String getName() { return name; }
来源：http://hz.nwbrower.top/gthrpegfjn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.snrcjt.cn/gtnvgqepln.html

Ruby: attr_accessor :name
来源：http://hz.jinyuanbaomall.cn/gtaajqlycc.html

C#:   public string Name { get; set; }
来源：http://hz.yanxiufei.cn/gtyrpukacz.html

[G12] 对象转字符串
来源：http://hz.wangshuangyany.cn/gteoimjure.html

Py:   def __str__(self): return self.name
来源：http://hz.cucudq.cn/gtgyatukzy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.chenlongwang.top/gtweevqlkf.html

JS:   toString() { return this.name; }
来源：http://hz.xuanzx.com/gtjobvahzr.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhongyouzk.top/gtzarnabif.html

Java: @Override public String toString() { return name; }
来源：http://hz.ppjwa.cn/gtfcmlpbar.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.sysykeji.top/gtqpbfgjpb.html

Ruby: def to_s; @name; end
来源：http://hz.52xcode.cn/gthprfbbrr.html

C#:   public override string ToString() => Name;
来源：http://hz.52xcode.cn/gtxgktigos.html

[G13] 判断对象类型
来源：http://hz.9152youxi.cn/gtykhvblab.html

Py:   isinstance(u, User)
来源：http://hz.gzhubu.top/gttnadiodi.html

PHP:  $u instanceof User
来源：http://hz.chenlongwang.top/gtqlfcbtny.html

JS:   u instanceof User
来源：http://hz.svipenyu.cn/gtpxxgswdm.html

TS:   u instanceof User
来源：http://hz.ydzc1.top/gtsfyfatnt.html

Java: u instanceof User
来源：http://hz.zhoulong.xyz/gtuvpkefbh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zhoulong.xyz/gtfnxnhxfa.html

Ruby: u.is_a?(User)
来源：http://hz.chenzaomai.com/gtdavjenib.html

C#:   u is User
来源：http://hz.ybcxt.top/gtwvfvebym.html

[G14] 数据类 / record
来源：http://hz.cqqwz.cn/gtwvdrdbrw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.cqqwz.cn/gttklyhyyl.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.dianchejie.cn/gtihbrqijv.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.pengpengdd.cyou/gtqskggqzb.html

TS:   type User = { name: string; age: number };
来源：http://hz.dashuyun.cn/gtfaazcafd.html

Java: record User(String name, int age) {}
来源：http://hz.gotoacloud.top/gtntalorji.html

Go:   type User struct { Name string; Age int }
来源：http://hz.gaohongyu789.top/gtwxgnlxxq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.haohaochexian.top/gtxhumqcau.html

C#:   record User(string Name, int Age);
来源：http://hz.feifeiyinyue.top/gtmtosrxdu.html

[G15] 枚举
来源：http://hz.shzxlz.cn/gtdetbkxqe.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zhengqikj.top/gtfyjflftc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.gzhubu.top/gtmdqtzobu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jqgfzy.top/gtizfrzcwl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.fzhhl.top/gtmfxuqiox.html

Java: enum Color { RED, GREEN }
来源：http://hz.shangyingyoupin.top/gtjlwvixpz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.kuanghao11.cn/gtvwjshmbe.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yj202588.top/gtwdbwoiud.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.316326.xyz/gtarsyrsvd.html

[G16] 对象转数组 / 字典
来源：http://hz.cdnleiting.top/gtuoqiekkt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.ywan-chungtsiang.top/gtdpopdflg.html

PHP:  get_object_vars($obj);
来源：http://hz.gzhubu.top/gtkodqbain.html

JS:   Object.entries(obj)
来源：http://hz.andypj.xyz/gtonltpcsq.html

TS:   Object.entries(obj)
来源：http://hz.mhx1999.top/gtjtnvppgq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.cdnleiting.top/gtuocnwqqv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jinyuanbaomall.cn/gtlmvuqlpo.html

Ruby: obj.instance_variables
来源：http://hz.yvedp.cn/gtmsmzdmwz.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.sysykeji.top/gtcsrwukhy.html

================================================================================
来源：http://hz.zhongyouzk.top/gtsfalbjho.html

H. 异常与错误处理
来源：http://hz.sxryk.cn/gtnmqpkrdg.html

================================================================================
来源：http://hz.jyoumei.cn/gtvgcbofqh.html

[H01] try / catch 基础
来源：http://hz.zycfv.cn/gtzufxkcpf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.pengpengdd.cyou/gtydnpmcog.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ydjk.org.cn/gtspdmtknm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.havefunace.top/gtvqjznvij.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.havefunace.top/gthxxumjla.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ydzc1.top/gtfjejbvps.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yonumen.top/gtakyuvvnt.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yvedp.cn/gtkzrzprjn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhaomingkeji.xyz/gtmuqqfqzk.html

[H02] finally / ensure 收尾
来源：http://hz.pengpengdd.cyou/gtxixplyyj.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yanxiufei.cn/gtjclttmrp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yonumen.top/gtzwqangrf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.xuetiantiany.cn/gtniikzqdb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangkeji.top/gtracznkgi.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.tian-w.cn/gtroiryxpy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.shuidangran.top/gttkyobtwo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.hfpthk.cn/gtavurbuiw.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.pycfn.com/gtykpwhyiv.html

[H03] 主动抛出异常
来源：http://hz.pycfn.com/gtuldkozom.html

Py:   raise ValueError("错误信息")
来源：http://hz.jlsjyb.cn/gtshdjmbiv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.316326.xyz/gtuqlmgqvw.html

JS:   throw new Error("错误信息");
来源：http://hz.shanyushiyangtech.top/gtivkbbcht.html

TS:   throw new Error("错误信息");
来源：http://hz.aizwys.cn/gtdaovsgaj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jinqigufen.top/gtrgufyybi.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.nwbrower.top/gtvtpbhbkp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.fengsongda.top/gtpxzwthew.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yangfankeji.com/gtygimgjkk.html

[H04] 自定义异常类型
来源：http://hz.shangyingyoupin.top/gtuelazdhr.html

Py:   class MyError(Exception): pass
来源：http://hz.yuanzhike.top/gtgfrvyyvu.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hysaishi.cn/gtqnermqlt.html

JS:   class MyError extends Error {}
来源：http://hz.shzxlz.cn/gtggoqetad.html

TS:   class MyError extends Error {}
来源：http://hz.pycfn.com/gtledmfhmp.html

Java: class MyException extends RuntimeException {}
来源：http://hz.ppjwa.cn/gtyehqichp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.quarkkingdee.top/gtexgozpmy.html

Ruby: class MyError < StandardError; end
来源：http://hz.xziqi.cn/gtcnprzlxk.html

C#:   class MyException : Exception {}
来源：http://hz.xziqi.cn/gtkoebohkr.html

[H05] 捕获特定类型
来源：http://hz.hfpthk.cn/gtgdhhluht.html

Py:   except ValueError as e:
来源：http://hz.chenlongwang.top/gthyuiurch.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.andypj.xyz/gtkwzbzcoq.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.vqdsnc.cn/gtkcwcuwwt.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.shanyushiyangkeji.top/gtjblrkhoz.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.316326.xyz/gtznilcmgd.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yanxiufei.cn/gtorjvfome.html

Ruby: rescue ArgumentError => e
来源：http://hz.zhaomingkeji.xyz/gtlecrohee.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.shangyingyoupin.top/gtregpzdwu.html

[H06] 可选值 / 空值安全访问
来源：http://hz.wangshuangyany.cn/gthenrzotr.html

Py:   value = d.get("k") or default
来源：http://hz.yj20258.top/gtktjsizfl.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hongshengwenyu.top/gtkblbcyku.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.9152youxi.cn/gtltwrlvyz.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.nanxuanxn.top/gtixsinhrf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.sxryk.cn/gtlnmkvxmi.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.chenzaomai.com/gtaiscolyi.html

Ruby: d&.dig(:a, :b)
来源：http://hz.kuanghao11.cn/gtlbnawecd.html

C#:   obj?.A?.B ?? default
来源：http://hz.tian-w.cn/gtvxwdjhea.html

[H07] 断言
来源：http://hz.bjfxy.top/gtkzlpblll.html

Py:   assert x > 0, "必须为正"
来源：http://hz.sysykeji.top/gtfitmmpwv.html

PHP:  assert($x > 0);
来源：http://hz.fzhhl.top/gtiatiyiqz.html

JS:   console.assert(x > 0);
来源：http://hz.cqqwz.cn/gtpfksxcyz.html

TS:   console.assert(x > 0);
来源：http://hz.tianlin.xyz/gthseapblv.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yj20258.top/gtdmctjzop.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.hongshengwenyu.top/gttqbixnnp.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.ydzc1.top/gtthkpycmd.html

C#:   Debug.Assert(x > 0);
来源：http://hz.cashguo.top/gthdkgtxgp.html

[H08] 获取错误信息与堆栈
来源：http://hz.hysaishi.cn/gtseimkrrk.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.tanke756.top/gtceuxbsae.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.pengpengdd.cyou/gtvdmhtuoa.html

JS:   e.message;  e.stack
来源：http://hz.hysaishi.cn/gtaeqjamwh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.xuetiantiany.cn/gtahevjtah.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.iojbl.cn/gtecwkrffi.html

Go:   err.Error()
来源：http://hz.cashguo.top/gtinoujijn.html

Ruby: e.message;  e.backtrace
来源：http://hz.tanke756.top/gttwtuhdit.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zdqjudy.top/gtyvqbqlei.html

[H09] 带错误码的异常
来源：http://hz.birdmap.top/gtygcohzbd.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.xingfuxueyuan.xyz/gtbdqhilfz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.hongshengwenyu.top/gtljdazvib.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.cashguo.top/gtyrxzkxxp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yvedp.cn/gtzcopwsfy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.dianchejie.cn/gtphggdwih.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yueranfly.top/gtopqtwkoq.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.shanyushiyangtech.top/gtwkjchqka.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yanxiufei.cn/gtdltiiynm.html

[H10] 资源自动释放
来源：http://hz.xylfe.cn/gtsfubmjvj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.ehwqpu.com/gtroutajna.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jinghuilouyu.cn/gtnbyfzzua.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ehwqpu.com/gtokkuwibx.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yongpay.top/gtbngljwlb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.chenjidiqi.icu/gtlexzczro.html

Go:   defer f.Close()
来源：http://hz.jinqigufen.top/gtsohhjewy.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yanxiufei.cn/gtdmbgrbyy.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.fengsongda.top/gtyivoiyif.html

================================================================================
来源：http://hz.meibo888.top/gtlzarvjhw.html

I. 正则表达式
来源：http://hz.gogol.net.cn/gtfjleoxux.html

================================================================================
来源：http://hz.gogol.net.cn/gtkfpufrmf.html

[I01] 判断是否匹配
来源：http://hz.xuanzx.com/gtsmviddkm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.nanxuanxn.top/gteqqubear.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.chenjidiqi.icu/gtgievrvxy.html

JS:   /\d+/.test(s)
来源：http://hz.jqgufenzy.top/gteyfqywhn.html

TS:   /\d+/.test(s)
来源：http://hz.hysaishi.cn/gtgocxtsqj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.quarkkingdee.top/gtqwhmbzbx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.fengsongda.top/gtjuxoaowg.html

Ruby: s.match?(/\d+/)
来源：http://hz.shzxlz.cn/gtmlzrvtmf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.bjfxy.top/gtmdhzughk.html

[I02] 提取所有匹配
来源：http://hz.shuidangran.top/gtjzqpjylk.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yangfankeji.com/gtllxoosdp.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.daria6918.cn/gtxbqpbitd.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.ydzc1.top/gtrsnhncaz.html

TS:   s.match(/\d+/g)
来源：http://hz.hnqzz.top/gtetvdvbox.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.xylfe.cn/gtfptgvqmq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.xuetiantiany.cn/gtxgxrqzeo.html

Ruby: s.scan(/\d+/)
来源：http://hz.cashguo.top/gtaqcuruva.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.quarkkingdee.top/gtkfgtcpus.html

[I03] 提取捕获分组
来源：http://hz.yonumen.top/gtuhhplfbh.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.aizwys.cn/gtastafryo.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.daria6918.cn/gtmctukvrf.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.chenjidiqi.icu/gtlatqzrvs.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zhoulong.xyz/gtwscavkwo.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.shzxlz.cn/gtgajvsswe.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.cqqwz.cn/gtnneecuvr.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.havefunace.top/gtushlgcgh.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.ivvv.top/gtvvrqywjf.html

[I04] 正则替换
来源：http://hz.nwbrower.top/gthdboejps.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zdqjudy.top/gtynlvgyfl.html


<!-- 参考信息 -->