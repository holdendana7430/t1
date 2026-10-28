代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.havefunace.top/gtfblownlp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jinyuanbaomall.cn/gtbtpigcyv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.daxiang520.top/gtoiyiryww.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.ivvv.top/gtgyejpbtc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.andypj.xyz/gtvsnayupg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.fengsongda.top/gtzhbwbmmx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.guowangkeji.top/gturksnnsl.html

[F08] 遍历目录
来源：http://hz.shanyushiyangkeji.top/gtrvsdbzmk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.haohaochexian.top/gtlnerlmjp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yj20258.top/gtcuypfobr.html

JS:   fs.readdirSync("dir")
来源：http://hz.jinyuanbaomall.cn/gtiqugkidu.html

TS:   fs.readdirSync("dir")
来源：http://hz.hnxiangtu.top/gtfkhbsqkh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.gotoacloud.top/gthnkqerxd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.pycfn.com/gtwwqykpkv.html

Ruby: Dir.children("dir")
来源：http://hz.quarkkingdee.top/gtjzvimdey.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zycfv.cn/gtogvvhwfd.html

[F09] 获取文件大小
来源：http://hz.jyoumei.cn/gtachzmrqb.html

Py:   os.path.getsize("a.txt")
来源：http://hz.sxryk.cn/gtgaqmcghe.html

PHP:  filesize("a.txt");
来源：http://hz.cashguo.top/gthalpnmqd.html

JS:   fs.statSync("a.txt").size
来源：http://hz.snrcjt.cn/gttmxawjjb.html

TS:   fs.statSync("a.txt").size
来源：http://hz.daria6918.cn/gtvkjjyanh.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.tian-w.cn/gtmycygykr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.cdnleiting.top/gtjwowjjdr.html

Ruby: File.size("a.txt")
来源：http://hz.wangdashe.top/gtzotskppo.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jinyuanbaomall.cn/gtufdfhzan.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.tanke756.top/gtjjdksbwx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.havefunace.top/gtmeairoio.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.sufxvd.cn/gtbovzzloq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.hongshengwenyu.top/gtlttpbtdt.html

TS:   path.extname("a.txt")
来源：http://hz.xuanzx.com/gtyuciiwfm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jinqigufen.top/gtgwdxmibn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.andypj.xyz/gtdbueiips.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.haohaochexian.top/gtijjsnddw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.shanyushiyangkeji.top/gtootzmggv.html

[F11] 复制与移动文件
来源：http://hz.xuanzx.com/gtwkbfusah.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.9152youxi.cn/gtyguzjnsz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.gaohongyu789.top/gtfzyswskv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xingfuxueyuan.xyz/gtjzkftzfq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hysaishi.cn/gthbpcvssm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.ydjk.org.cn/gtefqewqxb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.hnxiangtu.top/gtotiiyhmm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.chenjidiqi.icu/gtulmdyvje.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.pengpengdd.cyou/gtjzbhaiya.html

[F12] CSV 读写
来源：http://hz.shangyingyoupin.top/gtvvesweqz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.hnqzz.top/gtnotdnbsq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yonumen.top/gtltjgtrkx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.tanke756.top/gtytmyywxj.html

TS:   // 同上
来源：http://hz.cheryme.top/gttlaibdby.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.hammf.cn/gtwfrfxjhr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.wangdashe.top/gtlqubyxlc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.xylfe.cn/gtgneogtwj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.hfpthk.cn/gtbrcwevew.html

================================================================================
来源：http://hz.ehwqpu.com/gtnrbrtadj.html

G. 面向对象
来源：http://hz.chenzaomai.com/gtmrfhepmz.html

================================================================================
来源：http://hz.redwolf501.top/gtbatvmbmi.html

[G01] 定义类
来源：http://hz.zhijiandao.cn/gtjnsjpwod.html

Py:   class User: pass
来源：http://hz.yuxming.cn/gtinovlxey.html

PHP:  class User {}
来源：http://hz.cheryme.top/gtjfchspcw.html

JS:   class User {}
来源：http://hz.jqgfzy.top/gthmvrarjw.html

TS:   class User { name: string = ""; }
来源：http://hz.wangdashe.top/gthvjymayd.html

Java: class User {}
来源：http://hz.zhijiandao.cn/gtmlbtjwpj.html

Go:   type User struct { Name string }
来源：http://hz.aibaodan.cn/gtmrwxcsrl.html

Ruby: class User; end
来源：http://hz.tianlin.xyz/gtrsgqupdm.html

C#:   class User {}
来源：http://hz.zdqjudy.top/gtnozbxixn.html

[G02] 构造函数
来源：http://hz.sweek.top/gtsoynzrjv.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.guowangkeji.top/gtnsjtdntc.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zhiwuduotai.top/gttxwcrujf.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.shuidangran.top/gtylligyho.html

TS:   constructor(public name: string) {}
来源：http://hz.aibaodan.cn/gtdjxsuszq.html

Java: User(String name) { this.name = name; }
来源：http://hz.daxiang520.top/gtahhecdob.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.tanke756.top/gtrhfapkag.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.daxiang520.top/gtprkazcbj.html

C#:   public User(string name) { Name = name; }
来源：http://hz.tianlin.xyz/gtawgkfhqi.html

[G03] 实例属性
来源：http://hz.feifeiyinyue.top/gtknaxjruz.html

Py:   self.name = "x"
来源：http://hz.yanxiufei.cn/gtnqsiotnr.html

PHP:  public string $name = "x";
来源：http://hz.haohaochexian.top/gtcwavhktu.html

JS:   this.name = "x";
来源：http://hz.ppjwa.cn/gtkdtvcqqy.html

TS:   name: string = "x";
来源：http://hz.jianghu66.top/gtbqfujfjd.html

Java: private String name;
来源：http://hz.xuanzx.com/gtujejqhpx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.quarkkingdee.top/gteyucpmuj.html

Ruby: @name = "x"
来源：http://hz.tanke756.top/gtbzqanriv.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hammf.cn/gtyrreuxpv.html

[G04] 定义方法
来源：http://hz.cashguo.top/gtjgcnflqq.html

Py:   def greet(self): return self.name
来源：http://hz.pengpengdd.cyou/gtottxhfqy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.svipenyu.cn/gtpopsxdjn.html

JS:   greet() { return this.name; }
来源：http://hz.fzhhl.top/gtcabvqotj.html

TS:   greet(): string { return this.name; }
来源：http://hz.hnqzz.top/gtgnyzschg.html

Java: String greet() { return name; }
来源：http://hz.gogol.net.cn/gtlsxpsfdn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hfpthk.cn/gthhslvjxt.html

Ruby: def greet; @name; end
来源：http://hz.zdqjudy.top/gtyyjywukc.html

C#:   public string Greet() => Name;
来源：http://hz.dianchejie.cn/gtzdcfzcfb.html

[G05] 继承
来源：http://hz.gogol.net.cn/gtduzzowwm.html

Py:   class Admin(User): pass
来源：http://hz.andypj.xyz/gtdxrgmrlw.html

PHP:  class Admin extends User {}
来源：http://hz.0kj1m.cn/gtbbukpuvs.html

JS:   class Admin extends User {}
来源：http://hz.mhx1999.top/gtgxfmejll.html

TS:   class Admin extends User {}
来源：http://hz.ywan-chungtsiang.top/gtuhutsddh.html

Java: class Admin extends User {}
来源：http://hz.cqqwz.cn/gtxjxpzlmc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.shanyushiyangtech.top/gtlaquzake.html

Ruby: class Admin < User; end
来源：http://hz.svipenyu.cn/gtrihlfcjp.html

C#:   class Admin : User {}
来源：http://hz.sweek.top/gtnrabowsr.html

[G06] 重写方法
来源：http://hz.0kj1m.cn/gttfirgbgv.html

Py:   def greet(self): return "admin"
来源：http://hz.sweek.top/gtwxaofwup.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ydzc1.top/gtansiqyly.html

JS:   greet() { return "admin"; }
来源：http://hz.mhx1999.top/gtdglyxuvc.html

TS:   greet(): string { return "admin"; }
来源：http://hz.shuidangran.top/gtgbxibpzr.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.aibaodan.cn/gtwvitfjeo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.xuanzx.com/gtakfdochx.html

Ruby: def greet; "admin"; end
来源：http://hz.fzhhl.top/gtxrilyuzb.html

C#:   public override string Greet() => "admin";
来源：http://hz.jlsjyb.cn/gtglcissto.html

[G07] 调用父类方法
来源：http://hz.zhijiandao.cn/gtxbiskmis.html

Py:   super().greet()
来源：http://hz.redwolf501.top/gtqoosnfth.html

PHP:  parent::greet();
来源：http://hz.xingfuxueyuan.xyz/gtjxpbzcbt.html

JS:   super.greet();
来源：http://hz.yj20258.top/gtwcmfbxbd.html

TS:   super.greet();
来源：http://hz.hnqzz.top/gtylwjfhdo.html

Java: super.greet();
来源：http://hz.sxryk.cn/gtpabksugq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jinqigufen.top/gtmvvvoiyi.html

Ruby: super
来源：http://hz.havefunace.top/gtbgkzfmvb.html

C#:   base.Greet();
来源：http://hz.hnqzz.top/gtgwxanpra.html

[G08] 静态方法与属性
来源：http://hz.jianghu66.top/gtfgiufzcq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.sweek.top/gtateyxrxs.html

PHP:  public static function f() {}
来源：http://hz.gzhubu.top/gtbdfpbpmg.html

JS:   static f() {}
来源：http://hz.ydzc1.top/gtrmigzbci.html

TS:   static f(): void {}
来源：http://hz.xinyue.icu/gtgzchpzdx.html

Java: static void f() {}
来源：http://hz.xziqi.cn/gtuueamsco.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.gogol.net.cn/gtmhyqiqcz.html

Ruby: def self.f; end
来源：http://hz.sufxvd.cn/gtdafpizje.html

C#:   public static void F() {}
来源：http://hz.gogol.net.cn/gtnjpfcsbl.html

[G09] 接口 / 抽象类
来源：http://hz.hnxiangtu.top/gthpbmnpwd.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.dashuyun.cn/gtjetjbjag.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.nanxinkj.top/gtxxyqanlq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.fzhhl.top/gtoojcbvbq.html

TS:   interface Shape { area(): number; }
来源：http://hz.jqgufenzy.top/gtzhuhxshq.html

Java: interface Shape { double area(); }
来源：http://hz.pengpengdd.cyou/gtcsegybdn.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jinyuanbaomall.cn/gtuhujyphn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.wangshuangyany.cn/gtklmimhww.html

C#:   interface IShape { double Area(); }
来源：http://hz.shanyushiyangkeji.top/gtyhqrojwq.html

[G10] 访问控制
来源：http://hz.kuanghao11.cn/gtrktjycoa.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.ybcxt.top/gthgvzvvcp.html

PHP:  public / protected / private
来源：http://hz.vqdsnc.cn/gtzaujygbq.html

JS:   #private 字段；其余公开
来源：http://hz.yangfankeji.com/gtpuwyhbam.html

TS:   public / protected / private
来源：http://hz.svipenyu.cn/gttkwtgxsh.html

Java: public / protected / private / 默认包级
来源：http://hz.hnqzz.top/gtxhitewve.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.9152youxi.cn/gtfolwtzis.html

Ruby: public / protected / private
来源：http://hz.xinyue.icu/gtqvfladyo.html

C#:   public / protected / private / internal
来源：http://hz.zhaomingkeji.xyz/gtkrbwtgys.html

[G11] getter / setter
来源：http://hz.daria6918.cn/gtscpeevki.html

Py:   @property 与 @x.setter
来源：http://hz.chenjidiqi.icu/gtsquefmww.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.shuidangran.top/gtxofjztwk.html

JS:   get name() { return this._name; }
来源：http://hz.9152youxi.cn/gtjrzztcod.html

TS:   get name(): string { return this._name; }
来源：http://hz.jiagoushi.top/gttdjvctla.html

Java: public String getName() { return name; }
来源：http://hz.ppjwa.cn/gtevmaupwz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.dashuyun.cn/gtoohbzohu.html

Ruby: attr_accessor :name
来源：http://hz.chenlongwang.top/gtswsyyhdh.html

C#:   public string Name { get; set; }
来源：http://hz.feifeiyinyue.top/gtgdhffgma.html

[G12] 对象转字符串
来源：http://hz.jqgufenzy.top/gtbiggnelh.html

Py:   def __str__(self): return self.name
来源：http://hz.hywenlv.cn/gtyshmykmr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.daria6918.cn/gtcnooorfv.html

JS:   toString() { return this.name; }
来源：http://hz.gaohongyu789.top/gtjrkpfdib.html

TS:   toString(): string { return this.name; }
来源：http://hz.yonumen.top/gtxcftznww.html

Java: @Override public String toString() { return name; }
来源：http://hz.hnxiangtu.top/gtdnhihqxt.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.gzhubu.top/gtjelildre.html

Ruby: def to_s; @name; end
来源：http://hz.hnxiangtu.top/gtdgzgboeb.html

C#:   public override string ToString() => Name;
来源：http://hz.tianlin.xyz/gtfuvjkwyb.html

[G13] 判断对象类型
来源：http://hz.tian-w.cn/gtrbqekvfg.html

Py:   isinstance(u, User)
来源：http://hz.ywan-chungtsiang.top/gtvkzngjuq.html

PHP:  $u instanceof User
来源：http://hz.jqgufenzy.top/gtsylchkdu.html

JS:   u instanceof User
来源：http://hz.zhongyouzk.top/gtdkpgyphq.html

TS:   u instanceof User
来源：http://hz.hysaishi.cn/gtddulxfad.html

Java: u instanceof User
来源：http://hz.yongpay.top/gtyclpctum.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yj202588.top/gtytrzyxdk.html

Ruby: u.is_a?(User)
来源：http://hz.tanke756.top/gtubgakjtt.html

C#:   u is User
来源：http://hz.ybcxt.top/gtrsvalksh.html

[G14] 数据类 / record
来源：http://hz.ivvv.top/gtxzesvidp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.pengpengdd.cyou/gtpvtfqzsb.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zhiwuduotai.top/gtstvlegqb.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.nanxinkj.top/gthckpjpje.html

TS:   type User = { name: string; age: number };
来源：http://hz.jqgufenzy.top/gtylqujnac.html

Java: record User(String name, int age) {}
来源：http://hz.redwolf501.top/gtdcojoute.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yangfankeji.com/gtjantnyas.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.aizwys.cn/gtjhrwrywj.html

C#:   record User(string Name, int Age);
来源：http://hz.shuidangran.top/gtnzmbnjdm.html

[G15] 枚举
来源：http://hz.hammf.cn/gtapwdrmxe.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.bjfxy.top/gtkymbubxp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yvedp.cn/gtbcvgyctv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.gogol.net.cn/gtzrqkrjcl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.gaohongyu789.top/gtktyizwbo.html

Java: enum Color { RED, GREEN }
来源：http://hz.gogol.net.cn/gtcmvmiaob.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.quarkkingdee.top/gtatadtsnp.html

Ruby: Color = %i[red green].freeze
来源：http://hz.guowangkeji.top/gtflxtsehb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xylfe.cn/gtingwqrlj.html

[G16] 对象转数组 / 字典
来源：http://hz.shangyingyoupin.top/gtimuxhgkn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.pengpengdd.cyou/gtuqswuvow.html

PHP:  get_object_vars($obj);
来源：http://hz.daxiang520.top/gtozlmlrjb.html

JS:   Object.entries(obj)
来源：http://hz.ybcxt.top/gtdmpylsdb.html

TS:   Object.entries(obj)
来源：http://hz.pycfn.com/gtwgpvkhsp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.wangshuangyany.cn/gtbrkhnxev.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.haohaochexian.top/gtskbrgteh.html

Ruby: obj.instance_variables
来源：http://hz.kuanghao11.cn/gtlfrdlomm.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jinqigfzy.top/gtjsdqbyjp.html

================================================================================
来源：http://hz.yangfankeji.com/gttsxakyqd.html

H. 异常与错误处理
来源：http://hz.yj20258.top/gtykkgtymb.html

================================================================================
来源：http://hz.cucudq.cn/gtoxgxhtwi.html

[H01] try / catch 基础
来源：http://hz.shanyushiyangtech.top/gtyxyvsatw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.9152youxi.cn/gticaqvzaz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.gaohongyu789.top/gtiaocowbj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yvedp.cn/gtyzfezruu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.daria6918.cn/gtrszkxyon.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.feifeiyinyue.top/gttlxwqhja.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.kuanghao11.cn/gtbbrwskhm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yj20258888.top/gtfftjxraa.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jianghu66.top/gtedsvogna.html

[H02] finally / ensure 收尾
来源：http://hz.c1oappe.top/gtujfickeh.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yueranfly.top/gtpfheseed.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.aibaodan.cn/gtvehsenaz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hywenlv.cn/gtywifplcx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.aizwys.cn/gtmllcpayi.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.bjfxy.top/gtrjgmexxa.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yj20258.top/gtthkkgaic.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.vqdsnc.cn/gtzlfkaovj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.shuidangran.top/gtpztyjrat.html

[H03] 主动抛出异常
来源：http://hz.jinyuanbaomall.cn/gtfxqbliab.html

Py:   raise ValueError("错误信息")
来源：http://hz.vqdsnc.cn/gtzweygoue.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.quarkkingdee.top/gtdlpjzeoj.html

JS:   throw new Error("错误信息");
来源：http://hz.sufxvd.cn/gtsenmgvrl.html

TS:   throw new Error("错误信息");
来源：http://hz.chenlongwang.top/gtxcplujic.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.guowangkeji.top/gtcyugagci.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.shanyushiyangkeji.top/gtguqfsgoz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.hysaishi.cn/gtjletigsw.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.feifeiyinyue.top/gtgzenwarn.html

[H04] 自定义异常类型
来源：http://hz.yuxming.cn/gtkervmyxn.html

Py:   class MyError(Exception): pass
来源：http://hz.jlsjyb.cn/gtjzuwqnwp.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yangfankeji.com/gtdkhwikyp.html

JS:   class MyError extends Error {}
来源：http://hz.jinqigufen.top/gtfrfblfto.html

TS:   class MyError extends Error {}
来源：http://hz.jinyuanbaomall.cn/gtqkotllmb.html

Java: class MyException extends RuntimeException {}
来源：http://hz.gzhubu.top/gticwtbhia.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.chenlongwang.top/gtfqmyixvq.html

Ruby: class MyError < StandardError; end
来源：http://hz.haohaochexian.top/gtbyvrqios.html

C#:   class MyException : Exception {}
来源：http://hz.pycfn.com/gtojhkaxvw.html

[H05] 捕获特定类型
来源：http://hz.gaohongyu789.top/gtldsvkhhl.html

Py:   except ValueError as e:
来源：http://hz.birdmap.top/gtzzkhlytz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.tian-w.cn/gtgxegekcs.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.iojbl.cn/gtugijlzgm.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.hongshengwenyu.top/gtqjzgkncm.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.aibaodan.cn/gtacaiiaja.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.ydzc1.top/gtghreuwch.html

Ruby: rescue ArgumentError => e
来源：http://hz.meibo888.top/gtmmspwgnv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.xuanzx.com/gtqrxfxvuy.html

[H06] 可选值 / 空值安全访问
来源：http://hz.daria6918.cn/gthlgpyuyu.html

Py:   value = d.get("k") or default
来源：http://hz.jinyuanbaomall.cn/gtlxzjfahl.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yj20258888.top/gtslcmriny.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zhiwuduotai.top/gtvhmddswm.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.chenzaomai.com/gtjpbsozba.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.nwbrower.top/gtdouywlun.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.ydzc1.top/gtraprmqvw.html

Ruby: d&.dig(:a, :b)
来源：http://hz.ybcxt.top/gtygtmkfjh.html

C#:   obj?.A?.B ?? default
来源：http://hz.yj20258888.top/gtrbizdtsw.html

[H07] 断言
来源：http://hz.havefunace.top/gtotlxipam.html

Py:   assert x > 0, "必须为正"
来源：http://hz.svipenyu.cn/gtrlcpgeta.html

PHP:  assert($x > 0);
来源：http://hz.wangshuangyany.cn/gtxjglupyc.html

JS:   console.assert(x > 0);
来源：http://hz.zhongyouzk.top/gtmxmsqvpg.html

TS:   console.assert(x > 0);
来源：http://hz.jyoumei.cn/gtkhylxrap.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yangfankeji.com/gtgelbcbcq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.52xcode.cn/gtqdvqdwbx.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.mhx1999.top/gteczimyed.html

C#:   Debug.Assert(x > 0);
来源：http://hz.quarkkingdee.top/gtukokccuh.html

[H08] 获取错误信息与堆栈
来源：http://hz.yvedp.cn/gtbhzoszum.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.hfpthk.cn/gteaxowbwm.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.ppjwa.cn/gtpohqciaq.html

JS:   e.message;  e.stack
来源：http://hz.zdqjudy.top/gtlmmduzes.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yuxming.cn/gtmgwxibcy.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.ydzc1.top/gtjmpapzvn.html

Go:   err.Error()
来源：http://hz.zhengqikj.top/gtkayvyvwd.html

Ruby: e.message;  e.backtrace
来源：http://hz.nanxuanxn.top/gtnqeifxqc.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jinqigufen.top/gtctzqbzfm.html

[H09] 带错误码的异常
来源：http://hz.chenjidiqi.icu/gtgkwfxfdw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.cucudq.cn/gtbrfdmksf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.gzhubu.top/gtoyxdenhj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.aizwys.cn/gtuudlvenf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.xuetiantiany.cn/gttfqlxcua.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.xylfe.cn/gtxykfvqif.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jinyuanbaomall.cn/gtfmzbofiv.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.shanyushiyangkeji.top/gtwqbbnbsw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jyoumei.cn/gtqezvldhh.html

[H10] 资源自动释放
来源：http://hz.cheryme.top/gtgbvjkqfj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jinyuanbaomall.cn/gtrpbyqdst.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.daria6918.cn/gtabujwqkb.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jqgfzy.top/gtwapfcryh.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhoulong.xyz/gtgvwrlykz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.xylfe.cn/gtlxqboqnj.html

Go:   defer f.Close()
来源：http://hz.shuidangran.top/gtvthqzkzp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.pycfn.com/gtrtyufkxl.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.feifeiyinyue.top/gtjrwzkjrn.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtizxoqpqw.html

I. 正则表达式
来源：http://hz.gaohongyu789.top/gtxfcdlvwe.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtinfbaeko.html

[I01] 判断是否匹配
来源：http://hz.wangshuangyany.cn/gtdvfteqqr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yj202588.top/gtsacyhlob.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yvedp.cn/gtrgbqhhlq.html

JS:   /\d+/.test(s)
来源：http://hz.sweek.top/gtbdejssei.html

TS:   /\d+/.test(s)
来源：http://hz.cdnleiting.top/gtltzlnoiw.html


<!-- 参考信息 -->