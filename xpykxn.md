代发 wailian999

[F09] 获取文件大小
来源：http://hz.xziqi.cn/gtycwetsjr.html

Py:   os.path.getsize("a.txt")
来源：http://hz.fengsongda.top/gtjanrdesc.html

PHP:  filesize("a.txt");
来源：http://hz.yueranfly.top/gtjwtydpsw.html

JS:   fs.statSync("a.txt").size
来源：http://hz.0kj1m.cn/gtlforhcdj.html

TS:   fs.statSync("a.txt").size
来源：http://hz.guowangkeji.top/gttsfsmcbk.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.hammf.cn/gtlxclwxsj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.dianchejie.cn/gtvaucxgss.html

Ruby: File.size("a.txt")
来源：http://hz.cucudq.cn/gtlqbwxehe.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.316326.xyz/gttmsappej.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.cheryme.top/gtqamuwwdu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtnnbakjid.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.guowangkeji.top/gtwaffanjv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yvedp.cn/gtqjwxgsaj.html

TS:   path.extname("a.txt")
来源：http://hz.zhiwuduotai.top/gtbevwspwr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.feifeiyinyue.top/gtyxhszoyi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.gotoacloud.top/gtwomolgka.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jqgfzy.top/gtsrlwjxbu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.guannengcc.top/gtjpfuevxb.html

[F11] 复制与移动文件
来源：http://hz.cashguo.top/gtwsjfmfxr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.cqqwz.cn/gtoaaenvot.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jinyuanbaomall.cn/gtjawrjwxb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yj20258.top/gtciatpgbk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yuanzhike.top/gtclrneeml.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.shanyushiyangtech.top/gtwrvzlhzp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.cqqwz.cn/gtxtgshhxg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.shangyingyoupin.top/gtvtycaiwl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.9152youxi.cn/gtkjgwgxsw.html

[F12] CSV 读写
来源：http://hz.feifeiyinyue.top/gtbduyozbx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jinqigfzy.top/gthqvlaotf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hongshengwenyu.top/gthydjyaxs.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.fzhhl.top/gtnojthsam.html

TS:   // 同上
来源：http://hz.guowangkeji.top/gtfmycudpk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yuanzhike.top/gtktqitdjb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yj202588.top/gtdqfcnbzk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.shangyingyoupin.top/gthcyfcfkw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jianghu66.top/gtwqlfkzmj.html

================================================================================
来源：http://hz.iojbl.cn/gthazcmdto.html

G. 面向对象
来源：http://hz.pycfn.com/gtddxabquw.html

================================================================================
来源：http://hz.zhixingplan.top/gtkmxmhkke.html

[G01] 定义类
来源：http://hz.bjfxy.top/gtyzkktjap.html

Py:   class User: pass
来源：http://hz.hnxiangtu.top/gtxsrgnuwg.html

PHP:  class User {}
来源：http://hz.chenjidiqi.icu/gtqjpemhbt.html

JS:   class User {}
来源：http://hz.smart0.xyz/gtjzeuykbn.html

TS:   class User { name: string = ""; }
来源：http://hz.dashuyun.cn/gtqmuebkbx.html

Java: class User {}
来源：http://hz.daria6918.cn/gtwwcskzkw.html

Go:   type User struct { Name string }
来源：http://hz.havefunace.top/gtbkyrncdp.html

Ruby: class User; end
来源：http://hz.jyoumei.cn/gtulybfzvv.html

C#:   class User {}
来源：http://hz.xylfe.cn/gtdmeynhrh.html

[G02] 构造函数
来源：http://hz.zhixingplan.top/gtnbkudboe.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jqgfzy.top/gtweygdpom.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.sufxvd.cn/gteosxtfwh.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.fengsongda.top/gtbdvceqgp.html

TS:   constructor(public name: string) {}
来源：http://hz.hywenlv.cn/gtlhhfyope.html

Java: User(String name) { this.name = name; }
来源：http://hz.sufxvd.cn/gtjxplcluv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.52xcode.cn/gtntvsiypf.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.andypj.xyz/gtzwvgizue.html

C#:   public User(string name) { Name = name; }
来源：http://hz.havefunace.top/gtymymrooe.html

[G03] 实例属性
来源：http://hz.gotoacloud.top/gtuoosxccy.html

Py:   self.name = "x"
来源：http://hz.fzhhl.top/gtdjtlxgds.html

PHP:  public string $name = "x";
来源：http://hz.zhijiandao.cn/gtvuljjufw.html

JS:   this.name = "x";
来源：http://hz.quarkkingdee.top/gtaseamgxb.html

TS:   name: string = "x";
来源：http://hz.zhengqikj.top/gtlnlczxuy.html

Java: private String name;
来源：http://hz.feifeiyinyue.top/gtkzopvvdi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.cashguo.top/gtrrkdekkc.html

Ruby: @name = "x"
来源：http://hz.guowangkeji.top/gtfxyctemu.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.shangyingyoupin.top/gtnywqdpaa.html

[G04] 定义方法
来源：http://hz.jlsjyb.cn/gtglymvaia.html

Py:   def greet(self): return self.name
来源：http://hz.cheryme.top/gtxgtmteuw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.sysykeji.top/gtquslxukc.html

JS:   greet() { return this.name; }
来源：http://hz.zhiwuduotai.top/gtqajayayh.html

TS:   greet(): string { return this.name; }
来源：http://hz.yj20258.top/gttcfqosec.html

Java: String greet() { return name; }
来源：http://hz.bjfxy.top/gtqhgantmj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hfpthk.cn/gtdrbwwrtk.html

Ruby: def greet; @name; end
来源：http://hz.xinyue.icu/gtiufvzmqy.html

C#:   public string Greet() => Name;
来源：http://hz.meibo888.top/gtglxqbpxr.html

[G05] 继承
来源：http://hz.yj20258.top/gtivllgedb.html

Py:   class Admin(User): pass
来源：http://hz.quarkkingdee.top/gttqpuwung.html

PHP:  class Admin extends User {}
来源：http://hz.zhiwuduotai.top/gtxnyxykka.html

JS:   class Admin extends User {}
来源：http://hz.redwolf501.top/gtebyqxybd.html

TS:   class Admin extends User {}
来源：http://hz.9152youxi.cn/gtzkzwoevg.html

Java: class Admin extends User {}
来源：http://hz.hongshengwenyu.top/gtjzlmbamc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.andypj.xyz/gtrcriyftd.html

Ruby: class Admin < User; end
来源：http://hz.jianghu66.top/gtlplkgmfk.html

C#:   class Admin : User {}
来源：http://hz.zhoulong.xyz/gtbwclyssh.html

[G06] 重写方法
来源：http://hz.jiagoushi.top/gtemsefjxg.html

Py:   def greet(self): return "admin"
来源：http://hz.pycfn.com/gtfmyulbur.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jinghuilouyu.cn/gtgkvwhyta.html

JS:   greet() { return "admin"; }
来源：http://hz.birdmap.top/gtxchtdliy.html

TS:   greet(): string { return "admin"; }
来源：http://hz.shanyushiyangtech.top/gtfgraffgi.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jlsjyb.cn/gtnbqbafth.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.guannengcc.top/gtpxrszmmt.html

Ruby: def greet; "admin"; end
来源：http://hz.zhaomingkeji.xyz/gtddvlaxln.html

C#:   public override string Greet() => "admin";
来源：http://hz.shanyushiyangtech.top/gtyjfgfkrp.html

[G07] 调用父类方法
来源：http://hz.jinghuilouyu.cn/gtczajgkyz.html

Py:   super().greet()
来源：http://hz.hysaishi.cn/gtfdkvekii.html

PHP:  parent::greet();
来源：http://hz.yonumen.top/gtejwffawp.html

JS:   super.greet();
来源：http://hz.jqgfzy.top/gthfohpcfm.html

TS:   super.greet();
来源：http://hz.zhijiandao.cn/gtzcumltno.html

Java: super.greet();
来源：http://hz.smart0.xyz/gtriwqnfbw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.dashuyun.cn/gtcgkgeovo.html

Ruby: super
来源：http://hz.snrcjt.cn/gtszbbikui.html

C#:   base.Greet();
来源：http://hz.sufxvd.cn/gtomyfnhtq.html

[G08] 静态方法与属性
来源：http://hz.zhaomingkeji.xyz/gtnzkrjdyu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.sxryk.cn/gtjycbefmm.html

PHP:  public static function f() {}
来源：http://hz.cheryme.top/gtdmstnkso.html

JS:   static f() {}
来源：http://hz.yonumen.top/gtwomzfiug.html

TS:   static f(): void {}
来源：http://hz.zhixingplan.top/gtyzyizylk.html

Java: static void f() {}
来源：http://hz.andypj.xyz/gtqtruyjch.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.c1oappe.top/gtfbetxvie.html

Ruby: def self.f; end
来源：http://hz.sysykeji.top/gtzbkfezql.html

C#:   public static void F() {}
来源：http://hz.ppjwa.cn/gtcnyqzzcf.html

[G09] 接口 / 抽象类
来源：http://hz.xuanzx.com/gtrtrhnshj.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.hfpthk.cn/gtmtfcmtxo.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.wangshuangyany.cn/gtnwftgkit.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.xuetiantiany.cn/gtwfgnukbp.html

TS:   interface Shape { area(): number; }
来源：http://hz.haohaochexian.top/gtimuzigwp.html

Java: interface Shape { double area(); }
来源：http://hz.hywenlv.cn/gtcllzfdzi.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.cucudq.cn/gtcyjdsdbu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.shzxlz.cn/gtlbdotzkn.html

C#:   interface IShape { double Area(); }
来源：http://hz.pycfn.com/gtzbvzhjtb.html

[G10] 访问控制
来源：http://hz.xuetiantiany.cn/gttrprvort.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.cdnleiting.top/gtkoodwfvt.html

PHP:  public / protected / private
来源：http://hz.xinyue.icu/gtermzgxbe.html

JS:   #private 字段；其余公开
来源：http://hz.sweek.top/gtmosthuud.html

TS:   public / protected / private
来源：http://hz.dianchejie.cn/gtqyfhgznj.html

Java: public / protected / private / 默认包级
来源：http://hz.yuanzhike.top/gtqfqcpvib.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.52xcode.cn/gtuujzabup.html

Ruby: public / protected / private
来源：http://hz.zhixingplan.top/gtvvzbmcio.html

C#:   public / protected / private / internal
来源：http://hz.gzhubu.top/gtchtmfwjf.html

[G11] getter / setter
来源：http://hz.yangfankeji.com/gtmrkywcvk.html

Py:   @property 与 @x.setter
来源：http://hz.yanxiufei.cn/gtdmhffwxc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.52xcode.cn/gtkhyxomzz.html

JS:   get name() { return this._name; }
来源：http://hz.xylfe.cn/gtjpbtkokr.html

TS:   get name(): string { return this._name; }
来源：http://hz.ywan-chungtsiang.top/gtaxxssluw.html

Java: public String getName() { return name; }
来源：http://hz.nanxuanxn.top/gtknhjkqxn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zhijiandao.cn/gtqjattxas.html

Ruby: attr_accessor :name
来源：http://hz.xuetiantiany.cn/gtjokprhfk.html

C#:   public string Name { get; set; }
来源：http://hz.dashuyun.cn/gtleavubuk.html

[G12] 对象转字符串
来源：http://hz.iojbl.cn/gtfqskmuab.html

Py:   def __str__(self): return self.name
来源：http://hz.sufxvd.cn/gtzsuytmot.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.smart0.xyz/gtyoyspirt.html

JS:   toString() { return this.name; }
来源：http://hz.jyoumei.cn/gtyypiwauf.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhongyouzk.top/gtqzbrshuz.html

Java: @Override public String toString() { return name; }
来源：http://hz.tianlin.xyz/gtrrnmllno.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.nwbrower.top/gtoluyfnco.html

Ruby: def to_s; @name; end
来源：http://hz.iojbl.cn/gtbdepwdqf.html

C#:   public override string ToString() => Name;
来源：http://hz.shanyushiyangkeji.top/gthaftelra.html

[G13] 判断对象类型
来源：http://hz.xuetiantiany.cn/gtxbohkhtm.html

Py:   isinstance(u, User)
来源：http://hz.dashuyun.cn/gtcoavhndv.html

PHP:  $u instanceof User
来源：http://hz.yangfankeji.com/gtdplntpmt.html

JS:   u instanceof User
来源：http://hz.smart0.xyz/gtonbmzqqv.html

TS:   u instanceof User
来源：http://hz.aizwys.cn/gtiwnctndu.html

Java: u instanceof User
来源：http://hz.shanyushiyangtech.top/gtkquyipag.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jlsjyb.cn/gtsdxmglnq.html

Ruby: u.is_a?(User)
来源：http://hz.shangyingyoupin.top/gtnddkwhmk.html

C#:   u is User
来源：http://hz.yj202588.top/gtnewxmivw.html

[G14] 数据类 / record
来源：http://hz.nanxuanxn.top/gtiakdbywr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.pengpengdd.cyou/gttigldcmh.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.gotoacloud.top/gtspiuptfb.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.xziqi.cn/gtuqiusito.html

TS:   type User = { name: string; age: number };
来源：http://hz.nanxinkj.top/gtkukzvxqz.html

Java: record User(String name, int age) {}
来源：http://hz.chenjidiqi.icu/gtgmyjplfm.html

Go:   type User struct { Name string; Age int }
来源：http://hz.feifeiyinyue.top/gtcorshxsf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.hnxiangtu.top/gtxnpyrsgj.html

C#:   record User(string Name, int Age);
来源：http://hz.fzhhl.top/gtxocowenk.html

[G15] 枚举
来源：http://hz.quarkkingdee.top/gtgaagovlj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jyoumei.cn/gtujenljsc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.316326.xyz/gtachujxxq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.gzhubu.top/gtmxhwkntg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhengqikj.top/gtjonzhpcl.html

Java: enum Color { RED, GREEN }
来源：http://hz.xinyue.icu/gtqtqtskwn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ydjk.org.cn/gtxxdduifk.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jinghuilouyu.cn/gtexwnvgye.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.daria6918.cn/gteueqtzql.html

[G16] 对象转数组 / 字典
来源：http://hz.fengsongda.top/gtsvkaakrv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.hongshengwenyu.top/gtnqpqdqzb.html

PHP:  get_object_vars($obj);
来源：http://hz.cucudq.cn/gthsonaqlj.html

JS:   Object.entries(obj)
来源：http://hz.hysaishi.cn/gttnefutwt.html

TS:   Object.entries(obj)
来源：http://hz.guannengcc.top/gteetombcm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhaomingkeji.xyz/gtacfnzlrd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.gzhubu.top/gtayxdccjl.html

Ruby: obj.instance_variables
来源：http://hz.gogol.net.cn/gtoewspbyc.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.cucudq.cn/gtzjgwvczu.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtpeughdmz.html

H. 异常与错误处理
来源：http://hz.wangshuangyany.cn/gtugoakcsk.html

================================================================================
来源：http://hz.daria6918.cn/gtdmezotdm.html

[H01] try / catch 基础
来源：http://hz.yuxming.cn/gtnwhnsial.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.chenzaomai.com/gtxsclpyzn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.birdmap.top/gtwynbakef.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.sweek.top/gtvtlouvxz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.fengsongda.top/gtajxcdqnk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.sufxvd.cn/gtjvccblsa.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.nanxuanxn.top/gtmgrxvbck.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.chenzaomai.com/gtritxxwwa.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.ywan-chungtsiang.top/gtzbaupsha.html

[H02] finally / ensure 收尾
来源：http://hz.gogol.net.cn/gtcffigbur.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yongpay.top/gtqokqtcuo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xuanzx.com/gtflzsthqr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jiagoushi.top/gtswdtfygb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangtech.top/gtpptgibau.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.aizwys.cn/gtdqgbavvu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ydjk.org.cn/gtpkzapmty.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.wangshuangyany.cn/gtmlpxqdkr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.snrcjt.cn/gttiyubdiw.html

[H03] 主动抛出异常
来源：http://hz.sysykeji.top/gtuuzfczbx.html

Py:   raise ValueError("错误信息")
来源：http://hz.guowangkeji.top/gtqvarfplo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.shuidangran.top/gtzgpswmnq.html

JS:   throw new Error("错误信息");
来源：http://hz.0kj1m.cn/gtmjvfcypn.html

TS:   throw new Error("错误信息");
来源：http://hz.jiagoushi.top/gtcizvrhuw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yueranfly.top/gtvxpqbzge.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hysaishi.cn/gtohciczce.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zhaomingkeji.xyz/gtodjrxcqx.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.guannengcc.top/gtdogmwlar.html

[H04] 自定义异常类型
来源：http://hz.quarkkingdee.top/gtzekmxbmz.html

Py:   class MyError(Exception): pass
来源：http://hz.aibaodan.cn/gtxtbwkmop.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yongpay.top/gttjtiuann.html

JS:   class MyError extends Error {}
来源：http://hz.iojbl.cn/gtailpgbzd.html

TS:   class MyError extends Error {}
来源：http://hz.zdqjudy.top/gtghfcsxfy.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zhongyouzk.top/gttkokkyun.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yj20258888.top/gtgaljawxy.html

Ruby: class MyError < StandardError; end
来源：http://hz.hysaishi.cn/gtfdcasrsm.html

C#:   class MyException : Exception {}
来源：http://hz.ehwqpu.com/gtzmvcucqq.html

[H05] 捕获特定类型
来源：http://hz.cashguo.top/gtvglklnjj.html

Py:   except ValueError as e:
来源：http://hz.shzxlz.cn/gtmduywymd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhixingplan.top/gtjhcgsorl.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.havefunace.top/gtndmlxqqt.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.nanxinkj.top/gtmfwjuybd.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.ehwqpu.com/gtqohyscvw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yueranfly.top/gtupzvvres.html

Ruby: rescue ArgumentError => e
来源：http://hz.ydjk.org.cn/gtblexlebo.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.redwolf501.top/gttkxgunmi.html

[H06] 可选值 / 空值安全访问
来源：http://hz.shanyushiyangkeji.top/gtxdpcflwl.html

Py:   value = d.get("k") or default
来源：http://hz.zhijiandao.cn/gtipfpddiv.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hysaishi.cn/gtcszwnfyk.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.vqdsnc.cn/gtkehrbplb.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.cdnleiting.top/gtayvpvotr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.redwolf501.top/gttsaxxmsi.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.9152youxi.cn/gtryozqjwt.html

Ruby: d&.dig(:a, :b)
来源：http://hz.smart0.xyz/gtybsdrteu.html

C#:   obj?.A?.B ?? default
来源：http://hz.gotoacloud.top/gtikeapavm.html

[H07] 断言
来源：http://hz.yangfankeji.com/gtqqvcefaw.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yanxiufei.cn/gtahkkhicc.html

PHP:  assert($x > 0);
来源：http://hz.aibaodan.cn/gtuykgcvvm.html

JS:   console.assert(x > 0);
来源：http://hz.feifeiyinyue.top/gtystwkdau.html

TS:   console.assert(x > 0);
来源：http://hz.nwbrower.top/gtrhldejax.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jiagoushi.top/gtrsamfmig.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.dashuyun.cn/gtcejodcbd.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.ehwqpu.com/gttcpwoubr.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yvedp.cn/gtestjkzjt.html

[H08] 获取错误信息与堆栈
来源：http://hz.jinqigufen.top/gtkkkrifhx.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.bjfxy.top/gtebzzimmu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.xylfe.cn/gtrajecane.html

JS:   e.message;  e.stack
来源：http://hz.sufxvd.cn/gtjyleqbnv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.pycfn.com/gtvfqmhgll.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.dianchejie.cn/gtzqbbvzrl.html

Go:   err.Error()
来源：http://hz.ydzc1.top/gtrozgznuo.html

Ruby: e.message;  e.backtrace
来源：http://hz.gaohongyu789.top/gtwgibpkdj.html

C#:   e.Message;  e.StackTrace
来源：http://hz.daria6918.cn/gtaxuawzlf.html

[H09] 带错误码的异常
来源：http://hz.c1oappe.top/gtbzksowck.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.sweek.top/gtxxwgdqcf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zhengqikj.top/gtlxcbnpxz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.bjfxy.top/gtvljbdyfw.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yangfankeji.com/gttkcqftuq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.chenjidiqi.icu/gtzxiistnd.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hnqzz.top/gtuzzfbttb.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yanxiufei.cn/gtbcpajwod.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.hammf.cn/gtolfbdfbl.html

[H10] 资源自动释放
来源：http://hz.meibo888.top/gtplfnmwym.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.birdmap.top/gthuwjluzs.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.zhoulong.xyz/gtacuigaur.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ywan-chungtsiang.top/gtucpmtlrf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shzxlz.cn/gtzyaxbmai.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.dashuyun.cn/gtzulcwdhz.html

Go:   defer f.Close()
来源：http://hz.xuanzx.com/gtiyyqduvk.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yongpay.top/gtxyestzit.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.hnqzz.top/gtenvwejzl.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtalfsaqyj.html

I. 正则表达式
来源：http://hz.316326.xyz/gteeoimmkc.html

================================================================================
来源：http://hz.gogol.net.cn/gthcncjfkb.html

[I01] 判断是否匹配
来源：http://hz.zhaomingkeji.xyz/gtqzyxisbh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.cdnleiting.top/gtahxwuhsq.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.cqqwz.cn/gtgvdzzqtk.html

JS:   /\d+/.test(s)
来源：http://hz.haohaochexian.top/gtlkfohbfc.html

TS:   /\d+/.test(s)
来源：http://hz.iojbl.cn/gtorgamgmi.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.shuidangran.top/gtwmsjfukc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yongpay.top/gtizkgtpxd.html

Ruby: s.match?(/\d+/)
来源：http://hz.hywenlv.cn/gtlyirngri.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.snrcjt.cn/gtppnpjnvq.html

[I02] 提取所有匹配
来源：http://hz.zhiwuduotai.top/gtydhqdskm.html

Py:   re.findall(r"\d+", s)
来源：http://hz.sysykeji.top/gttujxppse.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.smart0.xyz/gtslnttyie.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.xuanzx.com/gtstrpjolk.html

TS:   s.match(/\d+/g)
来源：http://hz.xuanzx.com/gtlljnqjgd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.316326.xyz/gtswctgmus.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yvedp.cn/gtbrnghhat.html

Ruby: s.scan(/\d+/)
来源：http://hz.ywan-chungtsiang.top/gtaiwmubnv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.guowangkeji.top/gtdoehpwxw.html

[I03] 提取捕获分组
来源：http://hz.chenjidiqi.icu/gtdgzjwext.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yvedp.cn/gthoqdplyp.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zhiwuduotai.top/gtklhyqgyl.html


<!-- 参考信息 -->