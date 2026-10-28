代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://hz.zdqjudy.top/gtsargveme.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.xuetiantiany.cn/gtyqxtzruj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.nwbrower.top/gtyuzcnwbl.html

Ruby: File.exist?("a.txt")
来源：http://hz.hnxiangtu.top/gtbrcxztul.html

C#:   File.Exists("a.txt")
来源：http://hz.jinqigufen.top/gtgxodgxfm.html

[F06] 删除文件
来源：http://hz.sxryk.cn/gtzshbdnbt.html

Py:   os.remove("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtauezncmg.html

PHP:  unlink("a.txt");
来源：http://hz.gotoacloud.top/gtkovbhfms.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.pycfn.com/gtdznruytu.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.haohaochexian.top/gttrubskac.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.sxryk.cn/gtdggnvomx.html

Go:   os.Remove("a.txt")
来源：http://hz.jinqigfzy.top/gtopttbvrc.html

Ruby: File.delete("a.txt")
来源：http://hz.meibo888.top/gtyumoztyu.html

C#:   File.Delete("a.txt");
来源：http://hz.yj202588.top/gtdjfkxtbr.html

[F07] 创建目录（含多级）
来源：http://hz.dianchejie.cn/gtmrqhhzrc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jinqigufen.top/gtrpsdrehv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.gotoacloud.top/gtwyobqpok.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.sweek.top/gtpczkymms.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jinqigfzy.top/gtvstsfwtc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.dashuyun.cn/gtzfhnppph.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.ydzc1.top/gtpqifpbeh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.svipenyu.cn/gthrqayhhu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.tian-w.cn/gtvgptoklw.html

[F08] 遍历目录
来源：http://hz.52xcode.cn/gtkpprnfpn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.daria6918.cn/gtxzvrgsze.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.xuetiantiany.cn/gtgztwmqhb.html

JS:   fs.readdirSync("dir")
来源：http://hz.feifeiyinyue.top/gtqkdntxpv.html

TS:   fs.readdirSync("dir")
来源：http://hz.ybcxt.top/gtlrsmmhyd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.shzxlz.cn/gtapcsadog.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.cdnleiting.top/gthlqrjnsi.html

Ruby: Dir.children("dir")
来源：http://hz.jqgfzy.top/gtrkhzsoar.html

C#:   Directory.GetFiles("dir")
来源：http://hz.chenlongwang.top/gteoouftup.html

[F09] 获取文件大小
来源：http://hz.pycfn.com/gtlvbdzzah.html

Py:   os.path.getsize("a.txt")
来源：http://hz.cucudq.cn/gtvzgolgzu.html

PHP:  filesize("a.txt");
来源：http://hz.cqqwz.cn/gtscthytqb.html

JS:   fs.statSync("a.txt").size
来源：http://hz.dashuyun.cn/gtmbbiyssq.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yj20258.top/gtdbsgckcx.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jinghuilouyu.cn/gtnocubtwo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.quarkkingdee.top/gtsvqjitmt.html

Ruby: File.size("a.txt")
来源：http://hz.zhijiandao.cn/gtjmahviqv.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jiagoushi.top/gtqggbzdsc.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.nwbrower.top/gtzxmmyjrs.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.ehwqpu.com/gtidpusubb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jyoumei.cn/gtrftcxiqm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zdqjudy.top/gthwmakous.html

TS:   path.extname("a.txt")
来源：http://hz.chenzaomai.com/gtypprjfvy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.feifeiyinyue.top/gtdafycgrt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jinyuanbaomall.cn/gtqejfiseh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yj202588.top/gtmzezghvn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jinyuanbaomall.cn/gtwpydbnjv.html

[F11] 复制与移动文件
来源：http://hz.52xcode.cn/gtvysgtyyx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.feifeiyinyue.top/gtbamjclxy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zhoulong.xyz/gtozeebdfr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.gaohongyu789.top/gtlgybshga.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.gzhubu.top/gtagxqmnjt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.ydjk.org.cn/gtsxxtngrs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.dashuyun.cn/gtofiuzetq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zhengqikj.top/gtnlufrgho.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jianghu66.top/gtuygqyrno.html

[F12] CSV 读写
来源：http://hz.xuetiantiany.cn/gttyvpfwss.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.shanyushiyangtech.top/gtkgacekza.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jinghuilouyu.cn/gtcqobnhzb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yuanzhike.top/gtduzsnmgu.html

TS:   // 同上
来源：http://hz.jinyuanbaomall.cn/gtmsmczavc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.xziqi.cn/gtjngipjas.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.chenlongwang.top/gtndonqwit.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zhoulong.xyz/gtxsgmuvux.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zdqjudy.top/gtijhwhrpu.html

================================================================================
来源：http://hz.gogol.net.cn/gtzgsoivmt.html

G. 面向对象
来源：http://hz.shangyingyoupin.top/gtdjzzqayi.html

================================================================================
来源：http://hz.gotoacloud.top/gtzeazbaux.html

[G01] 定义类
来源：http://hz.xziqi.cn/gttsycwqcw.html

Py:   class User: pass
来源：http://hz.snrcjt.cn/gtpfeabkmb.html

PHP:  class User {}
来源：http://hz.pycfn.com/gtvpyfjbht.html

JS:   class User {}
来源：http://hz.haohaochexian.top/gteaahblkh.html

TS:   class User { name: string = ""; }
来源：http://hz.zycfv.cn/gtkgbkskzn.html

Java: class User {}
来源：http://hz.aibaodan.cn/gtsolbqkel.html

Go:   type User struct { Name string }
来源：http://hz.xinyue.icu/gtvdddycmw.html

Ruby: class User; end
来源：http://hz.tian-w.cn/gtjbcfjhxd.html

C#:   class User {}
来源：http://hz.dashuyun.cn/gtqocnolym.html

[G02] 构造函数
来源：http://hz.jinqigfzy.top/gtmzbovuxw.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.havefunace.top/gtgaftpwhr.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zhoulong.xyz/gtqvjzoekj.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yongpay.top/gtybvgbqew.html

TS:   constructor(public name: string) {}
来源：http://hz.ywan-chungtsiang.top/gtvzlnwxzm.html

Java: User(String name) { this.name = name; }
来源：http://hz.jinqigufen.top/gtpauigxgj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.sufxvd.cn/gtpnwkhdoy.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.feifeiyinyue.top/gthzaonzea.html

C#:   public User(string name) { Name = name; }
来源：http://hz.gogol.net.cn/gtfpnotklw.html

[G03] 实例属性
来源：http://hz.ywan-chungtsiang.top/gtbrabstjz.html

Py:   self.name = "x"
来源：http://hz.ppjwa.cn/gtkvfjohco.html

PHP:  public string $name = "x";
来源：http://hz.wangdashe.top/gtzueawqzq.html

JS:   this.name = "x";
来源：http://hz.sysykeji.top/gtwoqkyvvt.html

TS:   name: string = "x";
来源：http://hz.cdnleiting.top/gtzszbajyo.html

Java: private String name;
来源：http://hz.hammf.cn/gtcazznzqk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.dashuyun.cn/gtjlwubekc.html

Ruby: @name = "x"
来源：http://hz.gogol.net.cn/gtdbnkxzuc.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yj20258.top/gthcrokibq.html

[G04] 定义方法
来源：http://hz.ywan-chungtsiang.top/gtawicaloa.html

Py:   def greet(self): return self.name
来源：http://hz.jinghuilouyu.cn/gttqmpsjxk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yj20258.top/gtkcyztbux.html

JS:   greet() { return this.name; }
来源：http://hz.jiagoushi.top/gtebxbysgt.html

TS:   greet(): string { return this.name; }
来源：http://hz.redwolf501.top/gtuwmiwalv.html

Java: String greet() { return name; }
来源：http://hz.quarkkingdee.top/gtyxuvkmth.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.xylfe.cn/gtpghbgcht.html

Ruby: def greet; @name; end
来源：http://hz.yuanzhike.top/gthfccofha.html

C#:   public string Greet() => Name;
来源：http://hz.yvedp.cn/gtwzhooejg.html

[G05] 继承
来源：http://hz.ybcxt.top/gtwmilbsns.html

Py:   class Admin(User): pass
来源：http://hz.fengsongda.top/gtlufuljhz.html

PHP:  class Admin extends User {}
来源：http://hz.jinqigfzy.top/gtyncsdmxb.html

JS:   class Admin extends User {}
来源：http://hz.xuanzx.com/gtnnabjrrg.html

TS:   class Admin extends User {}
来源：http://hz.aibaodan.cn/gtbqcfumhe.html

Java: class Admin extends User {}
来源：http://hz.xuanzx.com/gtybazkpay.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.gogol.net.cn/gtavtwnwtc.html

Ruby: class Admin < User; end
来源：http://hz.haohaochexian.top/gtxgpkaaxk.html

C#:   class Admin : User {}
来源：http://hz.jiagoushi.top/gtxntpmaov.html

[G06] 重写方法
来源：http://hz.chenlongwang.top/gtcenkmsrg.html

Py:   def greet(self): return "admin"
来源：http://hz.birdmap.top/gtgugvimdg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.sysykeji.top/gtklmtdfvc.html

JS:   greet() { return "admin"; }
来源：http://hz.hnqzz.top/gtyszccziw.html

TS:   greet(): string { return "admin"; }
来源：http://hz.cqqwz.cn/gtzktyncyb.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yj202588.top/gtulfusllx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.smart0.xyz/gtnxpgylqh.html

Ruby: def greet; "admin"; end
来源：http://hz.tian-w.cn/gtxysbhfmn.html

C#:   public override string Greet() => "admin";
来源：http://hz.sufxvd.cn/gtfnvtbqof.html

[G07] 调用父类方法
来源：http://hz.birdmap.top/gtlyqdkwqo.html

Py:   super().greet()
来源：http://hz.zhixingplan.top/gtmbrihjxs.html

PHP:  parent::greet();
来源：http://hz.yangfankeji.com/gtlemiacod.html

JS:   super.greet();
来源：http://hz.gaohongyu789.top/gtxfwoxkpt.html

TS:   super.greet();
来源：http://hz.yj202588.top/gtvpaknums.html

Java: super.greet();
来源：http://hz.jyoumei.cn/gtdjgvufcj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.pengpengdd.cyou/gttgjnjzji.html

Ruby: super
来源：http://hz.tianlin.xyz/gtkrnrmdpx.html

C#:   base.Greet();
来源：http://hz.ydzc1.top/gtarrxfynp.html

[G08] 静态方法与属性
来源：http://hz.jianghu66.top/gtjukbzcfg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.tanke756.top/gtqgfgkjnn.html

PHP:  public static function f() {}
来源：http://hz.guannengcc.top/gtnicdzbkc.html

JS:   static f() {}
来源：http://hz.ppjwa.cn/gtzajsifno.html

TS:   static f(): void {}
来源：http://hz.sysykeji.top/gtpfvctcox.html

Java: static void f() {}
来源：http://hz.nanxuanxn.top/gtiidnnkwp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yonumen.top/gteslinyeo.html

Ruby: def self.f; end
来源：http://hz.sufxvd.cn/gtqddhrata.html

C#:   public static void F() {}
来源：http://hz.cdnleiting.top/gtvcpgocld.html

[G09] 接口 / 抽象类
来源：http://hz.ydjk.org.cn/gthtewbwlb.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.cashguo.top/gtgnydugbu.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zhongyouzk.top/gtgxvcetoy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.shangyingyoupin.top/gtuysdgcns.html

TS:   interface Shape { area(): number; }
来源：http://hz.wangshuangyany.cn/gtehroqkzw.html

Java: interface Shape { double area(); }
来源：http://hz.xinyue.icu/gtbxngcwih.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yuanzhike.top/gtdqxpskgl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhoulong.xyz/gtfamksvwg.html

C#:   interface IShape { double Area(); }
来源：http://hz.yj202588.top/gtfuybxmem.html

[G10] 访问控制
来源：http://hz.cheryme.top/gtmcdrgses.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jinyuanbaomall.cn/gtcsqrfsck.html

PHP:  public / protected / private
来源：http://hz.aibaodan.cn/gtfwzdcjpl.html

JS:   #private 字段；其余公开
来源：http://hz.gzhubu.top/gtbeefsgwz.html

TS:   public / protected / private
来源：http://hz.jianghu66.top/gtuaqvgels.html

Java: public / protected / private / 默认包级
来源：http://hz.yvedp.cn/gtgkjttbaq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zdqjudy.top/gtzuyxsorh.html

Ruby: public / protected / private
来源：http://hz.haohaochexian.top/gtywkjwike.html

C#:   public / protected / private / internal
来源：http://hz.tian-w.cn/gtkhnjuwdd.html

[G11] getter / setter
来源：http://hz.dianchejie.cn/gthrrkonzq.html

Py:   @property 与 @x.setter
来源：http://hz.zhongyouzk.top/gtnzebfavh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.tanke756.top/gtcxujnrpr.html

JS:   get name() { return this._name; }
来源：http://hz.sysykeji.top/gtvggytesa.html

TS:   get name(): string { return this._name; }
来源：http://hz.guannengcc.top/gtlepanuel.html

Java: public String getName() { return name; }
来源：http://hz.bjfxy.top/gtscesexkz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.0kj1m.cn/gtcecwxsqk.html

Ruby: attr_accessor :name
来源：http://hz.nwbrower.top/gtkflaudmi.html

C#:   public string Name { get; set; }
来源：http://hz.redwolf501.top/gtriwjtdlh.html

[G12] 对象转字符串
来源：http://hz.zhijiandao.cn/gtzlbafgpz.html

Py:   def __str__(self): return self.name
来源：http://hz.316326.xyz/gtieqadtxp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ywan-chungtsiang.top/gtvgplumhu.html

JS:   toString() { return this.name; }
来源：http://hz.316326.xyz/gtbjuldsih.html

TS:   toString(): string { return this.name; }
来源：http://hz.guannengcc.top/gtlmvghrup.html

Java: @Override public String toString() { return name; }
来源：http://hz.52xcode.cn/gtlfjxfkls.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.dashuyun.cn/gteyckqejt.html

Ruby: def to_s; @name; end
来源：http://hz.jqgufenzy.top/gtkozmyecm.html

C#:   public override string ToString() => Name;
来源：http://hz.ppjwa.cn/gtxmyfalot.html

[G13] 判断对象类型
来源：http://hz.316326.xyz/gtumaeifsj.html

Py:   isinstance(u, User)
来源：http://hz.dashuyun.cn/gtyqxwqgrl.html

PHP:  $u instanceof User
来源：http://hz.0kj1m.cn/gtfkzohzsc.html

JS:   u instanceof User
来源：http://hz.sysykeji.top/gtuqvkckwk.html

TS:   u instanceof User
来源：http://hz.jqgfzy.top/gtvrhgayvi.html

Java: u instanceof User
来源：http://hz.zhijiandao.cn/gtvlocfqxi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.andypj.xyz/gttehuulmv.html

Ruby: u.is_a?(User)
来源：http://hz.dashuyun.cn/gtscymyash.html

C#:   u is User
来源：http://hz.zhaomingkeji.xyz/gteyklbsvh.html

[G14] 数据类 / record
来源：http://hz.zdqjudy.top/gtgzkmpxjc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.andypj.xyz/gtzwyzluag.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jqgufenzy.top/gtlmtavepf.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhixingplan.top/gtwqpgjuia.html

TS:   type User = { name: string; age: number };
来源：http://hz.quarkkingdee.top/gtawuxmrdq.html

Java: record User(String name, int age) {}
来源：http://hz.xingfuxueyuan.xyz/gtironksos.html

Go:   type User struct { Name string; Age int }
来源：http://hz.hfpthk.cn/gthkhnxvgo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.chenjidiqi.icu/gthlybzaur.html

C#:   record User(string Name, int Age);
来源：http://hz.yueranfly.top/gtlyvfayzx.html

[G15] 枚举
来源：http://hz.chenjidiqi.icu/gtesxpezus.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.gzhubu.top/gtjdivnryt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhengqikj.top/gtqakwsymj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yueranfly.top/gtdxxhnkds.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cucudq.cn/gtpasojasf.html

Java: enum Color { RED, GREEN }
来源：http://hz.0kj1m.cn/gtbhsaiyou.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.chenjidiqi.icu/gtjfnxjoap.html

Ruby: Color = %i[red green].freeze
来源：http://hz.vqdsnc.cn/gtqbxunecl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.nwbrower.top/gtiuelvior.html

[G16] 对象转数组 / 字典
来源：http://hz.yj202588.top/gtbkaebwqx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yj20258888.top/gtejtjobyq.html

PHP:  get_object_vars($obj);
来源：http://hz.jianghu66.top/gtpxpvtsat.html

JS:   Object.entries(obj)
来源：http://hz.cqqwz.cn/gtwvihzkyo.html

TS:   Object.entries(obj)
来源：http://hz.pycfn.com/gtpmebiacu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.cheryme.top/gtpaorlcza.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.andypj.xyz/gtvbtxrklq.html

Ruby: obj.instance_variables
来源：http://hz.hammf.cn/gtouqeyglp.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.sxryk.cn/gtdeyezxab.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtaingmosi.html

H. 异常与错误处理
来源：http://hz.pycfn.com/gtnbsztcnj.html

================================================================================
来源：http://hz.chenlongwang.top/gtskeqxxlk.html

[H01] try / catch 基础
来源：http://hz.ybcxt.top/gtumkwtfsr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.dashuyun.cn/gtlhdbilxd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jlsjyb.cn/gtpsckbwir.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.c1oappe.top/gtjkumakvn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jqgfzy.top/gtfbwnnczc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.sxryk.cn/gtsmtazmio.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.tian-w.cn/gtdvbgbnzi.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.xinyue.icu/gtrvhpodfi.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.daria6918.cn/gtpyotceru.html

[H02] finally / ensure 收尾
来源：http://hz.shzxlz.cn/gtdfmarixe.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.xuanzx.com/gthphkevtn.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.nanxinkj.top/gtrxefuyqt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.ppjwa.cn/gtazjvqlnw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.chenjidiqi.icu/gtdtinnwpj.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yongpay.top/gtktqrmxlw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ehwqpu.com/gtvgrkfiik.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.meibo888.top/gtvyxcpkhf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.tianlin.xyz/gtaicnahzr.html

[H03] 主动抛出异常
来源：http://hz.cheryme.top/gtvxsazxqm.html

Py:   raise ValueError("错误信息")
来源：http://hz.hnqzz.top/gtasvnywik.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.ehwqpu.com/gtcaidyaat.html

JS:   throw new Error("错误信息");
来源：http://hz.nwbrower.top/gthgrvhoap.html

TS:   throw new Error("错误信息");
来源：http://hz.fzhhl.top/gtzididhlx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yuanzhike.top/gtqxytkqom.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yuanzhike.top/gtnxicuuqg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.sweek.top/gtgzdccodg.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.pycfn.com/gtecfffizl.html

[H04] 自定义异常类型
来源：http://hz.shzxlz.cn/gtohumnbpj.html

Py:   class MyError(Exception): pass
来源：http://hz.zycfv.cn/gtqasuryna.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zhoulong.xyz/gtkwknangz.html

JS:   class MyError extends Error {}
来源：http://hz.jiagoushi.top/gtoxnqejcd.html

TS:   class MyError extends Error {}
来源：http://hz.hnxiangtu.top/gtcblsoiyh.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yj20258888.top/gtwwcxhqjt.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.havefunace.top/gttfafesvv.html

Ruby: class MyError < StandardError; end
来源：http://hz.sysykeji.top/gtoruclsfk.html

C#:   class MyException : Exception {}
来源：http://hz.ppjwa.cn/gtetgqtyxu.html

[H05] 捕获特定类型
来源：http://hz.sweek.top/gttzzxkbov.html

Py:   except ValueError as e:
来源：http://hz.zhoulong.xyz/gtwamvbsso.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.guowangkeji.top/gtjpaufzmw.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.fzhhl.top/gtweluhzfw.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jyoumei.cn/gtzeznbmsb.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.hywenlv.cn/gtquvnczwi.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jiagoushi.top/gtiwathkjl.html

Ruby: rescue ArgumentError => e
来源：http://hz.redwolf501.top/gtbnqiqcze.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.ydjk.org.cn/gtacjdyxqi.html

[H06] 可选值 / 空值安全访问
来源：http://hz.smart0.xyz/gthihukkbt.html

Py:   value = d.get("k") or default
来源：http://hz.zhongyouzk.top/gtxzroroej.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.pycfn.com/gtbuutairk.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jinqigfzy.top/gtytdukhvm.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.hfpthk.cn/gtrskrdakm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.shanyushiyangtech.top/gtzzrcorhf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.shuidangran.top/gtwckmgjxc.html

Ruby: d&.dig(:a, :b)
来源：http://hz.9152youxi.cn/gtxbpeuqxd.html

C#:   obj?.A?.B ?? default
来源：http://hz.fzhhl.top/gtogernwpg.html

[H07] 断言
来源：http://hz.snrcjt.cn/gthywimrjx.html

Py:   assert x > 0, "必须为正"
来源：http://hz.ehwqpu.com/gtxtnwuozb.html

PHP:  assert($x > 0);
来源：http://hz.redwolf501.top/gtomqpzqsj.html

JS:   console.assert(x > 0);
来源：http://hz.havefunace.top/gtcnjwshdx.html

TS:   console.assert(x > 0);
来源：http://hz.xinyue.icu/gtnoydrxvi.html

Java: assert x > 0 : "必须为正";
来源：http://hz.shanyushiyangkeji.top/gtkrjuivth.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.shanyushiyangkeji.top/gtnqhbvxso.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.meibo888.top/gtglskqgeh.html

C#:   Debug.Assert(x > 0);
来源：http://hz.cheryme.top/gtodxnogxn.html

[H08] 获取错误信息与堆栈
来源：http://hz.chenzaomai.com/gtiashxbnf.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.0kj1m.cn/gtkbublwcx.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.nanxinkj.top/gtrtonvxlz.html

JS:   e.message;  e.stack
来源：http://hz.gogol.net.cn/gtpmkyiuke.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jinqigufen.top/gteggbjzrb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.wangshuangyany.cn/gtcaylfkly.html

Go:   err.Error()
来源：http://hz.nanxuanxn.top/gtduihriny.html

Ruby: e.message;  e.backtrace
来源：http://hz.xziqi.cn/gteomcbdqf.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jyoumei.cn/gtqrwoyflk.html

[H09] 带错误码的异常
来源：http://hz.0kj1m.cn/gtkrpswapu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hywenlv.cn/gtscxmsiek.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.tanke756.top/gtzbegihbu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.hnqzz.top/gtwbjynqtm.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.9152youxi.cn/gtaulaxtut.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.iojbl.cn/gttjxlrqnu.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.gaohongyu789.top/gtlqtcxbln.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jianghu66.top/gtyivgfpgq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yj20258888.top/gtkxvhmuap.html

[H10] 资源自动释放
来源：http://hz.shzxlz.cn/gtlzlquchg.html


<!-- 参考信息 -->