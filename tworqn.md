代发 wailian999

[F09] 获取文件大小
来源：http://hz.chenzaomai.com/gtykpsgeaj.html

Py:   os.path.getsize("a.txt")
来源：http://hz.vqdsnc.cn/gtmzfnpvrw.html

PHP:  filesize("a.txt");
来源：http://hz.tianlin.xyz/gttgsryxqb.html

JS:   fs.statSync("a.txt").size
来源：http://hz.aibaodan.cn/gtkmlqcopj.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zhoulong.xyz/gtpxewzryw.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.0kj1m.cn/gtlzsiyhje.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.ehwqpu.com/gtydezmwmd.html

Ruby: File.size("a.txt")
来源：http://hz.xuetiantiany.cn/gtrmhjolcs.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.daria6918.cn/gtwfsqzhps.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yj20258.top/gthahoyjgp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.chenjidiqi.icu/gtpyayjhsj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.nanxuanxn.top/gtcqulmgrn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yj20258.top/gtjiefhyzp.html

TS:   path.extname("a.txt")
来源：http://hz.shanyushiyangtech.top/gtfqithjuq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.dianchejie.cn/gtzphehdqm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.sweek.top/gttpzbqcar.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jianghu66.top/gtdpzltayn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.nwbrower.top/gttcktreec.html

[F11] 复制与移动文件
来源：http://hz.ybcxt.top/gtomqcwiup.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.iojbl.cn/gtwyovoncn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.dashuyun.cn/gtafufhety.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yvedp.cn/gtfroluddi.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zdqjudy.top/gtqaatngax.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.shanyushiyangkeji.top/gtlkdmcpua.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.nwbrower.top/gtcrzmwgkk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.gogol.net.cn/gtcvnrmkkx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.hnqzz.top/gtyejrgzmy.html

[F12] CSV 读写
来源：http://hz.gaohongyu789.top/gtcenwtuap.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jlsjyb.cn/gtlfvggudk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.xinyue.icu/gtpgbekspq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.cheryme.top/gtcoxdsyvh.html

TS:   // 同上
来源：http://hz.gogol.net.cn/gtvwzmytrw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.sysykeji.top/gthcgppial.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.sxryk.cn/gtysqomggq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.xuanzx.com/gthfbowrhf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yvedp.cn/gtjbxxhyrz.html

================================================================================
来源：http://hz.cqqwz.cn/gtyildzjtf.html

G. 面向对象
来源：http://hz.xingfuxueyuan.xyz/gtqfebewgl.html

================================================================================
来源：http://hz.pycfn.com/gttpxbniwe.html

[G01] 定义类
来源：http://hz.fengsongda.top/gtmfwrjctj.html

Py:   class User: pass
来源：http://hz.yvedp.cn/gtwhtfmryx.html

PHP:  class User {}
来源：http://hz.yj20258888.top/gtfozlzgzv.html

JS:   class User {}
来源：http://hz.jqgufenzy.top/gtyjtdmbsv.html

TS:   class User { name: string = ""; }
来源：http://hz.shangyingyoupin.top/gtjyezhusa.html

Java: class User {}
来源：http://hz.cheryme.top/gtjnrepzhm.html

Go:   type User struct { Name string }
来源：http://hz.hywenlv.cn/gtwbxmdnvs.html

Ruby: class User; end
来源：http://hz.shanyushiyangtech.top/gtrftkyyvx.html

C#:   class User {}
来源：http://hz.chenlongwang.top/gtvzemftfe.html

[G02] 构造函数
来源：http://hz.hysaishi.cn/gtnmdzbapm.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yonumen.top/gtngwqmptp.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zhijiandao.cn/gtvpolizqq.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.xinyue.icu/gtoarnidaw.html

TS:   constructor(public name: string) {}
来源：http://hz.tianlin.xyz/gtdxsvdnag.html

Java: User(String name) { this.name = name; }
来源：http://hz.yonumen.top/gtnnrpeotn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jinqigufen.top/gtfytxtaor.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.sysykeji.top/gtseoxrkod.html

C#:   public User(string name) { Name = name; }
来源：http://hz.cheryme.top/gtqthimhom.html

[G03] 实例属性
来源：http://hz.xingfuxueyuan.xyz/gtmugqsbox.html

Py:   self.name = "x"
来源：http://hz.wangdashe.top/gtfkgdjukm.html

PHP:  public string $name = "x";
来源：http://hz.zhoulong.xyz/gttrjnbjxp.html

JS:   this.name = "x";
来源：http://hz.cucudq.cn/gtmvykotpp.html

TS:   name: string = "x";
来源：http://hz.chenzaomai.com/gtbdsrbvwu.html

Java: private String name;
来源：http://hz.jinyuanbaomall.cn/gtgucjcmyi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hywenlv.cn/gtiksbzsqx.html

Ruby: @name = "x"
来源：http://hz.gogol.net.cn/gtvcvomahp.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yuxming.cn/gthcfnjtar.html

[G04] 定义方法
来源：http://hz.redwolf501.top/gtzfsihlas.html

Py:   def greet(self): return self.name
来源：http://hz.daxiang520.top/gttelesufg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.316326.xyz/gtgepzrhea.html

JS:   greet() { return this.name; }
来源：http://hz.shzxlz.cn/gtmxeujord.html

TS:   greet(): string { return this.name; }
来源：http://hz.zhoulong.xyz/gthnfdzyox.html

Java: String greet() { return name; }
来源：http://hz.snrcjt.cn/gtwmlpgvud.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.aizwys.cn/gtybyjpcoy.html

Ruby: def greet; @name; end
来源：http://hz.dianchejie.cn/gtmdffjwjp.html

C#:   public string Greet() => Name;
来源：http://hz.cucudq.cn/gtohbffwol.html

[G05] 继承
来源：http://hz.guannengcc.top/gtrxzashbv.html

Py:   class Admin(User): pass
来源：http://hz.zycfv.cn/gtmwfzpigm.html

PHP:  class Admin extends User {}
来源：http://hz.zhengqikj.top/gtqjmzqomd.html

JS:   class Admin extends User {}
来源：http://hz.zhiwuduotai.top/gtdwybxlrd.html

TS:   class Admin extends User {}
来源：http://hz.hywenlv.cn/gtoqmtccyp.html

Java: class Admin extends User {}
来源：http://hz.mhx1999.top/gtdcrbhdhe.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.chenjidiqi.icu/gtwdlpxxam.html

Ruby: class Admin < User; end
来源：http://hz.snrcjt.cn/gtikxxeylx.html

C#:   class Admin : User {}
来源：http://hz.mhx1999.top/gtsriboxob.html

[G06] 重写方法
来源：http://hz.jiagoushi.top/gtwwoltvbv.html

Py:   def greet(self): return "admin"
来源：http://hz.xziqi.cn/gtvadfhpzu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ybcxt.top/gttjesnkiv.html

JS:   greet() { return "admin"; }
来源：http://hz.ehwqpu.com/gtqpdmkpio.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hnxiangtu.top/gtjzxooroj.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hywenlv.cn/gtdfxxhgro.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.cqqwz.cn/gtvucsoixh.html

Ruby: def greet; "admin"; end
来源：http://hz.zhixingplan.top/gtlfmfxmuv.html

C#:   public override string Greet() => "admin";
来源：http://hz.shuidangran.top/gtuodwyxbg.html

[G07] 调用父类方法
来源：http://hz.316326.xyz/gtxeokqgkd.html

Py:   super().greet()
来源：http://hz.cashguo.top/gtkfdejlkb.html

PHP:  parent::greet();
来源：http://hz.jinyuanbaomall.cn/gtynmgkctm.html

JS:   super.greet();
来源：http://hz.0kj1m.cn/gtirfjxscf.html

TS:   super.greet();
来源：http://hz.hnqzz.top/gtpsntgqrw.html

Java: super.greet();
来源：http://hz.smart0.xyz/gtnmfcauej.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.xuetiantiany.cn/gtiwuuvwzs.html

Ruby: super
来源：http://hz.yongpay.top/gtrqilxhcs.html

C#:   base.Greet();
来源：http://hz.ydjk.org.cn/gtahxfmswm.html

[G08] 静态方法与属性
来源：http://hz.yueranfly.top/gtqgyhaors.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.tian-w.cn/gtmrwooatt.html

PHP:  public static function f() {}
来源：http://hz.andypj.xyz/gtsrrwqrzo.html

JS:   static f() {}
来源：http://hz.gaohongyu789.top/gtnmosoget.html

TS:   static f(): void {}
来源：http://hz.birdmap.top/gtyznkqhnb.html

Java: static void f() {}
来源：http://hz.jinqigfzy.top/gtpgcoucss.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.gogol.net.cn/gtiumlnluq.html

Ruby: def self.f; end
来源：http://hz.xuetiantiany.cn/gtkniwtkmn.html

C#:   public static void F() {}
来源：http://hz.birdmap.top/gtphzjtlyu.html

[G09] 接口 / 抽象类
来源：http://hz.haohaochexian.top/gtmoeuplth.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.hongshengwenyu.top/gtingowpau.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.cheryme.top/gtctlzjjvh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.hammf.cn/gtxvtlamhm.html

TS:   interface Shape { area(): number; }
来源：http://hz.zycfv.cn/gtuglmsgqn.html

Java: interface Shape { double area(); }
来源：http://hz.zhongyouzk.top/gtjtucform.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.xuetiantiany.cn/gtckyhytdn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yonumen.top/gtbqrcauqc.html

C#:   interface IShape { double Area(); }
来源：http://hz.svipenyu.cn/gtjwlycuhh.html

[G10] 访问控制
来源：http://hz.zhijiandao.cn/gtglnonxwe.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.aibaodan.cn/gtyquspbqu.html

PHP:  public / protected / private
来源：http://hz.wangdashe.top/gthuslkfcv.html

JS:   #private 字段；其余公开
来源：http://hz.cqqwz.cn/gtpkwngtmx.html

TS:   public / protected / private
来源：http://hz.ivvv.top/gtlswdgodw.html

Java: public / protected / private / 默认包级
来源：http://hz.fengsongda.top/gtjlxaagfa.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.pycfn.com/gtxvadzrsg.html

Ruby: public / protected / private
来源：http://hz.zhixingplan.top/gttxokqimr.html

C#:   public / protected / private / internal
来源：http://hz.shanyushiyangkeji.top/gtigzyzeep.html

[G11] getter / setter
来源：http://hz.0kj1m.cn/gtnwhqqnwg.html

Py:   @property 与 @x.setter
来源：http://hz.ivvv.top/gtasyftdwg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jinghuilouyu.cn/gtdbfvybjo.html

JS:   get name() { return this._name; }
来源：http://hz.andypj.xyz/gtivzinatw.html

TS:   get name(): string { return this._name; }
来源：http://hz.ydjk.org.cn/gtlmjorpij.html

Java: public String getName() { return name; }
来源：http://hz.cashguo.top/gtbgemyfzq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.wangdashe.top/gtqamltuog.html

Ruby: attr_accessor :name
来源：http://hz.yuxming.cn/gtsbcgaqrl.html

C#:   public string Name { get; set; }
来源：http://hz.aibaodan.cn/gtvjxdvmil.html

[G12] 对象转字符串
来源：http://hz.yangfankeji.com/gtrezjqpur.html

Py:   def __str__(self): return self.name
来源：http://hz.hysaishi.cn/gtsyjotsfq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yonumen.top/gtwkmoavfc.html

JS:   toString() { return this.name; }
来源：http://hz.shanyushiyangkeji.top/gteamsrbho.html

TS:   toString(): string { return this.name; }
来源：http://hz.xuetiantiany.cn/gthytxztbz.html

Java: @Override public String toString() { return name; }
来源：http://hz.daria6918.cn/gttzzvrswv.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.vqdsnc.cn/gtdsvshmqi.html

Ruby: def to_s; @name; end
来源：http://hz.jqgufenzy.top/gtcsfxlatq.html

C#:   public override string ToString() => Name;
来源：http://hz.cqqwz.cn/gtorgidkzb.html

[G13] 判断对象类型
来源：http://hz.ybcxt.top/gtbzdhuukn.html

Py:   isinstance(u, User)
来源：http://hz.feifeiyinyue.top/gtbywgaska.html

PHP:  $u instanceof User
来源：http://hz.shanyushiyangkeji.top/gtujtqrwaw.html

JS:   u instanceof User
来源：http://hz.ydzc1.top/gtvpsrkfwf.html

TS:   u instanceof User
来源：http://hz.meibo888.top/gtetemizmf.html

Java: u instanceof User
来源：http://hz.yueranfly.top/gtrwrevvtu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.cdnleiting.top/gtiogjrock.html

Ruby: u.is_a?(User)
来源：http://hz.kuanghao11.cn/gtznxmrxah.html

C#:   u is User
来源：http://hz.jyoumei.cn/gtxvxlnugq.html

[G14] 数据类 / record
来源：http://hz.gotoacloud.top/gtbywopsyw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.ybcxt.top/gtqvpalkya.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.hammf.cn/gtpzdwoint.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.ivvv.top/gtvglhbboa.html

TS:   type User = { name: string; age: number };
来源：http://hz.ywan-chungtsiang.top/gtkaosjdkn.html

Java: record User(String name, int age) {}
来源：http://hz.52xcode.cn/gtnqhietah.html

Go:   type User struct { Name string; Age int }
来源：http://hz.sysykeji.top/gtpngiajwm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.nwbrower.top/gthndoanhj.html

C#:   record User(string Name, int Age);
来源：http://hz.zhaomingkeji.xyz/gtrihsvboq.html

[G15] 枚举
来源：http://hz.jinyuanbaomall.cn/gtjwjdnrpz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.feifeiyinyue.top/gtzitotoed.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ehwqpu.com/gtgtkneujc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.ybcxt.top/gtwphbfrds.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.0kj1m.cn/gtttotbcyz.html

Java: enum Color { RED, GREEN }
来源：http://hz.yonumen.top/gtjpxdszvn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yj202588.top/gtrefvtphl.html

Ruby: Color = %i[red green].freeze
来源：http://hz.tianlin.xyz/gtdpdgfygc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.wangdashe.top/gtoequvaqo.html

[G16] 对象转数组 / 字典
来源：http://hz.shanyushiyangtech.top/gtmcifqpby.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.guowangkeji.top/gtyqsruase.html

PHP:  get_object_vars($obj);
来源：http://hz.cqqwz.cn/gtuiupqiyj.html

JS:   Object.entries(obj)
来源：http://hz.tanke756.top/gtvjgifnyj.html

TS:   Object.entries(obj)
来源：http://hz.guannengcc.top/gtjalswbkh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yuxming.cn/gtexezezmv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.cashguo.top/gtrxqligmc.html

Ruby: obj.instance_variables
来源：http://hz.yueranfly.top/gtbnzugvua.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.xuetiantiany.cn/gtelqkzqur.html

================================================================================
来源：http://hz.yj202588.top/gtmkbzyads.html

H. 异常与错误处理
来源：http://hz.ydzc1.top/gtnlyufgbt.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtekyjxhnt.html

[H01] try / catch 基础
来源：http://hz.0kj1m.cn/gtaihvyiyn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.ehwqpu.com/gtrdhbiozt.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.gzhubu.top/gtuoppqtjz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.xuetiantiany.cn/gtluiityum.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jqgufenzy.top/gtydombxzy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jinqigufen.top/gttrdzyfyr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.chenjidiqi.icu/gtjlrnzjzm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yueranfly.top/gtmrgvpbqb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zycfv.cn/gtyivmgnvu.html

[H02] finally / ensure 收尾
来源：http://hz.nwbrower.top/gtzbrulbgf.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yongpay.top/gtzymxxozw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.iojbl.cn/gtdhymrkhc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jinqigfzy.top/gtqlggvddq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhiwuduotai.top/gtqlqijbfl.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.dashuyun.cn/gttitswdhq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ivvv.top/gtdcbnztwx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.c1oappe.top/gtsnuahtsc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.redwolf501.top/gtkglmexod.html

[H03] 主动抛出异常
来源：http://hz.jyoumei.cn/gtaaljfkfa.html

Py:   raise ValueError("错误信息")
来源：http://hz.yueranfly.top/gtfyylnjja.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.tianlin.xyz/gtnjjotppd.html

JS:   throw new Error("错误信息");
来源：http://hz.9152youxi.cn/gtqejyevyr.html

TS:   throw new Error("错误信息");
来源：http://hz.nanxinkj.top/gtgulzlymy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jinqigfzy.top/gtptkhfehc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hongshengwenyu.top/gthpqoocjg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zhixingplan.top/gtxlygpsld.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.ehwqpu.com/gtpbgjutpi.html

[H04] 自定义异常类型
来源：http://hz.zhoulong.xyz/gtlwsczkvu.html

Py:   class MyError(Exception): pass
来源：http://hz.chenjidiqi.icu/gtdfroueqw.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.ydjk.org.cn/gtazfwdwtz.html

JS:   class MyError extends Error {}
来源：http://hz.ehwqpu.com/gtodeepans.html

TS:   class MyError extends Error {}
来源：http://hz.havefunace.top/gtwurdenls.html

Java: class MyException extends RuntimeException {}
来源：http://hz.c1oappe.top/gtspqkcekb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jianghu66.top/gtxongqdpm.html

Ruby: class MyError < StandardError; end
来源：http://hz.hfpthk.cn/gtsgnrybzw.html

C#:   class MyException : Exception {}
来源：http://hz.aibaodan.cn/gteijjyuve.html

[H05] 捕获特定类型
来源：http://hz.yj202588.top/gtpmuulroj.html

Py:   except ValueError as e:
来源：http://hz.pengpengdd.cyou/gtgjhzlalx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.wangshuangyany.cn/gtehsuxgsy.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.ydjk.org.cn/gttrjdtjjl.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.chenjidiqi.icu/gtixcvqgil.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.xingfuxueyuan.xyz/gtoanqvjds.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.smart0.xyz/gtuoxdznyq.html

Ruby: rescue ArgumentError => e
来源：http://hz.sufxvd.cn/gtgmfaoqlp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.52xcode.cn/gtboyxcgwd.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yj202588.top/gtxbiindqo.html

Py:   value = d.get("k") or default
来源：http://hz.pengpengdd.cyou/gtrkvhhnli.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yuxming.cn/gtdrhznrbv.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.daxiang520.top/gtmgijlgug.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jqgfzy.top/gtofavxegf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.mhx1999.top/gtorhuydca.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jinghuilouyu.cn/gtmncchfgi.html

Ruby: d&.dig(:a, :b)
来源：http://hz.ehwqpu.com/gtviyuqdhy.html

C#:   obj?.A?.B ?? default
来源：http://hz.xuetiantiany.cn/gtykbryhmz.html

[H07] 断言
来源：http://hz.yuxming.cn/gtydjhfjos.html

Py:   assert x > 0, "必须为正"
来源：http://hz.hnqzz.top/gtdkpmikjq.html

PHP:  assert($x > 0);
来源：http://hz.yuanzhike.top/gtntdbrxxb.html

JS:   console.assert(x > 0);
来源：http://hz.sweek.top/gtczxdtngi.html

TS:   console.assert(x > 0);
来源：http://hz.jianghu66.top/gtrqdqkxma.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jinqigufen.top/gtxboouixk.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yj202588.top/gtpxylxalp.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhiwuduotai.top/gtghxjcrpl.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jianghu66.top/gtpcfldkku.html

[H08] 获取错误信息与堆栈
来源：http://hz.ywan-chungtsiang.top/gtdyovrxob.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.xinyue.icu/gtdxaskprk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.chenzaomai.com/gtayyswzgg.html

JS:   e.message;  e.stack
来源：http://hz.0kj1m.cn/gtmoqqmxvv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zdqjudy.top/gtqmkjwpaw.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.shanyushiyangkeji.top/gtxwrirhhe.html

Go:   err.Error()
来源：http://hz.daxiang520.top/gtzvwgypsm.html

Ruby: e.message;  e.backtrace
来源：http://hz.iojbl.cn/gtztcdtxne.html

C#:   e.Message;  e.StackTrace
来源：http://hz.chenzaomai.com/gtjyvorlrf.html

[H09] 带错误码的异常
来源：http://hz.jinghuilouyu.cn/gtjuagfnyf.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zhiwuduotai.top/gtkrjfdjgp.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.gotoacloud.top/gtwrbnktuq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.mhx1999.top/gtphzuqpjx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.gaohongyu789.top/gtadwohnak.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.xuanzx.com/gtykgdhgux.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.shangyingyoupin.top/gtrzdofabr.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.nanxuanxn.top/gtemdroqvi.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.kuanghao11.cn/gtpuscgxpu.html

[H10] 资源自动释放
来源：http://hz.zhoulong.xyz/gtphurxkco.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.snrcjt.cn/gtkpfqjzwe.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.xingfuxueyuan.xyz/gtdozwkidh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.nanxuanxn.top/gtzcfwwrpp.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.birdmap.top/gtdyclpanz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.sweek.top/gtrxzjezzg.html

Go:   defer f.Close()
来源：http://hz.iojbl.cn/gtpkkmcyed.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.smart0.xyz/gtelydrhcn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ybcxt.top/gtasfnphek.html

================================================================================
来源：http://hz.jlsjyb.cn/gtgispxfnc.html

I. 正则表达式
来源：http://hz.wangshuangyany.cn/gtjldbwkkb.html

================================================================================
来源：http://hz.316326.xyz/gtpyjuhpmq.html

[I01] 判断是否匹配
来源：http://hz.snrcjt.cn/gtfoltnarg.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.ydzc1.top/gtjpdscudl.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.redwolf501.top/gtfsxbnvha.html

JS:   /\d+/.test(s)
来源：http://hz.cucudq.cn/gtbddmebtd.html

TS:   /\d+/.test(s)
来源：http://hz.52xcode.cn/gtwxpsouki.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.gaohongyu789.top/gtwjixohjh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.cashguo.top/gtlvogjbfp.html

Ruby: s.match?(/\d+/)
来源：http://hz.redwolf501.top/gtdnxlhxfs.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yonumen.top/gtfjojuhkt.html

[I02] 提取所有匹配
来源：http://hz.svipenyu.cn/gtccszbsmq.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jinyuanbaomall.cn/gtwmuhtlpn.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.c1oappe.top/gtrdodxhmq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhijiandao.cn/gtuzknzpcr.html

TS:   s.match(/\d+/g)
来源：http://hz.smart0.xyz/gtoqwavllj.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.shzxlz.cn/gtgfoevcvf.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hongshengwenyu.top/gtkgswahtc.html

Ruby: s.scan(/\d+/)
来源：http://hz.ivvv.top/gtwkpkmlck.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.svipenyu.cn/gtbrfhifvs.html

[I03] 提取捕获分组
来源：http://hz.tanke756.top/gtndbfuomn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.nanxinkj.top/gtcgcigskf.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.wangshuangyany.cn/gtloxhdtmr.html


<!-- 参考信息 -->