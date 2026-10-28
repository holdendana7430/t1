代发 wailian999

C#:   File.Exists("a.txt")
来源：http://hz.zhiwuduotai.top/gthyygiroz.html

[F06] 删除文件
来源：http://hz.yj202588.top/gtwnvgdlbw.html

Py:   os.remove("a.txt")
来源：http://hz.chenlongwang.top/gtbthcegjl.html

PHP:  unlink("a.txt");
来源：http://hz.yuanzhike.top/gtxzbbwntj.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.haohaochexian.top/gtiqhpwicx.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jiagoushi.top/gtcauubhrd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yj20258.top/gtodpeswib.html

Go:   os.Remove("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtakphyqqa.html

Ruby: File.delete("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtboukoqxt.html

C#:   File.Delete("a.txt");
来源：http://hz.daxiang520.top/gtvbtpgmqo.html

[F07] 创建目录（含多级）
来源：http://hz.sufxvd.cn/gtzhkgfvyx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.aizwys.cn/gtkgcmcskv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.birdmap.top/gtxavfkmvt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jyoumei.cn/gtvtovetfa.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yanxiufei.cn/gtulmavmxj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.aibaodan.cn/gtnxqynsqw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.dianchejie.cn/gtpxnawvmd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.quarkkingdee.top/gtrvyqllhc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.cashguo.top/gtlahrotxh.html

[F08] 遍历目录
来源：http://hz.cdnleiting.top/gttgacbvjy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.chenzaomai.com/gtjtnwxmst.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jinghuilouyu.cn/gtoceuxcvb.html

JS:   fs.readdirSync("dir")
来源：http://hz.cashguo.top/gtmkgfiixz.html

TS:   fs.readdirSync("dir")
来源：http://hz.nwbrower.top/gtbyccuaov.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.gaohongyu789.top/gtvhgydwwq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.sysykeji.top/gtlbhmlilb.html

Ruby: Dir.children("dir")
来源：http://hz.sxryk.cn/gtgakpkakw.html

C#:   Directory.GetFiles("dir")
来源：http://hz.xziqi.cn/gtgmnocdqp.html

[F09] 获取文件大小
来源：http://hz.tianlin.xyz/gtlhylohpp.html

Py:   os.path.getsize("a.txt")
来源：http://hz.wangdashe.top/gtzoofrthb.html

PHP:  filesize("a.txt");
来源：http://hz.jiagoushi.top/gtydwhtedv.html

JS:   fs.statSync("a.txt").size
来源：http://hz.sxryk.cn/gttuqzzozv.html

TS:   fs.statSync("a.txt").size
来源：http://hz.hysaishi.cn/gtukwmnvmd.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.sysykeji.top/gtxwgqbrco.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.dianchejie.cn/gtbmtkbxpx.html

Ruby: File.size("a.txt")
来源：http://hz.yuanzhike.top/gttilzodic.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.52xcode.cn/gtwtytymeu.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.pycfn.com/gtdsyjgsdq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.andypj.xyz/gtsetpdzng.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.c1oappe.top/gtirrorpyj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zhongyouzk.top/gtmaksdxaj.html

TS:   path.extname("a.txt")
来源：http://hz.xuetiantiany.cn/gttijnrtmd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.52xcode.cn/gtaotcxouu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.pengpengdd.cyou/gthmavfbns.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.daria6918.cn/gtrskaisye.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.0kj1m.cn/gtijpqpzph.html

[F11] 复制与移动文件
来源：http://hz.ppjwa.cn/gtgfimbskl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.sweek.top/gtcyumnjfl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.quarkkingdee.top/gtexmfsddg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ydzc1.top/gtvadewdyl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.svipenyu.cn/gtovwdjqgb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.dianchejie.cn/gtiwfqswxg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yj20258888.top/gtxrkhbchn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.hysaishi.cn/gtwadoocdb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ywan-chungtsiang.top/gtopukcbcc.html

[F12] CSV 读写
来源：http://hz.nanxuanxn.top/gtesmypjfe.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xinyue.icu/gtjtzagbwn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.sufxvd.cn/gtnkcrtkvs.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.gzhubu.top/gtipmpgweh.html

TS:   // 同上
来源：http://hz.chenlongwang.top/gtwjfygnbk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.birdmap.top/gtwqncejot.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.fengsongda.top/gtvelwtqmb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.aizwys.cn/gtgkickbhn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.316326.xyz/gtkilbaoos.html

================================================================================
来源：http://hz.quarkkingdee.top/gtwgmdhpkg.html

G. 面向对象
来源：http://hz.yueranfly.top/gtxqkbnaoz.html

================================================================================
来源：http://hz.ivvv.top/gttrckkhno.html

[G01] 定义类
来源：http://hz.zhoulong.xyz/gtpisbnjrt.html

Py:   class User: pass
来源：http://hz.haohaochexian.top/gthdhchslx.html

PHP:  class User {}
来源：http://hz.cheryme.top/gtoqotbceb.html

JS:   class User {}
来源：http://hz.jiagoushi.top/gtyysetqou.html

TS:   class User { name: string = ""; }
来源：http://hz.shanyushiyangtech.top/gtytanpjxp.html

Java: class User {}
来源：http://hz.cheryme.top/gtfudgcsah.html

Go:   type User struct { Name string }
来源：http://hz.sysykeji.top/gtyentmsen.html

Ruby: class User; end
来源：http://hz.dianchejie.cn/gtkmsifydb.html

C#:   class User {}
来源：http://hz.ydzc1.top/gtikwqhsdm.html

[G02] 构造函数
来源：http://hz.aibaodan.cn/gtozqpwcgk.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jinghuilouyu.cn/gtsfwxndpv.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.fengsongda.top/gtfnnijbhk.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.316326.xyz/gtsfnuoqls.html

TS:   constructor(public name: string) {}
来源：http://hz.ywan-chungtsiang.top/gtvsmqgxmj.html

Java: User(String name) { this.name = name; }
来源：http://hz.hywenlv.cn/gtzzuazlze.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.pycfn.com/gtadfinnoz.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yongpay.top/gtmyblxosn.html

C#:   public User(string name) { Name = name; }
来源：http://hz.pengpengdd.cyou/gtyicjbyzq.html

[G03] 实例属性
来源：http://hz.redwolf501.top/gtynaekxej.html

Py:   self.name = "x"
来源：http://hz.zhengqikj.top/gthoygeihe.html

PHP:  public string $name = "x";
来源：http://hz.yonumen.top/gteahvuffw.html

JS:   this.name = "x";
来源：http://hz.zhaomingkeji.xyz/gtvstapfse.html

TS:   name: string = "x";
来源：http://hz.xingfuxueyuan.xyz/gtpasknxnf.html

Java: private String name;
来源：http://hz.meibo888.top/gttlsyvxly.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.9152youxi.cn/gtvrhupajq.html

Ruby: @name = "x"
来源：http://hz.chenjidiqi.icu/gtaxzgxfek.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jinqigufen.top/gttwxummqs.html

[G04] 定义方法
来源：http://hz.cqqwz.cn/gtwlmnanev.html

Py:   def greet(self): return self.name
来源：http://hz.ybcxt.top/gtuhykwkhl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.ydzc1.top/gtvzmvykgb.html

JS:   greet() { return this.name; }
来源：http://hz.yangfankeji.com/gthttpjxur.html

TS:   greet(): string { return this.name; }
来源：http://hz.cqqwz.cn/gtyohccsaq.html

Java: String greet() { return name; }
来源：http://hz.shangyingyoupin.top/gthimuiqfb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.sxryk.cn/gtppkaccen.html

Ruby: def greet; @name; end
来源：http://hz.ydjk.org.cn/gtwunjeuev.html

C#:   public string Greet() => Name;
来源：http://hz.gogol.net.cn/gtuoahybpm.html

[G05] 继承
来源：http://hz.0kj1m.cn/gtyjnacwmi.html

Py:   class Admin(User): pass
来源：http://hz.hnqzz.top/gtjtkfsmxk.html

PHP:  class Admin extends User {}
来源：http://hz.hnxiangtu.top/gtsqogpzkj.html

JS:   class Admin extends User {}
来源：http://hz.ehwqpu.com/gtmsafqesm.html

TS:   class Admin extends User {}
来源：http://hz.zhoulong.xyz/gttozlttlx.html

Java: class Admin extends User {}
来源：http://hz.hfpthk.cn/gtoadhszwa.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.sweek.top/gtrxgsncne.html

Ruby: class Admin < User; end
来源：http://hz.hammf.cn/gtgpbmqdmo.html

C#:   class Admin : User {}
来源：http://hz.c1oappe.top/gtpbndmven.html

[G06] 重写方法
来源：http://hz.cdnleiting.top/gttqyvghgd.html

Py:   def greet(self): return "admin"
来源：http://hz.shanyushiyangtech.top/gtituhljvp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jianghu66.top/gtpxntpyet.html

JS:   greet() { return "admin"; }
来源：http://hz.bjfxy.top/gtwmezelmk.html

TS:   greet(): string { return "admin"; }
来源：http://hz.mhx1999.top/gtizwcwixp.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.xylfe.cn/gtavjnmbap.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.c1oappe.top/gtnkbiybxf.html

Ruby: def greet; "admin"; end
来源：http://hz.tanke756.top/gtdcsecesf.html

C#:   public override string Greet() => "admin";
来源：http://hz.yuanzhike.top/gtotlekbjt.html

[G07] 调用父类方法
来源：http://hz.hongshengwenyu.top/gtskhjzrhk.html

Py:   super().greet()
来源：http://hz.havefunace.top/gtunxfvsmt.html

PHP:  parent::greet();
来源：http://hz.jinqigufen.top/gttwczeezj.html

JS:   super.greet();
来源：http://hz.gaohongyu789.top/gteyycvved.html

TS:   super.greet();
来源：http://hz.bjfxy.top/gthhqnqiyh.html

Java: super.greet();
来源：http://hz.jinghuilouyu.cn/gtwhafodcy.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.birdmap.top/gtqzluyoxl.html

Ruby: super
来源：http://hz.316326.xyz/gtxtvuqgpx.html

C#:   base.Greet();
来源：http://hz.chenzaomai.com/gtysikyvya.html

[G08] 静态方法与属性
来源：http://hz.havefunace.top/gtnubevlys.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.kuanghao11.cn/gtgcsvsljb.html

PHP:  public static function f() {}
来源：http://hz.fengsongda.top/gtvsxqykmr.html

JS:   static f() {}
来源：http://hz.guowangkeji.top/gtghhlnenr.html

TS:   static f(): void {}
来源：http://hz.xuanzx.com/gtcfhylkgw.html

Java: static void f() {}
来源：http://hz.jiagoushi.top/gtqhbjuneb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.mhx1999.top/gttgujqddj.html

Ruby: def self.f; end
来源：http://hz.zycfv.cn/gtkixuajrn.html

C#:   public static void F() {}
来源：http://hz.dashuyun.cn/gthfzjtdke.html

[G09] 接口 / 抽象类
来源：http://hz.chenzaomai.com/gtqngbqvnp.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.aizwys.cn/gtpprntdcp.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.52xcode.cn/gtahlcpnos.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.gotoacloud.top/gtbguxrbmh.html

TS:   interface Shape { area(): number; }
来源：http://hz.xinyue.icu/gtbynotzly.html

Java: interface Shape { double area(); }
来源：http://hz.hnqzz.top/gthttlblfo.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.aizwys.cn/gtgfpfjbfu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.snrcjt.cn/gtimaubbdr.html

C#:   interface IShape { double Area(); }
来源：http://hz.andypj.xyz/gtkxpembzf.html

[G10] 访问控制
来源：http://hz.aizwys.cn/gtuysexdec.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhiwuduotai.top/gtsvokuvya.html

PHP:  public / protected / private
来源：http://hz.shuidangran.top/gtcagoohzb.html

JS:   #private 字段；其余公开
来源：http://hz.gzhubu.top/gtghgvhrcs.html

TS:   public / protected / private
来源：http://hz.yj20258888.top/gtgoutliwa.html

Java: public / protected / private / 默认包级
来源：http://hz.fzhhl.top/gtykvjvpdl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.316326.xyz/gtywdldoyk.html

Ruby: public / protected / private
来源：http://hz.jiagoushi.top/gtsxwkxqte.html

C#:   public / protected / private / internal
来源：http://hz.sufxvd.cn/gtalsknccm.html

[G11] getter / setter
来源：http://hz.shanyushiyangtech.top/gtfmddxmbj.html

Py:   @property 与 @x.setter
来源：http://hz.jinyuanbaomall.cn/gtnkojomxe.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.svipenyu.cn/gtmjchvcss.html

JS:   get name() { return this._name; }
来源：http://hz.fzhhl.top/gtglhwcysh.html

TS:   get name(): string { return this._name; }
来源：http://hz.havefunace.top/gtfgbmvjsg.html

Java: public String getName() { return name; }
来源：http://hz.shzxlz.cn/gtdquepxxb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zhijiandao.cn/gtkmpcfplc.html

Ruby: attr_accessor :name
来源：http://hz.zdqjudy.top/gtublqumyi.html

C#:   public string Name { get; set; }
来源：http://hz.316326.xyz/gtxztpvunj.html

[G12] 对象转字符串
来源：http://hz.zhaomingkeji.xyz/gtkhrepcmd.html

Py:   def __str__(self): return self.name
来源：http://hz.ivvv.top/gtcztgfwko.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yj20258888.top/gtgehgkcje.html

JS:   toString() { return this.name; }
来源：http://hz.ywan-chungtsiang.top/gtsymwxccp.html

TS:   toString(): string { return this.name; }
来源：http://hz.shangyingyoupin.top/gtjkyguaqh.html

Java: @Override public String toString() { return name; }
来源：http://hz.hywenlv.cn/gtwydqnmdq.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.smart0.xyz/gtwjemveet.html

Ruby: def to_s; @name; end
来源：http://hz.birdmap.top/gtxrmfdosf.html

C#:   public override string ToString() => Name;
来源：http://hz.yongpay.top/gtmfovkuav.html

[G13] 判断对象类型
来源：http://hz.cdnleiting.top/gttnkyajqo.html

Py:   isinstance(u, User)
来源：http://hz.ydjk.org.cn/gtmahsczdh.html

PHP:  $u instanceof User
来源：http://hz.gzhubu.top/gtykzjmcfj.html

JS:   u instanceof User
来源：http://hz.zhiwuduotai.top/gtvrtxktcq.html

TS:   u instanceof User
来源：http://hz.smart0.xyz/gtmzleuhvc.html

Java: u instanceof User
来源：http://hz.sufxvd.cn/gtqignquoy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ppjwa.cn/gtawydnbsi.html

Ruby: u.is_a?(User)
来源：http://hz.shuidangran.top/gthxxsysou.html

C#:   u is User
来源：http://hz.hywenlv.cn/gtcjtfjlkd.html

[G14] 数据类 / record
来源：http://hz.sufxvd.cn/gtnlhfpzzc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yj20258888.top/gtrohkkwpk.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.tanke756.top/gtmksyfqpd.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.wangdashe.top/gtlvrygjnw.html

TS:   type User = { name: string; age: number };
来源：http://hz.jiagoushi.top/gtaauecxzn.html

Java: record User(String name, int age) {}
来源：http://hz.pengpengdd.cyou/gtsxwhvwjv.html

Go:   type User struct { Name string; Age int }
来源：http://hz.9152youxi.cn/gtiiykympz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jyoumei.cn/gtynbwxrxz.html

C#:   record User(string Name, int Age);
来源：http://hz.feifeiyinyue.top/gtjchvjtve.html

[G15] 枚举
来源：http://hz.zhongyouzk.top/gtxdbdsful.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.c1oappe.top/gtyxknhxme.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.dianchejie.cn/gtgoykiuqr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jinghuilouyu.cn/gttxvgiddj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.meibo888.top/gtszgkjtmc.html

Java: enum Color { RED, GREEN }
来源：http://hz.jqgufenzy.top/gtjhvhymuh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.dashuyun.cn/gtemnnijua.html

Ruby: Color = %i[red green].freeze
来源：http://hz.tian-w.cn/gttugwvlbx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jqgufenzy.top/gthtcrckjr.html

[G16] 对象转数组 / 字典
来源：http://hz.vqdsnc.cn/gtnejddkdm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.hammf.cn/gtjbthecwm.html

PHP:  get_object_vars($obj);
来源：http://hz.xylfe.cn/gtwhumynfp.html

JS:   Object.entries(obj)
来源：http://hz.snrcjt.cn/gtjoahqulf.html

TS:   Object.entries(obj)
来源：http://hz.sxryk.cn/gtnmtkapwh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.dianchejie.cn/gtlrtzxslk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.pycfn.com/gtdurehvlk.html

Ruby: obj.instance_variables
来源：http://hz.fengsongda.top/gthhqlaozx.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.andypj.xyz/gteexcsige.html

================================================================================
来源：http://hz.316326.xyz/gtjzftshwp.html

H. 异常与错误处理
来源：http://hz.sufxvd.cn/gtagqwxvht.html

================================================================================
来源：http://hz.zhixingplan.top/gtgogqqxqr.html

[H01] try / catch 基础
来源：http://hz.yuxming.cn/gtpkgszvze.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.316326.xyz/gtoplryzid.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.quarkkingdee.top/gtyrslnipg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zhijiandao.cn/gtnptmgyai.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.nanxuanxn.top/gtpeftqjmv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.iojbl.cn/gtlwoowddm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.feifeiyinyue.top/gtlxyozddd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.sysykeji.top/gtdhvwssdk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.guowangkeji.top/gtbvpaqahd.html

[H02] finally / ensure 收尾
来源：http://hz.zhiwuduotai.top/gtmdcthloy.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.meibo888.top/gtkvasbfgp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yuanzhike.top/gtmkvammbq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.cucudq.cn/gtaeofbojn.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ydjk.org.cn/gtazpidpcc.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jinghuilouyu.cn/gtulowshnd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.sxryk.cn/gtlrzsbwfi.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.wangshuangyany.cn/gtubtvjarq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.xziqi.cn/gtnxlhudhi.html

[H03] 主动抛出异常
来源：http://hz.havefunace.top/gtpvumxhly.html

Py:   raise ValueError("错误信息")
来源：http://hz.wangshuangyany.cn/gtinyxukcu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.xuanzx.com/gtnsyifgjt.html

JS:   throw new Error("错误信息");
来源：http://hz.jinghuilouyu.cn/gttapoerdo.html

TS:   throw new Error("错误信息");
来源：http://hz.nanxuanxn.top/gtpjtndjuh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jinqigufen.top/gttpopmfpr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.xingfuxueyuan.xyz/gtzyqhzwrx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.chenlongwang.top/gtkebcyxwm.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.shangyingyoupin.top/gtabpxxcjt.html

[H04] 自定义异常类型
来源：http://hz.yvedp.cn/gthznwvghk.html

Py:   class MyError(Exception): pass
来源：http://hz.cucudq.cn/gtttikgpey.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.ehwqpu.com/gtbircexhd.html

JS:   class MyError extends Error {}
来源：http://hz.dianchejie.cn/gtwtfmxmkm.html

TS:   class MyError extends Error {}
来源：http://hz.hysaishi.cn/gtmrwhqccg.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jlsjyb.cn/gtzmhdqfby.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yueranfly.top/gtiooxxxbv.html

Ruby: class MyError < StandardError; end
来源：http://hz.yuxming.cn/gtdhrtoiak.html

C#:   class MyException : Exception {}
来源：http://hz.hfpthk.cn/gtqnekeymd.html

[H05] 捕获特定类型
来源：http://hz.sxryk.cn/gttwurzoux.html

Py:   except ValueError as e:
来源：http://hz.ydzc1.top/gtcrcanopc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zycfv.cn/gtiwicjlhz.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zhaomingkeji.xyz/gtbgocyusl.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.sxryk.cn/gtasuyrjdc.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.wangdashe.top/gtqzogvdzc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zhixingplan.top/gtvzvxolua.html

Ruby: rescue ArgumentError => e
来源：http://hz.sweek.top/gtiyqdpwcb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yj20258888.top/gtgwyfaskk.html

[H06] 可选值 / 空值安全访问
来源：http://hz.shzxlz.cn/gtrcytsmvd.html

Py:   value = d.get("k") or default
来源：http://hz.ehwqpu.com/gtvurjhphr.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhengqikj.top/gtcfzgrrrs.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.xuetiantiany.cn/gtavvjhrxg.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.shuidangran.top/gtzszwgzpu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.chenjidiqi.icu/gtyivpnttl.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.shuidangran.top/gtshqmxxii.html

Ruby: d&.dig(:a, :b)
来源：http://hz.gaohongyu789.top/gtmeouhzib.html

C#:   obj?.A?.B ?? default
来源：http://hz.wangshuangyany.cn/gtogkyrrbb.html

[H07] 断言
来源：http://hz.tanke756.top/gthihcvziw.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yueranfly.top/gtsejafbuk.html

PHP:  assert($x > 0);
来源：http://hz.yj20258888.top/gtyovmfwhi.html

JS:   console.assert(x > 0);
来源：http://hz.meibo888.top/gtwbigisdq.html

TS:   console.assert(x > 0);
来源：http://hz.hysaishi.cn/gtadgqpbse.html

Java: assert x > 0 : "必须为正";
来源：http://hz.tianlin.xyz/gthhbuwddx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.birdmap.top/gtlcywnujw.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jinyuanbaomall.cn/gtynbcynke.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zhoulong.xyz/gtttbbmgjj.html

[H08] 获取错误信息与堆栈
来源：http://hz.yvedp.cn/gtxgacoltu.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ppjwa.cn/gttypeoyqg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jinyuanbaomall.cn/gtijyftzcm.html

JS:   e.message;  e.stack
来源：http://hz.shangyingyoupin.top/gtzxlxoitt.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jiagoushi.top/gtwcbahkle.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.chenzaomai.com/gtavmianit.html

Go:   err.Error()
来源：http://hz.gogol.net.cn/gtnkiwrtcv.html

Ruby: e.message;  e.backtrace
来源：http://hz.yvedp.cn/gtrpulussk.html

C#:   e.Message;  e.StackTrace
来源：http://hz.andypj.xyz/gtmfhrpctz.html

[H09] 带错误码的异常
来源：http://hz.yanxiufei.cn/gtvmdmfhnf.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.xuanzx.com/gtmorpaflu.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.nanxinkj.top/gthcjmqtry.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.ydjk.org.cn/gtqzwnesbt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.kuanghao11.cn/gtwilhoemj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.c1oappe.top/gtchmlrbcn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hnxiangtu.top/gtqtulptdk.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jyoumei.cn/gtfqaegyou.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhijiandao.cn/gtsybpjxsj.html

[H10] 资源自动释放
来源：http://hz.bjfxy.top/gtfjhswbxd.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.iojbl.cn/gtsxvoqfbi.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jinyuanbaomall.cn/gtmsvnzkrw.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shanyushiyangkeji.top/gtajflrwrl.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xuanzx.com/gttrtqtfky.html


<!-- 参考信息 -->