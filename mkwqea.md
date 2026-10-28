代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.smart0.xyz/gttwfatoko.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.kuanghao11.cn/gtmbermvky.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.guowangkeji.top/gtkigtdhkq.html

[F08] 遍历目录
来源：http://hz.tianlin.xyz/gttyzbezte.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.jianghu66.top/gtlxaicevs.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yvedp.cn/gtmpazrmsr.html

JS:   fs.readdirSync("dir")
来源：http://hz.snrcjt.cn/gtrdpuacpa.html

TS:   fs.readdirSync("dir")
来源：http://hz.xuanzx.com/gtifdiqlia.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.0kj1m.cn/gtnjahdfqv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.sufxvd.cn/gtpkxgcqxi.html

Ruby: Dir.children("dir")
来源：http://hz.tanke756.top/gtecugqokh.html

C#:   Directory.GetFiles("dir")
来源：http://hz.wangshuangyany.cn/gtssiybxjm.html

[F09] 获取文件大小
来源：http://hz.gotoacloud.top/gtarvrskcn.html

Py:   os.path.getsize("a.txt")
来源：http://hz.hysaishi.cn/gtbfccteur.html

PHP:  filesize("a.txt");
来源：http://hz.cashguo.top/gtdmtdxjrj.html

JS:   fs.statSync("a.txt").size
来源：http://hz.sufxvd.cn/gtgnctbiqc.html

TS:   fs.statSync("a.txt").size
来源：http://hz.nanxuanxn.top/gterpapycw.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.feifeiyinyue.top/gtrvhsbfdq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.redwolf501.top/gtflhhdrzq.html

Ruby: File.size("a.txt")
来源：http://hz.birdmap.top/gtpmfjufvb.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.hnxiangtu.top/gtrymhsnek.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.wangdashe.top/gtxdqlgtyt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.birdmap.top/gtukrpwejk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.tianlin.xyz/gtyvaymkuh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.sweek.top/gtkodkghxi.html

TS:   path.extname("a.txt")
来源：http://hz.nanxuanxn.top/gtioxrjble.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.iojbl.cn/gttanimafn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jyoumei.cn/gtasfrtvot.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.feifeiyinyue.top/gtznijftqp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.tian-w.cn/gtzmcxaduj.html

[F11] 复制与移动文件
来源：http://hz.xuanzx.com/gtisfttzyv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.sxryk.cn/gtmffidguo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.ybcxt.top/gtferlrbmd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.chenlongwang.top/gthblqzpeq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xylfe.cn/gttphuywyn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zhengqikj.top/gtvshutihd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.hfpthk.cn/gtfdfrpfqw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zdqjudy.top/gtnqqzthuj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.birdmap.top/gtzlhmvzmo.html

[F12] CSV 读写
来源：http://hz.zhixingplan.top/gtciqsembv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.pycfn.com/gtwemxexyu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zhongyouzk.top/gtvowsvexr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.sysykeji.top/gtxiebmmmq.html

TS:   // 同上
来源：http://hz.zhiwuduotai.top/gtjblkmrtb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.cdnleiting.top/gtauwnbnac.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.hywenlv.cn/gtbtigkvdd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.quarkkingdee.top/gtcbnuvghy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.ppjwa.cn/gtmukaubke.html

================================================================================
来源：http://hz.ybcxt.top/gtdbuswnwo.html

G. 面向对象
来源：http://hz.pycfn.com/gtpdedejha.html

================================================================================
来源：http://hz.meibo888.top/gtksksfuot.html

[G01] 定义类
来源：http://hz.daria6918.cn/gtqmkrfwei.html

Py:   class User: pass
来源：http://hz.nwbrower.top/gtourzuqvf.html

PHP:  class User {}
来源：http://hz.guowangkeji.top/gtcpkolakw.html

JS:   class User {}
来源：http://hz.bjfxy.top/gtryyzvxeq.html

TS:   class User { name: string = ""; }
来源：http://hz.birdmap.top/gtzjwuwsxk.html

Java: class User {}
来源：http://hz.guowangkeji.top/gtbbbwvgtb.html

Go:   type User struct { Name string }
来源：http://hz.daxiang520.top/gthllmkgtn.html

Ruby: class User; end
来源：http://hz.ppjwa.cn/gtxjlnprqh.html

C#:   class User {}
来源：http://hz.sufxvd.cn/gtsgibcdhs.html

[G02] 构造函数
来源：http://hz.gotoacloud.top/gtbjlxeivs.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.gaohongyu789.top/gtaygerrat.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yuxming.cn/gtangouopb.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.vqdsnc.cn/gtytmcfhzd.html

TS:   constructor(public name: string) {}
来源：http://hz.guannengcc.top/gtzmwoyxck.html

Java: User(String name) { this.name = name; }
来源：http://hz.svipenyu.cn/gtjokebatw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.iojbl.cn/gtxiolkatd.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.daxiang520.top/gtfafrtebz.html

C#:   public User(string name) { Name = name; }
来源：http://hz.bjfxy.top/gtrqmvdmkh.html

[G03] 实例属性
来源：http://hz.cucudq.cn/gtiqvjrpix.html

Py:   self.name = "x"
来源：http://hz.dashuyun.cn/gtvsfuhgvz.html

PHP:  public string $name = "x";
来源：http://hz.ppjwa.cn/gtypvfssuf.html

JS:   this.name = "x";
来源：http://hz.hysaishi.cn/gthjobxuiu.html

TS:   name: string = "x";
来源：http://hz.pengpengdd.cyou/gtgcnduehl.html

Java: private String name;
来源：http://hz.pycfn.com/gttpysyslw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yj20258888.top/gtxenzokbv.html

Ruby: @name = "x"
来源：http://hz.daria6918.cn/gtsufdlkqm.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.cqqwz.cn/gtsqjpihpr.html

[G04] 定义方法
来源：http://hz.kuanghao11.cn/gtagccryfa.html

Py:   def greet(self): return self.name
来源：http://hz.tanke756.top/gtcchalunn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.redwolf501.top/gtelwpjjwu.html

JS:   greet() { return this.name; }
来源：http://hz.bjfxy.top/gtwbsnpjai.html

TS:   greet(): string { return this.name; }
来源：http://hz.guannengcc.top/gttsslxlsz.html

Java: String greet() { return name; }
来源：http://hz.jiagoushi.top/gtjbtpjlve.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ybcxt.top/gtumxqokdr.html

Ruby: def greet; @name; end
来源：http://hz.yonumen.top/gtxjsxkgjd.html

C#:   public string Greet() => Name;
来源：http://hz.0kj1m.cn/gtquqkcmbu.html

[G05] 继承
来源：http://hz.kuanghao11.cn/gtoqywdccy.html

Py:   class Admin(User): pass
来源：http://hz.sysykeji.top/gtxfsarbty.html

PHP:  class Admin extends User {}
来源：http://hz.hongshengwenyu.top/gtacpmaqpu.html

JS:   class Admin extends User {}
来源：http://hz.yangfankeji.com/gtdxlmdgug.html

TS:   class Admin extends User {}
来源：http://hz.smart0.xyz/gtkxlwnmpu.html

Java: class Admin extends User {}
来源：http://hz.ivvv.top/gtmgbzrrpv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.cheryme.top/gtxzbwxtvr.html

Ruby: class Admin < User; end
来源：http://hz.redwolf501.top/gtizmmbehb.html

C#:   class Admin : User {}
来源：http://hz.smart0.xyz/gtyrdewudj.html

[G06] 重写方法
来源：http://hz.pengpengdd.cyou/gtynlmwvoa.html

Py:   def greet(self): return "admin"
来源：http://hz.shuidangran.top/gtjwyxrhpg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ydzc1.top/gtoqnbtjyb.html

JS:   greet() { return "admin"; }
来源：http://hz.zdqjudy.top/gtgkbuxxno.html

TS:   greet(): string { return "admin"; }
来源：http://hz.ivvv.top/gtglayvpto.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.smart0.xyz/gtkonkedtv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.shuidangran.top/gtkqwqhlhi.html

Ruby: def greet; "admin"; end
来源：http://hz.yvedp.cn/gtdkqoeylu.html

C#:   public override string Greet() => "admin";
来源：http://hz.quarkkingdee.top/gtdxdhnato.html

[G07] 调用父类方法
来源：http://hz.jinghuilouyu.cn/gtlgbghqjt.html

Py:   super().greet()
来源：http://hz.aibaodan.cn/gtlzhhysuc.html

PHP:  parent::greet();
来源：http://hz.ydjk.org.cn/gtrztglyrd.html

JS:   super.greet();
来源：http://hz.hnqzz.top/gtuwyhesdu.html

TS:   super.greet();
来源：http://hz.shangyingyoupin.top/gtgeihogsp.html

Java: super.greet();
来源：http://hz.jlsjyb.cn/gtdlcujbks.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.meibo888.top/gtfdgyehjj.html

Ruby: super
来源：http://hz.zhengqikj.top/gtthilmeam.html

C#:   base.Greet();
来源：http://hz.yanxiufei.cn/gtyiwcunlu.html

[G08] 静态方法与属性
来源：http://hz.sufxvd.cn/gtgsapphkm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.ivvv.top/gtdtszftpf.html

PHP:  public static function f() {}
来源：http://hz.shuidangran.top/gtnrkdxrca.html

JS:   static f() {}
来源：http://hz.yongpay.top/gtxzjqqawz.html

TS:   static f(): void {}
来源：http://hz.nwbrower.top/gtkiiambpy.html

Java: static void f() {}
来源：http://hz.ydzc1.top/gttpspyfkz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhiwuduotai.top/gtyluhrvhj.html

Ruby: def self.f; end
来源：http://hz.sufxvd.cn/gtloyfoets.html

C#:   public static void F() {}
来源：http://hz.zhiwuduotai.top/gtuhzmihzz.html

[G09] 接口 / 抽象类
来源：http://hz.quarkkingdee.top/gtmriwcgia.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.nanxuanxn.top/gtodkwcafo.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jlsjyb.cn/gtfakroizy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jinyuanbaomall.cn/gthdwnjpqe.html

TS:   interface Shape { area(): number; }
来源：http://hz.nwbrower.top/gtnxgrbiox.html

Java: interface Shape { double area(); }
来源：http://hz.xingfuxueyuan.xyz/gtxqugaxin.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.iojbl.cn/gtqmoecffa.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhaomingkeji.xyz/gtxprzazio.html

C#:   interface IShape { double Area(); }
来源：http://hz.zhongyouzk.top/gthtknbmrh.html

[G10] 访问控制
来源：http://hz.yj20258.top/gthxdiumpo.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.sxryk.cn/gtngmfvncu.html

PHP:  public / protected / private
来源：http://hz.fengsongda.top/gtnajsbhhp.html

JS:   #private 字段；其余公开
来源：http://hz.xziqi.cn/gtwzplajze.html

TS:   public / protected / private
来源：http://hz.pengpengdd.cyou/gthnvlubrs.html

Java: public / protected / private / 默认包级
来源：http://hz.zhengqikj.top/gtsklojicy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.xylfe.cn/gtshhkfgfe.html

Ruby: public / protected / private
来源：http://hz.jinyuanbaomall.cn/gtdwndvrcs.html

C#:   public / protected / private / internal
来源：http://hz.svipenyu.cn/gthnttrgso.html

[G11] getter / setter
来源：http://hz.xuetiantiany.cn/gtzgbnsjhr.html

Py:   @property 与 @x.setter
来源：http://hz.haohaochexian.top/gtqmvtxaed.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.cucudq.cn/gtoxkpbtdu.html

JS:   get name() { return this._name; }
来源：http://hz.cheryme.top/gtcoprgmkb.html

TS:   get name(): string { return this._name; }
来源：http://hz.shuidangran.top/gtncfbccrk.html

Java: public String getName() { return name; }
来源：http://hz.sxryk.cn/gtzjlcddpc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jinqigufen.top/gtchapbfto.html

Ruby: attr_accessor :name
来源：http://hz.chenlongwang.top/gtopkqmsfs.html

C#:   public string Name { get; set; }
来源：http://hz.svipenyu.cn/gtnkxxgbox.html

[G12] 对象转字符串
来源：http://hz.xylfe.cn/gtrbikmyep.html

Py:   def __str__(self): return self.name
来源：http://hz.sweek.top/gttpdccyju.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.dashuyun.cn/gtgsddrhah.html

JS:   toString() { return this.name; }
来源：http://hz.yangfankeji.com/gthnbqevgf.html

TS:   toString(): string { return this.name; }
来源：http://hz.vqdsnc.cn/gtizeujznt.html

Java: @Override public String toString() { return name; }
来源：http://hz.zhijiandao.cn/gtdmlfovtm.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.chenzaomai.com/gtdaqgafnn.html

Ruby: def to_s; @name; end
来源：http://hz.andypj.xyz/gtlabhyjjt.html

C#:   public override string ToString() => Name;
来源：http://hz.pycfn.com/gtibcibjrr.html

[G13] 判断对象类型
来源：http://hz.9152youxi.cn/gtalrnutin.html

Py:   isinstance(u, User)
来源：http://hz.jinghuilouyu.cn/gtbjgsqcch.html

PHP:  $u instanceof User
来源：http://hz.hysaishi.cn/gtpulphihs.html

JS:   u instanceof User
来源：http://hz.haohaochexian.top/gtyzjctisp.html

TS:   u instanceof User
来源：http://hz.sufxvd.cn/gtmqzdmzwe.html

Java: u instanceof User
来源：http://hz.wangdashe.top/gteczwuoyx.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.daxiang520.top/gtwjdwztdd.html

Ruby: u.is_a?(User)
来源：http://hz.jianghu66.top/gtbppniris.html

C#:   u is User
来源：http://hz.shanyushiyangtech.top/gttpexbtxj.html

[G14] 数据类 / record
来源：http://hz.daria6918.cn/gtsjlcoscr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.cheryme.top/gtvbwnibnm.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.gotoacloud.top/gtjnrtfwyz.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.chenzaomai.com/gtpnklcuns.html

TS:   type User = { name: string; age: number };
来源：http://hz.vqdsnc.cn/gtytxvxzpa.html

Java: record User(String name, int age) {}
来源：http://hz.yvedp.cn/gteywabdog.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yuanzhike.top/gtsoiebyqz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jinyuanbaomall.cn/gtspzosdma.html

C#:   record User(string Name, int Age);
来源：http://hz.guowangkeji.top/gtlxwiagfs.html

[G15] 枚举
来源：http://hz.shanyushiyangkeji.top/gtfrjonkta.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.shangyingyoupin.top/gtwxqduuzb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhongyouzk.top/gtlusaijke.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.chenzaomai.com/gtziizqgje.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhijiandao.cn/gtwkgahokf.html

Java: enum Color { RED, GREEN }
来源：http://hz.dianchejie.cn/gtyxoohrnt.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.xziqi.cn/gtgowghivg.html

Ruby: Color = %i[red green].freeze
来源：http://hz.cqqwz.cn/gtrakckwov.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ydzc1.top/gtibogkbxk.html

[G16] 对象转数组 / 字典
来源：http://hz.ehwqpu.com/gtjkuerqgu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.gaohongyu789.top/gtbueofals.html

PHP:  get_object_vars($obj);
来源：http://hz.kuanghao11.cn/gtriqydytl.html

JS:   Object.entries(obj)
来源：http://hz.yvedp.cn/gtwkdtfkwu.html

TS:   Object.entries(obj)
来源：http://hz.xinyue.icu/gtjeluwgiq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.xuetiantiany.cn/gtbevchihv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.tian-w.cn/gtdnhmirtd.html

Ruby: obj.instance_variables
来源：http://hz.cucudq.cn/gtpvoyfceg.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.316326.xyz/gtzrbcstse.html

================================================================================
来源：http://hz.yj202588.top/gtdfghjczy.html

H. 异常与错误处理
来源：http://hz.tanke756.top/gtwvmmdhhl.html

================================================================================
来源：http://hz.andypj.xyz/gtliuiwrxa.html

[H01] try / catch 基础
来源：http://hz.shuidangran.top/gtgtfmjewx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.chenzaomai.com/gtelopddri.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.pycfn.com/gtvdiesjdz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jiagoushi.top/gtcxqtcpmr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.tanke756.top/gtxdenftos.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.316326.xyz/gtzcstmynl.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.daria6918.cn/gteaxsqbot.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.xinyue.icu/gtelgyyzjp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhongyouzk.top/gtmenfbcap.html

[H02] finally / ensure 收尾
来源：http://hz.jinghuilouyu.cn/gtnnhmsbdt.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.gaohongyu789.top/gtvwtbcjau.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yanxiufei.cn/gtyuubpbyl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jinghuilouyu.cn/gtllthqjml.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhengqikj.top/gtfakwwoxg.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.nanxuanxn.top/gtpwqgesfz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.mhx1999.top/gtihvwiacf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.0kj1m.cn/gtizefdesr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.sysykeji.top/gtvhuuxxws.html

[H03] 主动抛出异常
来源：http://hz.tianlin.xyz/gtkwiposcw.html

Py:   raise ValueError("错误信息")
来源：http://hz.gogol.net.cn/gttkbcmqoy.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.tianlin.xyz/gtmovhynoo.html

JS:   throw new Error("错误信息");
来源：http://hz.xuetiantiany.cn/gtrcpikpae.html

TS:   throw new Error("错误信息");
来源：http://hz.zycfv.cn/gthingmwba.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.hongshengwenyu.top/gtwbuspifj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hfpthk.cn/gthsdgqjfa.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.xylfe.cn/gteeqcmncy.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.shzxlz.cn/gturcsrdbg.html

[H04] 自定义异常类型
来源：http://hz.daxiang520.top/gttywuzqjm.html

Py:   class MyError(Exception): pass
来源：http://hz.ydjk.org.cn/gtkmbcfxwz.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yueranfly.top/gtcdjhatxh.html

JS:   class MyError extends Error {}
来源：http://hz.xuanzx.com/gthhqtbrng.html

TS:   class MyError extends Error {}
来源：http://hz.hysaishi.cn/gtprgyofqh.html

Java: class MyException extends RuntimeException {}
来源：http://hz.kuanghao11.cn/gtppfwwhty.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.shzxlz.cn/gtznbdudwe.html

Ruby: class MyError < StandardError; end
来源：http://hz.nanxinkj.top/gtwpytbztb.html

C#:   class MyException : Exception {}
来源：http://hz.dianchejie.cn/gtrejmkpjo.html

[H05] 捕获特定类型
来源：http://hz.tian-w.cn/gtvrrnndoe.html

Py:   except ValueError as e:
来源：http://hz.daria6918.cn/gtsyofoukg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.gaohongyu789.top/gtphafuvuw.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.dashuyun.cn/gtjpldmtmo.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yuanzhike.top/gtzwlpyfea.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.sufxvd.cn/gtytfkxhho.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.sufxvd.cn/gtdxrudifd.html

Ruby: rescue ArgumentError => e
来源：http://hz.shanyushiyangtech.top/gtqkpfhixr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.gogol.net.cn/gtdcpkzoxz.html

[H06] 可选值 / 空值安全访问
来源：http://hz.shangyingyoupin.top/gtkmwycfay.html

Py:   value = d.get("k") or default
来源：http://hz.kuanghao11.cn/gtugwjzhhd.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.fzhhl.top/gtjhglpvht.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jqgufenzy.top/gtfovgfiwf.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.gaohongyu789.top/gtyjrwgttl.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.kuanghao11.cn/gtbssuxepq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.nanxinkj.top/gtapwutpzv.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zycfv.cn/gtwlrvknsb.html

C#:   obj?.A?.B ?? default
来源：http://hz.zhongyouzk.top/gtnjunypjt.html

[H07] 断言
来源：http://hz.yj20258888.top/gtddhgnbyp.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zhaomingkeji.xyz/gtwylilbdd.html

PHP:  assert($x > 0);
来源：http://hz.cucudq.cn/gtmrfjvqev.html

JS:   console.assert(x > 0);
来源：http://hz.zhongyouzk.top/gtglvxrdsk.html

TS:   console.assert(x > 0);
来源：http://hz.hnxiangtu.top/gtqsivrqpe.html

Java: assert x > 0 : "必须为正";
来源：http://hz.chenjidiqi.icu/gtzfaegjba.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yj20258.top/gtuagfqdfn.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.cucudq.cn/gtymbnjdbq.html

C#:   Debug.Assert(x > 0);
来源：http://hz.tanke756.top/gtjkittfrj.html

[H08] 获取错误信息与堆栈
来源：http://hz.yj20258.top/gtmqbhyjok.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.dashuyun.cn/gtdzxpmkni.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.chenzaomai.com/gtvtvbzjsa.html

JS:   e.message;  e.stack
来源：http://hz.jianghu66.top/gtuzvrxnux.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.fzhhl.top/gtgmlbvfgs.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.tian-w.cn/gtuezcssjd.html

Go:   err.Error()
来源：http://hz.aibaodan.cn/gtghqmxzbr.html

Ruby: e.message;  e.backtrace
来源：http://hz.aizwys.cn/gtbyalhkmc.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhaomingkeji.xyz/gtpbekvupd.html

[H09] 带错误码的异常
来源：http://hz.hfpthk.cn/gtzqxeejba.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.xinyue.icu/gtkgemtvyn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ybcxt.top/gtwxrvvrag.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.ppjwa.cn/gtahdacyic.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.vqdsnc.cn/gtqyekcigr.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.gogol.net.cn/gteyqjkyzz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ybcxt.top/gtplvtqmkr.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.feifeiyinyue.top/gthzoysgra.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.xylfe.cn/gtwyedmhyo.html

[H10] 资源自动释放
来源：http://hz.mhx1999.top/gtigvxnior.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zdqjudy.top/gtpurtmxgh.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jinqigfzy.top/gtrkzlsrbo.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xylfe.cn/gteutrvlrc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yvedp.cn/gtlwtcjhpt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jinqigfzy.top/gtbboiwyeo.html

Go:   defer f.Close()
来源：http://hz.cashguo.top/gtdugympld.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.svipenyu.cn/gteeyxtmmu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.0kj1m.cn/gtdnzxpfgi.html

================================================================================
来源：http://hz.ybcxt.top/gtplbyadkc.html

I. 正则表达式
来源：http://hz.redwolf501.top/gtjkmsdguh.html

================================================================================
来源：http://hz.haohaochexian.top/gtvdljacnp.html

[I01] 判断是否匹配
来源：http://hz.xuanzx.com/gtqpwrpsez.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.ivvv.top/gtqxceyugz.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.hongshengwenyu.top/gtztmjmcia.html

JS:   /\d+/.test(s)
来源：http://hz.cheryme.top/gtjwdoorly.html

TS:   /\d+/.test(s)
来源：http://hz.316326.xyz/gtiwfwljhf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zhoulong.xyz/gtwocrsann.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.xylfe.cn/gthuyylgzk.html

Ruby: s.match?(/\d+/)
来源：http://hz.zhoulong.xyz/gtrefmqaql.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jqgfzy.top/gtvnqqgceh.html


<!-- 参考信息 -->