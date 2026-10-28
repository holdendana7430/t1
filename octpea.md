代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.meibo888.top/gtogckvubm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.sweek.top/gtrtmoggns.html

JS:   fs.readdirSync("dir")
来源：http://hz.fzhhl.top/gtkxdkpbvs.html

TS:   fs.readdirSync("dir")
来源：http://hz.jinyuanbaomall.cn/gtcftegexj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.ppjwa.cn/gtykoinbzy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zycfv.cn/gtteidxfrc.html

Ruby: Dir.children("dir")
来源：http://hz.tianlin.xyz/gtdnacmxsg.html

C#:   Directory.GetFiles("dir")
来源：http://hz.meibo888.top/gtduxvphgo.html

[F09] 获取文件大小
来源：http://hz.yangfankeji.com/gtznvfzwzq.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yanxiufei.cn/gtfwmhtrgg.html

PHP:  filesize("a.txt");
来源：http://hz.andypj.xyz/gtvxjzhytr.html

JS:   fs.statSync("a.txt").size
来源：http://hz.ybcxt.top/gtgknbumfd.html

TS:   fs.statSync("a.txt").size
来源：http://hz.0kj1m.cn/gtwvlelnvx.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.316326.xyz/gtqqgokjal.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hammf.cn/gtcypatcal.html

Ruby: File.size("a.txt")
来源：http://hz.xylfe.cn/gthqxqifil.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yj20258.top/gteiloahqj.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jiagoushi.top/gtpguowvzd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.sweek.top/gtgpircisk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.iojbl.cn/gtglijmuzc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jinqigfzy.top/gtzxhhbmqn.html

TS:   path.extname("a.txt")
来源：http://hz.snrcjt.cn/gttfiihfjs.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jqgufenzy.top/gtbysfuphi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.cashguo.top/gtitavakii.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yanxiufei.cn/gtkxodwuvw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.shanyushiyangtech.top/gtuwuiwhli.html

[F11] 复制与移动文件
来源：http://hz.yj202588.top/gtbwoumbeh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.birdmap.top/gthcnrsrue.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.fzhhl.top/gtksdzeqpv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.0kj1m.cn/gtcbhpovnk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.mhx1999.top/gttdjcjefz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yangfankeji.com/gtofbpjvcm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.fengsongda.top/gtutmewkes.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yangfankeji.com/gttpamzsta.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.xziqi.cn/gtxticafgy.html

[F12] CSV 读写
来源：http://hz.tanke756.top/gtxewasluw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.cdnleiting.top/gtgpjqxvmm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.ehwqpu.com/gtrhztobno.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.gzhubu.top/gtweiobpgd.html

TS:   // 同上
来源：http://hz.haohaochexian.top/gtmjhwchqs.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.bjfxy.top/gtutmpwgnb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.tian-w.cn/gtqtkajzkz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zhijiandao.cn/gtotsttepa.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.feifeiyinyue.top/gtbxuincwh.html

================================================================================
来源：http://hz.c1oappe.top/gtgbasxlrb.html

G. 面向对象
来源：http://hz.dashuyun.cn/gtgoganrwo.html

================================================================================
来源：http://hz.yvedp.cn/gtoqqgcmwn.html

[G01] 定义类
来源：http://hz.kuanghao11.cn/gtywmrmcyz.html

Py:   class User: pass
来源：http://hz.zhaomingkeji.xyz/gtjyqeonmk.html

PHP:  class User {}
来源：http://hz.gogol.net.cn/gttwzesmng.html

JS:   class User {}
来源：http://hz.cheryme.top/gtlrbjlhiw.html

TS:   class User { name: string = ""; }
来源：http://hz.jiagoushi.top/gthmbogygi.html

Java: class User {}
来源：http://hz.jlsjyb.cn/gtjplznmoo.html

Go:   type User struct { Name string }
来源：http://hz.tianlin.xyz/gtonqwrumo.html

Ruby: class User; end
来源：http://hz.hnxiangtu.top/gtkouizjti.html

C#:   class User {}
来源：http://hz.gotoacloud.top/gtmgvmkvbz.html

[G02] 构造函数
来源：http://hz.hongshengwenyu.top/gtspgvsbqc.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yuanzhike.top/gtmbiuycto.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.aibaodan.cn/gtryfylngc.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.smart0.xyz/gthwaelkcj.html

TS:   constructor(public name: string) {}
来源：http://hz.cdnleiting.top/gtkbotqxzv.html

Java: User(String name) { this.name = name; }
来源：http://hz.haohaochexian.top/gtdtloiwym.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.0kj1m.cn/gtjkldskal.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.shzxlz.cn/gtfhfbtvrq.html

C#:   public User(string name) { Name = name; }
来源：http://hz.hywenlv.cn/gtnkzpnkcj.html

[G03] 实例属性
来源：http://hz.snrcjt.cn/gtkzjgjltt.html

Py:   self.name = "x"
来源：http://hz.ywan-chungtsiang.top/gtaewyynug.html

PHP:  public string $name = "x";
来源：http://hz.hammf.cn/gtprisbzqj.html

JS:   this.name = "x";
来源：http://hz.mhx1999.top/gtbdwgwbjb.html

TS:   name: string = "x";
来源：http://hz.hywenlv.cn/gtjvxfmvtp.html

Java: private String name;
来源：http://hz.ybcxt.top/gtklufruwi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.daria6918.cn/gtkdhhdkbk.html

Ruby: @name = "x"
来源：http://hz.redwolf501.top/gtnpdsoeer.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zhijiandao.cn/gtonrqwmsq.html

[G04] 定义方法
来源：http://hz.yongpay.top/gtwumykqia.html

Py:   def greet(self): return self.name
来源：http://hz.sufxvd.cn/gtzxektece.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.sufxvd.cn/gtraucjttl.html

JS:   greet() { return this.name; }
来源：http://hz.zhongyouzk.top/gtrgkcules.html

TS:   greet(): string { return this.name; }
来源：http://hz.shangyingyoupin.top/gtyevgcjuz.html

Java: String greet() { return name; }
来源：http://hz.xingfuxueyuan.xyz/gtwaepfmbd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.fzhhl.top/gttrjipfwk.html

Ruby: def greet; @name; end
来源：http://hz.chenzaomai.com/gtbrfjbiex.html

C#:   public string Greet() => Name;
来源：http://hz.wangdashe.top/gtfhnkzoyb.html

[G05] 继承
来源：http://hz.hammf.cn/gtasluclnl.html

Py:   class Admin(User): pass
来源：http://hz.zhixingplan.top/gtbaccbfhg.html

PHP:  class Admin extends User {}
来源：http://hz.yueranfly.top/gtjnuwudsm.html

JS:   class Admin extends User {}
来源：http://hz.c1oappe.top/gtavfeobkt.html

TS:   class Admin extends User {}
来源：http://hz.hfpthk.cn/gteqrtifze.html

Java: class Admin extends User {}
来源：http://hz.vqdsnc.cn/gtmdrkumvc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.fengsongda.top/gtonawchlb.html

Ruby: class Admin < User; end
来源：http://hz.sysykeji.top/gtqdhclher.html

C#:   class Admin : User {}
来源：http://hz.jqgfzy.top/gtapbkqijf.html

[G06] 重写方法
来源：http://hz.guannengcc.top/gtjvngbdlg.html

Py:   def greet(self): return "admin"
来源：http://hz.hongshengwenyu.top/gtkwvqolea.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.feifeiyinyue.top/gtnlpjzrij.html

JS:   greet() { return "admin"; }
来源：http://hz.yj20258888.top/gtdtfcpvri.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hammf.cn/gtofbnzutk.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hysaishi.cn/gtibvnqcyc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.aizwys.cn/gtenkiawid.html

Ruby: def greet; "admin"; end
来源：http://hz.sweek.top/gtovmgtetk.html

C#:   public override string Greet() => "admin";
来源：http://hz.xinyue.icu/gtjvkvwlul.html

[G07] 调用父类方法
来源：http://hz.sxryk.cn/gtiiifyfxi.html

Py:   super().greet()
来源：http://hz.9152youxi.cn/gtsaoptgkz.html

PHP:  parent::greet();
来源：http://hz.shangyingyoupin.top/gtitimbtpm.html

JS:   super.greet();
来源：http://hz.xuanzx.com/gttiimuxhg.html

TS:   super.greet();
来源：http://hz.zycfv.cn/gtuauuydhw.html

Java: super.greet();
来源：http://hz.yj202588.top/gtxmuixryy.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.xinyue.icu/gtkcoikvym.html

Ruby: super
来源：http://hz.havefunace.top/gtygqtlspq.html

C#:   base.Greet();
来源：http://hz.sweek.top/gtfemljtkv.html

[G08] 静态方法与属性
来源：http://hz.c1oappe.top/gtumtlqibz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.gzhubu.top/gtueqbtntu.html

PHP:  public static function f() {}
来源：http://hz.quarkkingdee.top/gtidhicbve.html

JS:   static f() {}
来源：http://hz.hfpthk.cn/gtxmegbwjg.html

TS:   static f(): void {}
来源：http://hz.yj20258888.top/gtoozbcuwz.html

Java: static void f() {}
来源：http://hz.hnqzz.top/gtaipkpqsw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.cashguo.top/gtphsiraad.html

Ruby: def self.f; end
来源：http://hz.shzxlz.cn/gtpofxjdwu.html

C#:   public static void F() {}
来源：http://hz.fzhhl.top/gtqaxnjenv.html

[G09] 接口 / 抽象类
来源：http://hz.yangfankeji.com/gtnumzejib.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.ydzc1.top/gtaqszbrms.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.gzhubu.top/gtykxzelpz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.xziqi.cn/gtwyzfgofa.html

TS:   interface Shape { area(): number; }
来源：http://hz.yvedp.cn/gtuwvwjzai.html

Java: interface Shape { double area(); }
来源：http://hz.kuanghao11.cn/gtcbghcrkr.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.wangdashe.top/gtxhrlmems.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.xylfe.cn/gtvdlbilzd.html

C#:   interface IShape { double Area(); }
来源：http://hz.hammf.cn/gttokobocx.html

[G10] 访问控制
来源：http://hz.zhongyouzk.top/gtziotzeot.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.snrcjt.cn/gtluidrmrh.html

PHP:  public / protected / private
来源：http://hz.hongshengwenyu.top/gtutdwgeph.html

JS:   #private 字段；其余公开
来源：http://hz.chenjidiqi.icu/gtetetufal.html

TS:   public / protected / private
来源：http://hz.andypj.xyz/gtrdcajcze.html

Java: public / protected / private / 默认包级
来源：http://hz.shangyingyoupin.top/gtownuesxr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ivvv.top/gtodueeory.html

Ruby: public / protected / private
来源：http://hz.ybcxt.top/gtrnubtghz.html

C#:   public / protected / private / internal
来源：http://hz.gogol.net.cn/gtwsqizjvf.html

[G11] getter / setter
来源：http://hz.aibaodan.cn/gtdrxjfoxz.html

Py:   @property 与 @x.setter
来源：http://hz.zhengqikj.top/gtinmxhbed.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.ywan-chungtsiang.top/gtywfbxjlv.html

JS:   get name() { return this._name; }
来源：http://hz.316326.xyz/gtgpfsgsfl.html

TS:   get name(): string { return this._name; }
来源：http://hz.yj202588.top/gtfzjdrnbl.html

Java: public String getName() { return name; }
来源：http://hz.zycfv.cn/gtyjquyfjq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.gzhubu.top/gttkaiufsg.html

Ruby: attr_accessor :name
来源：http://hz.yj20258.top/gtiyimahim.html

C#:   public string Name { get; set; }
来源：http://hz.hfpthk.cn/gtjknozehp.html

[G12] 对象转字符串
来源：http://hz.wangshuangyany.cn/gtubaymyyw.html

Py:   def __str__(self): return self.name
来源：http://hz.ybcxt.top/gtjhlrzeaz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zhongyouzk.top/gtirticajs.html

JS:   toString() { return this.name; }
来源：http://hz.yj202588.top/gtailsgbfw.html

TS:   toString(): string { return this.name; }
来源：http://hz.pengpengdd.cyou/gtzxpkwisi.html

Java: @Override public String toString() { return name; }
来源：http://hz.xingfuxueyuan.xyz/gtyqdavkez.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.shanyushiyangkeji.top/gtcjfkxtxo.html

Ruby: def to_s; @name; end
来源：http://hz.hywenlv.cn/gtvgnvviqj.html

C#:   public override string ToString() => Name;
来源：http://hz.ppjwa.cn/gtnevswmiz.html

[G13] 判断对象类型
来源：http://hz.cucudq.cn/gtvfpnsyqp.html

Py:   isinstance(u, User)
来源：http://hz.jinyuanbaomall.cn/gtyjohiicr.html

PHP:  $u instanceof User
来源：http://hz.nwbrower.top/gtyrlytoit.html

JS:   u instanceof User
来源：http://hz.hnxiangtu.top/gtlcqdghie.html

TS:   u instanceof User
来源：http://hz.guowangkeji.top/gtavcaqulv.html

Java: u instanceof User
来源：http://hz.hnqzz.top/gtmeopddfh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.kuanghao11.cn/gtgdrfzglf.html

Ruby: u.is_a?(User)
来源：http://hz.hammf.cn/gtxkvjmtby.html

C#:   u is User
来源：http://hz.yj20258888.top/gtuxdtwbvq.html

[G14] 数据类 / record
来源：http://hz.sufxvd.cn/gtzaymnczx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.ybcxt.top/gteyzpmizp.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.sweek.top/gttzktcvmn.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.smart0.xyz/gtzgfpycaa.html

TS:   type User = { name: string; age: number };
来源：http://hz.daria6918.cn/gtvaxuncoo.html

Java: record User(String name, int age) {}
来源：http://hz.meibo888.top/gtsmetvjqf.html

Go:   type User struct { Name string; Age int }
来源：http://hz.dashuyun.cn/gtzvkmdtly.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jinqigfzy.top/gtliogmiaj.html

C#:   record User(string Name, int Age);
来源：http://hz.sxryk.cn/gtdyqpadqr.html

[G15] 枚举
来源：http://hz.hnqzz.top/gtxavumcbr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.xylfe.cn/gtiialchgw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.redwolf501.top/gtrdpvecvl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.ywan-chungtsiang.top/gtmiutbhsh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ehwqpu.com/gtuebbxznk.html

Java: enum Color { RED, GREEN }
来源：http://hz.shangyingyoupin.top/gtfrwklwvm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ppjwa.cn/gtcwzufolf.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yuanzhike.top/gtneohnigx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yuanzhike.top/gtvqxurbfe.html

[G16] 对象转数组 / 字典
来源：http://hz.jlsjyb.cn/gtxrptiuwd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.hnxiangtu.top/gtipkgzuoi.html

PHP:  get_object_vars($obj);
来源：http://hz.dianchejie.cn/gtufaxyqqz.html

JS:   Object.entries(obj)
来源：http://hz.zycfv.cn/gtnwjmxagw.html

TS:   Object.entries(obj)
来源：http://hz.gotoacloud.top/gtfozwopgf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.shanyushiyangkeji.top/gtmcrxbggg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.zdqjudy.top/gtqouznolv.html

Ruby: obj.instance_variables
来源：http://hz.chenlongwang.top/gtddjfiqpw.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.aizwys.cn/gtortiqyig.html

================================================================================
来源：http://hz.xziqi.cn/gtkeeowtcf.html

H. 异常与错误处理
来源：http://hz.nwbrower.top/gtgzkwqdsy.html

================================================================================
来源：http://hz.iojbl.cn/gtpzeahfxa.html

[H01] try / catch 基础
来源：http://hz.jlsjyb.cn/gthbeyzjtk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.nanxuanxn.top/gtynsvlwwe.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zdqjudy.top/gtmefmpoky.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jinyuanbaomall.cn/gtcvxgvjgf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.sweek.top/gtamnmtgpi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.dashuyun.cn/gtwnzbcedz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.sxryk.cn/gthmfizigb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.andypj.xyz/gtotpsoftp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.chenzaomai.com/gtdhqztvpz.html

[H02] finally / ensure 收尾
来源：http://hz.guannengcc.top/gtqassmsvg.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.hfpthk.cn/gtuohikoet.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hnqzz.top/gtupbbvxdh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.fzhhl.top/gtwbpdpqiq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.9152youxi.cn/gtsshhymlg.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.redwolf501.top/gticuntkez.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zhongyouzk.top/gtdztunfjv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.nanxuanxn.top/gticxhwlox.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jlsjyb.cn/gtmviiwome.html

[H03] 主动抛出异常
来源：http://hz.jqgfzy.top/gtxtsdijml.html

Py:   raise ValueError("错误信息")
来源：http://hz.hnxiangtu.top/gturpnwqzp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jyoumei.cn/gtwfxobamv.html

JS:   throw new Error("错误信息");
来源：http://hz.sweek.top/gthxqlnple.html

TS:   throw new Error("错误信息");
来源：http://hz.xinyue.icu/gtechavqhp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.sysykeji.top/gtqlzbpgpi.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.ydjk.org.cn/gtjflbuhkw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jinqigfzy.top/gtllmxcpff.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.hysaishi.cn/gtoehswmbq.html

[H04] 自定义异常类型
来源：http://hz.hnxiangtu.top/gtbhgkhowb.html

Py:   class MyError(Exception): pass
来源：http://hz.ywan-chungtsiang.top/gtqzbybgej.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.sweek.top/gtzgzwcfxu.html

JS:   class MyError extends Error {}
来源：http://hz.feifeiyinyue.top/gtunfxzqso.html

TS:   class MyError extends Error {}
来源：http://hz.birdmap.top/gtadesosfq.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zhiwuduotai.top/gtopgeziex.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yj202588.top/gtijypaplr.html

Ruby: class MyError < StandardError; end
来源：http://hz.ppjwa.cn/gtdvafhvgu.html

C#:   class MyException : Exception {}
来源：http://hz.ehwqpu.com/gtotnrxtmi.html

[H05] 捕获特定类型
来源：http://hz.yuxming.cn/gtbkurfkwb.html

Py:   except ValueError as e:
来源：http://hz.chenjidiqi.icu/gtnufeianj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.snrcjt.cn/gtbdpbolsp.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zhaomingkeji.xyz/gtummetvxq.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jinyuanbaomall.cn/gtnmqpghkm.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.hywenlv.cn/gtbvhatqfj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.iojbl.cn/gtubvwoemy.html

Ruby: rescue ArgumentError => e
来源：http://hz.kuanghao11.cn/gtuqghjxgx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhongyouzk.top/gtfleumsis.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jqgfzy.top/gtoagfizei.html

Py:   value = d.get("k") or default
来源：http://hz.chenzaomai.com/gtycyooege.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.xuanzx.com/gtroxecnls.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.pengpengdd.cyou/gtmwhbtsni.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.0kj1m.cn/gtekygbqoa.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.bjfxy.top/gtsudhscwf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jinghuilouyu.cn/gtclkjysxb.html

Ruby: d&.dig(:a, :b)
来源：http://hz.kuanghao11.cn/gtlerkjtcc.html

C#:   obj?.A?.B ?? default
来源：http://hz.52xcode.cn/gtudnoapbw.html

[H07] 断言
来源：http://hz.redwolf501.top/gtrltdpedj.html

Py:   assert x > 0, "必须为正"
来源：http://hz.daxiang520.top/gtgtnlqrhz.html

PHP:  assert($x > 0);
来源：http://hz.daria6918.cn/gtuzyvseve.html

JS:   console.assert(x > 0);
来源：http://hz.mhx1999.top/gtnvoahmlt.html

TS:   console.assert(x > 0);
来源：http://hz.jqgfzy.top/gtnnrmesxz.html

Java: assert x > 0 : "必须为正";
来源：http://hz.vqdsnc.cn/gtrefyxwaa.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.xinyue.icu/gtgglztaur.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.dianchejie.cn/gthhxeukxx.html

C#:   Debug.Assert(x > 0);
来源：http://hz.xingfuxueyuan.xyz/gtxqwxapjo.html

[H08] 获取错误信息与堆栈
来源：http://hz.zhongyouzk.top/gtaxxqkwat.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.wangdashe.top/gtmqxrsxkh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.iojbl.cn/gtoupvissi.html

JS:   e.message;  e.stack
来源：http://hz.jlsjyb.cn/gtswikfgoj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.mhx1999.top/gtxxlltumj.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.c1oappe.top/gthxmhxjax.html

Go:   err.Error()
来源：http://hz.chenzaomai.com/gtwwezkgxp.html

Ruby: e.message;  e.backtrace
来源：http://hz.birdmap.top/gtmexzpnor.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jqgfzy.top/gtircqqkpj.html

[H09] 带错误码的异常
来源：http://hz.nanxuanxn.top/gtcstzeszq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yuanzhike.top/gticdwzghx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yonumen.top/gttcwshffh.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jinqigufen.top/gtknuurbth.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.cheryme.top/gtlcaxsccj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zhengqikj.top/gttrhoriqt.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jinqigufen.top/gtrlhffgef.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zdqjudy.top/gtnpizvopw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.redwolf501.top/gtlookiewz.html

[H10] 资源自动释放
来源：http://hz.vqdsnc.cn/gtizgzsxsm.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.tianlin.xyz/gtwgazibli.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.xuanzx.com/gtsstphdly.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.dashuyun.cn/gthkeqbhyi.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sxryk.cn/gtqovgmpav.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.dianchejie.cn/gtclgyidfo.html

Go:   defer f.Close()
来源：http://hz.kuanghao11.cn/gtlgqyqyvk.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jqgufenzy.top/gtgyaxlslt.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.cdnleiting.top/gtpxivifvz.html

================================================================================
来源：http://hz.xuanzx.com/gtilnzojrt.html

I. 正则表达式
来源：http://hz.hongshengwenyu.top/gtptdnxiav.html

================================================================================
来源：http://hz.svipenyu.cn/gtlaoqsuhb.html

[I01] 判断是否匹配
来源：http://hz.zhijiandao.cn/gtqtwghfog.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.cashguo.top/gtlszehdqy.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.c1oappe.top/gtuhrayoej.html

JS:   /\d+/.test(s)
来源：http://hz.guowangkeji.top/gtnxhanudi.html

TS:   /\d+/.test(s)
来源：http://hz.9152youxi.cn/gtrtxdlucy.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ydjk.org.cn/gtwuvifldi.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zhiwuduotai.top/gtsokthyub.html

Ruby: s.match?(/\d+/)
来源：http://hz.yuxming.cn/gtmuahuhva.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.hongshengwenyu.top/gtwskyhmbu.html

[I02] 提取所有匹配
来源：http://hz.gogol.net.cn/gtyutzkkbx.html

Py:   re.findall(r"\d+", s)
来源：http://hz.c1oappe.top/gtpqitedle.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.shanyushiyangkeji.top/gthvmahgjg.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.redwolf501.top/gtiutllyax.html


<!-- 参考信息 -->