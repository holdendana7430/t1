代发 wailian999

Ruby: File.delete("a.txt")
来源：http://hz.redwolf501.top/gtxthvetkh.html

C#:   File.Delete("a.txt");
来源：http://hz.zycfv.cn/gtnzugslbr.html

[F07] 创建目录（含多级）
来源：http://hz.gaohongyu789.top/gthgltqxds.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.sweek.top/gtkmbhbhqt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.xinyue.icu/gtkcahegej.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.wangdashe.top/gtsxtgrskx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ivvv.top/gtuwlleups.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.xylfe.cn/gtayxuzlwi.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jianghu66.top/gtmxtcvtdb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.shzxlz.cn/gtmuoshoyo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.nanxinkj.top/gthakxshve.html

[F08] 遍历目录
来源：http://hz.daxiang520.top/gttysqlqfr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.c1oappe.top/gtxfugtwsn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.hnqzz.top/gthqakowab.html

JS:   fs.readdirSync("dir")
来源：http://hz.xuetiantiany.cn/gtimhqscjo.html

TS:   fs.readdirSync("dir")
来源：http://hz.yuxming.cn/gtacvgfgdm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.gotoacloud.top/gtsoajlozd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yangfankeji.com/gtjgsjuqqh.html

Ruby: Dir.children("dir")
来源：http://hz.shangyingyoupin.top/gtolqobyzz.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yongpay.top/gtarsrjxoe.html

[F09] 获取文件大小
来源：http://hz.shanyushiyangtech.top/gtksoycofu.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zhoulong.xyz/gtcgbwtfey.html

PHP:  filesize("a.txt");
来源：http://hz.iojbl.cn/gtphnbwygq.html

JS:   fs.statSync("a.txt").size
来源：http://hz.nanxuanxn.top/gtcaubwvrq.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jlsjyb.cn/gtqacxviap.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.shzxlz.cn/gtmeqkkvav.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.52xcode.cn/gtcvausoiv.html

Ruby: File.size("a.txt")
来源：http://hz.snrcjt.cn/gtwozrdxuh.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.sxryk.cn/gtqnhxghug.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.ppjwa.cn/gttzjeibdx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.birdmap.top/gtbngmpgfx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.xinyue.icu/gtvtdpbysy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yueranfly.top/gttaecdfap.html

TS:   path.extname("a.txt")
来源：http://hz.zhoulong.xyz/gtbfwlzqjv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yuxming.cn/gtoqfimroj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.guowangkeji.top/gtyracboab.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.guannengcc.top/gtfzngzgfw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.wangshuangyany.cn/gttbkhmqbx.html

[F11] 复制与移动文件
来源：http://hz.dashuyun.cn/gtfafaexff.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jinghuilouyu.cn/gtdczyfoxl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.pengpengdd.cyou/gteiphlimn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hnxiangtu.top/gtqfvlcmsx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jyoumei.cn/gtgyfbeygn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.hywenlv.cn/gtyldwedzm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.xingfuxueyuan.xyz/gtptehvfdq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.haohaochexian.top/gtxqucwzvp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ydzc1.top/gtylurjyna.html

[F12] CSV 读写
来源：http://hz.nanxinkj.top/gtatuwpnlm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xinyue.icu/gtnpbkmnpt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.sxryk.cn/gtlhffbtyj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yj20258.top/gtkldczvbw.html

TS:   // 同上
来源：http://hz.chenlongwang.top/gtocctmfrn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jianghu66.top/gthuzoqwka.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.316326.xyz/gtsamypnxl.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.hnqzz.top/gtxagxfnml.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jiagoushi.top/gtctynuldk.html

================================================================================
来源：http://hz.andypj.xyz/gtimugvdxl.html

G. 面向对象
来源：http://hz.jlsjyb.cn/gtwfiwoejz.html

================================================================================
来源：http://hz.yj202588.top/gtmxfoqkbd.html

[G01] 定义类
来源：http://hz.sysykeji.top/gtiaojbpod.html

Py:   class User: pass
来源：http://hz.jinqigufen.top/gtbjyqrpbw.html

PHP:  class User {}
来源：http://hz.yuxming.cn/gtralpnxnz.html

JS:   class User {}
来源：http://hz.ybcxt.top/gtmkkxqbgf.html

TS:   class User { name: string = ""; }
来源：http://hz.jinyuanbaomall.cn/gtwtfctcct.html

Java: class User {}
来源：http://hz.jqgufenzy.top/gtmzvhwvsf.html

Go:   type User struct { Name string }
来源：http://hz.316326.xyz/gtfkaeeajp.html

Ruby: class User; end
来源：http://hz.jinqigfzy.top/gtqswxzzgp.html

C#:   class User {}
来源：http://hz.jlsjyb.cn/gtxdwtguzk.html

[G02] 构造函数
来源：http://hz.shuidangran.top/gtbmyqqnmu.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.nanxuanxn.top/gtotbkcsdr.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.sufxvd.cn/gtdlzrsnwh.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.iojbl.cn/gttdqknofy.html

TS:   constructor(public name: string) {}
来源：http://hz.bjfxy.top/gtvvbraaaj.html

Java: User(String name) { this.name = name; }
来源：http://hz.xylfe.cn/gtkqzootug.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yueranfly.top/gtdahfwckc.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.dashuyun.cn/gtmfzlkvfg.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zhijiandao.cn/gtbaxpwcxy.html

[G03] 实例属性
来源：http://hz.jqgfzy.top/gtvosmsdsa.html

Py:   self.name = "x"
来源：http://hz.yj20258888.top/gtoilecupt.html

PHP:  public string $name = "x";
来源：http://hz.guannengcc.top/gtdwoppsfa.html

JS:   this.name = "x";
来源：http://hz.ydjk.org.cn/gtzlakutys.html

TS:   name: string = "x";
来源：http://hz.ehwqpu.com/gtpdtkpclj.html

Java: private String name;
来源：http://hz.gotoacloud.top/gthbkcksov.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jlsjyb.cn/gtlizpwdvd.html

Ruby: @name = "x"
来源：http://hz.zhijiandao.cn/gtbedjlmyk.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.xuetiantiany.cn/gtiapsrazq.html

[G04] 定义方法
来源：http://hz.zhoulong.xyz/gtkovywdlw.html

Py:   def greet(self): return self.name
来源：http://hz.316326.xyz/gtgnvbryze.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhoulong.xyz/gtzofhhlog.html

JS:   greet() { return this.name; }
来源：http://hz.jinqigfzy.top/gtonxovgfm.html

TS:   greet(): string { return this.name; }
来源：http://hz.daxiang520.top/gthywzugbn.html

Java: String greet() { return name; }
来源：http://hz.gotoacloud.top/gtyakkxdno.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yuanzhike.top/gtnrfpzung.html

Ruby: def greet; @name; end
来源：http://hz.zycfv.cn/gthvjmhwpp.html

C#:   public string Greet() => Name;
来源：http://hz.zycfv.cn/gtwsxqamvs.html

[G05] 继承
来源：http://hz.yuxming.cn/gttxjnnypf.html

Py:   class Admin(User): pass
来源：http://hz.shanyushiyangtech.top/gtblzszmoo.html

PHP:  class Admin extends User {}
来源：http://hz.yj20258.top/gthkchsbrq.html

JS:   class Admin extends User {}
来源：http://hz.aibaodan.cn/gttgdynece.html

TS:   class Admin extends User {}
来源：http://hz.yj20258.top/gtzkmxnvxa.html

Java: class Admin extends User {}
来源：http://hz.redwolf501.top/gtxkunidgi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.cdnleiting.top/gtafmuvjye.html

Ruby: class Admin < User; end
来源：http://hz.cdnleiting.top/gtexadthgl.html

C#:   class Admin : User {}
来源：http://hz.ppjwa.cn/gttpzcrnku.html

[G06] 重写方法
来源：http://hz.jqgfzy.top/gtloaxytyv.html

Py:   def greet(self): return "admin"
来源：http://hz.yuxming.cn/gtqkqebrqu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jinghuilouyu.cn/gtfgiddzyt.html

JS:   greet() { return "admin"; }
来源：http://hz.gotoacloud.top/gtasxopgqg.html

TS:   greet(): string { return "admin"; }
来源：http://hz.ydjk.org.cn/gtboemhsyd.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hnqzz.top/gtxtduubbe.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yj20258888.top/gtpcxpibjg.html

Ruby: def greet; "admin"; end
来源：http://hz.xinyue.icu/gtrwyqhcha.html

C#:   public override string Greet() => "admin";
来源：http://hz.xylfe.cn/gtabebyanx.html

[G07] 调用父类方法
来源：http://hz.yonumen.top/gtxpddzmhl.html

Py:   super().greet()
来源：http://hz.pycfn.com/gtrldvubit.html

PHP:  parent::greet();
来源：http://hz.guannengcc.top/gteedkrdsr.html

JS:   super.greet();
来源：http://hz.sufxvd.cn/gtxcureniz.html

TS:   super.greet();
来源：http://hz.guannengcc.top/gtfavohdfd.html

Java: super.greet();
来源：http://hz.xziqi.cn/gtfigjvkob.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.smart0.xyz/gtxqlhpxzt.html

Ruby: super
来源：http://hz.mhx1999.top/gtaiovbufr.html

C#:   base.Greet();
来源：http://hz.cashguo.top/gtvvptsesi.html

[G08] 静态方法与属性
来源：http://hz.zhoulong.xyz/gtmprdvgtq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.sxryk.cn/gtnqxkzydb.html

PHP:  public static function f() {}
来源：http://hz.fengsongda.top/gtwcqutzpx.html

JS:   static f() {}
来源：http://hz.daria6918.cn/gtvhcmzcwf.html

TS:   static f(): void {}
来源：http://hz.sxryk.cn/gtydqjuqru.html

Java: static void f() {}
来源：http://hz.jinghuilouyu.cn/gtjadyxzcz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.xziqi.cn/gtqymmxzkz.html

Ruby: def self.f; end
来源：http://hz.fengsongda.top/gtxuujixjt.html

C#:   public static void F() {}
来源：http://hz.shanyushiyangkeji.top/gtfnhqrume.html

[G09] 接口 / 抽象类
来源：http://hz.jianghu66.top/gtwrktwozu.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.nanxuanxn.top/gtmyeorxkp.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ydzc1.top/gtkgrrqcmt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zhijiandao.cn/gtejizsxni.html

TS:   interface Shape { area(): number; }
来源：http://hz.tianlin.xyz/gtnasxkywd.html

Java: interface Shape { double area(); }
来源：http://hz.xinyue.icu/gtagyazqgv.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yangfankeji.com/gtuxxvaryg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhixingplan.top/gtrkrktmzd.html

C#:   interface IShape { double Area(); }
来源：http://hz.snrcjt.cn/gtjpkbpiwo.html

[G10] 访问控制
来源：http://hz.zhongyouzk.top/gtcxrdnbir.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.tian-w.cn/gtoqhvdqap.html

PHP:  public / protected / private
来源：http://hz.zhaomingkeji.xyz/gtipxtgkwp.html

JS:   #private 字段；其余公开
来源：http://hz.9152youxi.cn/gtwjaotfjv.html

TS:   public / protected / private
来源：http://hz.yj20258.top/gthlggsapu.html

Java: public / protected / private / 默认包级
来源：http://hz.yuxming.cn/gtrhoeqrim.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.hywenlv.cn/gteaczpbwp.html

Ruby: public / protected / private
来源：http://hz.meibo888.top/gtafyeryzb.html

C#:   public / protected / private / internal
来源：http://hz.cheryme.top/gtdruwjbad.html

[G11] getter / setter
来源：http://hz.daria6918.cn/gtoimfkahz.html

Py:   @property 与 @x.setter
来源：http://hz.yueranfly.top/gtsfbpigbh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.shanyushiyangkeji.top/gtsqodweey.html

JS:   get name() { return this._name; }
来源：http://hz.daxiang520.top/gtulimrlmp.html

TS:   get name(): string { return this._name; }
来源：http://hz.xziqi.cn/gtxlwtactk.html

Java: public String getName() { return name; }
来源：http://hz.jinqigfzy.top/gtqtaqefcq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.xuetiantiany.cn/gtnxreyxye.html

Ruby: attr_accessor :name
来源：http://hz.wangshuangyany.cn/gtwfdegirn.html

C#:   public string Name { get; set; }
来源：http://hz.jiagoushi.top/gttixxdyyk.html

[G12] 对象转字符串
来源：http://hz.kuanghao11.cn/gtolrjoliu.html

Py:   def __str__(self): return self.name
来源：http://hz.ywan-chungtsiang.top/gtrhzmvebx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.feifeiyinyue.top/gtcmovplun.html

JS:   toString() { return this.name; }
来源：http://hz.xuetiantiany.cn/gtnmldiplc.html

TS:   toString(): string { return this.name; }
来源：http://hz.tanke756.top/gtjbjbfwnr.html

Java: @Override public String toString() { return name; }
来源：http://hz.cdnleiting.top/gttaqccxvi.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.c1oappe.top/gtkmzvtuth.html

Ruby: def to_s; @name; end
来源：http://hz.sweek.top/gtusakogpk.html

C#:   public override string ToString() => Name;
来源：http://hz.yvedp.cn/gtuxohxrqc.html

[G13] 判断对象类型
来源：http://hz.redwolf501.top/gtgilyobap.html

Py:   isinstance(u, User)
来源：http://hz.shanyushiyangkeji.top/gtcbxtohhl.html

PHP:  $u instanceof User
来源：http://hz.sysykeji.top/gtcxtzhhim.html

JS:   u instanceof User
来源：http://hz.ybcxt.top/gtiryiyxqs.html

TS:   u instanceof User
来源：http://hz.daxiang520.top/gthrwhgghp.html

Java: u instanceof User
来源：http://hz.andypj.xyz/gtericqzie.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.cucudq.cn/gtsvpkimkv.html

Ruby: u.is_a?(User)
来源：http://hz.ydjk.org.cn/gtvyfmdgxv.html

C#:   u is User
来源：http://hz.sxryk.cn/gturflzeci.html

[G14] 数据类 / record
来源：http://hz.yvedp.cn/gtajiakoes.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.tanke756.top/gtpyvcfldd.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.fzhhl.top/gtgrsrzmod.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.shanyushiyangkeji.top/gtqnyouslc.html

TS:   type User = { name: string; age: number };
来源：http://hz.shangyingyoupin.top/gtuvfbrrfb.html

Java: record User(String name, int age) {}
来源：http://hz.havefunace.top/gtfaxkzsrh.html

Go:   type User struct { Name string; Age int }
来源：http://hz.dashuyun.cn/gtqvczaenu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.aibaodan.cn/gteajhufys.html

C#:   record User(string Name, int Age);
来源：http://hz.wangshuangyany.cn/gtfanydatr.html

[G15] 枚举
来源：http://hz.sweek.top/gtdmhowiht.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yangfankeji.com/gtlfsnbudd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.xingfuxueyuan.xyz/gtvnqabael.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.xziqi.cn/gtjeblykyy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cheryme.top/gtpogqptay.html

Java: enum Color { RED, GREEN }
来源：http://hz.yongpay.top/gtntysaxle.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.cdnleiting.top/gtndtgfxad.html

Ruby: Color = %i[red green].freeze
来源：http://hz.shanyushiyangkeji.top/gtdajqgqzs.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shanyushiyangkeji.top/gtkulzspji.html

[G16] 对象转数组 / 字典
来源：http://hz.chenlongwang.top/gtnteepqer.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.guannengcc.top/gtjveqsnjj.html

PHP:  get_object_vars($obj);
来源：http://hz.shanyushiyangkeji.top/gtjprdnjlh.html

JS:   Object.entries(obj)
来源：http://hz.gzhubu.top/gtdnxfqibq.html

TS:   Object.entries(obj)
来源：http://hz.quarkkingdee.top/gtopllurmy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yvedp.cn/gtzgwvwgna.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jinqigufen.top/gtboahnskc.html

Ruby: obj.instance_variables
来源：http://hz.svipenyu.cn/gtazaxtqjh.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhiwuduotai.top/gtverwzqis.html

================================================================================
来源：http://hz.zhijiandao.cn/gtddpjdvcw.html

H. 异常与错误处理
来源：http://hz.xingfuxueyuan.xyz/gtkskrmzne.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gthefgwzuw.html

[H01] try / catch 基础
来源：http://hz.jinyuanbaomall.cn/gtnpdvsyxi.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.wangshuangyany.cn/gtvlzjrthz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.xylfe.cn/gtpfdaqhxb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yueranfly.top/gtetxaplmq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jqgufenzy.top/gteqtkylbc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.kuanghao11.cn/gtwjidcwpk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.haohaochexian.top/gtyiuymdof.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.cashguo.top/gtpocrplob.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.aizwys.cn/gtyhvdnnyw.html

[H02] finally / ensure 收尾
来源：http://hz.feifeiyinyue.top/gtnemxcrrk.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zhijiandao.cn/gtyrywywhv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.ivvv.top/gtnyrzklnb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.xuanzx.com/gtcfqwzols.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.cucudq.cn/gtxjchrbix.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhaomingkeji.xyz/gtoebtbfyq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zhoulong.xyz/gtummlkyxd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jqgfzy.top/gtfymhyoth.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.tanke756.top/gtrxglhkfx.html

[H03] 主动抛出异常
来源：http://hz.dianchejie.cn/gtaueocafz.html

Py:   raise ValueError("错误信息")
来源：http://hz.pycfn.com/gtiwpfbfip.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zycfv.cn/gttbdsxexj.html

JS:   throw new Error("错误信息");
来源：http://hz.yangfankeji.com/gtjhntkved.html

TS:   throw new Error("错误信息");
来源：http://hz.yj202588.top/gtdpbtpkoi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.0kj1m.cn/gtyqcznplq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.sxryk.cn/gtykxoatje.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.cdnleiting.top/gtxvaguiru.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.fzhhl.top/gtxerdqdae.html

[H04] 自定义异常类型
来源：http://hz.sysykeji.top/gtaaccdjxf.html

Py:   class MyError(Exception): pass
来源：http://hz.ydzc1.top/gtzcwoyhhb.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.ydjk.org.cn/gtwcijxurk.html

JS:   class MyError extends Error {}
来源：http://hz.feifeiyinyue.top/gtmtdhbwnq.html

TS:   class MyError extends Error {}
来源：http://hz.zhoulong.xyz/gtrvckwaug.html

Java: class MyException extends RuntimeException {}
来源：http://hz.chenzaomai.com/gtmcgvmzkp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.gzhubu.top/gtzinprjuo.html

Ruby: class MyError < StandardError; end
来源：http://hz.daxiang520.top/gtxijxfdjf.html

C#:   class MyException : Exception {}
来源：http://hz.zycfv.cn/gtamgivmkh.html

[H05] 捕获特定类型
来源：http://hz.shzxlz.cn/gtkiyhraxz.html

Py:   except ValueError as e:
来源：http://hz.vqdsnc.cn/gtitahrbrx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.nwbrower.top/gttpnupgzs.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.hfpthk.cn/gttaadfymx.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jinghuilouyu.cn/gtbedwcqud.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.nanxinkj.top/gtljfxzegp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.shangyingyoupin.top/gtzfxgtzeb.html

Ruby: rescue ArgumentError => e
来源：http://hz.daxiang520.top/gtnktpozve.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.andypj.xyz/gtofemczeg.html

[H06] 可选值 / 空值安全访问
来源：http://hz.ivvv.top/gtaiiaprue.html

Py:   value = d.get("k") or default
来源：http://hz.zycfv.cn/gtjpkyegbs.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.shzxlz.cn/gtfqlsvxsb.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.dashuyun.cn/gtzgzdtiye.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.hnqzz.top/gttcxeigcw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.wangdashe.top/gtmizrxaos.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.ywan-chungtsiang.top/gtrvtdgoxk.html

Ruby: d&.dig(:a, :b)
来源：http://hz.kuanghao11.cn/gtaxuhqnkt.html

C#:   obj?.A?.B ?? default
来源：http://hz.zhiwuduotai.top/gtoyemnbxv.html

[H07] 断言
来源：http://hz.cashguo.top/gtkwtpmmni.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zhoulong.xyz/gtynchzlzj.html

PHP:  assert($x > 0);
来源：http://hz.9152youxi.cn/gttyierkla.html

JS:   console.assert(x > 0);
来源：http://hz.ivvv.top/gtdkzbmvxk.html

TS:   console.assert(x > 0);
来源：http://hz.mhx1999.top/gtziqqqajw.html

Java: assert x > 0 : "必须为正";
来源：http://hz.havefunace.top/gtnkajbnir.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.andypj.xyz/gtpoccbmdv.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.xinyue.icu/gtomcyynpe.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yonumen.top/gtnpcjduup.html

[H08] 获取错误信息与堆栈
来源：http://hz.meibo888.top/gtjefabiyf.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.redwolf501.top/gtabuolsti.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.hfpthk.cn/gtdfvblunv.html

JS:   e.message;  e.stack
来源：http://hz.wangdashe.top/gtjbpyvfuw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.guannengcc.top/gtokhxmtue.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.ywan-chungtsiang.top/gtilhiqvxx.html

Go:   err.Error()
来源：http://hz.aibaodan.cn/gturismqlu.html

Ruby: e.message;  e.backtrace
来源：http://hz.vqdsnc.cn/gteycpxrwc.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yongpay.top/gtefdaoxca.html

[H09] 带错误码的异常
来源：http://hz.tanke756.top/gtnxbmkglk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hnxiangtu.top/gtehnjresi.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.nwbrower.top/gtfdbnoqzw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jqgfzy.top/gtwjutzwkb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.shanyushiyangkeji.top/gtauzarpcl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.xuetiantiany.cn/gtymikgumo.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yuxming.cn/gtnzbhafjg.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.guannengcc.top/gtrfntkrdy.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.wangshuangyany.cn/gtaxiytavk.html

[H10] 资源自动释放
来源：http://hz.andypj.xyz/gtrjzvcmbl.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.shanyushiyangtech.top/gtxxdlvgga.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.gzhubu.top/gtmuujfpdx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.kuanghao11.cn/gtxjmxpcac.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.fzhhl.top/gteoduzlkt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.hywenlv.cn/gtdihgxrlj.html

Go:   defer f.Close()
来源：http://hz.jyoumei.cn/gtvvaopspy.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.xuanzx.com/gtxffokxko.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.chenjidiqi.icu/gtwiodjgyr.html

================================================================================
来源：http://hz.gaohongyu789.top/gtxzrthnkj.html

I. 正则表达式
来源：http://hz.xinyue.icu/gtlbbougoq.html

================================================================================
来源：http://hz.xylfe.cn/gtlhkfrdji.html

[I01] 判断是否匹配
来源：http://hz.jqgfzy.top/gttnwvnjmy.html


<!-- 参考信息 -->