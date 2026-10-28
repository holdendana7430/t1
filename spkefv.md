代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.nanxuanxn.top/gtptmwdbvc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yj20258888.top/gtsuyankii.html

Ruby: Dir.children("dir")
来源：http://hz.hammf.cn/gtttchwume.html

C#:   Directory.GetFiles("dir")
来源：http://hz.cdnleiting.top/gtyetppzvw.html

[F09] 获取文件大小
来源：http://hz.gogol.net.cn/gtwizkzbna.html

Py:   os.path.getsize("a.txt")
来源：http://hz.ydzc1.top/gtfcupxxit.html

PHP:  filesize("a.txt");
来源：http://hz.snrcjt.cn/gtgseapedz.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zhixingplan.top/gtngvqgfen.html

TS:   fs.statSync("a.txt").size
来源：http://hz.cashguo.top/gtinfcsisr.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.nanxuanxn.top/gtrhfmjaeo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.wangshuangyany.cn/gtrhfuakec.html

Ruby: File.size("a.txt")
来源：http://hz.hywenlv.cn/gtimfvhwvo.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.zdqjudy.top/gthtreipfn.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yongpay.top/gtswetvdgf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.guowangkeji.top/gtqjydcwek.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jinqigufen.top/gtqofhzilc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yangfankeji.com/gtlxmnsskx.html

TS:   path.extname("a.txt")
来源：http://hz.zhiwuduotai.top/gtfekvlqou.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yuanzhike.top/gtawoqzlcs.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zhixingplan.top/gtybuhptia.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.52xcode.cn/gtfqtkjshd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.pycfn.com/gtbxvoxscg.html

[F11] 复制与移动文件
来源：http://hz.yanxiufei.cn/gtlsbanpei.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yangfankeji.com/gtsixcekql.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.chenlongwang.top/gtdkqckpqw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.fengsongda.top/gtadjuhaqx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.haohaochexian.top/gtbmgbaytt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.shangyingyoupin.top/gtaotefbkx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.hongshengwenyu.top/gtvsuqxwnr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.xuanzx.com/gtrmwzloyw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ppjwa.cn/gtldxxntde.html

[F12] CSV 读写
来源：http://hz.pycfn.com/gtvmnwtuio.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.cqqwz.cn/gtxkzdjwwe.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jiagoushi.top/gtijvrmsmc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.pengpengdd.cyou/gtyqhrjafl.html

TS:   // 同上
来源：http://hz.yuanzhike.top/gtupjyxcxf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jiagoushi.top/gtgnqegftn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.tianlin.xyz/gtpayzxgsi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.kuanghao11.cn/gtyxrvceqo.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.cheryme.top/gthjydqkyk.html

================================================================================
来源：http://hz.cashguo.top/gtgyeqehyi.html

G. 面向对象
来源：http://hz.yonumen.top/gtqtbwaclz.html

================================================================================
来源：http://hz.hnxiangtu.top/gtcikemmnv.html

[G01] 定义类
来源：http://hz.guannengcc.top/gtakafvfyo.html

Py:   class User: pass
来源：http://hz.xylfe.cn/gtdqqsnscc.html

PHP:  class User {}
来源：http://hz.gotoacloud.top/gtwrvwrxey.html

JS:   class User {}
来源：http://hz.ppjwa.cn/gtolbgtkvv.html

TS:   class User { name: string = ""; }
来源：http://hz.shanyushiyangkeji.top/gtcikpbxsv.html

Java: class User {}
来源：http://hz.smart0.xyz/gtjfzmncpe.html

Go:   type User struct { Name string }
来源：http://hz.feifeiyinyue.top/gtgkslsjrr.html

Ruby: class User; end
来源：http://hz.dashuyun.cn/gtqbrxcfjo.html

C#:   class User {}
来源：http://hz.jinqigufen.top/gtsjwsstzr.html

[G02] 构造函数
来源：http://hz.fzhhl.top/gtvyhlhymc.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.sysykeji.top/gtyznmudel.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yuanzhike.top/gtloxocugt.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.cucudq.cn/gtsyrzyysu.html

TS:   constructor(public name: string) {}
来源：http://hz.havefunace.top/gtqwvaauat.html

Java: User(String name) { this.name = name; }
来源：http://hz.zycfv.cn/gtbptomntu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zhiwuduotai.top/gtykjfbads.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.pengpengdd.cyou/gtfkfmevnp.html

C#:   public User(string name) { Name = name; }
来源：http://hz.shanyushiyangkeji.top/gtwyasbhxr.html

[G03] 实例属性
来源：http://hz.feifeiyinyue.top/gtnwoftemo.html

Py:   self.name = "x"
来源：http://hz.gaohongyu789.top/gtckfduzdv.html

PHP:  public string $name = "x";
来源：http://hz.daxiang520.top/gtdckvasbf.html

JS:   this.name = "x";
来源：http://hz.hongshengwenyu.top/gtcgbttbtx.html

TS:   name: string = "x";
来源：http://hz.c1oappe.top/gtaivawpgq.html

Java: private String name;
来源：http://hz.dashuyun.cn/gtczadgsoj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.guowangkeji.top/gtzyeenxyr.html

Ruby: @name = "x"
来源：http://hz.jyoumei.cn/gtwbehihag.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.ydjk.org.cn/gtehxvdqcz.html

[G04] 定义方法
来源：http://hz.yuxming.cn/gteeoksalh.html

Py:   def greet(self): return self.name
来源：http://hz.nanxuanxn.top/gtvlwihiax.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.ydzc1.top/gtyrtfanhf.html

JS:   greet() { return this.name; }
来源：http://hz.hysaishi.cn/gtqapkmhjz.html

TS:   greet(): string { return this.name; }
来源：http://hz.sufxvd.cn/gtinhxtoqc.html

Java: String greet() { return name; }
来源：http://hz.chenjidiqi.icu/gttpmlcybu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hfpthk.cn/gtyotlejqr.html

Ruby: def greet; @name; end
来源：http://hz.yuxming.cn/gtfvaxemvu.html

C#:   public string Greet() => Name;
来源：http://hz.chenzaomai.com/gtcyjmzcwk.html

[G05] 继承
来源：http://hz.quarkkingdee.top/gtfydqqhxu.html

Py:   class Admin(User): pass
来源：http://hz.wangshuangyany.cn/gtjqtctysu.html

PHP:  class Admin extends User {}
来源：http://hz.guowangkeji.top/gtxklzzody.html

JS:   class Admin extends User {}
来源：http://hz.cucudq.cn/gtjmgxygny.html

TS:   class Admin extends User {}
来源：http://hz.fzhhl.top/gtpxniirue.html

Java: class Admin extends User {}
来源：http://hz.gaohongyu789.top/gtblzbhmki.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jianghu66.top/gtgedawmjp.html

Ruby: class Admin < User; end
来源：http://hz.hnqzz.top/gtnfttgmnf.html

C#:   class Admin : User {}
来源：http://hz.snrcjt.cn/gtawjftffb.html

[G06] 重写方法
来源：http://hz.hammf.cn/gteyekjqia.html

Py:   def greet(self): return "admin"
来源：http://hz.xuanzx.com/gtnvmledic.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ydzc1.top/gtmqhqeyan.html

JS:   greet() { return "admin"; }
来源：http://hz.wangshuangyany.cn/gtbauwynxv.html

TS:   greet(): string { return "admin"; }
来源：http://hz.shzxlz.cn/gtmfzosstw.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yj20258.top/gtqqjdxrev.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.gzhubu.top/gtystuoits.html

Ruby: def greet; "admin"; end
来源：http://hz.jyoumei.cn/gtyjrpmcdt.html

C#:   public override string Greet() => "admin";
来源：http://hz.chenzaomai.com/gttmrbxqex.html

[G07] 调用父类方法
来源：http://hz.c1oappe.top/gtsmjghwcj.html

Py:   super().greet()
来源：http://hz.aibaodan.cn/gtatyuvqxw.html

PHP:  parent::greet();
来源：http://hz.guannengcc.top/gtdhexcdfa.html

JS:   super.greet();
来源：http://hz.redwolf501.top/gtdmcxmack.html

TS:   super.greet();
来源：http://hz.pengpengdd.cyou/gtwoxdywkm.html

Java: super.greet();
来源：http://hz.gzhubu.top/gthsynvhyz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.hnqzz.top/gtqiwdnyjv.html

Ruby: super
来源：http://hz.zycfv.cn/gtijsgkgqk.html

C#:   base.Greet();
来源：http://hz.xylfe.cn/gtwihjrwvq.html

[G08] 静态方法与属性
来源：http://hz.mhx1999.top/gtqjbghfyd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.snrcjt.cn/gtpbeqtqty.html

PHP:  public static function f() {}
来源：http://hz.zdqjudy.top/gtzcvwrawf.html

JS:   static f() {}
来源：http://hz.feifeiyinyue.top/gtuzqkjdrf.html

TS:   static f(): void {}
来源：http://hz.yongpay.top/gtzrhzmfpn.html

Java: static void f() {}
来源：http://hz.zhijiandao.cn/gttqnrpoiv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yuxming.cn/gtecuqhoxt.html

Ruby: def self.f; end
来源：http://hz.fengsongda.top/gteyballth.html

C#:   public static void F() {}
来源：http://hz.fengsongda.top/gtoonbcmtu.html

[G09] 接口 / 抽象类
来源：http://hz.9152youxi.cn/gtkshkucdr.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.shangyingyoupin.top/gttnqcxkfh.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.snrcjt.cn/gtapxadsid.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jinghuilouyu.cn/gtqoxsjzzc.html

TS:   interface Shape { area(): number; }
来源：http://hz.ppjwa.cn/gtusqaqgjl.html

Java: interface Shape { double area(); }
来源：http://hz.tian-w.cn/gtnfzsvcri.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.cashguo.top/gthfdzqmsm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.xinyue.icu/gtjyearaoj.html

C#:   interface IShape { double Area(); }
来源：http://hz.guannengcc.top/gtzzckljfr.html

[G10] 访问控制
来源：http://hz.sxryk.cn/gtncptviek.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.cqqwz.cn/gtpkgqhfgc.html

PHP:  public / protected / private
来源：http://hz.hongshengwenyu.top/gtgkhnpzgx.html

JS:   #private 字段；其余公开
来源：http://hz.zycfv.cn/gtkhwafjuw.html

TS:   public / protected / private
来源：http://hz.hysaishi.cn/gtvnjkwpwm.html

Java: public / protected / private / 默认包级
来源：http://hz.xinyue.icu/gtnufxeulg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.andypj.xyz/gtrxikclcc.html

Ruby: public / protected / private
来源：http://hz.andypj.xyz/gtvhjyfmwr.html

C#:   public / protected / private / internal
来源：http://hz.xziqi.cn/gtvyeqxxan.html

[G11] getter / setter
来源：http://hz.cdnleiting.top/gtedoqfhfx.html

Py:   @property 与 @x.setter
来源：http://hz.cdnleiting.top/gtnnasanxn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.svipenyu.cn/gtvpzosbdu.html

JS:   get name() { return this._name; }
来源：http://hz.birdmap.top/gtsjhformb.html

TS:   get name(): string { return this._name; }
来源：http://hz.mhx1999.top/gtsaocxcmy.html

Java: public String getName() { return name; }
来源：http://hz.shzxlz.cn/gtvcgigdcf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.ivvv.top/gtznufpvez.html

Ruby: attr_accessor :name
来源：http://hz.gaohongyu789.top/gtmspsmcex.html

C#:   public string Name { get; set; }
来源：http://hz.sysykeji.top/gtyzdjsciz.html

[G12] 对象转字符串
来源：http://hz.xylfe.cn/gtcqhzwebt.html

Py:   def __str__(self): return self.name
来源：http://hz.haohaochexian.top/gtqkpciagm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.cucudq.cn/gtwsvktxme.html

JS:   toString() { return this.name; }
来源：http://hz.xylfe.cn/gtheclieii.html

TS:   toString(): string { return this.name; }
来源：http://hz.hnqzz.top/gtopknpfra.html

Java: @Override public String toString() { return name; }
来源：http://hz.shuidangran.top/gtigawdlqn.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.fengsongda.top/gtkbstbagz.html

Ruby: def to_s; @name; end
来源：http://hz.hfpthk.cn/gtrlqtktcy.html

C#:   public override string ToString() => Name;
来源：http://hz.hammf.cn/gteweumqem.html

[G13] 判断对象类型
来源：http://hz.tian-w.cn/gtmjmahmdl.html

Py:   isinstance(u, User)
来源：http://hz.yongpay.top/gttqotmwpx.html

PHP:  $u instanceof User
来源：http://hz.redwolf501.top/gtevnocoow.html

JS:   u instanceof User
来源：http://hz.haohaochexian.top/gtpjziqruk.html

TS:   u instanceof User
来源：http://hz.hywenlv.cn/gtjaqgxnng.html

Java: u instanceof User
来源：http://hz.jianghu66.top/gtvkxjadfl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.redwolf501.top/gtsmeowrfl.html

Ruby: u.is_a?(User)
来源：http://hz.dianchejie.cn/gtpdnxqwoi.html

C#:   u is User
来源：http://hz.cqqwz.cn/gtrcoewivu.html

[G14] 数据类 / record
来源：http://hz.hnxiangtu.top/gtotbmzojp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.ydjk.org.cn/gtpusocpnv.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.chenjidiqi.icu/gtytcvsflg.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.sufxvd.cn/gtnwcluddd.html

TS:   type User = { name: string; age: number };
来源：http://hz.bjfxy.top/gteqcfhfvv.html

Java: record User(String name, int age) {}
来源：http://hz.gzhubu.top/gtlrpkkmye.html

Go:   type User struct { Name string; Age int }
来源：http://hz.ywan-chungtsiang.top/gtkmyigoya.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.wangdashe.top/gtibbwirqb.html

C#:   record User(string Name, int Age);
来源：http://hz.aibaodan.cn/gtichgpqyn.html

[G15] 枚举
来源：http://hz.ydzc1.top/gtpxaqgrzv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zhongyouzk.top/gtqdprcpjz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhongyouzk.top/gtlntbocjb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.9152youxi.cn/gtqokhudxp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hywenlv.cn/gtscpydsmi.html

Java: enum Color { RED, GREEN }
来源：http://hz.aibaodan.cn/gtdhfowcqu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.chenzaomai.com/gthmkgsjdv.html

Ruby: Color = %i[red green].freeze
来源：http://hz.nanxinkj.top/gtfpyjbxgt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.dashuyun.cn/gtfwyuwyes.html

[G16] 对象转数组 / 字典
来源：http://hz.hywenlv.cn/gtnrdwddkt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.cqqwz.cn/gtfuvredaa.html

PHP:  get_object_vars($obj);
来源：http://hz.wangshuangyany.cn/gtwekdlsuf.html

JS:   Object.entries(obj)
来源：http://hz.tianlin.xyz/gtygdwuppk.html

TS:   Object.entries(obj)
来源：http://hz.zhaomingkeji.xyz/gtmknruymh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jyoumei.cn/gtjmgqwywf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.birdmap.top/gtsebmnfrh.html

Ruby: obj.instance_variables
来源：http://hz.meibo888.top/gtklrlzliq.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.shuidangran.top/gtljpgadvo.html

================================================================================
来源：http://hz.jinqigfzy.top/gtvixrstes.html

H. 异常与错误处理
来源：http://hz.redwolf501.top/gtmdbulqib.html

================================================================================
来源：http://hz.9152youxi.cn/gtablyqcuc.html

[H01] try / catch 基础
来源：http://hz.dianchejie.cn/gtpxsbndza.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.snrcjt.cn/gtyltqshqv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.tian-w.cn/gtuwrqsvgi.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.ydjk.org.cn/gtiruimiex.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.9152youxi.cn/gtvmadbozr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.tanke756.top/gtctkuqgul.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zycfv.cn/gtqkcnqsrz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.cheryme.top/gtpupfrqap.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jyoumei.cn/gtgfofbnik.html

[H02] finally / ensure 收尾
来源：http://hz.tanke756.top/gtenmutnfe.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yuxming.cn/gtslwgvcnu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.sufxvd.cn/gtrazcbnxq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jiagoushi.top/gtlreihapo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.tian-w.cn/gtisoaduhe.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.guowangkeji.top/gtwnrktnff.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.chenlongwang.top/gtwxgglagb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yueranfly.top/gtmdryknuh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.cqqwz.cn/gtdwtbtkkh.html

[H03] 主动抛出异常
来源：http://hz.0kj1m.cn/gtiyoylvgv.html

Py:   raise ValueError("错误信息")
来源：http://hz.dashuyun.cn/gtbeklhnim.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.xuetiantiany.cn/gtwwwvzpnl.html

JS:   throw new Error("错误信息");
来源：http://hz.nwbrower.top/gtywpbmgcf.html

TS:   throw new Error("错误信息");
来源：http://hz.iojbl.cn/gtpwaaqwcf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.andypj.xyz/gtechggord.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.52xcode.cn/gtwgxfqxfb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zhiwuduotai.top/gtwntevmsm.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.cucudq.cn/gtasomzzmi.html

[H04] 自定义异常类型
来源：http://hz.andypj.xyz/gtwuampjfo.html

Py:   class MyError(Exception): pass
来源：http://hz.gaohongyu789.top/gtcjxkzdpr.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yj202588.top/gtnryqsrhm.html

JS:   class MyError extends Error {}
来源：http://hz.feifeiyinyue.top/gtrjtrjbbw.html

TS:   class MyError extends Error {}
来源：http://hz.birdmap.top/gtwrcsgovd.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zhongyouzk.top/gtibavplnl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ydjk.org.cn/gtzyinyelq.html

Ruby: class MyError < StandardError; end
来源：http://hz.sufxvd.cn/gtwtthpqxm.html

C#:   class MyException : Exception {}
来源：http://hz.guowangkeji.top/gtknzepivx.html

[H05] 捕获特定类型
来源：http://hz.hfpthk.cn/gtzauyxhhf.html

Py:   except ValueError as e:
来源：http://hz.sufxvd.cn/gtbypgcdqu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhixingplan.top/gtvjirclbh.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.haohaochexian.top/gtpvtplnhn.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jinghuilouyu.cn/gtlmgbskbv.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.hysaishi.cn/gtbgdyadqh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.shanyushiyangkeji.top/gtfrbrdbhw.html

Ruby: rescue ArgumentError => e
来源：http://hz.jqgufenzy.top/gtacdjitkd.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.0kj1m.cn/gtuqmonijz.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yj202588.top/gtebwptcfs.html

Py:   value = d.get("k") or default
来源：http://hz.ehwqpu.com/gtzgquimed.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.xuetiantiany.cn/gtprhaovhv.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yuanzhike.top/gtljolclbv.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.gotoacloud.top/gtvifhvcic.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.quarkkingdee.top/gtzzrmkrqf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zhixingplan.top/gtorxtjqyr.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhengqikj.top/gtqemwrwoy.html

C#:   obj?.A?.B ?? default
来源：http://hz.c1oappe.top/gtjbtjnntw.html

[H07] 断言
来源：http://hz.316326.xyz/gtkdbukrfs.html

Py:   assert x > 0, "必须为正"
来源：http://hz.sxryk.cn/gtpizvcrws.html

PHP:  assert($x > 0);
来源：http://hz.52xcode.cn/gtrrhmhdal.html

JS:   console.assert(x > 0);
来源：http://hz.nanxuanxn.top/gtjnehwghe.html

TS:   console.assert(x > 0);
来源：http://hz.ydzc1.top/gtwbnexrzr.html

Java: assert x > 0 : "必须为正";
来源：http://hz.shuidangran.top/gthhdpdtbb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.cucudq.cn/gtspvvvxss.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.mhx1999.top/gtrotgsmnb.html

C#:   Debug.Assert(x > 0);
来源：http://hz.mhx1999.top/gtyuldfuhk.html

[H08] 获取错误信息与堆栈
来源：http://hz.haohaochexian.top/gtkkllqoiv.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.meibo888.top/gtjduvmnaq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.tian-w.cn/gtfysxlaga.html

JS:   e.message;  e.stack
来源：http://hz.sufxvd.cn/gttucqponm.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.aizwys.cn/gtrqyczuay.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.daxiang520.top/gthqlnxyxk.html

Go:   err.Error()
来源：http://hz.yongpay.top/gtdjxqgafb.html

Ruby: e.message;  e.backtrace
来源：http://hz.ydjk.org.cn/gtttlqcvll.html

C#:   e.Message;  e.StackTrace
来源：http://hz.hysaishi.cn/gtmtrohgkh.html

[H09] 带错误码的异常
来源：http://hz.cashguo.top/gtkuuqwinz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yj20258.top/gtvphijazj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ydzc1.top/gtdhsrtyff.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.guannengcc.top/gtujkldflv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jinqigfzy.top/gtgjyojctz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yanxiufei.cn/gtsyjtedgi.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.haohaochexian.top/gtgzblkeje.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.cheryme.top/gtxhzkseti.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yj20258888.top/gtjnyvffhk.html

[H10] 资源自动释放
来源：http://hz.smart0.xyz/gtrmmssedn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.xuetiantiany.cn/gteeazksyv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yuxming.cn/gtcmhobauq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.nwbrower.top/gteoocjcbw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.tanke756.top/gtgnacunwx.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.cucudq.cn/gtpvyjmsnn.html

Go:   defer f.Close()
来源：http://hz.feifeiyinyue.top/gtwpoasumb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.shzxlz.cn/gtwtnbkcyf.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.xylfe.cn/gttbjbctuj.html

================================================================================
来源：http://hz.jiagoushi.top/gtfppghpes.html

I. 正则表达式
来源：http://hz.zycfv.cn/gtfsemfhna.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtqwxsullq.html

[I01] 判断是否匹配
来源：http://hz.nanxinkj.top/gtedtljyul.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yueranfly.top/gtsqztybvq.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.bjfxy.top/gtiqvsxymo.html

JS:   /\d+/.test(s)
来源：http://hz.gogol.net.cn/gtdvoraixb.html

TS:   /\d+/.test(s)
来源：http://hz.xinyue.icu/gtvtvxprlb.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jiagoushi.top/gthkcnozxu.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.gotoacloud.top/gtgblogoir.html

Ruby: s.match?(/\d+/)
来源：http://hz.zdqjudy.top/gtlkezwnlv.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.tianlin.xyz/gtqshbuwbl.html

[I02] 提取所有匹配
来源：http://hz.316326.xyz/gtbccplogl.html

Py:   re.findall(r"\d+", s)
来源：http://hz.svipenyu.cn/gtmpubkylq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.redwolf501.top/gtnfvesrle.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.cashguo.top/gtcmqxbfaj.html

TS:   s.match(/\d+/g)
来源：http://hz.cucudq.cn/gtunfyvigz.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jiagoushi.top/gtuzkkgmmi.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.svipenyu.cn/gtdydmwynu.html

Ruby: s.scan(/\d+/)
来源：http://hz.fengsongda.top/gtxqedzcst.html


<!-- 参考信息 -->