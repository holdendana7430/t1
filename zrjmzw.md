代发 wailian999

[F09] 获取文件大小
来源：http://hz.shanyushiyangkeji.top/gtwtyrbyzd.html

Py:   os.path.getsize("a.txt")
来源：http://hz.fengsongda.top/gtqafobduc.html

PHP:  filesize("a.txt");
来源：http://hz.mhx1999.top/gtnmaksims.html

JS:   fs.statSync("a.txt").size
来源：http://hz.ywan-chungtsiang.top/gtiqrjsuur.html

TS:   fs.statSync("a.txt").size
来源：http://hz.cdnleiting.top/gtuhshnbys.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.svipenyu.cn/gtouudnrvs.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.52xcode.cn/gtopzbzzgt.html

Ruby: File.size("a.txt")
来源：http://hz.zdqjudy.top/gttfwefcld.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.guannengcc.top/gtjnkncvam.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.ehwqpu.com/gtzwpxisii.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jiagoushi.top/gtixrkqzcg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.fengsongda.top/gtyfgmrytl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zhiwuduotai.top/gtaodkmtxn.html

TS:   path.extname("a.txt")
来源：http://hz.svipenyu.cn/gtkemjfivf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.gaohongyu789.top/gtoseqvpfw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.chenlongwang.top/gtmximylzf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.daxiang520.top/gtxcwhjhkl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.shuidangran.top/gtbxvhohao.html

[F11] 复制与移动文件
来源：http://hz.zhixingplan.top/gtmsfjjpfn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.xingfuxueyuan.xyz/gtyxgslyrf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.tianlin.xyz/gtqytazvxa.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yueranfly.top/gtyprraucd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ybcxt.top/gtsrcpcinn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jiagoushi.top/gtpttaumiz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.shanyushiyangtech.top/gtqzpaszum.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.hysaishi.cn/gtuerfqdov.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ydjk.org.cn/gtqcoaiubh.html

[F12] CSV 读写
来源：http://hz.meibo888.top/gtknfqityq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xuetiantiany.cn/gtgixzydnn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.guannengcc.top/gtulsuwkvm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.cucudq.cn/gteayasdtn.html

TS:   // 同上
来源：http://hz.snrcjt.cn/gtcppmifke.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zhixingplan.top/gtbngbrylk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhijiandao.cn/gtrqxoitqn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.chenlongwang.top/gtehvivvkg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.xylfe.cn/gtmzqovyiq.html

================================================================================
来源：http://hz.xylfe.cn/gtmuapstro.html

G. 面向对象
来源：http://hz.iojbl.cn/gtjfgzwscc.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtdwrnbzju.html

[G01] 定义类
来源：http://hz.tanke756.top/gtfhhfniqu.html

Py:   class User: pass
来源：http://hz.hammf.cn/gtypvkuruu.html

PHP:  class User {}
来源：http://hz.ppjwa.cn/gtachmoqfc.html

JS:   class User {}
来源：http://hz.yueranfly.top/gtdgjrbjyx.html

TS:   class User { name: string = ""; }
来源：http://hz.cqqwz.cn/gtnabceqpy.html

Java: class User {}
来源：http://hz.cucudq.cn/gtiioamlxs.html

Go:   type User struct { Name string }
来源：http://hz.guowangkeji.top/gtiisvxobr.html

Ruby: class User; end
来源：http://hz.smart0.xyz/gtrbaxdnbe.html

C#:   class User {}
来源：http://hz.yangfankeji.com/gtlaqqwhdo.html

[G02] 构造函数
来源：http://hz.vqdsnc.cn/gtpdtytvgc.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jianghu66.top/gtlslzbfxz.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hfpthk.cn/gtnktgdyiw.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.daxiang520.top/gtwpxcjcrj.html

TS:   constructor(public name: string) {}
来源：http://hz.ppjwa.cn/gtuvoeuhgz.html

Java: User(String name) { this.name = name; }
来源：http://hz.chenlongwang.top/gtfubxizgm.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.guowangkeji.top/gtjbatvxbp.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.shanyushiyangkeji.top/gtqfsfsquq.html

C#:   public User(string name) { Name = name; }
来源：http://hz.hywenlv.cn/gtvscqfzgt.html

[G03] 实例属性
来源：http://hz.shanyushiyangkeji.top/gtsdswhzgk.html

Py:   self.name = "x"
来源：http://hz.jqgufenzy.top/gtpsownlhi.html

PHP:  public string $name = "x";
来源：http://hz.wangdashe.top/gtvescehyx.html

JS:   this.name = "x";
来源：http://hz.zhoulong.xyz/gtgunuevwk.html

TS:   name: string = "x";
来源：http://hz.tianlin.xyz/gtcgodnwbv.html

Java: private String name;
来源：http://hz.yangfankeji.com/gtotfxzvie.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yuxming.cn/gtuljfxmes.html

Ruby: @name = "x"
来源：http://hz.xingfuxueyuan.xyz/gtpvvwxwlo.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zhongyouzk.top/gtazbumrbh.html

[G04] 定义方法
来源：http://hz.chenzaomai.com/gtgszyctgw.html

Py:   def greet(self): return self.name
来源：http://hz.yueranfly.top/gtrqpyffkb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yuanzhike.top/gtwmkqcmcb.html

JS:   greet() { return this.name; }
来源：http://hz.jianghu66.top/gtppaylpyy.html

TS:   greet(): string { return this.name; }
来源：http://hz.pycfn.com/gtvmeepcbw.html

Java: String greet() { return name; }
来源：http://hz.c1oappe.top/gtrkkbbgyu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.xuanzx.com/gtxfhvwjkf.html

Ruby: def greet; @name; end
来源：http://hz.wangshuangyany.cn/gttsmizkxo.html

C#:   public string Greet() => Name;
来源：http://hz.mhx1999.top/gtmspmhcza.html

[G05] 继承
来源：http://hz.redwolf501.top/gtoedacjhi.html

Py:   class Admin(User): pass
来源：http://hz.sweek.top/gtywhbgdiw.html

PHP:  class Admin extends User {}
来源：http://hz.ppjwa.cn/gttnwmaebk.html

JS:   class Admin extends User {}
来源：http://hz.yuanzhike.top/gtvzsvfsuc.html

TS:   class Admin extends User {}
来源：http://hz.zhongyouzk.top/gtunvphfyg.html

Java: class Admin extends User {}
来源：http://hz.yuxming.cn/gtxnaiwgju.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hammf.cn/gtzellpvoi.html

Ruby: class Admin < User; end
来源：http://hz.havefunace.top/gtwojkcubg.html

C#:   class Admin : User {}
来源：http://hz.yuxming.cn/gtfprezxpv.html

[G06] 重写方法
来源：http://hz.jinyuanbaomall.cn/gtkvvrtqbh.html

Py:   def greet(self): return "admin"
来源：http://hz.shanyushiyangtech.top/gtcgtqzfjc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.nanxinkj.top/gtthvickiw.html

JS:   greet() { return "admin"; }
来源：http://hz.jqgfzy.top/gtmzhytpwz.html

TS:   greet(): string { return "admin"; }
来源：http://hz.ivvv.top/gtuwpmlsjg.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhongyouzk.top/gtwiqqycbw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.0kj1m.cn/gtoliicvjo.html

Ruby: def greet; "admin"; end
来源：http://hz.shanyushiyangkeji.top/gtguarhdqd.html

C#:   public override string Greet() => "admin";
来源：http://hz.xingfuxueyuan.xyz/gtzspaavsx.html

[G07] 调用父类方法
来源：http://hz.tian-w.cn/gtqujnsgqz.html

Py:   super().greet()
来源：http://hz.ehwqpu.com/gtnawtmsiw.html

PHP:  parent::greet();
来源：http://hz.chenlongwang.top/gtehzfojrg.html

JS:   super.greet();
来源：http://hz.haohaochexian.top/gtfsikweek.html

TS:   super.greet();
来源：http://hz.smart0.xyz/gtajszghjr.html

Java: super.greet();
来源：http://hz.shanyushiyangtech.top/gtrgoldrbr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.ivvv.top/gtfnodqjzn.html

Ruby: super
来源：http://hz.aizwys.cn/gtxhxmyjau.html

C#:   base.Greet();
来源：http://hz.feifeiyinyue.top/gtnlbugpof.html

[G08] 静态方法与属性
来源：http://hz.dashuyun.cn/gtjktnebsm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jinghuilouyu.cn/gtabqvinsd.html

PHP:  public static function f() {}
来源：http://hz.havefunace.top/gtgcwvxkbw.html

JS:   static f() {}
来源：http://hz.nwbrower.top/gtwikzanxb.html

TS:   static f(): void {}
来源：http://hz.shanyushiyangtech.top/gtosnidtfq.html

Java: static void f() {}
来源：http://hz.zdqjudy.top/gtwuvqmrty.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.hnxiangtu.top/gtsurehsjq.html

Ruby: def self.f; end
来源：http://hz.c1oappe.top/gtxkcmkhib.html

C#:   public static void F() {}
来源：http://hz.ppjwa.cn/gtiffjmjbp.html

[G09] 接口 / 抽象类
来源：http://hz.iojbl.cn/gtkslrtfkv.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.bjfxy.top/gtsakrosbv.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zhiwuduotai.top/gtfalekpxh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.aibaodan.cn/gteksgwrgy.html

TS:   interface Shape { area(): number; }
来源：http://hz.zhoulong.xyz/gtigunfpbm.html

Java: interface Shape { double area(); }
来源：http://hz.ywan-chungtsiang.top/gtwtpwkxuy.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.gzhubu.top/gtmbpoiyvl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yj202588.top/gtfhmxadvt.html

C#:   interface IShape { double Area(); }
来源：http://hz.jinqigfzy.top/gtqqptxhai.html

[G10] 访问控制
来源：http://hz.316326.xyz/gtwillvjzj.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.shanyushiyangtech.top/gtwsokegje.html

PHP:  public / protected / private
来源：http://hz.birdmap.top/gtxxellkvb.html

JS:   #private 字段；其余公开
来源：http://hz.hywenlv.cn/gtvaxyyeft.html

TS:   public / protected / private
来源：http://hz.fzhhl.top/gthxrgfsov.html

Java: public / protected / private / 默认包级
来源：http://hz.havefunace.top/gtkkiehpoo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yj20258.top/gtkpebeowe.html

Ruby: public / protected / private
来源：http://hz.xingfuxueyuan.xyz/gtytthknws.html

C#:   public / protected / private / internal
来源：http://hz.daria6918.cn/gtzlbdkamo.html

[G11] getter / setter
来源：http://hz.vqdsnc.cn/gtixpbcfju.html

Py:   @property 与 @x.setter
来源：http://hz.dianchejie.cn/gtkgzjpsfo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yvedp.cn/gtgmgxfgar.html

JS:   get name() { return this._name; }
来源：http://hz.haohaochexian.top/gtuimslpul.html

TS:   get name(): string { return this._name; }
来源：http://hz.sweek.top/gtdpxeplcv.html

Java: public String getName() { return name; }
来源：http://hz.0kj1m.cn/gtjzdatyyd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.gzhubu.top/gtwdntliod.html

Ruby: attr_accessor :name
来源：http://hz.haohaochexian.top/gtmdkayxqc.html

C#:   public string Name { get; set; }
来源：http://hz.xylfe.cn/gtptwczlvj.html

[G12] 对象转字符串
来源：http://hz.yanxiufei.cn/gtmoyvmtjg.html

Py:   def __str__(self): return self.name
来源：http://hz.ydjk.org.cn/gtcudihljf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yanxiufei.cn/gtiwmytebc.html

JS:   toString() { return this.name; }
来源：http://hz.shanyushiyangtech.top/gthdckixag.html

TS:   toString(): string { return this.name; }
来源：http://hz.9152youxi.cn/gtxpcrsfia.html

Java: @Override public String toString() { return name; }
来源：http://hz.fengsongda.top/gtzapenkvy.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.0kj1m.cn/gtipikhbyp.html

Ruby: def to_s; @name; end
来源：http://hz.zhiwuduotai.top/gttxnrpnaq.html

C#:   public override string ToString() => Name;
来源：http://hz.iojbl.cn/gtenegdvvi.html

[G13] 判断对象类型
来源：http://hz.hfpthk.cn/gtjyidzdjj.html

Py:   isinstance(u, User)
来源：http://hz.yuxming.cn/gtzntjcmpk.html

PHP:  $u instanceof User
来源：http://hz.yueranfly.top/gtgjlqzfgo.html

JS:   u instanceof User
来源：http://hz.dianchejie.cn/gtcukyvkgu.html

TS:   u instanceof User
来源：http://hz.aizwys.cn/gtqlebbipl.html

Java: u instanceof User
来源：http://hz.ehwqpu.com/gtbvmzskvn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jqgfzy.top/gtyngtlrrc.html

Ruby: u.is_a?(User)
来源：http://hz.hnxiangtu.top/gtsmthtupk.html

C#:   u is User
来源：http://hz.tanke756.top/gtvnvutrvm.html

[G14] 数据类 / record
来源：http://hz.jlsjyb.cn/gtpcvwfycy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.meibo888.top/gttnyqdstr.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yvedp.cn/gtwmbhyqaq.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.havefunace.top/gtsvkdgols.html

TS:   type User = { name: string; age: number };
来源：http://hz.yangfankeji.com/gtjfuqzsba.html

Java: record User(String name, int age) {}
来源：http://hz.shuidangran.top/gtckkzxvep.html

Go:   type User struct { Name string; Age int }
来源：http://hz.sxryk.cn/gtsqjsytqi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.chenzaomai.com/gtnitnzmzc.html

C#:   record User(string Name, int Age);
来源：http://hz.zhaomingkeji.xyz/gtuqyjlkxv.html

[G15] 枚举
来源：http://hz.sufxvd.cn/gtqyosabpe.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.chenzaomai.com/gtmsouldam.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.hysaishi.cn/gtkgkturll.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.ehwqpu.com/gtenekiegf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.chenlongwang.top/gtlamywlqu.html

Java: enum Color { RED, GREEN }
来源：http://hz.9152youxi.cn/gtnytiyyld.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.andypj.xyz/gtzbgtcemf.html

Ruby: Color = %i[red green].freeze
来源：http://hz.cqqwz.cn/gtradlqaqi.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jlsjyb.cn/gtdidlhwpz.html

[G16] 对象转数组 / 字典
来源：http://hz.jyoumei.cn/gthnqaitiq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.tanke756.top/gtvactbvlz.html

PHP:  get_object_vars($obj);
来源：http://hz.bjfxy.top/gtuocpemwx.html

JS:   Object.entries(obj)
来源：http://hz.dashuyun.cn/gtuncbrakr.html

TS:   Object.entries(obj)
来源：http://hz.jinyuanbaomall.cn/gtbaczlyoq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.xziqi.cn/gtgxdydwlw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.zhongyouzk.top/gtprhzoxic.html

Ruby: obj.instance_variables
来源：http://hz.xinyue.icu/gtzeazbfnw.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.xinyue.icu/gtofyulaqt.html

================================================================================
来源：http://hz.ppjwa.cn/gtpaaepfok.html

H. 异常与错误处理
来源：http://hz.shzxlz.cn/gttyxxshdf.html

================================================================================
来源：http://hz.jqgfzy.top/gtwohwiuls.html

[H01] try / catch 基础
来源：http://hz.52xcode.cn/gtnrjcakhk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jyoumei.cn/gtwzpjlpdy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.dianchejie.cn/gtjqmtgdqu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.xylfe.cn/gtgwkqktqi.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.cucudq.cn/gtvqsagzht.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.sweek.top/gtrtzppeuk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.cdnleiting.top/gtzxoxnpek.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yueranfly.top/gtarddoqng.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.shanyushiyangkeji.top/gthpagttbm.html

[H02] finally / ensure 收尾
来源：http://hz.sxryk.cn/gtiprgquuu.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zhixingplan.top/gtireaxffw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.shzxlz.cn/gtarxlkzdh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.cashguo.top/gtgilnovhm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.cucudq.cn/gtdgqpgnwr.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.cheryme.top/gtbwvvfyhc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.dashuyun.cn/gtqqkyomwy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jinqigfzy.top/gtqgqfddkb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zhoulong.xyz/gtlszcaufl.html

[H03] 主动抛出异常
来源：http://hz.jinyuanbaomall.cn/gtmgxbsrkp.html

Py:   raise ValueError("错误信息")
来源：http://hz.xziqi.cn/gthjzriykv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jinqigufen.top/gtstkeruqr.html

JS:   throw new Error("错误信息");
来源：http://hz.yvedp.cn/gtmcarsjcx.html

TS:   throw new Error("错误信息");
来源：http://hz.cheryme.top/gtoyhtzkkt.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yj20258.top/gthsztdhzb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhiwuduotai.top/gtzegrkchq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.c1oappe.top/gtnrpzjovg.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.havefunace.top/gtynixhmiv.html

[H04] 自定义异常类型
来源：http://hz.jlsjyb.cn/gtpoloxlqs.html

Py:   class MyError(Exception): pass
来源：http://hz.daxiang520.top/gtpoqxwgkp.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.vqdsnc.cn/gtsoonqoam.html

JS:   class MyError extends Error {}
来源：http://hz.quarkkingdee.top/gtcnurryjz.html

TS:   class MyError extends Error {}
来源：http://hz.sweek.top/gtthldebsc.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yanxiufei.cn/gtgykkfuvi.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ppjwa.cn/gtacfgzeoi.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhiwuduotai.top/gtkobviyok.html

C#:   class MyException : Exception {}
来源：http://hz.jlsjyb.cn/gtzugdysvy.html

[H05] 捕获特定类型
来源：http://hz.yonumen.top/gtafiebuym.html

Py:   except ValueError as e:
来源：http://hz.hfpthk.cn/gtowpfywpq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.gotoacloud.top/gtspxmoxwc.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zhiwuduotai.top/gtdxneuwdo.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.nanxuanxn.top/gtjigmqmrx.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yj20258.top/gthtuplicj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hysaishi.cn/gtkdcihzvv.html

Ruby: rescue ArgumentError => e
来源：http://hz.zycfv.cn/gtflifpmse.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhixingplan.top/gtijzjjulm.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yongpay.top/gtftvfbdmh.html

Py:   value = d.get("k") or default
来源：http://hz.sufxvd.cn/gtrcsnvjuy.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.wangdashe.top/gtnywmitsm.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.gotoacloud.top/gtcplrpxzr.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.vqdsnc.cn/gttavaqmhl.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.fengsongda.top/gtvnqcekaq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.nanxinkj.top/gtsdhnenap.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jyoumei.cn/gtnmkusxcj.html

C#:   obj?.A?.B ?? default
来源：http://hz.smart0.xyz/gtbmiphsml.html

[H07] 断言
来源：http://hz.meibo888.top/gtxkokysep.html

Py:   assert x > 0, "必须为正"
来源：http://hz.quarkkingdee.top/gtsttwlthf.html

PHP:  assert($x > 0);
来源：http://hz.smart0.xyz/gtxvtealbl.html

JS:   console.assert(x > 0);
来源：http://hz.fengsongda.top/gtntvfqtmr.html

TS:   console.assert(x > 0);
来源：http://hz.zhongyouzk.top/gtultrhafo.html

Java: assert x > 0 : "必须为正";
来源：http://hz.aizwys.cn/gtafeyqvjg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yj202588.top/gtyvlveduj.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yuxming.cn/gtpqrqrevu.html

C#:   Debug.Assert(x > 0);
来源：http://hz.hnxiangtu.top/gtubnbsvge.html

[H08] 获取错误信息与堆栈
来源：http://hz.yonumen.top/gtccngedrs.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jinqigufen.top/gttlnyeuez.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.guowangkeji.top/gtldbmvrmz.html

JS:   e.message;  e.stack
来源：http://hz.52xcode.cn/gtrqoehlnw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jinghuilouyu.cn/gtxtzzdsgi.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.tian-w.cn/gtgajafaob.html

Go:   err.Error()
来源：http://hz.shuidangran.top/gtseqmkbaf.html

Ruby: e.message;  e.backtrace
来源：http://hz.snrcjt.cn/gtgxpioygj.html

C#:   e.Message;  e.StackTrace
来源：http://hz.bjfxy.top/gtchbvnohw.html

[H09] 带错误码的异常
来源：http://hz.jqgufenzy.top/gtanwytolw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.c1oappe.top/gtnlvpphwn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yueranfly.top/gtzwbvuszj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.hysaishi.cn/gtkohzksor.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jlsjyb.cn/gtypatsepu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.0kj1m.cn/gtdrqpwlco.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.gogol.net.cn/gtnxpxsafq.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.ybcxt.top/gttjykdcyb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhongyouzk.top/gtsuzrlqwh.html

[H10] 资源自动释放
来源：http://hz.svipenyu.cn/gthecedwdy.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.shuidangran.top/gtxhzzmrjr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.hnxiangtu.top/gtgafrvfoh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jinqigfzy.top/gtqqnodrjl.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.nwbrower.top/gtrqkzndhg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zhixingplan.top/gtpvjudfhd.html

Go:   defer f.Close()
来源：http://hz.gotoacloud.top/gtxoowchis.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.aizwys.cn/gtvamvybwp.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.chenjidiqi.icu/gtkwoommct.html

================================================================================
来源：http://hz.hfpthk.cn/gtelvjvoqt.html

I. 正则表达式
来源：http://hz.52xcode.cn/gtpyrnpvca.html

================================================================================
来源：http://hz.iojbl.cn/gtduybbtiu.html

[I01] 判断是否匹配
来源：http://hz.kuanghao11.cn/gtnqgeezmg.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jinqigfzy.top/gtfbmxhaxt.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zhoulong.xyz/gtomqwwmuh.html

JS:   /\d+/.test(s)
来源：http://hz.tianlin.xyz/gtxqfumbue.html

TS:   /\d+/.test(s)
来源：http://hz.cdnleiting.top/gtlaojihcy.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jlsjyb.cn/gtvcqzrzns.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zhiwuduotai.top/gtefbwvqfc.html

Ruby: s.match?(/\d+/)
来源：http://hz.tian-w.cn/gtprqzlati.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.daxiang520.top/gttfxbozqt.html

[I02] 提取所有匹配
来源：http://hz.jlsjyb.cn/gtwiobhvwi.html

Py:   re.findall(r"\d+", s)
来源：http://hz.iojbl.cn/gtwsqidexm.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.xingfuxueyuan.xyz/gtxgberzsd.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.bjfxy.top/gtfgvikdkm.html

TS:   s.match(/\d+/g)
来源：http://hz.dianchejie.cn/gtyxeqxscg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.daria6918.cn/gtqhlidjyo.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.cashguo.top/gtdgqtoozb.html

Ruby: s.scan(/\d+/)
来源：http://hz.316326.xyz/gtxletcpoa.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.vqdsnc.cn/gtzukrdhro.html

[I03] 提取捕获分组
来源：http://hz.zhiwuduotai.top/gthqismmud.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hammf.cn/gtttrnixkh.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.nanxinkj.top/gthhlkihlw.html


<!-- 参考信息 -->