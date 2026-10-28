代发 wailian999

C#:   File.Exists("a.txt")
来源：http://hz.fzhhl.top/gtpphzjern.html

[F06] 删除文件
来源：http://hz.nwbrower.top/gtddmnevoi.html

Py:   os.remove("a.txt")
来源：http://hz.cucudq.cn/gtyxirqexz.html

PHP:  unlink("a.txt");
来源：http://hz.ydjk.org.cn/gtxikqvwhz.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.chenzaomai.com/gtdrdpswve.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.pycfn.com/gtunvhcuru.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.mhx1999.top/gttmwvmynq.html

Go:   os.Remove("a.txt")
来源：http://hz.zhixingplan.top/gtxmmveswe.html

Ruby: File.delete("a.txt")
来源：http://hz.52xcode.cn/gtdpnvjgyl.html

C#:   File.Delete("a.txt");
来源：http://hz.sxryk.cn/gtkalyltwj.html

[F07] 创建目录（含多级）
来源：http://hz.chenzaomai.com/gtrjysjjqe.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.c1oappe.top/gticvdkwcm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.ivvv.top/gtceajaqkx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.haohaochexian.top/gtxrxwidcw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.chenjidiqi.icu/gtiqefsdxt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jinyuanbaomall.cn/gttkarmdwc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yanxiufei.cn/gtulbrqtcm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.chenlongwang.top/gtpxtwhlyf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.pycfn.com/gtqkgjzdqp.html

[F08] 遍历目录
来源：http://hz.haohaochexian.top/gtecxrnggj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.xylfe.cn/gtqqznfxoh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.zhixingplan.top/gtzngpwmom.html

JS:   fs.readdirSync("dir")
来源：http://hz.xinyue.icu/gtqeoqqaqi.html

TS:   fs.readdirSync("dir")
来源：http://hz.yonumen.top/gtkchvrnig.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zhaomingkeji.xyz/gtjmmqefcr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zhoulong.xyz/gtbtrzlfln.html

Ruby: Dir.children("dir")
来源：http://hz.52xcode.cn/gtlqbsfshc.html

C#:   Directory.GetFiles("dir")
来源：http://hz.ydzc1.top/gttscwzyys.html

[F09] 获取文件大小
来源：http://hz.hongshengwenyu.top/gtaufsxztx.html

Py:   os.path.getsize("a.txt")
来源：http://hz.gogol.net.cn/gtvasjhsec.html

PHP:  filesize("a.txt");
来源：http://hz.kuanghao11.cn/gtqorlgsay.html

JS:   fs.statSync("a.txt").size
来源：http://hz.guannengcc.top/gttspdoupb.html

TS:   fs.statSync("a.txt").size
来源：http://hz.bjfxy.top/gtaxsuyejc.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.chenzaomai.com/gtyskkecjc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.fengsongda.top/gtnzmjowrm.html

Ruby: File.size("a.txt")
来源：http://hz.zhongyouzk.top/gtblzrxfmc.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.wangdashe.top/gtynvhabhb.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.cheryme.top/gtvyyeluzw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jinghuilouyu.cn/gtytnzcfcn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zhijiandao.cn/gtsytkjmur.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.hysaishi.cn/gtwnjiryvf.html

TS:   path.extname("a.txt")
来源：http://hz.xuanzx.com/gtfnpxyxlo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jinqigufen.top/gtnnmregij.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.haohaochexian.top/gtuznvqcmm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.fengsongda.top/gtxsmtqfab.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.fzhhl.top/gtyvupvodj.html

[F11] 复制与移动文件
来源：http://hz.hnqzz.top/gtzprjhifh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.shzxlz.cn/gtyxhymeqg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.chenzaomai.com/gtupegfcig.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhijiandao.cn/gthzgcntwd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cheryme.top/gtghdfhhhf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yj20258.top/gtxqfwwcpx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jqgufenzy.top/gttxjebmdu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.kuanghao11.cn/gtvqbktuwm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.cdnleiting.top/gtitlvxple.html

[F12] CSV 读写
来源：http://hz.feifeiyinyue.top/gtjmpnjdfy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.shanyushiyangtech.top/gtcrvnsogo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jqgufenzy.top/gtbrilwrxb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.tanke756.top/gtwghxaiji.html

TS:   // 同上
来源：http://hz.jinqigfzy.top/gtztkequir.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.52xcode.cn/gtzpdhpwmn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhengqikj.top/gtjckhvnum.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.gzhubu.top/gtjnmcaucr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.cqqwz.cn/gtudfefeij.html

================================================================================
来源：http://hz.yanxiufei.cn/gtrxgrotwo.html

G. 面向对象
来源：http://hz.tianlin.xyz/gtkzeomwsc.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtsolzwkxa.html

[G01] 定义类
来源：http://hz.haohaochexian.top/gtiioqyrrh.html

Py:   class User: pass
来源：http://hz.shangyingyoupin.top/gtzdipllbq.html

PHP:  class User {}
来源：http://hz.zhengqikj.top/gtqiejsjbj.html

JS:   class User {}
来源：http://hz.c1oappe.top/gtvvjtoeha.html

TS:   class User { name: string = ""; }
来源：http://hz.yuanzhike.top/gtuktvpgkh.html

Java: class User {}
来源：http://hz.jyoumei.cn/gtlakfhmsh.html

Go:   type User struct { Name string }
来源：http://hz.ydzc1.top/gtgpewcbyu.html

Ruby: class User; end
来源：http://hz.wangshuangyany.cn/gtjymaplwo.html

C#:   class User {}
来源：http://hz.ydjk.org.cn/gtmvwqxudr.html

[G02] 构造函数
来源：http://hz.yangfankeji.com/gtjupkmgnq.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.cqqwz.cn/gtnpbzizxp.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.tianlin.xyz/gtmdqsddss.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yuanzhike.top/gtpsbjqeum.html

TS:   constructor(public name: string) {}
来源：http://hz.zhongyouzk.top/gthihrcayu.html

Java: User(String name) { this.name = name; }
来源：http://hz.zhoulong.xyz/gtepnqhkrx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.316326.xyz/gtgataxuaf.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yongpay.top/gtaldxsyrd.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jqgfzy.top/gtogogdyvb.html

[G03] 实例属性
来源：http://hz.hongshengwenyu.top/gtukijzkvv.html

Py:   self.name = "x"
来源：http://hz.dianchejie.cn/gtlmstyesp.html

PHP:  public string $name = "x";
来源：http://hz.cdnleiting.top/gtmwqlbebm.html

JS:   this.name = "x";
来源：http://hz.shanyushiyangkeji.top/gtxwmczwku.html

TS:   name: string = "x";
来源：http://hz.andypj.xyz/gtkbcrzdcp.html

Java: private String name;
来源：http://hz.shanyushiyangkeji.top/gtqigvwzmj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hywenlv.cn/gtunqyuvva.html

Ruby: @name = "x"
来源：http://hz.birdmap.top/gtxmfqzrny.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.haohaochexian.top/gtuxlvandy.html

[G04] 定义方法
来源：http://hz.jinghuilouyu.cn/gtajvnqxop.html

Py:   def greet(self): return self.name
来源：http://hz.yuanzhike.top/gtfhsexezw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.ywan-chungtsiang.top/gtpahsnjuc.html

JS:   greet() { return this.name; }
来源：http://hz.zhijiandao.cn/gtpuaexaee.html

TS:   greet(): string { return this.name; }
来源：http://hz.gogol.net.cn/gtmofyvlgr.html

Java: String greet() { return name; }
来源：http://hz.tanke756.top/gtsydgbxaj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ppjwa.cn/gtptxfarqs.html

Ruby: def greet; @name; end
来源：http://hz.jqgufenzy.top/gtnezkwkzi.html

C#:   public string Greet() => Name;
来源：http://hz.iojbl.cn/gttfivicrp.html

[G05] 继承
来源：http://hz.jinghuilouyu.cn/gtdyyzbapt.html

Py:   class Admin(User): pass
来源：http://hz.havefunace.top/gtqxvwiafc.html

PHP:  class Admin extends User {}
来源：http://hz.hysaishi.cn/gtzhjwgwoe.html

JS:   class Admin extends User {}
来源：http://hz.jqgfzy.top/gtlrhvzxjb.html

TS:   class Admin extends User {}
来源：http://hz.xziqi.cn/gtesvpvrwm.html

Java: class Admin extends User {}
来源：http://hz.zhengqikj.top/gtgsgarfmi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yuanzhike.top/gtuxupmznk.html

Ruby: class Admin < User; end
来源：http://hz.yongpay.top/gtveyfkwxc.html

C#:   class Admin : User {}
来源：http://hz.cqqwz.cn/gtjkmtpppk.html

[G06] 重写方法
来源：http://hz.fengsongda.top/gtshfvzufl.html

Py:   def greet(self): return "admin"
来源：http://hz.bjfxy.top/gtddlfqfgz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.hnqzz.top/gtajaohlbh.html

JS:   greet() { return "admin"; }
来源：http://hz.shuidangran.top/gtnxbjpbao.html

TS:   greet(): string { return "admin"; }
来源：http://hz.nwbrower.top/gtsfhynrmc.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.sufxvd.cn/gtiscolmwk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.sxryk.cn/gtdqlelzic.html

Ruby: def greet; "admin"; end
来源：http://hz.shanyushiyangkeji.top/gtuoqivzqk.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhoulong.xyz/gtltygrtda.html

[G07] 调用父类方法
来源：http://hz.meibo888.top/gtvdwzikma.html

Py:   super().greet()
来源：http://hz.xingfuxueyuan.xyz/gtuhrmnwfd.html

PHP:  parent::greet();
来源：http://hz.hfpthk.cn/gtgzfkrzeo.html

JS:   super.greet();
来源：http://hz.tian-w.cn/gtsrxawxcq.html

TS:   super.greet();
来源：http://hz.yj202588.top/gtnydgmfkh.html

Java: super.greet();
来源：http://hz.jinghuilouyu.cn/gtnhiblkes.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.daria6918.cn/gtzblpbqkq.html

Ruby: super
来源：http://hz.shanyushiyangkeji.top/gtiujvwqpe.html

C#:   base.Greet();
来源：http://hz.jinqigfzy.top/gtkvxnprci.html

[G08] 静态方法与属性
来源：http://hz.wangshuangyany.cn/gtekicuovc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.sufxvd.cn/gtyousjaub.html

PHP:  public static function f() {}
来源：http://hz.svipenyu.cn/gtccyfbstq.html

JS:   static f() {}
来源：http://hz.jinyuanbaomall.cn/gtfpmathvo.html

TS:   static f(): void {}
来源：http://hz.yanxiufei.cn/gtzlgmxucg.html

Java: static void f() {}
来源：http://hz.havefunace.top/gtcamwljxr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.cheryme.top/gtwhsgudak.html

Ruby: def self.f; end
来源：http://hz.gaohongyu789.top/gthloenmev.html

C#:   public static void F() {}
来源：http://hz.hysaishi.cn/gtewwhbytl.html

[G09] 接口 / 抽象类
来源：http://hz.52xcode.cn/gtoqypoqhe.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.c1oappe.top/gtzckvjpzc.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jianghu66.top/gtknktjdfd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.guowangkeji.top/gtwigvdzou.html

TS:   interface Shape { area(): number; }
来源：http://hz.hfpthk.cn/gtzkmhuplh.html

Java: interface Shape { double area(); }
来源：http://hz.jianghu66.top/gthwpfqdfz.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yueranfly.top/gtkionvozk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yongpay.top/gtgurydxgk.html

C#:   interface IShape { double Area(); }
来源：http://hz.shanyushiyangtech.top/gttatdnxqm.html

[G10] 访问控制
来源：http://hz.gaohongyu789.top/gtmhwaxhop.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhijiandao.cn/gtqeiyudem.html

PHP:  public / protected / private
来源：http://hz.yj20258.top/gtdwssiadp.html

JS:   #private 字段；其余公开
来源：http://hz.yj202588.top/gtassovlzn.html

TS:   public / protected / private
来源：http://hz.xinyue.icu/gtsqvfgrnu.html

Java: public / protected / private / 默认包级
来源：http://hz.ydzc1.top/gtcdcimwvl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.hywenlv.cn/gtuestxakv.html

Ruby: public / protected / private
来源：http://hz.pycfn.com/gtlqdxvyar.html

C#:   public / protected / private / internal
来源：http://hz.jiagoushi.top/gtxobdqtir.html

[G11] getter / setter
来源：http://hz.cqqwz.cn/gtxusmxubl.html

Py:   @property 与 @x.setter
来源：http://hz.shangyingyoupin.top/gtvbyyoywa.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.tian-w.cn/gtokwwjcov.html

JS:   get name() { return this._name; }
来源：http://hz.aizwys.cn/gtywyznbvi.html

TS:   get name(): string { return this._name; }
来源：http://hz.jyoumei.cn/gtgqsdqprf.html

Java: public String getName() { return name; }
来源：http://hz.vqdsnc.cn/gtgwaahlai.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.316326.xyz/gtbaxcatmr.html

Ruby: attr_accessor :name
来源：http://hz.quarkkingdee.top/gtdbmiohuk.html

C#:   public string Name { get; set; }
来源：http://hz.yonumen.top/gtojdhuocy.html

[G12] 对象转字符串
来源：http://hz.yangfankeji.com/gtelkirgge.html

Py:   def __str__(self): return self.name
来源：http://hz.shanyushiyangkeji.top/gtsujawxdq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ydzc1.top/gtoblndama.html

JS:   toString() { return this.name; }
来源：http://hz.tianlin.xyz/gtddqblwmc.html

TS:   toString(): string { return this.name; }
来源：http://hz.hywenlv.cn/gtwkceuneb.html

Java: @Override public String toString() { return name; }
来源：http://hz.gzhubu.top/gthjppaaef.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhengqikj.top/gtlqbkwqvb.html

Ruby: def to_s; @name; end
来源：http://hz.redwolf501.top/gtawtnnmgo.html

C#:   public override string ToString() => Name;
来源：http://hz.zhoulong.xyz/gtvjefvrtv.html

[G13] 判断对象类型
来源：http://hz.jyoumei.cn/gtiojcrayx.html

Py:   isinstance(u, User)
来源：http://hz.jinyuanbaomall.cn/gtvydhtriu.html

PHP:  $u instanceof User
来源：http://hz.gotoacloud.top/gtnajhbreg.html

JS:   u instanceof User
来源：http://hz.xingfuxueyuan.xyz/gtbwwqwcib.html

TS:   u instanceof User
来源：http://hz.52xcode.cn/gtxikbcldy.html

Java: u instanceof User
来源：http://hz.jlsjyb.cn/gtwslmrtww.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ydjk.org.cn/gtfwrcrcft.html

Ruby: u.is_a?(User)
来源：http://hz.chenjidiqi.icu/gtaxfrhxcv.html

C#:   u is User
来源：http://hz.yuxming.cn/gtjfdjwfzp.html

[G14] 数据类 / record
来源：http://hz.aizwys.cn/gtukqjcoew.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.ydjk.org.cn/gttamkgziq.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.daria6918.cn/gtbouhtlpu.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.iojbl.cn/gtizkcaiqi.html

TS:   type User = { name: string; age: number };
来源：http://hz.nwbrower.top/gtydmuqmin.html

Java: record User(String name, int age) {}
来源：http://hz.andypj.xyz/gthaalrsvc.html

Go:   type User struct { Name string; Age int }
来源：http://hz.wangshuangyany.cn/gtdbgikmoo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.52xcode.cn/gtpcwzwomb.html

C#:   record User(string Name, int Age);
来源：http://hz.jinqigfzy.top/gtataynbfr.html

[G15] 枚举
来源：http://hz.cdnleiting.top/gtttbkbvos.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yongpay.top/gtbiujuxpv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.cashguo.top/gtvqsyvfzk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yj20258.top/gtjcrmksxy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ybcxt.top/gtfuvnfsvo.html

Java: enum Color { RED, GREEN }
来源：http://hz.wangdashe.top/gtnuigpjbm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.haohaochexian.top/gtnzxhbbdm.html

Ruby: Color = %i[red green].freeze
来源：http://hz.kuanghao11.cn/gtukjvwnjk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jinyuanbaomall.cn/gtlhjeozgv.html

[G16] 对象转数组 / 字典
来源：http://hz.sxryk.cn/gtfgypzmsb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.ydzc1.top/gtzntssejq.html

PHP:  get_object_vars($obj);
来源：http://hz.yonumen.top/gtanhwagni.html

JS:   Object.entries(obj)
来源：http://hz.nanxinkj.top/gthzzhdhkf.html

TS:   Object.entries(obj)
来源：http://hz.dashuyun.cn/gtjaafgdgu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhengqikj.top/gtgqxxwftn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jinghuilouyu.cn/gtoimtnrks.html

Ruby: obj.instance_variables
来源：http://hz.jyoumei.cn/gtplgdxsmj.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.xylfe.cn/gtezslspuo.html

================================================================================
来源：http://hz.nwbrower.top/gtwrokvgfv.html

H. 异常与错误处理
来源：http://hz.shzxlz.cn/gtacwzhtsn.html

================================================================================
来源：http://hz.redwolf501.top/gtvoncrvgn.html

[H01] try / catch 基础
来源：http://hz.ywan-chungtsiang.top/gtujhsdzrm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yuxming.cn/gtaqvlvqkn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zhixingplan.top/gtdblkwjnd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.ywan-chungtsiang.top/gtrbqgxltp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.redwolf501.top/gtjrjuwlfl.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.pycfn.com/gteditjfyx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jinyuanbaomall.cn/gtqbvdkzhh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yj20258.top/gtqpbvtroq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zdqjudy.top/gtjtrvzwlo.html

[H02] finally / ensure 收尾
来源：http://hz.ywan-chungtsiang.top/gtkunjzfac.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.smart0.xyz/gthnkvuklo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.dianchejie.cn/gtysuqvybq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jiagoushi.top/gtmowtycrn.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.mhx1999.top/gtetkgccyo.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.cdnleiting.top/gtsrkravep.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.snrcjt.cn/gtsszabvzx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.daria6918.cn/gtwmwvwfse.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yvedp.cn/gtkatmenal.html

[H03] 主动抛出异常
来源：http://hz.yj20258.top/gtgjovtxnb.html

Py:   raise ValueError("错误信息")
来源：http://hz.xuetiantiany.cn/gtunceqytp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.dashuyun.cn/gtnvlxgazg.html

JS:   throw new Error("错误信息");
来源：http://hz.andypj.xyz/gtdybhfybt.html

TS:   throw new Error("错误信息");
来源：http://hz.jqgufenzy.top/gtxxkqcdoh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.nwbrower.top/gticwranah.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.sweek.top/gthhaaarfi.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.iojbl.cn/gtbfanjlee.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.hongshengwenyu.top/gtualjvewv.html

[H04] 自定义异常类型
来源：http://hz.c1oappe.top/gtbwfzbzpc.html

Py:   class MyError(Exception): pass
来源：http://hz.yangfankeji.com/gtrowoqsyb.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.wangdashe.top/gtlkrbuerk.html

JS:   class MyError extends Error {}
来源：http://hz.9152youxi.cn/gtmvosdmrz.html

TS:   class MyError extends Error {}
来源：http://hz.shangyingyoupin.top/gtultltkri.html

Java: class MyException extends RuntimeException {}
来源：http://hz.sxryk.cn/gtkukyxzri.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.hnxiangtu.top/gtmkcatwhx.html

Ruby: class MyError < StandardError; end
来源：http://hz.yuxming.cn/gttxcmelhv.html

C#:   class MyException : Exception {}
来源：http://hz.jqgfzy.top/gtggnflqkc.html

[H05] 捕获特定类型
来源：http://hz.zhiwuduotai.top/gtazxahrvp.html

Py:   except ValueError as e:
来源：http://hz.snrcjt.cn/gtfdvyehiz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.cheryme.top/gtgryfkgwi.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.feifeiyinyue.top/gtybikdfgm.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yuanzhike.top/gtlmqxzmdz.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.hnxiangtu.top/gtvpzrfren.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.dashuyun.cn/gtzaailykd.html

Ruby: rescue ArgumentError => e
来源：http://hz.cheryme.top/gtrotzlvfn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhijiandao.cn/gtggxyczhy.html

[H06] 可选值 / 空值安全访问
来源：http://hz.smart0.xyz/gtalmtzzmw.html

Py:   value = d.get("k") or default
来源：http://hz.316326.xyz/gtfgxrdyux.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jiagoushi.top/gtbevtzoys.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.meibo888.top/gtcephcmah.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.hywenlv.cn/gtyfqnwfdt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhongyouzk.top/gtejxajryt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.snrcjt.cn/gtpintzbof.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jyoumei.cn/gtufknbinb.html

C#:   obj?.A?.B ?? default
来源：http://hz.cucudq.cn/gtymkvefhm.html

[H07] 断言
来源：http://hz.xingfuxueyuan.xyz/gtdnjjsgem.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zhiwuduotai.top/gtbdllbgsr.html

PHP:  assert($x > 0);
来源：http://hz.yonumen.top/gtmieanakx.html

JS:   console.assert(x > 0);
来源：http://hz.pycfn.com/gthaevmqex.html

TS:   console.assert(x > 0);
来源：http://hz.zhoulong.xyz/gtjugtnytf.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yvedp.cn/gtbpwsxxpp.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jyoumei.cn/gtxzrmlcqr.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jiagoushi.top/gtuzycugml.html

C#:   Debug.Assert(x > 0);
来源：http://hz.guannengcc.top/gtzzoasqmu.html

[H08] 获取错误信息与堆栈
来源：http://hz.nanxuanxn.top/gtrfwiiqck.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.hnxiangtu.top/gtgnymgmfn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.gzhubu.top/gtnckdaqvb.html

JS:   e.message;  e.stack
来源：http://hz.hnxiangtu.top/gtfeotysir.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.dianchejie.cn/gtpcpbiprn.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zdqjudy.top/gtxguqhsmq.html

Go:   err.Error()
来源：http://hz.gaohongyu789.top/gtfmsvexfr.html

Ruby: e.message;  e.backtrace
来源：http://hz.zhiwuduotai.top/gtwkfvgqyy.html

C#:   e.Message;  e.StackTrace
来源：http://hz.svipenyu.cn/gtocurbuqw.html

[H09] 带错误码的异常
来源：http://hz.xinyue.icu/gtcjzyzcui.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.chenzaomai.com/gthfmjqiuq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jlsjyb.cn/gtbqmzmjcv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.sufxvd.cn/gtgejrnlbf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.hfpthk.cn/gtjvaoqsmm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jinqigufen.top/gtadkzmhts.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.dashuyun.cn/gtjqkpkuww.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yanxiufei.cn/gttzcyodam.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.nwbrower.top/gthhsnbnwz.html

[H10] 资源自动释放
来源：http://hz.wangshuangyany.cn/gtiqqfqtrm.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yj20258888.top/gtjceggixz.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.9152youxi.cn/gtmolojwwq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.9152youxi.cn/gtpgpdcjla.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cashguo.top/gttqmlvdlq.html


<!-- 参考信息 -->