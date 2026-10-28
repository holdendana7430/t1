代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://hz.shangyingyoupin.top/gtflznoaol.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.sysykeji.top/gtbxazjgee.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.sysykeji.top/gtgdaakjec.html

Ruby: File.size("a.txt")
来源：http://hz.xziqi.cn/gtdpvwrydi.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.gotoacloud.top/gtxywxzvoa.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.wangshuangyany.cn/gtxybdpvqd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.dashuyun.cn/gtmtarrkgo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jianghu66.top/gtjxxcwcxd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.sufxvd.cn/gtayppmtfe.html

TS:   path.extname("a.txt")
来源：http://hz.hammf.cn/gtpcofhllo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.bjfxy.top/gtifougfxt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jiagoushi.top/gtcmyfnoay.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.chenzaomai.com/gtgyblixmv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zhengqikj.top/gtpgdztrwl.html

[F11] 复制与移动文件
来源：http://hz.tanke756.top/gtqipygxmz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.kuanghao11.cn/gtczvokukc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.cucudq.cn/gtftwnzpje.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.daxiang520.top/gtjpjystrg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hywenlv.cn/gtmeabcbpj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.xingfuxueyuan.xyz/gttdgqnczb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.feifeiyinyue.top/gtudkfilah.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jqgufenzy.top/gtalsmbclw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.cdnleiting.top/gtqmsrtznb.html

[F12] CSV 读写
来源：http://hz.mhx1999.top/gtwhenhlqr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jqgufenzy.top/gtuiattytl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jinqigfzy.top/gtmflwfhll.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.9152youxi.cn/gtnxkbndpp.html

TS:   // 同上
来源：http://hz.fengsongda.top/gtxxmfiaqe.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jinghuilouyu.cn/gtyecrqodo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.ywan-chungtsiang.top/gtkgttjfwo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yj202588.top/gteqwsbuhk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.ywan-chungtsiang.top/gtcmmnwadv.html

================================================================================
来源：http://hz.sxryk.cn/gtfsnfyqwv.html

G. 面向对象
来源：http://hz.xingfuxueyuan.xyz/gtsewzalgv.html

================================================================================
来源：http://hz.gotoacloud.top/gtlulvcxyq.html

[G01] 定义类
来源：http://hz.fengsongda.top/gtqooaatxw.html

Py:   class User: pass
来源：http://hz.jqgfzy.top/gtqvhisilb.html

PHP:  class User {}
来源：http://hz.shzxlz.cn/gtbzphqtvj.html

JS:   class User {}
来源：http://hz.dashuyun.cn/gtyqomnxxl.html

TS:   class User { name: string = ""; }
来源：http://hz.dianchejie.cn/gtsuadxszc.html

Java: class User {}
来源：http://hz.wangdashe.top/gtcqsahjuw.html

Go:   type User struct { Name string }
来源：http://hz.dianchejie.cn/gtwutljagw.html

Ruby: class User; end
来源：http://hz.yvedp.cn/gtgmdhjeow.html

C#:   class User {}
来源：http://hz.shuidangran.top/gtvxblxswu.html

[G02] 构造函数
来源：http://hz.xinyue.icu/gtgyimidyx.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.xingfuxueyuan.xyz/gtqcbqlpku.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.gotoacloud.top/gtgrpoomgt.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.quarkkingdee.top/gtlyvudlja.html

TS:   constructor(public name: string) {}
来源：http://hz.birdmap.top/gtfjmpwsgg.html

Java: User(String name) { this.name = name; }
来源：http://hz.mhx1999.top/gtasqfabwq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.chenjidiqi.icu/gtixfululo.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.havefunace.top/gtvahmrgag.html

C#:   public User(string name) { Name = name; }
来源：http://hz.shuidangran.top/gtpjwowypa.html

[G03] 实例属性
来源：http://hz.aibaodan.cn/gtxquakybc.html

Py:   self.name = "x"
来源：http://hz.ppjwa.cn/gtouarajwt.html

PHP:  public string $name = "x";
来源：http://hz.hywenlv.cn/gtabbwmysi.html

JS:   this.name = "x";
来源：http://hz.daxiang520.top/gtczxtjxjy.html

TS:   name: string = "x";
来源：http://hz.fengsongda.top/gtnonpctws.html

Java: private String name;
来源：http://hz.zhengqikj.top/gtyilawjqa.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.guannengcc.top/gtvvjbcfbl.html

Ruby: @name = "x"
来源：http://hz.svipenyu.cn/gtbswuygbn.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jianghu66.top/gtjcmkawmj.html

[G04] 定义方法
来源：http://hz.cdnleiting.top/gtwybtuocl.html

Py:   def greet(self): return self.name
来源：http://hz.yangfankeji.com/gtyyetcgel.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.sxryk.cn/gtzrgmxzuw.html

JS:   greet() { return this.name; }
来源：http://hz.tianlin.xyz/gtvyfpkkwg.html

TS:   greet(): string { return this.name; }
来源：http://hz.svipenyu.cn/gtbxhhojuf.html

Java: String greet() { return name; }
来源：http://hz.mhx1999.top/gtbmxmalrs.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.pengpengdd.cyou/gtijupencj.html

Ruby: def greet; @name; end
来源：http://hz.sysykeji.top/gtmjeshgvm.html

C#:   public string Greet() => Name;
来源：http://hz.shanyushiyangkeji.top/gthiyfqlok.html

[G05] 继承
来源：http://hz.meibo888.top/gtrlnkrhve.html

Py:   class Admin(User): pass
来源：http://hz.smart0.xyz/gtdtttwnnd.html

PHP:  class Admin extends User {}
来源：http://hz.guowangkeji.top/gtmputnijh.html

JS:   class Admin extends User {}
来源：http://hz.jinyuanbaomall.cn/gtsgfwmecn.html

TS:   class Admin extends User {}
来源：http://hz.aibaodan.cn/gtzwozdmyu.html

Java: class Admin extends User {}
来源：http://hz.tian-w.cn/gtqobkgtvf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.gaohongyu789.top/gtwvbivado.html

Ruby: class Admin < User; end
来源：http://hz.nanxinkj.top/gtnydisxcr.html

C#:   class Admin : User {}
来源：http://hz.ydzc1.top/gtfizqermz.html

[G06] 重写方法
来源：http://hz.zhaomingkeji.xyz/gtyewozgvx.html

Py:   def greet(self): return "admin"
来源：http://hz.tianlin.xyz/gtoxyfjauy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yj20258.top/gtcagycqqq.html

JS:   greet() { return "admin"; }
来源：http://hz.snrcjt.cn/gtlztbtjzv.html

TS:   greet(): string { return "admin"; }
来源：http://hz.cdnleiting.top/gtbrnwyhjx.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.meibo888.top/gtpolifbra.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.haohaochexian.top/gtalswfdig.html

Ruby: def greet; "admin"; end
来源：http://hz.ehwqpu.com/gtrbxwxizi.html

C#:   public override string Greet() => "admin";
来源：http://hz.bjfxy.top/gttcfhoqsd.html

[G07] 调用父类方法
来源：http://hz.shangyingyoupin.top/gtcmsfkezt.html

Py:   super().greet()
来源：http://hz.0kj1m.cn/gtmwjqbpln.html

PHP:  parent::greet();
来源：http://hz.sufxvd.cn/gtwrxshsne.html

JS:   super.greet();
来源：http://hz.daria6918.cn/gtcffagdwv.html

TS:   super.greet();
来源：http://hz.yongpay.top/gtatdhqctv.html

Java: super.greet();
来源：http://hz.jqgufenzy.top/gtxpkranfo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yueranfly.top/gtmblpqevb.html

Ruby: super
来源：http://hz.snrcjt.cn/gtunofdmmd.html

C#:   base.Greet();
来源：http://hz.hysaishi.cn/gtcrqyvwwy.html

[G08] 静态方法与属性
来源：http://hz.sysykeji.top/gtqzcrtdmn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.sweek.top/gteybjdmdc.html

PHP:  public static function f() {}
来源：http://hz.iojbl.cn/gtypxsqosy.html

JS:   static f() {}
来源：http://hz.cheryme.top/gthjtghumh.html

TS:   static f(): void {}
来源：http://hz.ehwqpu.com/gtcjlruigw.html

Java: static void f() {}
来源：http://hz.zhoulong.xyz/gtcykoojjz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.c1oappe.top/gtmryljmza.html

Ruby: def self.f; end
来源：http://hz.hnxiangtu.top/gtncxtblbq.html

C#:   public static void F() {}
来源：http://hz.zhixingplan.top/gtuqjgysmj.html

[G09] 接口 / 抽象类
来源：http://hz.jqgfzy.top/gtzmzxiyyy.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.gogol.net.cn/gtczadnqlf.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zhongyouzk.top/gtzhxyhngc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.nanxuanxn.top/gtktkdllgn.html

TS:   interface Shape { area(): number; }
来源：http://hz.ybcxt.top/gtcwurchpb.html

Java: interface Shape { double area(); }
来源：http://hz.chenjidiqi.icu/gtkzuvbhtg.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.0kj1m.cn/gtpzqdnkzn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.tianlin.xyz/gthtkzigov.html

C#:   interface IShape { double Area(); }
来源：http://hz.sysykeji.top/gtmygjlvvd.html

[G10] 访问控制
来源：http://hz.chenlongwang.top/gtgnbqqtpl.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.pycfn.com/gtnjtamhyk.html

PHP:  public / protected / private
来源：http://hz.bjfxy.top/gtjukewawe.html

JS:   #private 字段；其余公开
来源：http://hz.zdqjudy.top/gtopyzphsx.html

TS:   public / protected / private
来源：http://hz.zdqjudy.top/gtukoexprl.html

Java: public / protected / private / 默认包级
来源：http://hz.sufxvd.cn/gtdkbnoqwb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhongyouzk.top/gtdbfafndb.html

Ruby: public / protected / private
来源：http://hz.sufxvd.cn/gtsrmpzfab.html

C#:   public / protected / private / internal
来源：http://hz.sweek.top/gtfbyebgos.html

[G11] getter / setter
来源：http://hz.gogol.net.cn/gtoeatdsab.html

Py:   @property 与 @x.setter
来源：http://hz.fzhhl.top/gtpnsbgadh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jinyuanbaomall.cn/gtpxyzcoic.html

JS:   get name() { return this._name; }
来源：http://hz.jiagoushi.top/gtskbvvetn.html

TS:   get name(): string { return this._name; }
来源：http://hz.yueranfly.top/gtfafwfwze.html

Java: public String getName() { return name; }
来源：http://hz.cashguo.top/gtdlvqruld.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.ivvv.top/gtlmwjrcnc.html

Ruby: attr_accessor :name
来源：http://hz.zhongyouzk.top/gtlytdxjly.html

C#:   public string Name { get; set; }
来源：http://hz.feifeiyinyue.top/gthgnybldd.html

[G12] 对象转字符串
来源：http://hz.ehwqpu.com/gtiyngviel.html

Py:   def __str__(self): return self.name
来源：http://hz.shzxlz.cn/gtmokdrvqv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zhijiandao.cn/gtszpjropd.html

JS:   toString() { return this.name; }
来源：http://hz.bjfxy.top/gtqvsndwar.html

TS:   toString(): string { return this.name; }
来源：http://hz.andypj.xyz/gtebdogefm.html

Java: @Override public String toString() { return name; }
来源：http://hz.jqgfzy.top/gtdzjymcvw.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.hnxiangtu.top/gtrqhuqwye.html

Ruby: def to_s; @name; end
来源：http://hz.ydjk.org.cn/gteqorigia.html

C#:   public override string ToString() => Name;
来源：http://hz.ivvv.top/gtmaasfnbq.html

[G13] 判断对象类型
来源：http://hz.tianlin.xyz/gtjpjkxbxf.html

Py:   isinstance(u, User)
来源：http://hz.jlsjyb.cn/gtkslgtnmy.html

PHP:  $u instanceof User
来源：http://hz.aizwys.cn/gtbbrymbsh.html

JS:   u instanceof User
来源：http://hz.hnxiangtu.top/gtuhgmshhy.html

TS:   u instanceof User
来源：http://hz.ydzc1.top/gtlplamwdm.html

Java: u instanceof User
来源：http://hz.jqgufenzy.top/gtxomqjjow.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.redwolf501.top/gtcalgksbd.html

Ruby: u.is_a?(User)
来源：http://hz.sxryk.cn/gtgvkykaaj.html

C#:   u is User
来源：http://hz.shangyingyoupin.top/gttfivufob.html

[G14] 数据类 / record
来源：http://hz.yvedp.cn/gtoixoprid.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.guannengcc.top/gtoszufdup.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.pycfn.com/gtaxkpirsy.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.hammf.cn/gtjcfauwoi.html

TS:   type User = { name: string; age: number };
来源：http://hz.0kj1m.cn/gtdsfrdumw.html

Java: record User(String name, int age) {}
来源：http://hz.jlsjyb.cn/gtzhkqqvgp.html

Go:   type User struct { Name string; Age int }
来源：http://hz.chenlongwang.top/gtwmaqbebl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.pycfn.com/gtevxzgqhc.html

C#:   record User(string Name, int Age);
来源：http://hz.fzhhl.top/gthshkvrep.html

[G15] 枚举
来源：http://hz.zhiwuduotai.top/gtajfchtqi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.316326.xyz/gthgotajka.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.xylfe.cn/gtmyqmbwgf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.feifeiyinyue.top/gtmdmmmoco.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jinqigufen.top/gtubnbepxf.html

Java: enum Color { RED, GREEN }
来源：http://hz.yongpay.top/gttyvbuhjs.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.cheryme.top/gtffghkupt.html

Ruby: Color = %i[red green].freeze
来源：http://hz.mhx1999.top/gtrdhdcmfl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.svipenyu.cn/gtgpmvhsrl.html

[G16] 对象转数组 / 字典
来源：http://hz.cheryme.top/gtiolrjxjg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.ywan-chungtsiang.top/gthcvxuzog.html

PHP:  get_object_vars($obj);
来源：http://hz.shzxlz.cn/gtzlroqfhj.html

JS:   Object.entries(obj)
来源：http://hz.mhx1999.top/gtcxfsijnu.html

TS:   Object.entries(obj)
来源：http://hz.sxryk.cn/gtjpqtlzlc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.sufxvd.cn/gttmunzrkj.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.ydjk.org.cn/gtdomforou.html

Ruby: obj.instance_variables
来源：http://hz.yongpay.top/gtukcviwko.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.havefunace.top/gtcyywcrdr.html

================================================================================
来源：http://hz.aibaodan.cn/gtzlknocyu.html

H. 异常与错误处理
来源：http://hz.fengsongda.top/gtlexcqwey.html

================================================================================
来源：http://hz.yonumen.top/gtmbnfzhwn.html

[H01] try / catch 基础
来源：http://hz.ivvv.top/gtiknygpcm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.pycfn.com/gtlysjidyo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.sweek.top/gtulhwjxoh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.hysaishi.cn/gtwuoycgmn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.gaohongyu789.top/gtdapjqzve.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.hfpthk.cn/gtmatgkhub.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.quarkkingdee.top/gtpcujpsmj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.cdnleiting.top/gthivyknsp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.sweek.top/gtqhkkzsax.html

[H02] finally / ensure 收尾
来源：http://hz.ivvv.top/gtboditdrp.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yvedp.cn/gtjbvdtgno.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xinyue.icu/gtwygpbweg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.svipenyu.cn/gtdcgclnrw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhoulong.xyz/gtqpzpteop.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangtech.top/gtflihkimy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zhongyouzk.top/gtxjsubvbc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.gaohongyu789.top/gtufydgore.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.nanxuanxn.top/gtngokrusc.html

[H03] 主动抛出异常
来源：http://hz.hammf.cn/gtcmuzfpow.html

Py:   raise ValueError("错误信息")
来源：http://hz.ybcxt.top/gteyvgwfpw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.feifeiyinyue.top/gtshrfxvxa.html

JS:   throw new Error("错误信息");
来源：http://hz.jinghuilouyu.cn/gtdmtyvzov.html

TS:   throw new Error("错误信息");
来源：http://hz.9152youxi.cn/gtuwecaawf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.smart0.xyz/gtrtcgnqqw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.shangyingyoupin.top/gtrwpzmxjl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.gotoacloud.top/gtucdfldlw.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zycfv.cn/gtyvhkmudr.html

[H04] 自定义异常类型
来源：http://hz.zhaomingkeji.xyz/gtqjntossh.html

Py:   class MyError(Exception): pass
来源：http://hz.pycfn.com/gtrghlijdq.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.chenjidiqi.icu/gtdhihgbdw.html

JS:   class MyError extends Error {}
来源：http://hz.52xcode.cn/gtzzsdrsph.html

TS:   class MyError extends Error {}
来源：http://hz.vqdsnc.cn/gtafijhllu.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jqgfzy.top/gtrxokdqcm.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.xuanzx.com/gtwyeegxqx.html

Ruby: class MyError < StandardError; end
来源：http://hz.yj202588.top/gtqbuqsayo.html

C#:   class MyException : Exception {}
来源：http://hz.yanxiufei.cn/gtscpmvrok.html

[H05] 捕获特定类型
来源：http://hz.haohaochexian.top/gtpandsqia.html

Py:   except ValueError as e:
来源：http://hz.yueranfly.top/gthazearap.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.tianlin.xyz/gtzhxwribc.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.nwbrower.top/gtchbziidr.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.hywenlv.cn/gtowpcewzw.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jinqigufen.top/gtjxxtizps.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jqgfzy.top/gtgrwajrwl.html

Ruby: rescue ArgumentError => e
来源：http://hz.nanxinkj.top/gtdqcawanz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.chenzaomai.com/gtmwkncmfy.html

[H06] 可选值 / 空值安全访问
来源：http://hz.redwolf501.top/gtalxwvcsd.html

Py:   value = d.get("k") or default
来源：http://hz.yj20258888.top/gtlpqslmym.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.fengsongda.top/gtaellbxmf.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.tianlin.xyz/gtxywafnyo.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.sweek.top/gtaaianmyj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.pengpengdd.cyou/gttjaegsza.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yanxiufei.cn/gtebsdkdub.html

Ruby: d&.dig(:a, :b)
来源：http://hz.daxiang520.top/gtypvafskv.html

C#:   obj?.A?.B ?? default
来源：http://hz.mhx1999.top/gtnmyprhnw.html

[H07] 断言
来源：http://hz.aizwys.cn/gtwhjzqcrf.html

Py:   assert x > 0, "必须为正"
来源：http://hz.gogol.net.cn/gtrydfdacb.html

PHP:  assert($x > 0);
来源：http://hz.shzxlz.cn/gtoyanzzzo.html

JS:   console.assert(x > 0);
来源：http://hz.0kj1m.cn/gtnjkwyxui.html

TS:   console.assert(x > 0);
来源：http://hz.snrcjt.cn/gtwvohggld.html

Java: assert x > 0 : "必须为正";
来源：http://hz.shzxlz.cn/gtsktjkhie.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.cdnleiting.top/gtlpgfguhg.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.gogol.net.cn/gtgdwiiiik.html

C#:   Debug.Assert(x > 0);
来源：http://hz.xinyue.icu/gtfomazxcp.html

[H08] 获取错误信息与堆栈
来源：http://hz.quarkkingdee.top/gtldqbcvni.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.birdmap.top/gtlemhyxuo.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.daxiang520.top/gtqklvakbf.html

JS:   e.message;  e.stack
来源：http://hz.jianghu66.top/gtyjrslnza.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hongshengwenyu.top/gtioullkjg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhaomingkeji.xyz/gtdsslcivg.html

Go:   err.Error()
来源：http://hz.yuanzhike.top/gtmpevgzxc.html

Ruby: e.message;  e.backtrace
来源：http://hz.pycfn.com/gtzbbkalxj.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yueranfly.top/gtzgscrmln.html

[H09] 带错误码的异常
来源：http://hz.nanxinkj.top/gtaowwdhls.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hnxiangtu.top/gtmcdqimqc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.gotoacloud.top/gtcsawoyqj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jianghu66.top/gtxnyylwrb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.cashguo.top/gtquwihglg.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jiagoushi.top/gthmqagipw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ydjk.org.cn/gtjlrsqaas.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zdqjudy.top/gtxyuorldt.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yangfankeji.com/gtxbyhhbhs.html

[H10] 资源自动释放
来源：http://hz.chenjidiqi.icu/gtuxomyglg.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yuanzhike.top/gtladwssdu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.zhaomingkeji.xyz/gtlmfxbrsg.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jiagoushi.top/gtsiauwsdm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gogol.net.cn/gtdlpqrqpy.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.xziqi.cn/gtwnztqzen.html

Go:   defer f.Close()
来源：http://hz.gaohongyu789.top/gtwrascfdq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.gaohongyu789.top/gtnnjiaior.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zdqjudy.top/gtshvefvbv.html

================================================================================
来源：http://hz.yuxming.cn/gtmqysyhpg.html

I. 正则表达式
来源：http://hz.9152youxi.cn/gttiezwuha.html

================================================================================
来源：http://hz.mhx1999.top/gtyyhjicpo.html

[I01] 判断是否匹配
来源：http://hz.guowangkeji.top/gtnpbhpmhd.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.nwbrower.top/gtzahijpae.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.quarkkingdee.top/gtebgithnh.html

JS:   /\d+/.test(s)
来源：http://hz.cashguo.top/gtodxmzcac.html

TS:   /\d+/.test(s)
来源：http://hz.chenlongwang.top/gtzmldikoy.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hammf.cn/gtrecwqzex.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.quarkkingdee.top/gtktkpljsu.html

Ruby: s.match?(/\d+/)
来源：http://hz.xziqi.cn/gtmsvkczaj.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zycfv.cn/gtserxzltc.html

[I02] 提取所有匹配
来源：http://hz.fengsongda.top/gtgjswauym.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jqgufenzy.top/gtaecimosv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.mhx1999.top/gtmzrrersj.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.aibaodan.cn/gtogqnjmrm.html

TS:   s.match(/\d+/g)
来源：http://hz.jinqigfzy.top/gtyzkyluti.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jyoumei.cn/gtdpbmkkit.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.vqdsnc.cn/gtyowkkhua.html

Ruby: s.scan(/\d+/)
来源：http://hz.shanyushiyangkeji.top/gtococxsji.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.tian-w.cn/gtzrdrpqxy.html

[I03] 提取捕获分组
来源：http://hz.gogol.net.cn/gtkaesmvnm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jianghu66.top/gtkygvtwtb.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.shuidangran.top/gttpauifpi.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zhengqikj.top/gtivfqrghy.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jqgufenzy.top/gtehsansxu.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.fengsongda.top/gtonvqmjkm.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yvedp.cn/gtdumjjmjn.html


<!-- 参考信息 -->