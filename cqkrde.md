代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://hz.aibaodan.cn/gttgrlkxqh.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.c1oappe.top/gtvougntzb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.shanyushiyangkeji.top/gtgknwodks.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zhijiandao.cn/gtgjhvphsv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.316326.xyz/gtzrnyaaya.html

TS:   path.extname("a.txt")
来源：http://hz.xuetiantiany.cn/gtqpcvquhz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.cheryme.top/gtgighywhd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jianghu66.top/gtogzwfqnw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.shangyingyoupin.top/gtqofuprkn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zhaomingkeji.xyz/gtlxlsbivc.html

[F11] 复制与移动文件
来源：http://hz.zhaomingkeji.xyz/gtuwpvijax.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.pengpengdd.cyou/gtqethsmsb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.shanyushiyangkeji.top/gtsfhcjjwd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.kuanghao11.cn/gtdcwmghzn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.316326.xyz/gttfnblxnj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jiagoushi.top/gtejqtyfup.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.ybcxt.top/gtuqousxpe.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.cucudq.cn/gtndjargqo.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.hongshengwenyu.top/gtwespkuuo.html

[F12] CSV 读写
来源：http://hz.ydjk.org.cn/gtzdlqstyz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.ywan-chungtsiang.top/gtlytrxknt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.cashguo.top/gtizdshwqp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.ybcxt.top/gtggqgdgxf.html

TS:   // 同上
来源：http://hz.yongpay.top/gtfrcmlvro.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.svipenyu.cn/gtelslgnnk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhengqikj.top/gtevrlystr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.cdnleiting.top/gtehkqpxvq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.birdmap.top/gtauqafchz.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtzvapxgwb.html

G. 面向对象
来源：http://hz.kuanghao11.cn/gtvobzsgwd.html

================================================================================
来源：http://hz.snrcjt.cn/gteryolxcu.html

[G01] 定义类
来源：http://hz.ybcxt.top/gtdxxxxdoo.html

Py:   class User: pass
来源：http://hz.guowangkeji.top/gtqjxukfih.html

PHP:  class User {}
来源：http://hz.shuidangran.top/gtpnpsxfup.html

JS:   class User {}
来源：http://hz.quarkkingdee.top/gtejfyofvp.html

TS:   class User { name: string = ""; }
来源：http://hz.yuanzhike.top/gthmmktzwz.html

Java: class User {}
来源：http://hz.svipenyu.cn/gthpdilxdh.html

Go:   type User struct { Name string }
来源：http://hz.zhaomingkeji.xyz/gtkvcfenwh.html

Ruby: class User; end
来源：http://hz.zhiwuduotai.top/gtjovcrcws.html

C#:   class User {}
来源：http://hz.yangfankeji.com/gtjxutznzr.html

[G02] 构造函数
来源：http://hz.gogol.net.cn/gtnvnzivgm.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yanxiufei.cn/gtstmndkhk.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.52xcode.cn/gtjqtxlqaf.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.gaohongyu789.top/gtkdqzvxay.html

TS:   constructor(public name: string) {}
来源：http://hz.hammf.cn/gtitftnkkw.html

Java: User(String name) { this.name = name; }
来源：http://hz.jinqigfzy.top/gtpgbemdep.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yueranfly.top/gtlekubbvp.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.hysaishi.cn/gtxmuuhhfu.html

C#:   public User(string name) { Name = name; }
来源：http://hz.tian-w.cn/gtshcjqcqr.html

[G03] 实例属性
来源：http://hz.jiagoushi.top/gtibqcplzk.html

Py:   self.name = "x"
来源：http://hz.ppjwa.cn/gtugvkyxro.html

PHP:  public string $name = "x";
来源：http://hz.daxiang520.top/gtzjhsxivm.html

JS:   this.name = "x";
来源：http://hz.havefunace.top/gtsvuvzjfg.html

TS:   name: string = "x";
来源：http://hz.gotoacloud.top/gtepnrqitd.html

Java: private String name;
来源：http://hz.gotoacloud.top/gtgzpwgahq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.sxryk.cn/gtikvqtcch.html

Ruby: @name = "x"
来源：http://hz.xingfuxueyuan.xyz/gtzwdczkqj.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.chenlongwang.top/gthddimtcz.html

[G04] 定义方法
来源：http://hz.shuidangran.top/gtzhxxbjwq.html

Py:   def greet(self): return self.name
来源：http://hz.daria6918.cn/gtjbmpejwe.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhengqikj.top/gtjlyyhivr.html

JS:   greet() { return this.name; }
来源：http://hz.zdqjudy.top/gtqosxaigz.html

TS:   greet(): string { return this.name; }
来源：http://hz.9152youxi.cn/gtciyctobt.html

Java: String greet() { return name; }
来源：http://hz.zhengqikj.top/gtlgmrkvsa.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.nwbrower.top/gtopookuik.html

Ruby: def greet; @name; end
来源：http://hz.yonumen.top/gtsbddpxrk.html

C#:   public string Greet() => Name;
来源：http://hz.tanke756.top/gtzpjdjfpk.html

[G05] 继承
来源：http://hz.zhoulong.xyz/gtyysyywnn.html

Py:   class Admin(User): pass
来源：http://hz.shanyushiyangkeji.top/gtdvkvaioy.html

PHP:  class Admin extends User {}
来源：http://hz.jianghu66.top/gtggukczoc.html

JS:   class Admin extends User {}
来源：http://hz.zdqjudy.top/gtcysimepi.html

TS:   class Admin extends User {}
来源：http://hz.zhiwuduotai.top/gtzkxhpiek.html

Java: class Admin extends User {}
来源：http://hz.ydzc1.top/gtkxeicexv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.9152youxi.cn/gttpkdbcrk.html

Ruby: class Admin < User; end
来源：http://hz.zhijiandao.cn/gtfrgojlfd.html

C#:   class Admin : User {}
来源：http://hz.yj202588.top/gtvzulgygk.html

[G06] 重写方法
来源：http://hz.cucudq.cn/gtfhmupkki.html

Py:   def greet(self): return "admin"
来源：http://hz.kuanghao11.cn/gtgrdduxnk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jyoumei.cn/gtqevvkjut.html

JS:   greet() { return "admin"; }
来源：http://hz.wangshuangyany.cn/gtprkbieks.html

TS:   greet(): string { return "admin"; }
来源：http://hz.meibo888.top/gtmegdxzkz.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.andypj.xyz/gtuczeadma.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yueranfly.top/gtihrodpzv.html

Ruby: def greet; "admin"; end
来源：http://hz.yvedp.cn/gtxcyycsdf.html

C#:   public override string Greet() => "admin";
来源：http://hz.ywan-chungtsiang.top/gtevuymzbn.html

[G07] 调用父类方法
来源：http://hz.jinyuanbaomall.cn/gtscpxbasg.html

Py:   super().greet()
来源：http://hz.pengpengdd.cyou/gttzxndafm.html

PHP:  parent::greet();
来源：http://hz.hysaishi.cn/gtzgopybgm.html

JS:   super.greet();
来源：http://hz.ybcxt.top/gtsjsywhkg.html

TS:   super.greet();
来源：http://hz.ydjk.org.cn/gtxfxjnnyw.html

Java: super.greet();
来源：http://hz.gzhubu.top/gtbdszpnmo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.hammf.cn/gtjfgijxto.html

Ruby: super
来源：http://hz.zycfv.cn/gtkfcvrwcd.html

C#:   base.Greet();
来源：http://hz.xziqi.cn/gtahwoijsx.html

[G08] 静态方法与属性
来源：http://hz.ppjwa.cn/gtfdipwyad.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yj202588.top/gtrpiypkmc.html

PHP:  public static function f() {}
来源：http://hz.hnxiangtu.top/gtcnobfpfk.html

JS:   static f() {}
来源：http://hz.daria6918.cn/gtxwjrwnja.html

TS:   static f(): void {}
来源：http://hz.jinqigufen.top/gtmqjxhlrg.html

Java: static void f() {}
来源：http://hz.ywan-chungtsiang.top/gtuquxpowt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.52xcode.cn/gtgoanqalz.html

Ruby: def self.f; end
来源：http://hz.yuanzhike.top/gtzxxgguzb.html

C#:   public static void F() {}
来源：http://hz.jlsjyb.cn/gtggqkubft.html

[G09] 接口 / 抽象类
来源：http://hz.iojbl.cn/gtzvuuqufz.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.xuanzx.com/gtshhhjrsf.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.gotoacloud.top/gtqmqozjyj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.52xcode.cn/gtmsxjsjlq.html

TS:   interface Shape { area(): number; }
来源：http://hz.nanxinkj.top/gtpnhwcsdi.html

Java: interface Shape { double area(); }
来源：http://hz.yj20258.top/gtkexwayeu.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yongpay.top/gtxdmvsnem.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.tianlin.xyz/gtzzcpanmg.html

C#:   interface IShape { double Area(); }
来源：http://hz.aizwys.cn/gtsutdxdvj.html

[G10] 访问控制
来源：http://hz.dianchejie.cn/gtplwiutgt.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.52xcode.cn/gtcaxwypjp.html

PHP:  public / protected / private
来源：http://hz.xinyue.icu/gtiwuqzwnl.html

JS:   #private 字段；其余公开
来源：http://hz.c1oappe.top/gtubiemnhi.html

TS:   public / protected / private
来源：http://hz.svipenyu.cn/gtmrmzgeht.html

Java: public / protected / private / 默认包级
来源：http://hz.cdnleiting.top/gtmxvsxwjw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yongpay.top/gtvmefbkap.html

Ruby: public / protected / private
来源：http://hz.yj202588.top/gtcwdwzmrk.html

C#:   public / protected / private / internal
来源：http://hz.ydzc1.top/gtbkrlqqqj.html

[G11] getter / setter
来源：http://hz.jinghuilouyu.cn/gtroqkebce.html

Py:   @property 与 @x.setter
来源：http://hz.jianghu66.top/gtgdxxbpls.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.iojbl.cn/gtohwmdtwb.html

JS:   get name() { return this._name; }
来源：http://hz.ywan-chungtsiang.top/gtcwcyienp.html

TS:   get name(): string { return this._name; }
来源：http://hz.0kj1m.cn/gtydfjxepw.html

Java: public String getName() { return name; }
来源：http://hz.jinqigfzy.top/gtiolsgwwq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zhaomingkeji.xyz/gtvfxeglsi.html

Ruby: attr_accessor :name
来源：http://hz.nwbrower.top/gttvhuxbhr.html

C#:   public string Name { get; set; }
来源：http://hz.xziqi.cn/gtxzrfygdz.html

[G12] 对象转字符串
来源：http://hz.gotoacloud.top/gturtactac.html

Py:   def __str__(self): return self.name
来源：http://hz.c1oappe.top/gtuvvfjbri.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.cqqwz.cn/gtxkzzkyzr.html

JS:   toString() { return this.name; }
来源：http://hz.guowangkeji.top/gtizwpczsc.html

TS:   toString(): string { return this.name; }
来源：http://hz.dashuyun.cn/gtlqplzwor.html

Java: @Override public String toString() { return name; }
来源：http://hz.hammf.cn/gtjrlplkpc.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yj202588.top/gtkckbhpvv.html

Ruby: def to_s; @name; end
来源：http://hz.ehwqpu.com/gtskslttxc.html

C#:   public override string ToString() => Name;
来源：http://hz.zhiwuduotai.top/gtswfglwye.html

[G13] 判断对象类型
来源：http://hz.cheryme.top/gtqyrjnaky.html

Py:   isinstance(u, User)
来源：http://hz.xinyue.icu/gttuzmhbwj.html

PHP:  $u instanceof User
来源：http://hz.nanxuanxn.top/gtcccmrwrd.html

JS:   u instanceof User
来源：http://hz.cheryme.top/gtfrakconj.html

TS:   u instanceof User
来源：http://hz.xinyue.icu/gtgsrugvxp.html

Java: u instanceof User
来源：http://hz.0kj1m.cn/gtrqvplwfa.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yongpay.top/gtqwhzsyud.html

Ruby: u.is_a?(User)
来源：http://hz.xinyue.icu/gtrssiuovu.html

C#:   u is User
来源：http://hz.wangshuangyany.cn/gtyvivagot.html

[G14] 数据类 / record
来源：http://hz.yj202588.top/gtrjvubhuy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zhoulong.xyz/gtirunqqqj.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zhijiandao.cn/gtfgrcfglu.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhixingplan.top/gtwwtjcqem.html

TS:   type User = { name: string; age: number };
来源：http://hz.jinqigufen.top/gttkshgrec.html

Java: record User(String name, int age) {}
来源：http://hz.xinyue.icu/gtmjmreksg.html

Go:   type User struct { Name string; Age int }
来源：http://hz.shzxlz.cn/gtlfkbycsi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zhengqikj.top/gtsyelcjyb.html

C#:   record User(string Name, int Age);
来源：http://hz.fzhhl.top/gtjyqwtsxo.html

[G15] 枚举
来源：http://hz.dianchejie.cn/gtfudkpdad.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yuanzhike.top/gtmphnyuzm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jiagoushi.top/gtggajxhkv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.dianchejie.cn/gtlxhliapt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ivvv.top/gterwwzuli.html

Java: enum Color { RED, GREEN }
来源：http://hz.52xcode.cn/gtjzisamkj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.nanxinkj.top/gtpsffmnqs.html

Ruby: Color = %i[red green].freeze
来源：http://hz.fzhhl.top/gtijmzivkv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xuanzx.com/gtscckuxaf.html

[G16] 对象转数组 / 字典
来源：http://hz.yuxming.cn/gtffmevnwb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jiagoushi.top/gtgwvegkne.html

PHP:  get_object_vars($obj);
来源：http://hz.nanxuanxn.top/gtbpvaeoas.html

JS:   Object.entries(obj)
来源：http://hz.316326.xyz/gtywlimong.html

TS:   Object.entries(obj)
来源：http://hz.zhengqikj.top/gtzrcrnswt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.xuetiantiany.cn/gtcckuwcbt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jqgfzy.top/gtnyyhukvu.html

Ruby: obj.instance_variables
来源：http://hz.zhaomingkeji.xyz/gtvvhycwwc.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zdqjudy.top/gtsiktmwuy.html

================================================================================
来源：http://hz.ivvv.top/gtygbncdqi.html

H. 异常与错误处理
来源：http://hz.fzhhl.top/gtcpcskzkk.html

================================================================================
来源：http://hz.shzxlz.cn/gtjxbizetw.html

[H01] try / catch 基础
来源：http://hz.hywenlv.cn/gtutecskfk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhongyouzk.top/gtqgrmkwzk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zdqjudy.top/gtrgqpovna.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.316326.xyz/gtxvaoguih.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.ppjwa.cn/gtxhuobmoi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.nanxinkj.top/gtqvvdlahy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zhongyouzk.top/gtqnthgeiy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.cashguo.top/gtkqkifqts.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yj202588.top/gttesuuvts.html

[H02] finally / ensure 收尾
来源：http://hz.daria6918.cn/gtxegzpnkn.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.vqdsnc.cn/gtforcwbaz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.shangyingyoupin.top/gtmbtbjdpc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hnxiangtu.top/gtqinfkfun.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.fengsongda.top/gtqqgguegf.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangkeji.top/gtoptthtme.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jinghuilouyu.cn/gtifxwjpkl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.nanxuanxn.top/gtreqsaxpu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jyoumei.cn/gtcamnhjxc.html

[H03] 主动抛出异常
来源：http://hz.nwbrower.top/gteteoeigp.html

Py:   raise ValueError("错误信息")
来源：http://hz.andypj.xyz/gtqpbrodzs.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.fengsongda.top/gthscfksef.html

JS:   throw new Error("错误信息");
来源：http://hz.wangshuangyany.cn/gtdhimmiyu.html

TS:   throw new Error("错误信息");
来源：http://hz.jqgfzy.top/gttlsfnymj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.pengpengdd.cyou/gttgkwgibv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.quarkkingdee.top/gtwtjguwto.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zhongyouzk.top/gtpspkwkke.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zdqjudy.top/gtkdzzaxuw.html

[H04] 自定义异常类型
来源：http://hz.cucudq.cn/gtxeufvnkf.html

Py:   class MyError(Exception): pass
来源：http://hz.pengpengdd.cyou/gtaghcogdd.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.ywan-chungtsiang.top/gtmimfeviz.html

JS:   class MyError extends Error {}
来源：http://hz.ydjk.org.cn/gteacsmkdr.html

TS:   class MyError extends Error {}
来源：http://hz.hnxiangtu.top/gtgzngtlkn.html

Java: class MyException extends RuntimeException {}
来源：http://hz.shzxlz.cn/gtnteztdpp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.iojbl.cn/gtwldzyvtp.html

Ruby: class MyError < StandardError; end
来源：http://hz.jinghuilouyu.cn/gtfmrfwccy.html

C#:   class MyException : Exception {}
来源：http://hz.gzhubu.top/gtdgvbpysz.html

[H05] 捕获特定类型
来源：http://hz.jinqigfzy.top/gtnnosdkby.html

Py:   except ValueError as e:
来源：http://hz.jyoumei.cn/gtjujntvkq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.xingfuxueyuan.xyz/gtcuvlsyme.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.shangyingyoupin.top/gtjeutipvr.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.kuanghao11.cn/gtrguqbgzp.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.0kj1m.cn/gtrjpaxzsn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hongshengwenyu.top/gtfyfdhasj.html

Ruby: rescue ArgumentError => e
来源：http://hz.daxiang520.top/gtbiohuevf.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.gaohongyu789.top/gtqirnyyec.html

[H06] 可选值 / 空值安全访问
来源：http://hz.wangdashe.top/gtoxtwwlmd.html

Py:   value = d.get("k") or default
来源：http://hz.pycfn.com/gtmutjkhbc.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.quarkkingdee.top/gtrjgrbvmp.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zhoulong.xyz/gtgnwmitmi.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yuanzhike.top/gtrfeeozuy.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.smart0.xyz/gtwljschzy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jlsjyb.cn/gtdtavxfqb.html

Ruby: d&.dig(:a, :b)
来源：http://hz.guowangkeji.top/gtikuocfcw.html

C#:   obj?.A?.B ?? default
来源：http://hz.snrcjt.cn/gthbbmpdak.html

[H07] 断言
来源：http://hz.316326.xyz/gtfnzjkvnw.html

Py:   assert x > 0, "必须为正"
来源：http://hz.xingfuxueyuan.xyz/gtpqqandst.html

PHP:  assert($x > 0);
来源：http://hz.cheryme.top/gtllyzoqvm.html

JS:   console.assert(x > 0);
来源：http://hz.xylfe.cn/gtfynapoak.html

TS:   console.assert(x > 0);
来源：http://hz.aizwys.cn/gtsveglqyd.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jiagoushi.top/gtradoesoj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.quarkkingdee.top/gthjnlsciz.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.guowangkeji.top/gtunuruuqd.html

C#:   Debug.Assert(x > 0);
来源：http://hz.9152youxi.cn/gtpjehtlom.html

[H08] 获取错误信息与堆栈
来源：http://hz.daxiang520.top/gtyjbvrzrs.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.9152youxi.cn/gtukomrrgm.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.xinyue.icu/gttueflihf.html

JS:   e.message;  e.stack
来源：http://hz.xingfuxueyuan.xyz/gtmlkgwnoo.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.tian-w.cn/gtkewixqve.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.0kj1m.cn/gtyikthhew.html

Go:   err.Error()
来源：http://hz.hnqzz.top/gtqkzxoqfg.html

Ruby: e.message;  e.backtrace
来源：http://hz.quarkkingdee.top/gtpbcpnaqi.html

C#:   e.Message;  e.StackTrace
来源：http://hz.guowangkeji.top/gtfwffmsck.html

[H09] 带错误码的异常
来源：http://hz.yongpay.top/gtuxtcjhke.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.daxiang520.top/gtwibbszla.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zhengqikj.top/gtnmucwxqd.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.gotoacloud.top/gtqoszkyjq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.hfpthk.cn/gturuqmkmo.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.dianchejie.cn/gtmawpsulw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.feifeiyinyue.top/gttpfdqroc.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.sweek.top/gtzssxkksn.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.wangdashe.top/gtcagqtqba.html

[H10] 资源自动释放
来源：http://hz.guowangkeji.top/gtjfxukzbu.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.hnqzz.top/gtcnvnmgey.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ehwqpu.com/gtrfuekqpa.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhiwuduotai.top/gtglvxdrmj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shangyingyoupin.top/gtnmqdvbwf.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.bjfxy.top/gtrwgjcnok.html

Go:   defer f.Close()
来源：http://hz.xuetiantiany.cn/gthqzsklyg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.hfpthk.cn/gtuuhtasfy.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.nanxuanxn.top/gtzmllxvhv.html

================================================================================
来源：http://hz.hnqzz.top/gtlvutyotd.html

I. 正则表达式
来源：http://hz.gogol.net.cn/gtindwvxfd.html

================================================================================
来源：http://hz.9152youxi.cn/gtotkeqqku.html

[I01] 判断是否匹配
来源：http://hz.ydjk.org.cn/gtkrntnhfb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.ppjwa.cn/gtbjbchfcr.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.shuidangran.top/gtoohgkmsa.html

JS:   /\d+/.test(s)
来源：http://hz.316326.xyz/gtunktozkp.html

TS:   /\d+/.test(s)
来源：http://hz.52xcode.cn/gtcfyzfkjt.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.smart0.xyz/gtsqgoydqg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hnqzz.top/gtuwrrhyzf.html

Ruby: s.match?(/\d+/)
来源：http://hz.fengsongda.top/gtwedbuejq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.xuanzx.com/gtrxhmrshf.html

[I02] 提取所有匹配
来源：http://hz.jinqigufen.top/gtvcmkekze.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yj20258888.top/gtkdyuhmqo.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.xinyue.icu/gtrllnoyot.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yongpay.top/gtzxuzycpv.html

TS:   s.match(/\d+/g)
来源：http://hz.yj20258888.top/gtepuhrlys.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.chenzaomai.com/gtrhbbqcqd.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zhaomingkeji.xyz/gthznabhut.html

Ruby: s.scan(/\d+/)
来源：http://hz.cucudq.cn/gtirbzgazv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.iojbl.cn/gtrhwnxite.html

[I03] 提取捕获分组
来源：http://hz.gzhubu.top/gtvumabvgd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.ivvv.top/gtqwxzkrsz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.shanyushiyangkeji.top/gtheztvwya.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.havefunace.top/gtqqqxwhgz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.gogol.net.cn/gtcjgpdstv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.nanxinkj.top/gtobysznna.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.fzhhl.top/gtphvadeoc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.xinyue.icu/gtzhmgkvmx.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.xinyue.icu/gtlpiphhxu.html

[I04] 正则替换
来源：http://hz.chenlongwang.top/gttiqxyeod.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.hnxiangtu.top/gtwhpipogg.html


<!-- 参考信息 -->