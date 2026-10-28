代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.cucudq.cn/gtfcsvowuy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jiagoushi.top/gtjjpqdhff.html

JS:   fs.readdirSync("dir")
来源：http://hz.aibaodan.cn/gtisjlamrk.html

TS:   fs.readdirSync("dir")
来源：http://hz.jinyuanbaomall.cn/gtxvvdbifo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zhoulong.xyz/gtkjfuduin.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.ivvv.top/gtwosjdlnz.html

Ruby: Dir.children("dir")
来源：http://hz.jqgufenzy.top/gtnafrseuj.html

C#:   Directory.GetFiles("dir")
来源：http://hz.sufxvd.cn/gtwmtukvub.html

[F09] 获取文件大小
来源：http://hz.jinghuilouyu.cn/gtjaduglif.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jqgufenzy.top/gtqdfoyytj.html

PHP:  filesize("a.txt");
来源：http://hz.birdmap.top/gtahlljdpj.html

JS:   fs.statSync("a.txt").size
来源：http://hz.hfpthk.cn/gtpkprlzwq.html

TS:   fs.statSync("a.txt").size
来源：http://hz.guannengcc.top/gtzprhymtn.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.52xcode.cn/gtayjzfedj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jiagoushi.top/gtlmbqhajs.html

Ruby: File.size("a.txt")
来源：http://hz.jinqigufen.top/gtehjxxwdz.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.gaohongyu789.top/gtmiqkbjur.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.nanxinkj.top/gtgqhhedxh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.nanxuanxn.top/gtcudvjoex.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.cashguo.top/gttbrmkwxl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.52xcode.cn/gtiymcxzja.html

TS:   path.extname("a.txt")
来源：http://hz.gzhubu.top/gtsvpuchhw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.hnqzz.top/gtfioitslm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.havefunace.top/gtxqhalwtn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jiagoushi.top/gtlhgevhus.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.aizwys.cn/gtgbwmzroa.html

[F11] 复制与移动文件
来源：http://hz.ydjk.org.cn/gtnsgkxsjv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jinqigufen.top/gtglzyiwfk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.0kj1m.cn/gtdfaooahb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jyoumei.cn/gtsqcznwal.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cqqwz.cn/gtsnclpqln.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.chenjidiqi.icu/gtkrhbcrtb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.zhijiandao.cn/gtagqwbjtm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.shangyingyoupin.top/gtbfpzdbaf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yongpay.top/gteruyvhgn.html

[F12] CSV 读写
来源：http://hz.meibo888.top/gtusjezvda.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yj20258.top/gtcgbnlakl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jlsjyb.cn/gthaazgkip.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.bjfxy.top/gtbqxghuum.html

TS:   // 同上
来源：http://hz.guowangkeji.top/gtoldiyxwl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ivvv.top/gtwpldeqcc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.bjfxy.top/gthijhzizj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yuxming.cn/gtwjuwnnxn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.redwolf501.top/gtcrpsztlq.html

================================================================================
来源：http://hz.sysykeji.top/gtxdysumff.html

G. 面向对象
来源：http://hz.zhaomingkeji.xyz/gttzxljirz.html

================================================================================
来源：http://hz.yuanzhike.top/gtgqsebjst.html

[G01] 定义类
来源：http://hz.zhijiandao.cn/gtwxsgpxhn.html

Py:   class User: pass
来源：http://hz.xylfe.cn/gtamxoxaqy.html

PHP:  class User {}
来源：http://hz.xuanzx.com/gtndikbqwr.html

JS:   class User {}
来源：http://hz.xziqi.cn/gtmmixpbad.html

TS:   class User { name: string = ""; }
来源：http://hz.yvedp.cn/gtjwkjctbz.html

Java: class User {}
来源：http://hz.xziqi.cn/gtxtuhysmz.html

Go:   type User struct { Name string }
来源：http://hz.yvedp.cn/gtydshnvfc.html

Ruby: class User; end
来源：http://hz.meibo888.top/gtwzvwynvf.html

C#:   class User {}
来源：http://hz.cashguo.top/gtwohiriyi.html

[G02] 构造函数
来源：http://hz.shzxlz.cn/gtbxsvcszc.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.fengsongda.top/gtobqthmyv.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yvedp.cn/gtottsbavr.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.meibo888.top/gtksztrgkb.html

TS:   constructor(public name: string) {}
来源：http://hz.dashuyun.cn/gtodgytpio.html

Java: User(String name) { this.name = name; }
来源：http://hz.xylfe.cn/gtonmevrmw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.gzhubu.top/gtcjosvbpm.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.zhixingplan.top/gtcnqaxhgw.html

C#:   public User(string name) { Name = name; }
来源：http://hz.meibo888.top/gtahsjjwok.html

[G03] 实例属性
来源：http://hz.vqdsnc.cn/gtwdskkqxp.html

Py:   self.name = "x"
来源：http://hz.jianghu66.top/gtzhfddhgp.html

PHP:  public string $name = "x";
来源：http://hz.pengpengdd.cyou/gtiqalnaow.html

JS:   this.name = "x";
来源：http://hz.hywenlv.cn/gtmyhkpins.html

TS:   name: string = "x";
来源：http://hz.jinqigufen.top/gthgnkfshk.html

Java: private String name;
来源：http://hz.yongpay.top/gtjjizeljd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zdqjudy.top/gtghrcyait.html

Ruby: @name = "x"
来源：http://hz.zhiwuduotai.top/gtvpnvlvuw.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yvedp.cn/gtjorwxpay.html

[G04] 定义方法
来源：http://hz.gotoacloud.top/gtubzgllkb.html

Py:   def greet(self): return self.name
来源：http://hz.gotoacloud.top/gtbtrkrorg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yuanzhike.top/gtgppyqpug.html

JS:   greet() { return this.name; }
来源：http://hz.andypj.xyz/gtoripmvaf.html

TS:   greet(): string { return this.name; }
来源：http://hz.birdmap.top/gtftemxxmc.html

Java: String greet() { return name; }
来源：http://hz.tianlin.xyz/gtdmyysaug.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.birdmap.top/gtunhuruxz.html

Ruby: def greet; @name; end
来源：http://hz.shanyushiyangkeji.top/gtmzeujbkw.html

C#:   public string Greet() => Name;
来源：http://hz.dianchejie.cn/gtsspuqnti.html

[G05] 继承
来源：http://hz.cheryme.top/gtmeepergn.html

Py:   class Admin(User): pass
来源：http://hz.zycfv.cn/gtrquwuchp.html

PHP:  class Admin extends User {}
来源：http://hz.cqqwz.cn/gtzcobdwpb.html

JS:   class Admin extends User {}
来源：http://hz.jqgufenzy.top/gtfojhvxfd.html

TS:   class Admin extends User {}
来源：http://hz.0kj1m.cn/gtemnogpwl.html

Java: class Admin extends User {}
来源：http://hz.meibo888.top/gtobeykgxi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.316326.xyz/gtleidchlc.html

Ruby: class Admin < User; end
来源：http://hz.snrcjt.cn/gtsdcfcnul.html

C#:   class Admin : User {}
来源：http://hz.zhiwuduotai.top/gtlggxevdp.html

[G06] 重写方法
来源：http://hz.jianghu66.top/gttngwleae.html

Py:   def greet(self): return "admin"
来源：http://hz.yanxiufei.cn/gtvotabbbh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.cashguo.top/gtypbtcqjw.html

JS:   greet() { return "admin"; }
来源：http://hz.zhongyouzk.top/gtjdllefdd.html

TS:   greet(): string { return "admin"; }
来源：http://hz.iojbl.cn/gtflfecukl.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.chenzaomai.com/gthrkjlucj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.bjfxy.top/gtkvcelkst.html

Ruby: def greet; "admin"; end
来源：http://hz.zhoulong.xyz/gtkzubzurb.html

C#:   public override string Greet() => "admin";
来源：http://hz.xziqi.cn/gtcljgneaz.html

[G07] 调用父类方法
来源：http://hz.yj20258888.top/gtoykyolzk.html

Py:   super().greet()
来源：http://hz.yuxming.cn/gtycykddvz.html

PHP:  parent::greet();
来源：http://hz.wangshuangyany.cn/gtmvruausm.html

JS:   super.greet();
来源：http://hz.birdmap.top/gtozlmkusp.html

TS:   super.greet();
来源：http://hz.nanxuanxn.top/gtaskfnmbv.html

Java: super.greet();
来源：http://hz.nanxinkj.top/gtspqlsjmm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.gaohongyu789.top/gtmrapulsx.html

Ruby: super
来源：http://hz.chenjidiqi.icu/gtpboudjeh.html

C#:   base.Greet();
来源：http://hz.hongshengwenyu.top/gtvblbvcup.html

[G08] 静态方法与属性
来源：http://hz.sweek.top/gtbuektqeo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.havefunace.top/gtdthgbhzw.html

PHP:  public static function f() {}
来源：http://hz.wangshuangyany.cn/gtieaxjmbq.html

JS:   static f() {}
来源：http://hz.havefunace.top/gtrdxrsrbv.html

TS:   static f(): void {}
来源：http://hz.wangshuangyany.cn/gtnnpjeutc.html

Java: static void f() {}
来源：http://hz.yuanzhike.top/gtnqgkgqdg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yuanzhike.top/gturqurcgi.html

Ruby: def self.f; end
来源：http://hz.chenlongwang.top/gtpcriymui.html

C#:   public static void F() {}
来源：http://hz.hongshengwenyu.top/gtutjgmvzg.html

[G09] 接口 / 抽象类
来源：http://hz.yanxiufei.cn/gttxtyjakh.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yuanzhike.top/gtlcghflox.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jinqigfzy.top/gtwsbsrwre.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.chenjidiqi.icu/gtfvlvovbj.html

TS:   interface Shape { area(): number; }
来源：http://hz.9152youxi.cn/gtxngiupks.html

Java: interface Shape { double area(); }
来源：http://hz.hongshengwenyu.top/gtxgrqzbzc.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.daxiang520.top/gthseqgupi.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.xinyue.icu/gtyepioefb.html

C#:   interface IShape { double Area(); }
来源：http://hz.tian-w.cn/gtmzlkmxgi.html

[G10] 访问控制
来源：http://hz.hywenlv.cn/gtzcryaxnd.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhaomingkeji.xyz/gtbrdaurmc.html

PHP:  public / protected / private
来源：http://hz.gzhubu.top/gtgcpruaqo.html

JS:   #private 字段；其余公开
来源：http://hz.yj20258.top/gtkjgvyrll.html

TS:   public / protected / private
来源：http://hz.52xcode.cn/gtbdnlfeft.html

Java: public / protected / private / 默认包级
来源：http://hz.zhijiandao.cn/gtdwvobxkq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.guowangkeji.top/gtcfdqhadf.html

Ruby: public / protected / private
来源：http://hz.zhengqikj.top/gtjjhsxdto.html

C#:   public / protected / private / internal
来源：http://hz.hnqzz.top/gtoleoubqw.html

[G11] getter / setter
来源：http://hz.zdqjudy.top/gthflsvicx.html

Py:   @property 与 @x.setter
来源：http://hz.ydzc1.top/gtjaggdguc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.ydjk.org.cn/gtrvadklxd.html

JS:   get name() { return this._name; }
来源：http://hz.ybcxt.top/gtuglatdmc.html

TS:   get name(): string { return this._name; }
来源：http://hz.zdqjudy.top/gtvmmbklal.html

Java: public String getName() { return name; }
来源：http://hz.9152youxi.cn/gtjopzjgct.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yongpay.top/gtmeoekaml.html

Ruby: attr_accessor :name
来源：http://hz.mhx1999.top/gtjorgqadh.html

C#:   public string Name { get; set; }
来源：http://hz.ywan-chungtsiang.top/gtnujiakdq.html

[G12] 对象转字符串
来源：http://hz.zdqjudy.top/gtnnzdksny.html

Py:   def __str__(self): return self.name
来源：http://hz.xingfuxueyuan.xyz/gtcpmywyer.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.redwolf501.top/gtoiavswqb.html

JS:   toString() { return this.name; }
来源：http://hz.chenlongwang.top/gtbovenrwu.html

TS:   toString(): string { return this.name; }
来源：http://hz.hongshengwenyu.top/gtsoepcvzm.html

Java: @Override public String toString() { return name; }
来源：http://hz.yvedp.cn/gtapgpscfc.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.wangdashe.top/gtbiqcasnq.html

Ruby: def to_s; @name; end
来源：http://hz.wangdashe.top/gtokayuqxt.html

C#:   public override string ToString() => Name;
来源：http://hz.nanxinkj.top/gtsvkkewuy.html

[G13] 判断对象类型
来源：http://hz.tian-w.cn/gtcuzivech.html

Py:   isinstance(u, User)
来源：http://hz.shangyingyoupin.top/gtswcajkwk.html

PHP:  $u instanceof User
来源：http://hz.zhoulong.xyz/gtxyhahing.html

JS:   u instanceof User
来源：http://hz.316326.xyz/gtcusnxwzt.html

TS:   u instanceof User
来源：http://hz.hnxiangtu.top/gtlrczqiyb.html

Java: u instanceof User
来源：http://hz.yj20258.top/gtykinenvz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ivvv.top/gtkugmkusg.html

Ruby: u.is_a?(User)
来源：http://hz.smart0.xyz/gtlruscjxq.html

C#:   u is User
来源：http://hz.cqqwz.cn/gtyynditsl.html

[G14] 数据类 / record
来源：http://hz.yvedp.cn/gtroeiqtaa.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yuanzhike.top/gtjygsaxwe.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.cheryme.top/gtrteljiso.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.xuetiantiany.cn/gthshooajn.html

TS:   type User = { name: string; age: number };
来源：http://hz.daxiang520.top/gtxjwaqgnv.html

Java: record User(String name, int age) {}
来源：http://hz.yuxming.cn/gtfilvmxex.html

Go:   type User struct { Name string; Age int }
来源：http://hz.feifeiyinyue.top/gtabopiurc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.shangyingyoupin.top/gtdwqbplep.html

C#:   record User(string Name, int Age);
来源：http://hz.gogol.net.cn/gtnbsfdaol.html

[G15] 枚举
来源：http://hz.vqdsnc.cn/gtzpbqklgy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.nwbrower.top/gtevwyuyjw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yj20258888.top/gtwcyhwavz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.sysykeji.top/gtgmjjilrn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jlsjyb.cn/gtdsrbiiml.html

Java: enum Color { RED, GREEN }
来源：http://hz.hnqzz.top/gtaymiopab.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zhixingplan.top/gteoipgmji.html

Ruby: Color = %i[red green].freeze
来源：http://hz.quarkkingdee.top/gtrzrzdwhq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yueranfly.top/gtlofpqnxf.html

[G16] 对象转数组 / 字典
来源：http://hz.zhongyouzk.top/gtxpgcxyza.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.fengsongda.top/gtwoypbasw.html

PHP:  get_object_vars($obj);
来源：http://hz.aizwys.cn/gtsjbuzpaj.html

JS:   Object.entries(obj)
来源：http://hz.ppjwa.cn/gtfhegaacw.html

TS:   Object.entries(obj)
来源：http://hz.ydjk.org.cn/gtdbfwakzr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.guowangkeji.top/gtednximhx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.nanxuanxn.top/gtzemvgocw.html

Ruby: obj.instance_variables
来源：http://hz.0kj1m.cn/gtesivjzgz.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.hywenlv.cn/gtiyfzvktw.html

================================================================================
来源：http://hz.ehwqpu.com/gtfpxvjnnv.html

H. 异常与错误处理
来源：http://hz.fzhhl.top/gtauerksuw.html

================================================================================
来源：http://hz.redwolf501.top/gtqefqcvrp.html

[H01] try / catch 基础
来源：http://hz.ydzc1.top/gtjyeccujh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhoulong.xyz/gtrnqminwu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.sufxvd.cn/gtnbhdpijb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yj20258888.top/gtarwcxdkb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jlsjyb.cn/gtkzkbwvoy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.c1oappe.top/gtchnscole.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zdqjudy.top/gtruztgzck.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jlsjyb.cn/gtvokaqvwv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.gzhubu.top/gtwozzmdgx.html

[H02] finally / ensure 收尾
来源：http://hz.ehwqpu.com/gtyxmmiphi.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.9152youxi.cn/gtdxnoefia.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yvedp.cn/gtsifktuhk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yueranfly.top/gtgwethlfs.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.c1oappe.top/gtlsohucgy.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.pengpengdd.cyou/gtohkeqavw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.nanxuanxn.top/gtrwvllznm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.tian-w.cn/gtjbjsouig.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.pycfn.com/gthodmasmf.html

[H03] 主动抛出异常
来源：http://hz.ybcxt.top/gtltedxijv.html

Py:   raise ValueError("错误信息")
来源：http://hz.bjfxy.top/gtjjltwrvi.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.tian-w.cn/gtxdubhcey.html

JS:   throw new Error("错误信息");
来源：http://hz.feifeiyinyue.top/gtholqayhk.html

TS:   throw new Error("错误信息");
来源：http://hz.chenzaomai.com/gtonosjdnh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yongpay.top/gtjxjprccj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.c1oappe.top/gtnozhnolh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ehwqpu.com/gtobqthbpa.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.hywenlv.cn/gtmkdfmzsb.html

[H04] 自定义异常类型
来源：http://hz.vqdsnc.cn/gtyqbghfwi.html

Py:   class MyError(Exception): pass
来源：http://hz.yj202588.top/gtfyptmykw.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.gotoacloud.top/gtuacauarv.html

JS:   class MyError extends Error {}
来源：http://hz.yongpay.top/gtgnwtlykg.html

TS:   class MyError extends Error {}
来源：http://hz.cqqwz.cn/gttpuhxpoi.html

Java: class MyException extends RuntimeException {}
来源：http://hz.xylfe.cn/gtoijzbnhv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jqgufenzy.top/gtvcthqsrl.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhaomingkeji.xyz/gtmzyrmtiv.html

C#:   class MyException : Exception {}
来源：http://hz.jianghu66.top/gtsobzixae.html

[H05] 捕获特定类型
来源：http://hz.gzhubu.top/gtwdgqvcot.html

Py:   except ValueError as e:
来源：http://hz.vqdsnc.cn/gtgszueogf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.shanyushiyangkeji.top/gttjlhldey.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.guowangkeji.top/gtipbtbniy.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhijiandao.cn/gtmzsbaqyv.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.sysykeji.top/gtrslwuipp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yvedp.cn/gtlencphnj.html

Ruby: rescue ArgumentError => e
来源：http://hz.jqgufenzy.top/gtyjhdtdtr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.quarkkingdee.top/gtqvpgcdtu.html

[H06] 可选值 / 空值安全访问
来源：http://hz.vqdsnc.cn/gtzzxarupn.html

Py:   value = d.get("k") or default
来源：http://hz.hfpthk.cn/gtkkvzgntr.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hywenlv.cn/gtxrbyccfb.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.quarkkingdee.top/gtcqavmmut.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zhijiandao.cn/gtfqjitvfx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.svipenyu.cn/gttqaytjqm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yongpay.top/gtvtqurdqn.html

Ruby: d&.dig(:a, :b)
来源：http://hz.cucudq.cn/gtlaetzrby.html

C#:   obj?.A?.B ?? default
来源：http://hz.havefunace.top/gtimnukmdg.html

[H07] 断言
来源：http://hz.xinyue.icu/gtlzzyhjdw.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yonumen.top/gtkraufdyo.html

PHP:  assert($x > 0);
来源：http://hz.ppjwa.cn/gtgqqnglka.html

JS:   console.assert(x > 0);
来源：http://hz.iojbl.cn/gtjhnvtbzs.html

TS:   console.assert(x > 0);
来源：http://hz.meibo888.top/gtssnsjxbm.html

Java: assert x > 0 : "必须为正";
来源：http://hz.316326.xyz/gtcecaebuc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jiagoushi.top/gtuqjruknr.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.wangdashe.top/gtcjfpwlad.html

C#:   Debug.Assert(x > 0);
来源：http://hz.hammf.cn/gtijrcpiar.html

[H08] 获取错误信息与堆栈
来源：http://hz.cqqwz.cn/gtsquacjub.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.gzhubu.top/gtjluscdxi.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.hnqzz.top/gtxaicsdlt.html

JS:   e.message;  e.stack
来源：http://hz.zhongyouzk.top/gtyaxxvdge.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yuxming.cn/gtcewrscvy.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.gogol.net.cn/gtdqtxjbyb.html

Go:   err.Error()
来源：http://hz.daria6918.cn/gtxrdcchyy.html

Ruby: e.message;  e.backtrace
来源：http://hz.jiagoushi.top/gthkocrexx.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jlsjyb.cn/gtnqhyykyq.html

[H09] 带错误码的异常
来源：http://hz.pengpengdd.cyou/gtrkqhyjlq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.vqdsnc.cn/gtoygoladd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.gotoacloud.top/gtjrrcbwel.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.hammf.cn/gtxuyvghgx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zhiwuduotai.top/gtdppfjewq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.xuanzx.com/gtrjjrhmwx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.redwolf501.top/gtewpfmwbo.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zhaomingkeji.xyz/gtzsxqifyh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.cqqwz.cn/gtfburypjp.html

[H10] 资源自动释放
来源：http://hz.guannengcc.top/gtlthqxcvv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.shangyingyoupin.top/gtzquqoxiu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.shanyushiyangtech.top/gtwjwdemfe.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.daxiang520.top/gtihrugeis.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ivvv.top/gtqcxnoeba.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.sxryk.cn/gtplpgdyas.html

Go:   defer f.Close()
来源：http://hz.yanxiufei.cn/gtzwosqmfl.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.smart0.xyz/gtixotcybw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.tian-w.cn/gtwnhvmoff.html

================================================================================
来源：http://hz.jianghu66.top/gtidraaijl.html

I. 正则表达式
来源：http://hz.shanyushiyangkeji.top/gtvvdmgtfg.html

================================================================================
来源：http://hz.hfpthk.cn/gtouqmpzky.html

[I01] 判断是否匹配
来源：http://hz.redwolf501.top/gtzqjbdzvr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.smart0.xyz/gtztatvoel.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.snrcjt.cn/gtlkcttgmv.html

JS:   /\d+/.test(s)
来源：http://hz.jinqigfzy.top/gtndimnehj.html

TS:   /\d+/.test(s)
来源：http://hz.guowangkeji.top/gttnxdscax.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zhixingplan.top/gtjhhwwbcu.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.birdmap.top/gtodnflfcc.html

Ruby: s.match?(/\d+/)
来源：http://hz.gzhubu.top/gtpwogxdcq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.gaohongyu789.top/gtccaldyax.html

[I02] 提取所有匹配
来源：http://hz.daria6918.cn/gthyesmaed.html

Py:   re.findall(r"\d+", s)
来源：http://hz.chenjidiqi.icu/gtgxsxbkin.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.iojbl.cn/gtmwzfongu.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.dianchejie.cn/gtiynclogz.html


<!-- 参考信息 -->