代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.aibaodan.cn/gtotixoqcb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.svipenyu.cn/gteaptdxkv.html

JS:   fs.readdirSync("dir")
来源：http://hz.zhoulong.xyz/gtmpuxnqmb.html

TS:   fs.readdirSync("dir")
来源：http://hz.xylfe.cn/gtflbdythg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yvedp.cn/gtppiqyctn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.smart0.xyz/gtigffblpr.html

Ruby: Dir.children("dir")
来源：http://hz.dashuyun.cn/gtmwbrfacy.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yanxiufei.cn/gtjcbanycu.html

[F09] 获取文件大小
来源：http://hz.shanyushiyangkeji.top/gtkqyhbggm.html

Py:   os.path.getsize("a.txt")
来源：http://hz.svipenyu.cn/gtvalptthv.html

PHP:  filesize("a.txt");
来源：http://hz.ybcxt.top/gtezyahpxu.html

JS:   fs.statSync("a.txt").size
来源：http://hz.hongshengwenyu.top/gtidezybjh.html

TS:   fs.statSync("a.txt").size
来源：http://hz.ywan-chungtsiang.top/gtwdimrivc.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.haohaochexian.top/gtwedavhro.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.cashguo.top/gtnqiutshi.html

Ruby: File.size("a.txt")
来源：http://hz.yj202588.top/gtgxtfpyce.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.snrcjt.cn/gtpkxriebp.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.xylfe.cn/gtyiqdzzsd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.9152youxi.cn/gtetfmylrw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.ehwqpu.com/gtcsbognpu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yonumen.top/gtflrrcyqr.html

TS:   path.extname("a.txt")
来源：http://hz.ivvv.top/gtwlxugsvj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.hfpthk.cn/gtzvljveek.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.cheryme.top/gtgnxtslsa.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jinyuanbaomall.cn/gtydfjykaa.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yueranfly.top/gthntycslk.html

[F11] 复制与移动文件
来源：http://hz.yj20258.top/gtodopvluh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.wangshuangyany.cn/gtwvjhgzsg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jinghuilouyu.cn/gtcyrqykto.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ydzc1.top/gtkatsurbi.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.0kj1m.cn/gtsapaqioa.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.chenzaomai.com/gtuffhvbax.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.zhongyouzk.top/gtdtmaayss.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.chenjidiqi.icu/gtnctfzgzb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yonumen.top/gtdpnisvgk.html

[F12] CSV 读写
来源：http://hz.haohaochexian.top/gtihjwxmeo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yonumen.top/gtumephemn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yueranfly.top/gtxdaqaqmu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yuanzhike.top/gtjcibtizl.html

TS:   // 同上
来源：http://hz.mhx1999.top/gtqvjfbvzx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zycfv.cn/gtzxzbyfjk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yongpay.top/gtkgaotwaw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jlsjyb.cn/gtpvjcherv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yuxming.cn/gtxfopeiir.html

================================================================================
来源：http://hz.xylfe.cn/gtjokifawx.html

G. 面向对象
来源：http://hz.yj20258888.top/gtuopldyfi.html

================================================================================
来源：http://hz.ydzc1.top/gtbqzoygdd.html

[G01] 定义类
来源：http://hz.yj20258888.top/gtwgcqwfiq.html

Py:   class User: pass
来源：http://hz.xylfe.cn/gtpolswvwy.html

PHP:  class User {}
来源：http://hz.aibaodan.cn/gtxghnqeis.html

JS:   class User {}
来源：http://hz.hongshengwenyu.top/gtxxxogxjb.html

TS:   class User { name: string = ""; }
来源：http://hz.gogol.net.cn/gthcrssbyr.html

Java: class User {}
来源：http://hz.yj202588.top/gtjscfmvau.html

Go:   type User struct { Name string }
来源：http://hz.jinyuanbaomall.cn/gtlbmgiwub.html

Ruby: class User; end
来源：http://hz.zhijiandao.cn/gtoayoxauc.html

C#:   class User {}
来源：http://hz.svipenyu.cn/gterxrfwio.html

[G02] 构造函数
来源：http://hz.zhengqikj.top/gtlluqcmhu.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.nanxuanxn.top/gtxiqmdzpy.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.meibo888.top/gtrmmcsnrn.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.hysaishi.cn/gttzrlnvjm.html

TS:   constructor(public name: string) {}
来源：http://hz.sweek.top/gtffhshpvx.html

Java: User(String name) { this.name = name; }
来源：http://hz.guannengcc.top/gtuymjpasz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yonumen.top/gtvpqqanqu.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.cashguo.top/gtxnqompgt.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jianghu66.top/gtregqegzn.html

[G03] 实例属性
来源：http://hz.meibo888.top/gtqyhkaqcf.html

Py:   self.name = "x"
来源：http://hz.wangshuangyany.cn/gtkgdjjhnx.html

PHP:  public string $name = "x";
来源：http://hz.daxiang520.top/gtfabadktd.html

JS:   this.name = "x";
来源：http://hz.aizwys.cn/gtzfbjbwta.html

TS:   name: string = "x";
来源：http://hz.meibo888.top/gtwgitvhae.html

Java: private String name;
来源：http://hz.shuidangran.top/gtfwouieas.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.haohaochexian.top/gtkozdboem.html

Ruby: @name = "x"
来源：http://hz.9152youxi.cn/gtsmnafppf.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.havefunace.top/gtqmukyjid.html

[G04] 定义方法
来源：http://hz.chenjidiqi.icu/gtqswuvpmn.html

Py:   def greet(self): return self.name
来源：http://hz.svipenyu.cn/gtmuekerxz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.52xcode.cn/gtfekdnmwz.html

JS:   greet() { return this.name; }
来源：http://hz.smart0.xyz/gtscyfkfvf.html

TS:   greet(): string { return this.name; }
来源：http://hz.xziqi.cn/gtvqnhemul.html

Java: String greet() { return name; }
来源：http://hz.wangdashe.top/gtvnreawcd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ydjk.org.cn/gtvtstpmsm.html

Ruby: def greet; @name; end
来源：http://hz.gzhubu.top/gtfxdhgjrh.html

C#:   public string Greet() => Name;
来源：http://hz.xinyue.icu/gtymsaxxnu.html

[G05] 继承
来源：http://hz.cdnleiting.top/gtlgjdovof.html

Py:   class Admin(User): pass
来源：http://hz.jinyuanbaomall.cn/gtddymqsmk.html

PHP:  class Admin extends User {}
来源：http://hz.tianlin.xyz/gtzyajapqk.html

JS:   class Admin extends User {}
来源：http://hz.daria6918.cn/gtpuqqlysd.html

TS:   class Admin extends User {}
来源：http://hz.xuanzx.com/gtdceguncy.html

Java: class Admin extends User {}
来源：http://hz.pengpengdd.cyou/gtcrikyqee.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.iojbl.cn/gtgpbdesvc.html

Ruby: class Admin < User; end
来源：http://hz.wangshuangyany.cn/gtgqgyirpu.html

C#:   class Admin : User {}
来源：http://hz.cheryme.top/gtgobhbwct.html

[G06] 重写方法
来源：http://hz.andypj.xyz/gtctjbxomt.html

Py:   def greet(self): return "admin"
来源：http://hz.yongpay.top/gtvgfckwfj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yanxiufei.cn/gtpbxagytd.html

JS:   greet() { return "admin"; }
来源：http://hz.ppjwa.cn/gtekqcutkd.html

TS:   greet(): string { return "admin"; }
来源：http://hz.52xcode.cn/gtsomqkvzq.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.guowangkeji.top/gtsznunwnl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yj202588.top/gtgzwdvash.html

Ruby: def greet; "admin"; end
来源：http://hz.hnqzz.top/gthpheuevq.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhoulong.xyz/gtnmzcbmph.html

[G07] 调用父类方法
来源：http://hz.meibo888.top/gtxkppgqsn.html

Py:   super().greet()
来源：http://hz.sufxvd.cn/gtxrjesdkt.html

PHP:  parent::greet();
来源：http://hz.jinqigufen.top/gtytxjrjap.html

JS:   super.greet();
来源：http://hz.jlsjyb.cn/gtalfhtuut.html

TS:   super.greet();
来源：http://hz.vqdsnc.cn/gtbyegrmkz.html

Java: super.greet();
来源：http://hz.pengpengdd.cyou/gtondnnyup.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jyoumei.cn/gtpdwyqlwc.html

Ruby: super
来源：http://hz.zycfv.cn/gtpmruqucg.html

C#:   base.Greet();
来源：http://hz.xuetiantiany.cn/gtrgtwbttq.html

[G08] 静态方法与属性
来源：http://hz.316326.xyz/gtjvhwrcpj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhaomingkeji.xyz/gtdhkzsnta.html

PHP:  public static function f() {}
来源：http://hz.pengpengdd.cyou/gtdjyahddv.html

JS:   static f() {}
来源：http://hz.cdnleiting.top/gtddahsscq.html

TS:   static f(): void {}
来源：http://hz.hywenlv.cn/gtwtimphsv.html

Java: static void f() {}
来源：http://hz.yj202588.top/gtagbnlero.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jinqigufen.top/gtghyufxhq.html

Ruby: def self.f; end
来源：http://hz.yj20258888.top/gtvznrypfu.html

C#:   public static void F() {}
来源：http://hz.sysykeji.top/gtrvpvlczs.html

[G09] 接口 / 抽象类
来源：http://hz.sxryk.cn/gtcxnqhaem.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.316326.xyz/gtxnzwqlmf.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ywan-chungtsiang.top/gtqhudegvq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.xylfe.cn/gteocunstc.html

TS:   interface Shape { area(): number; }
来源：http://hz.meibo888.top/gtqgbsjstd.html

Java: interface Shape { double area(); }
来源：http://hz.jqgfzy.top/gtpsqxdeqd.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.gotoacloud.top/gtrdzozrmg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.52xcode.cn/gtclatawlw.html

C#:   interface IShape { double Area(); }
来源：http://hz.haohaochexian.top/gtttajvagt.html

[G10] 访问控制
来源：http://hz.cucudq.cn/gtnmmzvrve.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.dashuyun.cn/gttprxseia.html

PHP:  public / protected / private
来源：http://hz.c1oappe.top/gtesfdkmwa.html

JS:   #private 字段；其余公开
来源：http://hz.gotoacloud.top/gtlsalgrax.html

TS:   public / protected / private
来源：http://hz.wangdashe.top/gtghgmyyvh.html

Java: public / protected / private / 默认包级
来源：http://hz.zhoulong.xyz/gtegwbnolu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yuxming.cn/gtoyyryzgh.html

Ruby: public / protected / private
来源：http://hz.yuanzhike.top/gtcgjplwog.html

C#:   public / protected / private / internal
来源：http://hz.yj202588.top/gtsbnwtucn.html

[G11] getter / setter
来源：http://hz.hammf.cn/gtepfslgjv.html

Py:   @property 与 @x.setter
来源：http://hz.xingfuxueyuan.xyz/gtmxwsxolp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.xinyue.icu/gtbtrtccqm.html

JS:   get name() { return this._name; }
来源：http://hz.shzxlz.cn/gthwatpvao.html

TS:   get name(): string { return this._name; }
来源：http://hz.jinqigfzy.top/gtpwltwjet.html

Java: public String getName() { return name; }
来源：http://hz.shuidangran.top/gtcgqufgmo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.cucudq.cn/gtytdalzbi.html

Ruby: attr_accessor :name
来源：http://hz.xuanzx.com/gttfrqllfy.html

C#:   public string Name { get; set; }
来源：http://hz.sweek.top/gtarhmzjuv.html

[G12] 对象转字符串
来源：http://hz.ehwqpu.com/gtyirvvxbn.html

Py:   def __str__(self): return self.name
来源：http://hz.snrcjt.cn/gtgirgcrhc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yuanzhike.top/gtkroupfwl.html

JS:   toString() { return this.name; }
来源：http://hz.yangfankeji.com/gtuayrixqb.html

TS:   toString(): string { return this.name; }
来源：http://hz.daxiang520.top/gtqkurcyjw.html

Java: @Override public String toString() { return name; }
来源：http://hz.cdnleiting.top/gtaeoujisa.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.nanxuanxn.top/gtjpwevsuh.html

Ruby: def to_s; @name; end
来源：http://hz.yj20258.top/gtadytzhmz.html

C#:   public override string ToString() => Name;
来源：http://hz.jinghuilouyu.cn/gtkqygwukp.html

[G13] 判断对象类型
来源：http://hz.hongshengwenyu.top/gtovzvvjyb.html

Py:   isinstance(u, User)
来源：http://hz.snrcjt.cn/gtsnrreonz.html

PHP:  $u instanceof User
来源：http://hz.redwolf501.top/gtankcylgk.html

JS:   u instanceof User
来源：http://hz.wangshuangyany.cn/gtcaqsrjnd.html

TS:   u instanceof User
来源：http://hz.shanyushiyangtech.top/gtwgarteqo.html

Java: u instanceof User
来源：http://hz.ybcxt.top/gtoqqwtwyy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ivvv.top/gtrekhnuqt.html

Ruby: u.is_a?(User)
来源：http://hz.meibo888.top/gtgwnicuyg.html

C#:   u is User
来源：http://hz.zhengqikj.top/gtnjhfursu.html

[G14] 数据类 / record
来源：http://hz.gzhubu.top/gtkesuagam.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.cucudq.cn/gtbpkddgzk.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.cqqwz.cn/gtpkuwudsv.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.cheryme.top/gtwmksknbg.html

TS:   type User = { name: string; age: number };
来源：http://hz.andypj.xyz/gtexjzgsim.html

Java: record User(String name, int age) {}
来源：http://hz.cucudq.cn/gtjizpbmgs.html

Go:   type User struct { Name string; Age int }
来源：http://hz.hammf.cn/gtrckvoxyj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.tanke756.top/gtsfhkgdng.html

C#:   record User(string Name, int Age);
来源：http://hz.dianchejie.cn/gtnxayvhye.html

[G15] 枚举
来源：http://hz.hysaishi.cn/gtlfhpifhb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jlsjyb.cn/gtnhvukcnv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhixingplan.top/gtdwhzjafv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.ybcxt.top/gtlbamsygj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.birdmap.top/gtyedyfkca.html

Java: enum Color { RED, GREEN }
来源：http://hz.gzhubu.top/gtnfrmppii.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.snrcjt.cn/gtlfbdwxrp.html

Ruby: Color = %i[red green].freeze
来源：http://hz.shzxlz.cn/gtqeaqmzof.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.9152youxi.cn/gtjtiwbfum.html

[G16] 对象转数组 / 字典
来源：http://hz.gogol.net.cn/gtevybgdbf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.haohaochexian.top/gtbktjzbrm.html

PHP:  get_object_vars($obj);
来源：http://hz.haohaochexian.top/gtctjldcav.html

JS:   Object.entries(obj)
来源：http://hz.gotoacloud.top/gtokqclrdw.html

TS:   Object.entries(obj)
来源：http://hz.daria6918.cn/gthpxceflt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.c1oappe.top/gtiybwgzgv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.quarkkingdee.top/gtjhktjkqw.html

Ruby: obj.instance_variables
来源：http://hz.bjfxy.top/gtrwzivklv.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.hfpthk.cn/gtnwvzndiv.html

================================================================================
来源：http://hz.pycfn.com/gtdtoqwkhp.html

H. 异常与错误处理
来源：http://hz.shanyushiyangtech.top/gtjdbcpipl.html

================================================================================
来源：http://hz.hammf.cn/gtuuwibzni.html

[H01] try / catch 基础
来源：http://hz.tianlin.xyz/gtxpgcqwnr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.hywenlv.cn/gtgkikcmqi.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ydzc1.top/gtrbcguizz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.nwbrower.top/gtudqezwuv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zycfv.cn/gthgooggct.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.hammf.cn/gttbrcfqrg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.daria6918.cn/gthmxydbpw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.tanke756.top/gtmmnkfedh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jinyuanbaomall.cn/gtholvtjqg.html

[H02] finally / ensure 收尾
来源：http://hz.shzxlz.cn/gtwqjdoica.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.bjfxy.top/gtwcryzrxz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhengqikj.top/gtgyhaqotv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jyoumei.cn/gtdbalxbrm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.hnxiangtu.top/gtzswizmjp.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.gaohongyu789.top/gthuunavgz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hammf.cn/gtafxrwszd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.gogol.net.cn/gtihskvlhy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.xuetiantiany.cn/gtevmsdlil.html

[H03] 主动抛出异常
来源：http://hz.pengpengdd.cyou/gthnkrqtkz.html

Py:   raise ValueError("错误信息")
来源：http://hz.andypj.xyz/gtfhyjatco.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.aibaodan.cn/gtqpwxdbfq.html

JS:   throw new Error("错误信息");
来源：http://hz.jinqigfzy.top/gtgnfenygh.html

TS:   throw new Error("错误信息");
来源：http://hz.jqgfzy.top/gtjcrbkygo.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.haohaochexian.top/gtuexgvrnu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.cheryme.top/gtjproeswe.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.xingfuxueyuan.xyz/gtzjmsqlbn.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.daria6918.cn/gtkazwdxtm.html

[H04] 自定义异常类型
来源：http://hz.cqqwz.cn/gtzmwanobr.html

Py:   class MyError(Exception): pass
来源：http://hz.haohaochexian.top/gtwntoogfm.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.pengpengdd.cyou/gtykipodup.html

JS:   class MyError extends Error {}
来源：http://hz.redwolf501.top/gtyhqmuqog.html

TS:   class MyError extends Error {}
来源：http://hz.nanxinkj.top/gtslnkjojq.html

Java: class MyException extends RuntimeException {}
来源：http://hz.mhx1999.top/gtcxtmygnw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.tianlin.xyz/gtiziacprc.html

Ruby: class MyError < StandardError; end
来源：http://hz.wangshuangyany.cn/gtdztqnoak.html

C#:   class MyException : Exception {}
来源：http://hz.cucudq.cn/gtnsltlvce.html

[H05] 捕获特定类型
来源：http://hz.jinqigfzy.top/gtztlynsec.html

Py:   except ValueError as e:
来源：http://hz.pycfn.com/gtlszafjjv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jinqigfzy.top/gtsqxwieib.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.gotoacloud.top/gtkobhsuvc.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.316326.xyz/gtvccjfaqc.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.dianchejie.cn/gtyjeqaxzn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.wangshuangyany.cn/gtesxawcbe.html

Ruby: rescue ArgumentError => e
来源：http://hz.chenlongwang.top/gttgypzjsk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.xinyue.icu/gtzungfpmb.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zycfv.cn/gtkhyxjpso.html

Py:   value = d.get("k") or default
来源：http://hz.gotoacloud.top/gtuxmtzbhg.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.sxryk.cn/gtyydiewue.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yuxming.cn/gtvxrcbpja.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.gogol.net.cn/gtcjezcfab.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.haohaochexian.top/gtxktcitwl.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.wangshuangyany.cn/gtqoamhgkb.html

Ruby: d&.dig(:a, :b)
来源：http://hz.smart0.xyz/gtsmgkteuh.html

C#:   obj?.A?.B ?? default
来源：http://hz.fengsongda.top/gtegmeffzk.html

[H07] 断言
来源：http://hz.xuanzx.com/gtbupfxtqe.html

Py:   assert x > 0, "必须为正"
来源：http://hz.fzhhl.top/gtcwznddut.html

PHP:  assert($x > 0);
来源：http://hz.gzhubu.top/gtmrrqeiys.html

JS:   console.assert(x > 0);
来源：http://hz.jinghuilouyu.cn/gtxwrvttea.html

TS:   console.assert(x > 0);
来源：http://hz.ydjk.org.cn/gtlecuwleo.html

Java: assert x > 0 : "必须为正";
来源：http://hz.c1oappe.top/gtqkrwvoek.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.chenjidiqi.icu/gtjihfriit.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.gzhubu.top/gtmipwjnbz.html

C#:   Debug.Assert(x > 0);
来源：http://hz.cucudq.cn/gthjobdmus.html

[H08] 获取错误信息与堆栈
来源：http://hz.gzhubu.top/gtqlgfczdp.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jinghuilouyu.cn/gtovsyhvgw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.wangshuangyany.cn/gtmnrodfxz.html

JS:   e.message;  e.stack
来源：http://hz.sxryk.cn/gtyrqowipq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.haohaochexian.top/gtjshfogdy.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.cdnleiting.top/gtputhrlhv.html

Go:   err.Error()
来源：http://hz.mhx1999.top/gththtlyfd.html

Ruby: e.message;  e.backtrace
来源：http://hz.havefunace.top/gthqdxfoax.html

C#:   e.Message;  e.StackTrace
来源：http://hz.feifeiyinyue.top/gtyghueeyz.html

[H09] 带错误码的异常
来源：http://hz.pycfn.com/gtyztatcke.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.daria6918.cn/gtuemqtiwx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.shuidangran.top/gtfnfmebik.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.daxiang520.top/gtfnltstqn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.xingfuxueyuan.xyz/gtazufnqeg.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.52xcode.cn/gtsuulbrzs.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yuanzhike.top/gtuxjipjin.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.tianlin.xyz/gtskmtjfqe.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.shuidangran.top/gtwxqsbzfb.html

[H10] 资源自动释放
来源：http://hz.0kj1m.cn/gtssrzhhql.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.ydzc1.top/gtlqfeiptq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.zhijiandao.cn/gtawfzmdtl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.meibo888.top/gtkksdwjjl.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ppjwa.cn/gtsfgdaser.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.sxryk.cn/gtxmreatxe.html

Go:   defer f.Close()
来源：http://hz.hnqzz.top/gtohcobvbm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jinqigfzy.top/gtmikzhqqd.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.cashguo.top/gtuequwgyz.html

================================================================================
来源：http://hz.nanxuanxn.top/gtbnsyozko.html

I. 正则表达式
来源：http://hz.hnqzz.top/gtoywuugvc.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtidtxaqoo.html

[I01] 判断是否匹配
来源：http://hz.zhijiandao.cn/gtfbhpjmgr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.fzhhl.top/gtmvccxujs.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yvedp.cn/gtoseocbis.html

JS:   /\d+/.test(s)
来源：http://hz.0kj1m.cn/gtamxmpszk.html

TS:   /\d+/.test(s)
来源：http://hz.haohaochexian.top/gtlzgnnvfc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.wangshuangyany.cn/gtqwpbyhoy.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.nwbrower.top/gtttwrvyjl.html

Ruby: s.match?(/\d+/)
来源：http://hz.xuanzx.com/gthacpjxuv.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.pycfn.com/gtudoatttl.html

[I02] 提取所有匹配
来源：http://hz.chenlongwang.top/gtlqavepqx.html

Py:   re.findall(r"\d+", s)
来源：http://hz.zhoulong.xyz/gtvptuvorq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jyoumei.cn/gtsbksismv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.xinyue.icu/gtipqgonin.html


<!-- 参考信息 -->