代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://hz.birdmap.top/gtrtlsiuxz.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hysaishi.cn/gtohrxlkpc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jinyuanbaomall.cn/gtvogoucrt.html

Go:   os.Remove("a.txt")
来源：http://hz.jinqigfzy.top/gtqbmbenxg.html

Ruby: File.delete("a.txt")
来源：http://hz.tianlin.xyz/gtdosaugmc.html

C#:   File.Delete("a.txt");
来源：http://hz.zhijiandao.cn/gtmbbshvdc.html

[F07] 创建目录（含多级）
来源：http://hz.smart0.xyz/gteriqurhb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zhixingplan.top/gtqtzqvrtd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.feifeiyinyue.top/gtbtmwsycl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hywenlv.cn/gtgbmjdivm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yj202588.top/gtclhdltru.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.shangyingyoupin.top/gtmwnwstcg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.fzhhl.top/gtokkrwpjv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.316326.xyz/gtljyidsxx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.shanyushiyangkeji.top/gtbnbogdpb.html

[F08] 遍历目录
来源：http://hz.yonumen.top/gtypnloyuq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.xingfuxueyuan.xyz/gtilpvufqx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.snrcjt.cn/gtdeifsadh.html

JS:   fs.readdirSync("dir")
来源：http://hz.snrcjt.cn/gtmmaisicu.html

TS:   fs.readdirSync("dir")
来源：http://hz.chenzaomai.com/gtifsjlmom.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jinqigufen.top/gtgyerwjqi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jinqigufen.top/gtcdthrqwu.html

Ruby: Dir.children("dir")
来源：http://hz.cheryme.top/gtuwzpyibp.html

C#:   Directory.GetFiles("dir")
来源：http://hz.ehwqpu.com/gtsopracph.html

[F09] 获取文件大小
来源：http://hz.shuidangran.top/gttqprqsnf.html

Py:   os.path.getsize("a.txt")
来源：http://hz.guannengcc.top/gtwiboryic.html

PHP:  filesize("a.txt");
来源：http://hz.haohaochexian.top/gtgojwymvy.html

JS:   fs.statSync("a.txt").size
来源：http://hz.guowangkeji.top/gteolonism.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yvedp.cn/gtdsffvrrs.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.andypj.xyz/gtmxlqvqfo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hfpthk.cn/gtyctjlnik.html

Ruby: File.size("a.txt")
来源：http://hz.zhoulong.xyz/gtqmdxdjuv.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.zhiwuduotai.top/gtjiwzuuyj.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jianghu66.top/gtattjspjr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jinqigfzy.top/gtslcrfysm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.xylfe.cn/gttqcqbslp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.shangyingyoupin.top/gtgqgyzeit.html

TS:   path.extname("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtxlsjikss.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.hongshengwenyu.top/gtikpdmxio.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.daria6918.cn/gttohiouch.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.c1oappe.top/gtboaoabko.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.ybcxt.top/gtvfealfuq.html

[F11] 复制与移动文件
来源：http://hz.guowangkeji.top/gtemtikbpy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.pycfn.com/gtcdvsnycr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.hnqzz.top/gtoahwcafr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xinyue.icu/gthgypqdlg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.pengpengdd.cyou/gtdypzwnwz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jinqigfzy.top/gtjigelura.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.shzxlz.cn/gtrmugzkho.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.guowangkeji.top/gtsevgutaz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.nanxuanxn.top/gtyctinzrl.html

[F12] CSV 读写
来源：http://hz.svipenyu.cn/gtehhdbwjv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xziqi.cn/gtfrgrbrwn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jinghuilouyu.cn/gtkftdejfv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.xuetiantiany.cn/gttqteflyj.html

TS:   // 同上
来源：http://hz.sysykeji.top/gtqvztxwsv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.daria6918.cn/gtfqdcvana.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.gzhubu.top/gtwxeuuaii.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.sxryk.cn/gthhwjgqbz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.hongshengwenyu.top/gtzjdauzqd.html

================================================================================
来源：http://hz.ybcxt.top/gtkswizdbg.html

G. 面向对象
来源：http://hz.jiagoushi.top/gtnulitibd.html

================================================================================
来源：http://hz.jianghu66.top/gtbadynaov.html

[G01] 定义类
来源：http://hz.fengsongda.top/gtqkunooyg.html

Py:   class User: pass
来源：http://hz.gotoacloud.top/gtlkmtargr.html

PHP:  class User {}
来源：http://hz.hnqzz.top/gttwjjinho.html

JS:   class User {}
来源：http://hz.shzxlz.cn/gtazehhlsr.html

TS:   class User { name: string = ""; }
来源：http://hz.gotoacloud.top/gtiwepfptg.html

Java: class User {}
来源：http://hz.iojbl.cn/gttripsmnz.html

Go:   type User struct { Name string }
来源：http://hz.vqdsnc.cn/gtldyvpqil.html

Ruby: class User; end
来源：http://hz.kuanghao11.cn/gtixwrbidp.html

C#:   class User {}
来源：http://hz.xinyue.icu/gtameyateu.html

[G02] 构造函数
来源：http://hz.wangshuangyany.cn/gtcdebzoco.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.feifeiyinyue.top/gtqclfxpum.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.xylfe.cn/gtqsrycfta.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.iojbl.cn/gtcrnzxbzf.html

TS:   constructor(public name: string) {}
来源：http://hz.yangfankeji.com/gtzrfbaktu.html

Java: User(String name) { this.name = name; }
来源：http://hz.jinyuanbaomall.cn/gtlpbqacef.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.nanxinkj.top/gtwagofacj.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.9152youxi.cn/gtpkgaopqk.html

C#:   public User(string name) { Name = name; }
来源：http://hz.ppjwa.cn/gtzkjohtaq.html

[G03] 实例属性
来源：http://hz.cdnleiting.top/gtoulhbmux.html

Py:   self.name = "x"
来源：http://hz.gogol.net.cn/gtijszbwog.html

PHP:  public string $name = "x";
来源：http://hz.gzhubu.top/gtczmnnpvb.html

JS:   this.name = "x";
来源：http://hz.meibo888.top/gtruekjpkf.html

TS:   name: string = "x";
来源：http://hz.9152youxi.cn/gtbncfvjqv.html

Java: private String name;
来源：http://hz.xziqi.cn/gtimhnrypf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.cashguo.top/gtyswkgies.html

Ruby: @name = "x"
来源：http://hz.52xcode.cn/gthyivqtsq.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.ydzc1.top/gtxrlkjxfm.html

[G04] 定义方法
来源：http://hz.chenjidiqi.icu/gteizcdpwj.html

Py:   def greet(self): return self.name
来源：http://hz.jinyuanbaomall.cn/gtcbycuxnf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.nwbrower.top/gtuxbqxage.html

JS:   greet() { return this.name; }
来源：http://hz.aizwys.cn/gtdpwpfjgv.html

TS:   greet(): string { return this.name; }
来源：http://hz.9152youxi.cn/gtmotvzmob.html

Java: String greet() { return name; }
来源：http://hz.316326.xyz/gtbxtlxvlx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zycfv.cn/gtruyngkcr.html

Ruby: def greet; @name; end
来源：http://hz.cucudq.cn/gtslqqbanz.html

C#:   public string Greet() => Name;
来源：http://hz.guowangkeji.top/gtgsfdqgzz.html

[G05] 继承
来源：http://hz.ydzc1.top/gtxddvgtxz.html

Py:   class Admin(User): pass
来源：http://hz.haohaochexian.top/gtwfazszka.html

PHP:  class Admin extends User {}
来源：http://hz.aibaodan.cn/gtodjtzuzr.html

JS:   class Admin extends User {}
来源：http://hz.shanyushiyangkeji.top/gtxaxlytof.html

TS:   class Admin extends User {}
来源：http://hz.svipenyu.cn/gtkwemnouj.html

Java: class Admin extends User {}
来源：http://hz.jinqigufen.top/gtzhnqtymd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hnqzz.top/gtibxbjhqy.html

Ruby: class Admin < User; end
来源：http://hz.wangshuangyany.cn/gtcyuuujnt.html

C#:   class Admin : User {}
来源：http://hz.yj20258.top/gtdryovgjt.html

[G06] 重写方法
来源：http://hz.jianghu66.top/gtfjpspfzg.html

Py:   def greet(self): return "admin"
来源：http://hz.yj202588.top/gtvfmikbmr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ehwqpu.com/gtrnznonnw.html

JS:   greet() { return "admin"; }
来源：http://hz.9152youxi.cn/gtzplsrzcd.html

TS:   greet(): string { return "admin"; }
来源：http://hz.andypj.xyz/gtbslmudlr.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhixingplan.top/gtywnpczoz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.xziqi.cn/gtgqfwzkwe.html

Ruby: def greet; "admin"; end
来源：http://hz.cdnleiting.top/gtfdimspdo.html

C#:   public override string Greet() => "admin";
来源：http://hz.bjfxy.top/gtmpicqtxf.html

[G07] 调用父类方法
来源：http://hz.nanxuanxn.top/gtenvlbozn.html

Py:   super().greet()
来源：http://hz.dashuyun.cn/gtfrrdkohs.html

PHP:  parent::greet();
来源：http://hz.iojbl.cn/gtxxvhutkk.html

JS:   super.greet();
来源：http://hz.xuetiantiany.cn/gtlctoxdql.html

TS:   super.greet();
来源：http://hz.nwbrower.top/gtbynaxzqr.html

Java: super.greet();
来源：http://hz.shuidangran.top/gtgquyrbfk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yanxiufei.cn/gtsrslkhuy.html

Ruby: super
来源：http://hz.cdnleiting.top/gthvkdaamz.html

C#:   base.Greet();
来源：http://hz.pycfn.com/gtrpdixypt.html

[G08] 静态方法与属性
来源：http://hz.ehwqpu.com/gtjcimkema.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhengqikj.top/gtaeggdxhm.html

PHP:  public static function f() {}
来源：http://hz.yj20258.top/gtdppmmybu.html

JS:   static f() {}
来源：http://hz.jinghuilouyu.cn/gtopizjmmc.html

TS:   static f(): void {}
来源：http://hz.daxiang520.top/gtcuqvglyx.html

Java: static void f() {}
来源：http://hz.tanke756.top/gtfhduvfav.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhijiandao.cn/gtbszeoxbw.html

Ruby: def self.f; end
来源：http://hz.hfpthk.cn/gtfmfwmyce.html

C#:   public static void F() {}
来源：http://hz.zhaomingkeji.xyz/gtdrbgrcsz.html

[G09] 接口 / 抽象类
来源：http://hz.smart0.xyz/gtprviukqj.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zhaomingkeji.xyz/gtoqtusueb.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jinqigufen.top/gtcvrjassn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ydzc1.top/gtllasguwu.html

TS:   interface Shape { area(): number; }
来源：http://hz.redwolf501.top/gtceokbbsn.html

Java: interface Shape { double area(); }
来源：http://hz.xinyue.icu/gtnolahrwm.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.svipenyu.cn/gttkyjbjsr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.meibo888.top/gtebjbiwsl.html

C#:   interface IShape { double Area(); }
来源：http://hz.hysaishi.cn/gtoftheqkm.html

[G10] 访问控制
来源：http://hz.tianlin.xyz/gtvpmdfvny.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.xylfe.cn/gtzkhximya.html

PHP:  public / protected / private
来源：http://hz.yanxiufei.cn/gtifcqwyym.html

JS:   #private 字段；其余公开
来源：http://hz.zhaomingkeji.xyz/gtjbmtpokv.html

TS:   public / protected / private
来源：http://hz.zhixingplan.top/gtlxbmiksm.html

Java: public / protected / private / 默认包级
来源：http://hz.sysykeji.top/gtbdljpxxi.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.guowangkeji.top/gtedoqfsoq.html

Ruby: public / protected / private
来源：http://hz.shanyushiyangkeji.top/gtdkvsotvh.html

C#:   public / protected / private / internal
来源：http://hz.zycfv.cn/gtqrllketx.html

[G11] getter / setter
来源：http://hz.hammf.cn/gtbycikcfn.html

Py:   @property 与 @x.setter
来源：http://hz.zhixingplan.top/gtfdzoayrh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.wangdashe.top/gtxqtudtog.html

JS:   get name() { return this._name; }
来源：http://hz.zhongyouzk.top/gtpprplhif.html

TS:   get name(): string { return this._name; }
来源：http://hz.xziqi.cn/gttkkxylsv.html

Java: public String getName() { return name; }
来源：http://hz.ehwqpu.com/gtavyjwgcu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.ehwqpu.com/gtbdpsbgxq.html

Ruby: attr_accessor :name
来源：http://hz.shanyushiyangtech.top/gtqffjxenj.html

C#:   public string Name { get; set; }
来源：http://hz.zhengqikj.top/gttyaepxcy.html

[G12] 对象转字符串
来源：http://hz.nanxuanxn.top/gtararblnl.html

Py:   def __str__(self): return self.name
来源：http://hz.9152youxi.cn/gtmrfchqeg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.gzhubu.top/gtddtjxqgj.html

JS:   toString() { return this.name; }
来源：http://hz.guowangkeji.top/gtesfslbqv.html

TS:   toString(): string { return this.name; }
来源：http://hz.yj202588.top/gtpcdvwmmx.html

Java: @Override public String toString() { return name; }
来源：http://hz.andypj.xyz/gthbvzcbcb.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.chenzaomai.com/gtjklmlily.html

Ruby: def to_s; @name; end
来源：http://hz.dashuyun.cn/gtfyakzlnc.html

C#:   public override string ToString() => Name;
来源：http://hz.shzxlz.cn/gtxnkqffet.html

[G13] 判断对象类型
来源：http://hz.ybcxt.top/gtewokagyb.html

Py:   isinstance(u, User)
来源：http://hz.svipenyu.cn/gtfqgplwtc.html

PHP:  $u instanceof User
来源：http://hz.jqgufenzy.top/gtvblifdma.html

JS:   u instanceof User
来源：http://hz.zhixingplan.top/gtxqbghrcp.html

TS:   u instanceof User
来源：http://hz.aizwys.cn/gtwmbufkcj.html

Java: u instanceof User
来源：http://hz.zhoulong.xyz/gtisertnsi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ybcxt.top/gttdxlwtye.html

Ruby: u.is_a?(User)
来源：http://hz.sufxvd.cn/gtnyaopgze.html

C#:   u is User
来源：http://hz.haohaochexian.top/gtkjddlnpi.html

[G14] 数据类 / record
来源：http://hz.zhengqikj.top/gtwfjebgwx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.ivvv.top/gtzvfghthi.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.haohaochexian.top/gtaslfztob.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jinqigfzy.top/gtpykjaaxt.html

TS:   type User = { name: string; age: number };
来源：http://hz.jianghu66.top/gtgabfkwav.html

Java: record User(String name, int age) {}
来源：http://hz.hammf.cn/gtnksydxfp.html

Go:   type User struct { Name string; Age int }
来源：http://hz.gogol.net.cn/gtbihdzuta.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.hywenlv.cn/gtxkaoiqba.html

C#:   record User(string Name, int Age);
来源：http://hz.zhaomingkeji.xyz/gtncedglii.html

[G15] 枚举
来源：http://hz.yvedp.cn/gtqbtqsidr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jiagoushi.top/gttbjqvsuh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.svipenyu.cn/gtkjunlsyu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yueranfly.top/gtzdjuukza.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.vqdsnc.cn/gtzxwnowgr.html

Java: enum Color { RED, GREEN }
来源：http://hz.quarkkingdee.top/gtjuvjkcro.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ybcxt.top/gtoytysgct.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ywan-chungtsiang.top/gtfnbermvl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sxryk.cn/gtpcfubmpu.html

[G16] 对象转数组 / 字典
来源：http://hz.zhaomingkeji.xyz/gtzfuckwut.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yuxming.cn/gtifudpjdg.html

PHP:  get_object_vars($obj);
来源：http://hz.jinghuilouyu.cn/gtykqexqqw.html

JS:   Object.entries(obj)
来源：http://hz.hfpthk.cn/gtrfvarwuf.html

TS:   Object.entries(obj)
来源：http://hz.zhaomingkeji.xyz/gtrbfzesvp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.cqqwz.cn/gtoqfhixrc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.haohaochexian.top/gtxphhxtqh.html

Ruby: obj.instance_variables
来源：http://hz.jinyuanbaomall.cn/gtiywllmdt.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.hammf.cn/gtbffxcoxg.html

================================================================================
来源：http://hz.pycfn.com/gttibvafzu.html

H. 异常与错误处理
来源：http://hz.jlsjyb.cn/gtvsvwtphm.html

================================================================================
来源：http://hz.xylfe.cn/gtyiwckqns.html

[H01] try / catch 基础
来源：http://hz.zhaomingkeji.xyz/gthgptpgei.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.hfpthk.cn/gtxzrvnjue.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.wangshuangyany.cn/gthwgxelge.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jinqigfzy.top/gtavfkdruw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yongpay.top/gtxhjevkou.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.chenlongwang.top/gtvixxdqpz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.ppjwa.cn/gtbeuawbra.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yangfankeji.com/gtdtxxgaco.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.meibo888.top/gtqsdzzmoe.html

[H02] finally / ensure 收尾
来源：http://hz.redwolf501.top/gtdjdedfyq.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.chenjidiqi.icu/gtqhwhrciz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.nanxuanxn.top/gtfxgqkhhm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yongpay.top/gtwipgwwbv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.tanke756.top/gtjgsaqgza.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.wangshuangyany.cn/gtnngflhnl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.redwolf501.top/gttiiodqwn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.smart0.xyz/gtqvlqucvr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jlsjyb.cn/gtwxudcmsp.html

[H03] 主动抛出异常
来源：http://hz.quarkkingdee.top/gtlvnnaqle.html

Py:   raise ValueError("错误信息")
来源：http://hz.dianchejie.cn/gtregniqdp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yonumen.top/gtpozbvyqx.html

JS:   throw new Error("错误信息");
来源：http://hz.guowangkeji.top/gtdcoroldt.html

TS:   throw new Error("错误信息");
来源：http://hz.zhijiandao.cn/gtixyzlrqr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yj20258.top/gtwbjjrnic.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.c1oappe.top/gtqxqtbnti.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.kuanghao11.cn/gtaqgsmvzb.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.hnqzz.top/gtqjraplie.html

[H04] 自定义异常类型
来源：http://hz.ehwqpu.com/gtmdwchhlk.html

Py:   class MyError(Exception): pass
来源：http://hz.hammf.cn/gtwybpffub.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zhiwuduotai.top/gtkhquyufk.html

JS:   class MyError extends Error {}
来源：http://hz.jqgfzy.top/gtlmgglzrj.html

TS:   class MyError extends Error {}
来源：http://hz.zhongyouzk.top/gtarfjdaip.html

Java: class MyException extends RuntimeException {}
来源：http://hz.ywan-chungtsiang.top/gtevhexhwt.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.sweek.top/gtqivjynbd.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhijiandao.cn/gtocjbmoqq.html

C#:   class MyException : Exception {}
来源：http://hz.zhijiandao.cn/gtfvvbqjno.html

[H05] 捕获特定类型
来源：http://hz.meibo888.top/gtgvwdxgmv.html

Py:   except ValueError as e:
来源：http://hz.ydjk.org.cn/gtguzbeaub.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jinghuilouyu.cn/gtcgogbcxb.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.hfpthk.cn/gtotuouqbv.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jyoumei.cn/gthyozzgqu.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.dianchejie.cn/gtcyearoje.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jlsjyb.cn/gtlvwnccre.html

Ruby: rescue ArgumentError => e
来源：http://hz.nanxinkj.top/gtyybzimde.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hfpthk.cn/gthcsxgxmh.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jianghu66.top/gtlyqdchab.html

Py:   value = d.get("k") or default
来源：http://hz.cqqwz.cn/gtpdetqswl.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.wangdashe.top/gtjdpwpfhf.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.xingfuxueyuan.xyz/gttfygtokv.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yj20258.top/gtvohevutf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ivvv.top/gtsgxvzuav.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.cqqwz.cn/gtgzyfrtqf.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jinghuilouyu.cn/gtfkukmqvp.html

C#:   obj?.A?.B ?? default
来源：http://hz.ppjwa.cn/gttgkawplg.html

[H07] 断言
来源：http://hz.zycfv.cn/gtruragdly.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yj20258.top/gttwtatjlz.html

PHP:  assert($x > 0);
来源：http://hz.yvedp.cn/gtlhzuuwmg.html

JS:   console.assert(x > 0);
来源：http://hz.xingfuxueyuan.xyz/gtkmekupgq.html

TS:   console.assert(x > 0);
来源：http://hz.tian-w.cn/gtqtkjnzti.html

Java: assert x > 0 : "必须为正";
来源：http://hz.kuanghao11.cn/gtwhahvhyy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.gotoacloud.top/gtlwrjhlon.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.ivvv.top/gtlompvhhj.html

C#:   Debug.Assert(x > 0);
来源：http://hz.dianchejie.cn/gtnvsooibz.html

[H08] 获取错误信息与堆栈
来源：http://hz.sysykeji.top/gtdfarwbdw.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ydzc1.top/gtdievzpbk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.feifeiyinyue.top/gtdsplvgss.html

JS:   e.message;  e.stack
来源：http://hz.sufxvd.cn/gtstwcmrxl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yuanzhike.top/gthogtizhn.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.shanyushiyangtech.top/gtizbqkewc.html

Go:   err.Error()
来源：http://hz.guowangkeji.top/gtegxmerwv.html

Ruby: e.message;  e.backtrace
来源：http://hz.yanxiufei.cn/gtxihiargb.html

C#:   e.Message;  e.StackTrace
来源：http://hz.sufxvd.cn/gtomjsanro.html

[H09] 带错误码的异常
来源：http://hz.vqdsnc.cn/gtjcknmgho.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.ydzc1.top/gtsgzzaefo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ydjk.org.cn/gtixjrswku.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.cucudq.cn/gtqypxmohr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.chenjidiqi.icu/gtlqvmbqae.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.ydzc1.top/gtpbxugbuo.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jinghuilouyu.cn/gtgjkzpztn.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jyoumei.cn/gtskkngofi.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.52xcode.cn/gtmewkqzat.html

[H10] 资源自动释放
来源：http://hz.yanxiufei.cn/gtrkqzekrr.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zhiwuduotai.top/gtxgqxxeks.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yongpay.top/gtmceiomky.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.wangdashe.top/gtafveoetm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.9152youxi.cn/gtlinakpvm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.316326.xyz/gtobeelcgd.html

Go:   defer f.Close()
来源：http://hz.cdnleiting.top/gtrqqomrgq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yj20258888.top/gttktpzwfg.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.52xcode.cn/gtcgsttyil.html


<!-- 参考信息 -->