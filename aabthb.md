代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.chenjidiqi.icu/gtrjadzjsd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.xziqi.cn/gtsuzhhyyn.html

Ruby: Dir.children("dir")
来源：http://hz.jlsjyb.cn/gtwvqjpbsz.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zhixingplan.top/gtcelahsqh.html

[F09] 获取文件大小
来源：http://hz.snrcjt.cn/gtjgiizljm.html

Py:   os.path.getsize("a.txt")
来源：http://hz.xylfe.cn/gtsomzzcvz.html

PHP:  filesize("a.txt");
来源：http://hz.zhaomingkeji.xyz/gtnxwqfody.html

JS:   fs.statSync("a.txt").size
来源：http://hz.ehwqpu.com/gtxaewdjxo.html

TS:   fs.statSync("a.txt").size
来源：http://hz.c1oappe.top/gtkpsazbwx.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.tanke756.top/gtxoltxqpg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.dianchejie.cn/gtmrcjases.html

Ruby: File.size("a.txt")
来源：http://hz.mhx1999.top/gtcddmlmdp.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yueranfly.top/gtsedoquso.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zdqjudy.top/gtshrrxfgh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.hnxiangtu.top/gtigxwortz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.shzxlz.cn/gtgyuapxkd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.52xcode.cn/gtdbdibaax.html

TS:   path.extname("a.txt")
来源：http://hz.chenzaomai.com/gtxxbaetjo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.tanke756.top/gthjbwdgll.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.svipenyu.cn/gtwjjykqia.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yangfankeji.com/gtchmjepjs.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zhengqikj.top/gtsmeyirgf.html

[F11] 复制与移动文件
来源：http://hz.316326.xyz/gtlnypvxtp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.hywenlv.cn/gtpzstznmd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.cqqwz.cn/gtxgwtwpme.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cucudq.cn/gtsglruvxw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.nanxuanxn.top/gtuwencybf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.birdmap.top/gtzgpsolzk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.hfpthk.cn/gtqvtubcep.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.aibaodan.cn/gtybwgymes.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.mhx1999.top/gtbhsueolb.html

[F12] CSV 读写
来源：http://hz.svipenyu.cn/gtsfeuuqiq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zhiwuduotai.top/gtgknhwxsx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.pengpengdd.cyou/gtrgqniaxz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.fengsongda.top/gtigmeovsq.html

TS:   // 同上
来源：http://hz.shanyushiyangtech.top/gtlruzwaxn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.gogol.net.cn/gtdjgmfmwg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhengqikj.top/gtaqkexefq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.0kj1m.cn/gtcyxpcwzn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jlsjyb.cn/gtsxrtunhg.html

================================================================================
来源：http://hz.chenlongwang.top/gtirwjibwq.html

G. 面向对象
来源：http://hz.jinqigufen.top/gthczrzudt.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtgowjahhk.html

[G01] 定义类
来源：http://hz.pengpengdd.cyou/gtudkumajg.html

Py:   class User: pass
来源：http://hz.yongpay.top/gtxmpixeuu.html

PHP:  class User {}
来源：http://hz.jianghu66.top/gtbfydcvlv.html

JS:   class User {}
来源：http://hz.cashguo.top/gtlqhzzrwb.html

TS:   class User { name: string = ""; }
来源：http://hz.hnxiangtu.top/gtvsbzsrzx.html

Java: class User {}
来源：http://hz.zhiwuduotai.top/gtsnunqbhr.html

Go:   type User struct { Name string }
来源：http://hz.yonumen.top/gtdhegnxwr.html

Ruby: class User; end
来源：http://hz.guowangkeji.top/gtyspydwxt.html

C#:   class User {}
来源：http://hz.shuidangran.top/gttizvlgxc.html

[G02] 构造函数
来源：http://hz.nanxinkj.top/gtkanpcwss.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.chenlongwang.top/gtfbowajhz.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.mhx1999.top/gtjicpgoss.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.gzhubu.top/gtgjmjgkbs.html

TS:   constructor(public name: string) {}
来源：http://hz.aibaodan.cn/gtzmlqzndf.html

Java: User(String name) { this.name = name; }
来源：http://hz.xuanzx.com/gtbduyivgc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jyoumei.cn/gtdsankiww.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.52xcode.cn/gtgjbhajea.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yvedp.cn/gtdoraqrvq.html

[G03] 实例属性
来源：http://hz.tianlin.xyz/gtgzpddjty.html

Py:   self.name = "x"
来源：http://hz.daria6918.cn/gtdetmlxaa.html

PHP:  public string $name = "x";
来源：http://hz.xuetiantiany.cn/gthibaztzz.html

JS:   this.name = "x";
来源：http://hz.chenjidiqi.icu/gtfccvjpue.html

TS:   name: string = "x";
来源：http://hz.jlsjyb.cn/gtgtncbque.html

Java: private String name;
来源：http://hz.yj20258888.top/gtvivioqqb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.9152youxi.cn/gtwdcjpngy.html

Ruby: @name = "x"
来源：http://hz.zhijiandao.cn/gtrcsptudh.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jyoumei.cn/gtmehkccai.html

[G04] 定义方法
来源：http://hz.gogol.net.cn/gtxfbkuaaz.html

Py:   def greet(self): return self.name
来源：http://hz.havefunace.top/gtyczozjqi.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.xuanzx.com/gttxlcwuws.html

JS:   greet() { return this.name; }
来源：http://hz.sxryk.cn/gtrpeytgap.html

TS:   greet(): string { return this.name; }
来源：http://hz.ydjk.org.cn/gtsxsfdxyw.html

Java: String greet() { return name; }
来源：http://hz.shuidangran.top/gtgkvonvfa.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.wangshuangyany.cn/gtcybbebsa.html

Ruby: def greet; @name; end
来源：http://hz.nanxinkj.top/gtffypjgyv.html

C#:   public string Greet() => Name;
来源：http://hz.yuxming.cn/gtmhhijugm.html

[G05] 继承
来源：http://hz.hysaishi.cn/gtafhwlrra.html

Py:   class Admin(User): pass
来源：http://hz.nwbrower.top/gtnrsqnrzv.html

PHP:  class Admin extends User {}
来源：http://hz.aizwys.cn/gtdpmxnjkv.html

JS:   class Admin extends User {}
来源：http://hz.gotoacloud.top/gtpujnwmdh.html

TS:   class Admin extends User {}
来源：http://hz.wangdashe.top/gtmjwxdugl.html

Java: class Admin extends User {}
来源：http://hz.c1oappe.top/gtibttxove.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.nwbrower.top/gtbzjjkytq.html

Ruby: class Admin < User; end
来源：http://hz.hysaishi.cn/gtjablskze.html

C#:   class Admin : User {}
来源：http://hz.jqgfzy.top/gtwttzakcc.html

[G06] 重写方法
来源：http://hz.jlsjyb.cn/gtuujlkzpq.html

Py:   def greet(self): return "admin"
来源：http://hz.mhx1999.top/gtwppohgym.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.shuidangran.top/gtfogzpilj.html

JS:   greet() { return "admin"; }
来源：http://hz.jqgfzy.top/gtbqreyaxy.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hysaishi.cn/gtqsiqzhhj.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hysaishi.cn/gtneymrewl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.kuanghao11.cn/gtegvnijmf.html

Ruby: def greet; "admin"; end
来源：http://hz.snrcjt.cn/gtdflnaqtx.html

C#:   public override string Greet() => "admin";
来源：http://hz.jyoumei.cn/gtlehvxwfd.html

[G07] 调用父类方法
来源：http://hz.hongshengwenyu.top/gtwvtjyouv.html

Py:   super().greet()
来源：http://hz.xuetiantiany.cn/gthplkxupk.html

PHP:  parent::greet();
来源：http://hz.jyoumei.cn/gtrntoglhm.html

JS:   super.greet();
来源：http://hz.jqgfzy.top/gtesqeusso.html

TS:   super.greet();
来源：http://hz.yuxming.cn/gtxlcibbzc.html

Java: super.greet();
来源：http://hz.hfpthk.cn/gtgogsouwj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.guannengcc.top/gtjwswxmiz.html

Ruby: super
来源：http://hz.cdnleiting.top/gtpzbrpffb.html

C#:   base.Greet();
来源：http://hz.hfpthk.cn/gtowvmwvyj.html

[G08] 静态方法与属性
来源：http://hz.sweek.top/gtmfaihfit.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.wangshuangyany.cn/gtpcvkthpk.html

PHP:  public static function f() {}
来源：http://hz.zhengqikj.top/gtbozizbdd.html

JS:   static f() {}
来源：http://hz.andypj.xyz/gtylsocunw.html

TS:   static f(): void {}
来源：http://hz.cdnleiting.top/gtjwffsaef.html

Java: static void f() {}
来源：http://hz.ybcxt.top/gtgjfcgajj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.hysaishi.cn/gtorojtzgj.html

Ruby: def self.f; end
来源：http://hz.gaohongyu789.top/gtyyxduice.html

C#:   public static void F() {}
来源：http://hz.hysaishi.cn/gtlwtpwfbs.html

[G09] 接口 / 抽象类
来源：http://hz.zhixingplan.top/gtomjbjdab.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.pengpengdd.cyou/gtavphjtmg.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.gotoacloud.top/gtywutyjqc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.9152youxi.cn/gtrpsdjoha.html

TS:   interface Shape { area(): number; }
来源：http://hz.mhx1999.top/gthyirmauh.html

Java: interface Shape { double area(); }
来源：http://hz.guannengcc.top/gtjvduwwmx.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.xylfe.cn/gtjwekptts.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.xylfe.cn/gtfsmzepsv.html

C#:   interface IShape { double Area(); }
来源：http://hz.nwbrower.top/gtisjqirui.html

[G10] 访问控制
来源：http://hz.iojbl.cn/gtwuoasfyg.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhengqikj.top/gthoctmpnn.html

PHP:  public / protected / private
来源：http://hz.yj20258888.top/gtxtynwxit.html

JS:   #private 字段；其余公开
来源：http://hz.wangshuangyany.cn/gtvqjqpvba.html

TS:   public / protected / private
来源：http://hz.xingfuxueyuan.xyz/gtpcmhukwc.html

Java: public / protected / private / 默认包级
来源：http://hz.gotoacloud.top/gtljzilcke.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.dashuyun.cn/gtdeannnfj.html

Ruby: public / protected / private
来源：http://hz.yj202588.top/gtjobwnivq.html

C#:   public / protected / private / internal
来源：http://hz.shanyushiyangkeji.top/gtigkgcoxc.html

[G11] getter / setter
来源：http://hz.wangdashe.top/gtgcwlnsmy.html

Py:   @property 与 @x.setter
来源：http://hz.sweek.top/gtbjtekrtl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.iojbl.cn/gtbmxuuqnw.html

JS:   get name() { return this._name; }
来源：http://hz.hfpthk.cn/gtrhjaeuwj.html

TS:   get name(): string { return this._name; }
来源：http://hz.shzxlz.cn/gtlivvbyil.html

Java: public String getName() { return name; }
来源：http://hz.dianchejie.cn/gtlpqlzelw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.daxiang520.top/gtafzfkaav.html

Ruby: attr_accessor :name
来源：http://hz.pycfn.com/gtsdkavmjv.html

C#:   public string Name { get; set; }
来源：http://hz.tianlin.xyz/gtmjdrjafd.html

[G12] 对象转字符串
来源：http://hz.feifeiyinyue.top/gtflcotuae.html

Py:   def __str__(self): return self.name
来源：http://hz.chenjidiqi.icu/gtdinhegxj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ivvv.top/gttuziahxr.html

JS:   toString() { return this.name; }
来源：http://hz.smart0.xyz/gtuumrjzzt.html

TS:   toString(): string { return this.name; }
来源：http://hz.shzxlz.cn/gtowlhlsci.html

Java: @Override public String toString() { return name; }
来源：http://hz.guannengcc.top/gtfhqwugtm.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.shzxlz.cn/gtctrzvtbk.html

Ruby: def to_s; @name; end
来源：http://hz.hysaishi.cn/gtjoszgodc.html

C#:   public override string ToString() => Name;
来源：http://hz.jiagoushi.top/gtlxbumqiu.html

[G13] 判断对象类型
来源：http://hz.cdnleiting.top/gtkyjkakhm.html

Py:   isinstance(u, User)
来源：http://hz.xuetiantiany.cn/gtbncxcftz.html

PHP:  $u instanceof User
来源：http://hz.yvedp.cn/gtlpjqrfgu.html

JS:   u instanceof User
来源：http://hz.ywan-chungtsiang.top/gtpaqkzncz.html

TS:   u instanceof User
来源：http://hz.ivvv.top/gtrvqnfkdl.html

Java: u instanceof User
来源：http://hz.birdmap.top/gtjufmzypz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yueranfly.top/gtplxqgxzn.html

Ruby: u.is_a?(User)
来源：http://hz.cheryme.top/gtmmynkqyp.html

C#:   u is User
来源：http://hz.yuxming.cn/gtdjdiovbk.html

[G14] 数据类 / record
来源：http://hz.zhaomingkeji.xyz/gtwznnjbli.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.sufxvd.cn/gtastrizwd.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.aibaodan.cn/gtawqswgpp.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.fzhhl.top/gtkrmrqpae.html

TS:   type User = { name: string; age: number };
来源：http://hz.tanke756.top/gtavbyfxgf.html

Java: record User(String name, int age) {}
来源：http://hz.jinghuilouyu.cn/gtctszmjdj.html

Go:   type User struct { Name string; Age int }
来源：http://hz.cheryme.top/gteedxlmlx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.shanyushiyangtech.top/gtbpkeskur.html

C#:   record User(string Name, int Age);
来源：http://hz.jyoumei.cn/gtsszdszix.html

[G15] 枚举
来源：http://hz.xuetiantiany.cn/gtwbtzjpst.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.andypj.xyz/gtxvdbcdez.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.svipenyu.cn/gtvmxhysek.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.wangshuangyany.cn/gtpkiogyrm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yuxming.cn/gteulyapmf.html

Java: enum Color { RED, GREEN }
来源：http://hz.xingfuxueyuan.xyz/gtgeoosofe.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zhongyouzk.top/gtopfrsgws.html

Ruby: Color = %i[red green].freeze
来源：http://hz.guowangkeji.top/gtbrowqqbt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.bjfxy.top/gtctesdsul.html

[G16] 对象转数组 / 字典
来源：http://hz.xziqi.cn/gtnwpgojwq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.gzhubu.top/gtoljjiduc.html

PHP:  get_object_vars($obj);
来源：http://hz.jyoumei.cn/gtlqappxfn.html

JS:   Object.entries(obj)
来源：http://hz.yanxiufei.cn/gtouwpkaiy.html

TS:   Object.entries(obj)
来源：http://hz.yueranfly.top/gtgwxattjr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jiagoushi.top/gtiewafzrm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.tianlin.xyz/gtrqnqldai.html

Ruby: obj.instance_variables
来源：http://hz.gzhubu.top/gtonmjysne.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.haohaochexian.top/gtevphfubp.html

================================================================================
来源：http://hz.fzhhl.top/gtbvfnqpte.html

H. 异常与错误处理
来源：http://hz.nanxinkj.top/gtcrxluzwg.html

================================================================================
来源：http://hz.sysykeji.top/gtbzllcxqn.html

[H01] try / catch 基础
来源：http://hz.shangyingyoupin.top/gtflqewqua.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.fzhhl.top/gtzxtaobtq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zhaomingkeji.xyz/gtebxktqhp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zdqjudy.top/gtgmaqnqpp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.chenjidiqi.icu/gtnnvzmcbt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jiagoushi.top/gtymbzbogj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.sweek.top/gtfalflztu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.tianlin.xyz/gtgzoxohqr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.chenjidiqi.icu/gtdwgscbpa.html

[H02] finally / ensure 收尾
来源：http://hz.guowangkeji.top/gtqnjuqvuo.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jqgufenzy.top/gtkvzrvlvg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhixingplan.top/gtqksjalqm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hfpthk.cn/gtntpdffsu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.shangyingyoupin.top/gtvaaqeiid.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.aibaodan.cn/gtiyuhofkp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zdqjudy.top/gtswcqdino.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yuxming.cn/gtnzdwjnoh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.wangshuangyany.cn/gtuycfecnc.html

[H03] 主动抛出异常
来源：http://hz.wangshuangyany.cn/gtfccsurfs.html

Py:   raise ValueError("错误信息")
来源：http://hz.yongpay.top/gtdntpcfqa.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.xuanzx.com/gtkrzmuwtm.html

JS:   throw new Error("错误信息");
来源：http://hz.tianlin.xyz/gtqfwgkchv.html

TS:   throw new Error("错误信息");
来源：http://hz.gzhubu.top/gthvgulphz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.ybcxt.top/gttymcniud.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.tian-w.cn/gtxuqdhiek.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jlsjyb.cn/gtwqwpqhlv.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zhongyouzk.top/gtnfrepbgy.html

[H04] 自定义异常类型
来源：http://hz.shangyingyoupin.top/gtoobvibyp.html

Py:   class MyError(Exception): pass
来源：http://hz.haohaochexian.top/gtjniepgak.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jiagoushi.top/gtmappiebr.html

JS:   class MyError extends Error {}
来源：http://hz.gotoacloud.top/gtnzalgjti.html

TS:   class MyError extends Error {}
来源：http://hz.wangdashe.top/gtrdtvwige.html

Java: class MyException extends RuntimeException {}
来源：http://hz.cdnleiting.top/gthhoucslj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.quarkkingdee.top/gtirloztlx.html

Ruby: class MyError < StandardError; end
来源：http://hz.jqgufenzy.top/gtawoolxww.html

C#:   class MyException : Exception {}
来源：http://hz.9152youxi.cn/gtaretnkfc.html

[H05] 捕获特定类型
来源：http://hz.redwolf501.top/gtondgdzbh.html

Py:   except ValueError as e:
来源：http://hz.hysaishi.cn/gtixvbtrvq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.shzxlz.cn/gtibyozekt.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.c1oappe.top/gtbeyhztir.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.guowangkeji.top/gtakujgdmb.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.vqdsnc.cn/gtefjldwxf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jqgfzy.top/gtllesljkh.html

Ruby: rescue ArgumentError => e
来源：http://hz.cdnleiting.top/gtkdzozjgj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.mhx1999.top/gtpahaogcn.html

[H06] 可选值 / 空值安全访问
来源：http://hz.daxiang520.top/gtsqaxoegg.html

Py:   value = d.get("k") or default
来源：http://hz.cucudq.cn/gtgymzlcsm.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.vqdsnc.cn/gtkrxhflly.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ivvv.top/gtvxzworqf.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.pycfn.com/gtnnqdxejr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.hywenlv.cn/gtsjdccrtk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.shzxlz.cn/gttwgqclay.html

Ruby: d&.dig(:a, :b)
来源：http://hz.hnqzz.top/gtqmeguier.html

C#:   obj?.A?.B ?? default
来源：http://hz.vqdsnc.cn/gthpqghsow.html

[H07] 断言
来源：http://hz.zhengqikj.top/gtbeihumcx.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yj20258888.top/gtvcqphvzd.html

PHP:  assert($x > 0);
来源：http://hz.yongpay.top/gtuftlkmwa.html

JS:   console.assert(x > 0);
来源：http://hz.cashguo.top/gtovdgpodl.html

TS:   console.assert(x > 0);
来源：http://hz.yueranfly.top/gtywqtwlmn.html

Java: assert x > 0 : "必须为正";
来源：http://hz.cashguo.top/gtttytpmlf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yueranfly.top/gtzspicssd.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zycfv.cn/gtpvfohnez.html

C#:   Debug.Assert(x > 0);
来源：http://hz.hysaishi.cn/gtjxjeihmp.html

[H08] 获取错误信息与堆栈
来源：http://hz.yuxming.cn/gtuikbwjcl.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.hywenlv.cn/gtjzekoqle.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.xingfuxueyuan.xyz/gtzgahxycv.html

JS:   e.message;  e.stack
来源：http://hz.zhixingplan.top/gtmzfenyup.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.cqqwz.cn/gtvhnzejqv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.chenjidiqi.icu/gtvermxhao.html

Go:   err.Error()
来源：http://hz.yj20258.top/gtfanbytfw.html

Ruby: e.message;  e.backtrace
来源：http://hz.iojbl.cn/gtvmbtcyax.html

C#:   e.Message;  e.StackTrace
来源：http://hz.fengsongda.top/gtqbumxzxs.html

[H09] 带错误码的异常
来源：http://hz.pycfn.com/gtgsdwcmsx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.nanxinkj.top/gtslcbuiob.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.quarkkingdee.top/gtfvllnunj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.tanke756.top/gtmgmfzjzt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.tianlin.xyz/gtlowsedfn.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.0kj1m.cn/gtzxfdrbrm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yongpay.top/gteudevdsz.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.ppjwa.cn/gtznfiiwkx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.mhx1999.top/gttcadhcdz.html

[H10] 资源自动释放
来源：http://hz.sysykeji.top/gtdtkcgvxv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.birdmap.top/gtqwtsvefu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.feifeiyinyue.top/gtjdkkbmyl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.chenzaomai.com/gtvypvlhkp.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hysaishi.cn/gtrggmhxdl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.sysykeji.top/gtqtaltdkj.html

Go:   defer f.Close()
来源：http://hz.yuanzhike.top/gtavvdhipc.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.smart0.xyz/gtckkcvypy.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.shzxlz.cn/gtadznrmql.html

================================================================================
来源：http://hz.svipenyu.cn/gtiojsdoog.html

I. 正则表达式
来源：http://hz.cqqwz.cn/gtowgysjrm.html

================================================================================
来源：http://hz.hnxiangtu.top/gtnzfdoeix.html

[I01] 判断是否匹配
来源：http://hz.andypj.xyz/gtvtlzjyed.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.chenzaomai.com/gtvatykrfw.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.guannengcc.top/gtukkrqxsn.html

JS:   /\d+/.test(s)
来源：http://hz.xingfuxueyuan.xyz/gtqflftjqr.html

TS:   /\d+/.test(s)
来源：http://hz.jinqigufen.top/gtwoqlwjjq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.cashguo.top/gtqhpdfwup.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.shanyushiyangtech.top/gtsusabuun.html

Ruby: s.match?(/\d+/)
来源：http://hz.xinyue.icu/gtrwctkqoo.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jyoumei.cn/gtaiixvlhg.html

[I02] 提取所有匹配
来源：http://hz.zhaomingkeji.xyz/gthgijwnab.html

Py:   re.findall(r"\d+", s)
来源：http://hz.zhoulong.xyz/gtrcxmtsih.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.fzhhl.top/gtnkxzkdkd.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.gotoacloud.top/gtpwjfjsub.html

TS:   s.match(/\d+/g)
来源：http://hz.zhijiandao.cn/gtakladfnq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hfpthk.cn/gtzzxbcnri.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.guowangkeji.top/gttbhgapvl.html

Ruby: s.scan(/\d+/)
来源：http://hz.xuanzx.com/gtpxwvpppa.html


<!-- 参考信息 -->