代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.vqdsnc.cn/gtvdbolvut.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yongpay.top/gtqwbnenhq.html

Ruby: Dir.children("dir")
来源：http://hz.shanyushiyangkeji.top/gtpklojbrd.html

C#:   Directory.GetFiles("dir")
来源：http://hz.0kj1m.cn/gtpsqmvbxu.html

[F09] 获取文件大小
来源：http://hz.yj20258.top/gthbwmdkta.html

Py:   os.path.getsize("a.txt")
来源：http://hz.gogol.net.cn/gtrijrdafn.html

PHP:  filesize("a.txt");
来源：http://hz.316326.xyz/gtejvayzdj.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zhaomingkeji.xyz/gteiiauzzn.html

TS:   fs.statSync("a.txt").size
来源：http://hz.ivvv.top/gtqrgatxqv.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yanxiufei.cn/gtmvjtizga.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jyoumei.cn/gtxaddwbvv.html

Ruby: File.size("a.txt")
来源：http://hz.yuxming.cn/gtmboozfrc.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.9152youxi.cn/gtbztoxiyv.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.wangdashe.top/gtwyianvio.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yanxiufei.cn/gtoyzrbbud.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.gotoacloud.top/gtqofygnow.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.sysykeji.top/gtkjofhfhe.html

TS:   path.extname("a.txt")
来源：http://hz.52xcode.cn/gtnikmrnzj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.tanke756.top/gtxvsiorxm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.9152youxi.cn/gtzcqqjelu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.daria6918.cn/gtxxvrdgsi.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.tianlin.xyz/gtaipuqxgu.html

[F11] 复制与移动文件
来源：http://hz.sysykeji.top/gtuadvwxdu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.redwolf501.top/gtokaxuceu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.dashuyun.cn/gtyisjryfr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ydjk.org.cn/gtvtxfmytl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jianghu66.top/gtywheelfx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.daria6918.cn/gtwqsldtjn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.gotoacloud.top/gtzkdbwkfk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jyoumei.cn/gtvxkplvxh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.nanxuanxn.top/gtyqvminyk.html

[F12] CSV 读写
来源：http://hz.xuetiantiany.cn/gtumknmoob.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xuanzx.com/gtpeeqfsfy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.ydzc1.top/gtnbexggwc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.hammf.cn/gtxeriirws.html

TS:   // 同上
来源：http://hz.cashguo.top/gtzkklaggs.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.52xcode.cn/gtttajgmxa.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.birdmap.top/gtwmrjonka.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.gotoacloud.top/gtornvqiqy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.gotoacloud.top/gthjexyzhr.html

================================================================================
来源：http://hz.yuanzhike.top/gtymyiwuge.html

G. 面向对象
来源：http://hz.quarkkingdee.top/gtnyxajuin.html

================================================================================
来源：http://hz.jlsjyb.cn/gtadfgsldy.html

[G01] 定义类
来源：http://hz.jinqigufen.top/gtifxxsdvg.html

Py:   class User: pass
来源：http://hz.sysykeji.top/gtedbyvaul.html

PHP:  class User {}
来源：http://hz.havefunace.top/gtahceudzt.html

JS:   class User {}
来源：http://hz.jinqigufen.top/gtxyzvmnfr.html

TS:   class User { name: string = ""; }
来源：http://hz.aibaodan.cn/gtnvxhzroq.html

Java: class User {}
来源：http://hz.yj20258888.top/gtgggmnlyv.html

Go:   type User struct { Name string }
来源：http://hz.svipenyu.cn/gtfbphqplr.html

Ruby: class User; end
来源：http://hz.havefunace.top/gtxrcgqwua.html

C#:   class User {}
来源：http://hz.zhengqikj.top/gtkgftausd.html

[G02] 构造函数
来源：http://hz.kuanghao11.cn/gtbtajgwdu.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.aibaodan.cn/gtxrkuldrp.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.redwolf501.top/gtkghayofp.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.sxryk.cn/gtarkaplxc.html

TS:   constructor(public name: string) {}
来源：http://hz.guannengcc.top/gtmduwisuf.html

Java: User(String name) { this.name = name; }
来源：http://hz.ydzc1.top/gtxpzhdiza.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.shanyushiyangkeji.top/gtgvvoiioy.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.gotoacloud.top/gtctenwlpr.html

C#:   public User(string name) { Name = name; }
来源：http://hz.dianchejie.cn/gtctyrucki.html

[G03] 实例属性
来源：http://hz.fengsongda.top/gtvkodpily.html

Py:   self.name = "x"
来源：http://hz.sufxvd.cn/gtkvukvndr.html

PHP:  public string $name = "x";
来源：http://hz.0kj1m.cn/gtjmfecqzb.html

JS:   this.name = "x";
来源：http://hz.vqdsnc.cn/gtiqvqrykp.html

TS:   name: string = "x";
来源：http://hz.hnqzz.top/gtlifeoslv.html

Java: private String name;
来源：http://hz.zycfv.cn/gtnowogtkm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.ehwqpu.com/gthhuzpwzu.html

Ruby: @name = "x"
来源：http://hz.shanyushiyangkeji.top/gtivwvykny.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.guowangkeji.top/gtsdwiysfv.html

[G04] 定义方法
来源：http://hz.vqdsnc.cn/gtewoqejvc.html

Py:   def greet(self): return self.name
来源：http://hz.jqgufenzy.top/gtugtcdyiy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.tanke756.top/gtgsbmnbgu.html

JS:   greet() { return this.name; }
来源：http://hz.yongpay.top/gtcsclmmyu.html

TS:   greet(): string { return this.name; }
来源：http://hz.sysykeji.top/gtfmfciguq.html

Java: String greet() { return name; }
来源：http://hz.yvedp.cn/gtgqmxvowy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.nanxuanxn.top/gtaspxgwhq.html

Ruby: def greet; @name; end
来源：http://hz.nwbrower.top/gtxuwlocnh.html

C#:   public string Greet() => Name;
来源：http://hz.daxiang520.top/gtazafgyjf.html

[G05] 继承
来源：http://hz.jiagoushi.top/gttgilnbtk.html

Py:   class Admin(User): pass
来源：http://hz.jianghu66.top/gtlvnxugjz.html

PHP:  class Admin extends User {}
来源：http://hz.yueranfly.top/gtapjwcqis.html

JS:   class Admin extends User {}
来源：http://hz.yj202588.top/gtuthxgrez.html

TS:   class Admin extends User {}
来源：http://hz.zhongyouzk.top/gtrxoegmbi.html

Java: class Admin extends User {}
来源：http://hz.fengsongda.top/gtonmuktoq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.xuetiantiany.cn/gttcjnovgf.html

Ruby: class Admin < User; end
来源：http://hz.aizwys.cn/gtqthkatum.html

C#:   class Admin : User {}
来源：http://hz.gaohongyu789.top/gtyfojiuko.html

[G06] 重写方法
来源：http://hz.jinqigfzy.top/gtiwxirigx.html

Py:   def greet(self): return "admin"
来源：http://hz.cdnleiting.top/gtjbxdmtcz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jlsjyb.cn/gtsaspmyse.html

JS:   greet() { return "admin"; }
来源：http://hz.shanyushiyangtech.top/gtbjmvugff.html

TS:   greet(): string { return "admin"; }
来源：http://hz.ydzc1.top/gtahyhwfhq.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yuxming.cn/gtxcbtqxnz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jlsjyb.cn/gtxkrmbdwn.html

Ruby: def greet; "admin"; end
来源：http://hz.tian-w.cn/gtbauexyzf.html

C#:   public override string Greet() => "admin";
来源：http://hz.jiagoushi.top/gtlkmckomm.html

[G07] 调用父类方法
来源：http://hz.aizwys.cn/gthbksqugo.html

Py:   super().greet()
来源：http://hz.dashuyun.cn/gtmndfpfpq.html

PHP:  parent::greet();
来源：http://hz.hongshengwenyu.top/gtriymubjk.html

JS:   super.greet();
来源：http://hz.jiagoushi.top/gtynatppqy.html

TS:   super.greet();
来源：http://hz.jqgufenzy.top/gtlwspaoag.html

Java: super.greet();
来源：http://hz.andypj.xyz/gtvptmgnvg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.cucudq.cn/gtkenmwynk.html

Ruby: super
来源：http://hz.gogol.net.cn/gtjninjcnz.html

C#:   base.Greet();
来源：http://hz.ehwqpu.com/gtlkevewgg.html

[G08] 静态方法与属性
来源：http://hz.hysaishi.cn/gtqgpqnlnz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.chenlongwang.top/gtzoebduyi.html

PHP:  public static function f() {}
来源：http://hz.dianchejie.cn/gtnkehusbl.html

JS:   static f() {}
来源：http://hz.sufxvd.cn/gteqwkjnae.html

TS:   static f(): void {}
来源：http://hz.c1oappe.top/gtrlihukav.html

Java: static void f() {}
来源：http://hz.jinqigufen.top/gtomtjuriv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.gotoacloud.top/gtpdjroefw.html

Ruby: def self.f; end
来源：http://hz.nanxuanxn.top/gtwbxrwjmv.html

C#:   public static void F() {}
来源：http://hz.hfpthk.cn/gtshmkljdy.html

[G09] 接口 / 抽象类
来源：http://hz.0kj1m.cn/gtwhoxhypm.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.nanxuanxn.top/gtcnhfbwwn.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jinqigufen.top/gtzwgnnmpw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.sufxvd.cn/gtvoheysyg.html

TS:   interface Shape { area(): number; }
来源：http://hz.svipenyu.cn/gtnmdjewam.html

Java: interface Shape { double area(); }
来源：http://hz.guowangkeji.top/gtycwvnwam.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.snrcjt.cn/gtieuctnuo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.9152youxi.cn/gtptdyrwnn.html

C#:   interface IShape { double Area(); }
来源：http://hz.xingfuxueyuan.xyz/gtlsrfmwnl.html

[G10] 访问控制
来源：http://hz.c1oappe.top/gtizmpevyz.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhengqikj.top/gtougzovmh.html

PHP:  public / protected / private
来源：http://hz.316326.xyz/gthlwgeqec.html

JS:   #private 字段；其余公开
来源：http://hz.yj20258888.top/gtzoyrswkz.html

TS:   public / protected / private
来源：http://hz.52xcode.cn/gthcuhtwie.html

Java: public / protected / private / 默认包级
来源：http://hz.pengpengdd.cyou/gtfnkxtjld.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.redwolf501.top/gteufmhjvd.html

Ruby: public / protected / private
来源：http://hz.jqgufenzy.top/gtlscelfue.html

C#:   public / protected / private / internal
来源：http://hz.yj202588.top/gtdnrudbfm.html

[G11] getter / setter
来源：http://hz.xinyue.icu/gthlwlmphf.html

Py:   @property 与 @x.setter
来源：http://hz.shangyingyoupin.top/gtvdrilhvc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.cucudq.cn/gtajylwjkl.html

JS:   get name() { return this._name; }
来源：http://hz.hfpthk.cn/gtxjinlgxq.html

TS:   get name(): string { return this._name; }
来源：http://hz.gotoacloud.top/gtjasjgiht.html

Java: public String getName() { return name; }
来源：http://hz.nanxuanxn.top/gtoficqqfy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yj20258.top/gttjmouzpx.html

Ruby: attr_accessor :name
来源：http://hz.jqgufenzy.top/gtbefinhce.html

C#:   public string Name { get; set; }
来源：http://hz.dashuyun.cn/gtvxdjducf.html

[G12] 对象转字符串
来源：http://hz.birdmap.top/gtnitnfciu.html

Py:   def __str__(self): return self.name
来源：http://hz.gaohongyu789.top/gtslvzrrxv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.52xcode.cn/gtegaechea.html

JS:   toString() { return this.name; }
来源：http://hz.quarkkingdee.top/gtogwszhdj.html

TS:   toString(): string { return this.name; }
来源：http://hz.hnqzz.top/gtwybhvhrj.html

Java: @Override public String toString() { return name; }
来源：http://hz.zhiwuduotai.top/gtswxwvblk.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.ppjwa.cn/gtymyvobjg.html

Ruby: def to_s; @name; end
来源：http://hz.xuanzx.com/gtotoegvko.html

C#:   public override string ToString() => Name;
来源：http://hz.xinyue.icu/gtdronhrmj.html

[G13] 判断对象类型
来源：http://hz.nanxuanxn.top/gtjiuqeqke.html

Py:   isinstance(u, User)
来源：http://hz.hfpthk.cn/gtrlomrrxt.html

PHP:  $u instanceof User
来源：http://hz.ivvv.top/gtmnfzqcoj.html

JS:   u instanceof User
来源：http://hz.zhoulong.xyz/gtiqpgfjrm.html

TS:   u instanceof User
来源：http://hz.shzxlz.cn/gthfxhndqc.html

Java: u instanceof User
来源：http://hz.yongpay.top/gtxiibyjac.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.shanyushiyangtech.top/gtphgwakvx.html

Ruby: u.is_a?(User)
来源：http://hz.shanyushiyangkeji.top/gteysburcw.html

C#:   u is User
来源：http://hz.pycfn.com/gtoracynxt.html

[G14] 数据类 / record
来源：http://hz.nanxinkj.top/gthyzejurf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jyoumei.cn/gtachukzlb.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.0kj1m.cn/gtztmtuwkg.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.havefunace.top/gtunpfwzyb.html

TS:   type User = { name: string; age: number };
来源：http://hz.zhijiandao.cn/gtgxgpseux.html

Java: record User(String name, int age) {}
来源：http://hz.quarkkingdee.top/gtdpgwrtbd.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jiagoushi.top/gtxhzwwhjb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.dianchejie.cn/gtekxoyrkt.html

C#:   record User(string Name, int Age);
来源：http://hz.feifeiyinyue.top/gtqefshwjr.html

[G15] 枚举
来源：http://hz.ywan-chungtsiang.top/gtpmdrggqt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.gaohongyu789.top/gtlpdsdyty.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.0kj1m.cn/gtxpoumwbf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.shangyingyoupin.top/gtekuameva.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.snrcjt.cn/gtlngjumsr.html

Java: enum Color { RED, GREEN }
来源：http://hz.zhixingplan.top/gthfujfuzs.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.havefunace.top/gthdmwsmfq.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ydzc1.top/gtxvaxriis.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yj20258.top/gtfuyndtvc.html

[G16] 对象转数组 / 字典
来源：http://hz.zhongyouzk.top/gtmiziqzsz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.dianchejie.cn/gtopwgpddr.html

PHP:  get_object_vars($obj);
来源：http://hz.zhixingplan.top/gtphhwrsem.html

JS:   Object.entries(obj)
来源：http://hz.cdnleiting.top/gtklfwsjkv.html

TS:   Object.entries(obj)
来源：http://hz.wangdashe.top/gtnlzaveyx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.0kj1m.cn/gtekekiwfv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yueranfly.top/gtrtuocsob.html

Ruby: obj.instance_variables
来源：http://hz.zhengqikj.top/gtakzztbwg.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jlsjyb.cn/gtnzmmdtjl.html

================================================================================
来源：http://hz.sweek.top/gtxoqysltw.html

H. 异常与错误处理
来源：http://hz.daxiang520.top/gtpnvljblc.html

================================================================================
来源：http://hz.yvedp.cn/gttcfyrqif.html

[H01] try / catch 基础
来源：http://hz.cashguo.top/gtiddaoydr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.xingfuxueyuan.xyz/gtaxbujtfq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.nanxinkj.top/gtrhpiyudn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zhaomingkeji.xyz/gtcnjvbtod.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.gaohongyu789.top/gtxtyyoocg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.pycfn.com/gtyftsncny.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.hongshengwenyu.top/gtkdzqspmr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.tian-w.cn/gtrfbzciew.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.tianlin.xyz/gttbdkjquk.html

[H02] finally / ensure 收尾
来源：http://hz.zhaomingkeji.xyz/gtwmavxvup.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yonumen.top/gtxhqfeftt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.chenlongwang.top/gtzyvlylmt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.quarkkingdee.top/gtuumcbopn.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jinyuanbaomall.cn/gtfnzmgqve.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.shuidangran.top/gtsxkddcje.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zhijiandao.cn/gtqixkdktp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.shanyushiyangtech.top/gtyrzzxtmf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zhoulong.xyz/gtnywfffuw.html

[H03] 主动抛出异常
来源：http://hz.hnqzz.top/gtqrwwgvxo.html

Py:   raise ValueError("错误信息")
来源：http://hz.hnqzz.top/gttdojwrlg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.aizwys.cn/gtidcqcvfi.html

JS:   throw new Error("错误信息");
来源：http://hz.shanyushiyangtech.top/gtwwlgynoe.html

TS:   throw new Error("错误信息");
来源：http://hz.yueranfly.top/gtyncylazn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jinqigufen.top/gtmbzlsuhu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.dianchejie.cn/gtixmbbqgf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.shuidangran.top/gttuibkxcj.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.hnxiangtu.top/gtedjzsmba.html

[H04] 自定义异常类型
来源：http://hz.cqqwz.cn/gtiyeatzmc.html

Py:   class MyError(Exception): pass
来源：http://hz.shuidangran.top/gtophxzvus.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yueranfly.top/gtbifitoyr.html

JS:   class MyError extends Error {}
来源：http://hz.yvedp.cn/gtckeyqodz.html

TS:   class MyError extends Error {}
来源：http://hz.jinqigfzy.top/gtuooqkemw.html

Java: class MyException extends RuntimeException {}
来源：http://hz.gzhubu.top/gtqjvoqwdz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.xingfuxueyuan.xyz/gtxntzbide.html

Ruby: class MyError < StandardError; end
来源：http://hz.9152youxi.cn/gtvrxnyxzr.html

C#:   class MyException : Exception {}
来源：http://hz.yongpay.top/gtznjeqhyo.html

[H05] 捕获特定类型
来源：http://hz.shanyushiyangkeji.top/gtrctavhas.html

Py:   except ValueError as e:
来源：http://hz.pengpengdd.cyou/gtpvprtgrv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.nanxuanxn.top/gtlesaljqr.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yuxming.cn/gtajtgyzfx.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jinqigfzy.top/gtxsirbcey.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yueranfly.top/gtotflnyzi.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.cdnleiting.top/gtbhpklnxv.html

Ruby: rescue ArgumentError => e
来源：http://hz.shanyushiyangtech.top/gtyhizywvc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.feifeiyinyue.top/gttxgvzupj.html

[H06] 可选值 / 空值安全访问
来源：http://hz.quarkkingdee.top/gtlpozrjjw.html

Py:   value = d.get("k") or default
来源：http://hz.ywan-chungtsiang.top/gtknxyefrv.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.kuanghao11.cn/gtiqdpheek.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.andypj.xyz/gteoiqxvri.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yueranfly.top/gtsqinghwo.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhoulong.xyz/gtmjczvsdi.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.vqdsnc.cn/gtalwlmias.html

Ruby: d&.dig(:a, :b)
来源：http://hz.9152youxi.cn/gtiyvdwbki.html

C#:   obj?.A?.B ?? default
来源：http://hz.9152youxi.cn/gtfhuiaxlt.html

[H07] 断言
来源：http://hz.ywan-chungtsiang.top/gtvlwstktc.html

Py:   assert x > 0, "必须为正"
来源：http://hz.dashuyun.cn/gtlzeixlmx.html

PHP:  assert($x > 0);
来源：http://hz.hnqzz.top/gtnjgimqwv.html

JS:   console.assert(x > 0);
来源：http://hz.jinghuilouyu.cn/gtimtcmbom.html

TS:   console.assert(x > 0);
来源：http://hz.vqdsnc.cn/gtcydmalsy.html

Java: assert x > 0 : "必须为正";
来源：http://hz.sxryk.cn/gttujopxkz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.sweek.top/gtyljbcyhg.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.aibaodan.cn/gtdlyiezex.html

C#:   Debug.Assert(x > 0);
来源：http://hz.kuanghao11.cn/gtgdxkubwp.html

[H08] 获取错误信息与堆栈
来源：http://hz.dianchejie.cn/gtjnaezbqc.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.0kj1m.cn/gtxdoemsud.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.vqdsnc.cn/gtsxbvfnne.html

JS:   e.message;  e.stack
来源：http://hz.zhoulong.xyz/gtgywbanod.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.sysykeji.top/gtoxfvuuio.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.birdmap.top/gtpsigbaks.html

Go:   err.Error()
来源：http://hz.meibo888.top/gtbyomejno.html

Ruby: e.message;  e.backtrace
来源：http://hz.yanxiufei.cn/gtteqposvt.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ybcxt.top/gtztxbkcay.html

[H09] 带错误码的异常
来源：http://hz.ydjk.org.cn/gtcnkwjggp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jiagoushi.top/gtljrkejdy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zycfv.cn/gtlmohhzzz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.xuanzx.com/gtutipwowg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yuxming.cn/gtgfoeywyk.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.gaohongyu789.top/gtygkhavcw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.kuanghao11.cn/gtjbowflta.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jinqigfzy.top/gtsbsiotoj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jyoumei.cn/gtfwanxgth.html

[H10] 资源自动释放
来源：http://hz.snrcjt.cn/gtaornbjvg.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.chenjidiqi.icu/gtpxzfmqpm.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ppjwa.cn/gtbtlvpvzm.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cheryme.top/gteiafexvh.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xinyue.icu/gtgedxfcrw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zhongyouzk.top/gtgizspkaq.html

Go:   defer f.Close()
来源：http://hz.ybcxt.top/gtapcmmkjy.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jinqigufen.top/gtykrtanyf.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.bjfxy.top/gtkfdmcidp.html

================================================================================
来源：http://hz.svipenyu.cn/gtyunqnnnr.html

I. 正则表达式
来源：http://hz.gaohongyu789.top/gtayjkgvzu.html

================================================================================
来源：http://hz.yuxming.cn/gtixqfrsox.html

[I01] 判断是否匹配
来源：http://hz.jianghu66.top/gtmlzwduqf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.birdmap.top/gtiyxitpkp.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.daxiang520.top/gtjyavwbbr.html

JS:   /\d+/.test(s)
来源：http://hz.yonumen.top/gtajhiflmq.html

TS:   /\d+/.test(s)
来源：http://hz.sxryk.cn/gtdbafrqcx.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.birdmap.top/gtedpvubqz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.ywan-chungtsiang.top/gtchypzysx.html

Ruby: s.match?(/\d+/)
来源：http://hz.sysykeji.top/gtpjtyizfc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.shzxlz.cn/gtplfrhtzs.html

[I02] 提取所有匹配
来源：http://hz.svipenyu.cn/gtbjepywtx.html

Py:   re.findall(r"\d+", s)
来源：http://hz.iojbl.cn/gtsqqhvhhq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.316326.xyz/gtypyvfiwb.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jlsjyb.cn/gtyysveweo.html

TS:   s.match(/\d+/g)
来源：http://hz.gaohongyu789.top/gticqpixbz.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.cashguo.top/gtgtrododa.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.tianlin.xyz/gtymeyttmi.html

Ruby: s.scan(/\d+/)
来源：http://hz.shanyushiyangkeji.top/gtboduvcdt.html


<!-- 参考信息 -->