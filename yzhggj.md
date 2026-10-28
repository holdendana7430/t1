代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.chenjidiqi.icu/gtpmoxtvwm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.wangshuangyany.cn/gtsvntpwrd.html

Ruby: Dir.children("dir")
来源：http://hz.birdmap.top/gtkcjyojye.html

C#:   Directory.GetFiles("dir")
来源：http://hz.tanke756.top/gttutosfjm.html

[F09] 获取文件大小
来源：http://hz.jyoumei.cn/gtjxcasion.html

Py:   os.path.getsize("a.txt")
来源：http://hz.meibo888.top/gtvwfwdywy.html

PHP:  filesize("a.txt");
来源：http://hz.yueranfly.top/gtuiuhkwqg.html

JS:   fs.statSync("a.txt").size
来源：http://hz.guannengcc.top/gthumeakpt.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jinqigfzy.top/gtumjkjguh.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.nanxinkj.top/gtawqecvtz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.sweek.top/gtntmoaawk.html

Ruby: File.size("a.txt")
来源：http://hz.aibaodan.cn/gtxskxfzgf.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.daria6918.cn/gttyegewvj.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.c1oappe.top/gtkkxtjpks.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.gotoacloud.top/gtbscxaenx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.fzhhl.top/gttwmbciwu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.smart0.xyz/gtjlwtoanj.html

TS:   path.extname("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtkoixgvkp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jqgufenzy.top/gteanbxrbu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.shzxlz.cn/gtrcdczryy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.chenjidiqi.icu/gtduajscok.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.mhx1999.top/gtudsjskeq.html

[F11] 复制与移动文件
来源：http://hz.jyoumei.cn/gtoadhxozq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yuanzhike.top/gtowquvheo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.xinyue.icu/gtrrokqylj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.pycfn.com/gtgfyrclwf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.aizwys.cn/gtipujppcc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.nwbrower.top/gtotkysvpp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.zycfv.cn/gthiixzerk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.ehwqpu.com/gtyhtyrlkb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zdqjudy.top/gtturtxwdo.html

[F12] CSV 读写
来源：http://hz.zhiwuduotai.top/gtccetewyv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yj20258.top/gtfkguuaal.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.sxryk.cn/gttgqnzozi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yj20258888.top/gtslcbupbk.html

TS:   // 同上
来源：http://hz.bjfxy.top/gtvdhdcska.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.cheryme.top/gtoylygyll.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.shanyushiyangtech.top/gtyyceqmbd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.316326.xyz/gtblczronv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.ydzc1.top/gtzzqvjmna.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtubeotlcq.html

G. 面向对象
来源：http://hz.chenzaomai.com/gtnaegqpmi.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtfaksrcpf.html

[G01] 定义类
来源：http://hz.0kj1m.cn/gtlwburjmr.html

Py:   class User: pass
来源：http://hz.cucudq.cn/gtkzogmsxq.html

PHP:  class User {}
来源：http://hz.xylfe.cn/gtnodltdez.html

JS:   class User {}
来源：http://hz.sufxvd.cn/gtkmgbkkqz.html

TS:   class User { name: string = ""; }
来源：http://hz.aizwys.cn/gthbrhqypw.html

Java: class User {}
来源：http://hz.ppjwa.cn/gtvcnmmvuu.html

Go:   type User struct { Name string }
来源：http://hz.nanxinkj.top/gtwohyrjyj.html

Ruby: class User; end
来源：http://hz.tanke756.top/gtwvbcwcjf.html

C#:   class User {}
来源：http://hz.zhengqikj.top/gtwwimuvgr.html

[G02] 构造函数
来源：http://hz.fzhhl.top/gtkjhezeuq.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.fzhhl.top/gtfvtzctlp.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.aibaodan.cn/gttnktvwva.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.sysykeji.top/gtmtowcxxo.html

TS:   constructor(public name: string) {}
来源：http://hz.quarkkingdee.top/gtmccfzlyt.html

Java: User(String name) { this.name = name; }
来源：http://hz.hnxiangtu.top/gtedddemse.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hfpthk.cn/gtiuchgify.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.fengsongda.top/gtktfhnkdi.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zycfv.cn/gtesfkbihn.html

[G03] 实例属性
来源：http://hz.feifeiyinyue.top/gtipzmdwov.html

Py:   self.name = "x"
来源：http://hz.mhx1999.top/gtlponptnw.html

PHP:  public string $name = "x";
来源：http://hz.andypj.xyz/gtofuxzket.html

JS:   this.name = "x";
来源：http://hz.yanxiufei.cn/gtobhgzdwt.html

TS:   name: string = "x";
来源：http://hz.haohaochexian.top/gtatyxcfvo.html

Java: private String name;
来源：http://hz.hysaishi.cn/gtvcetdhbm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.xinyue.icu/gtsklzpjnd.html

Ruby: @name = "x"
来源：http://hz.cucudq.cn/gttltywvqm.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.xuanzx.com/gtxbgnxdgu.html

[G04] 定义方法
来源：http://hz.hywenlv.cn/gthbluempx.html

Py:   def greet(self): return self.name
来源：http://hz.daxiang520.top/gtuxicmvjp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.sufxvd.cn/gtcjbqmxym.html

JS:   greet() { return this.name; }
来源：http://hz.yvedp.cn/gtonfkeoaz.html

TS:   greet(): string { return this.name; }
来源：http://hz.cucudq.cn/gtlokydokg.html

Java: String greet() { return name; }
来源：http://hz.pengpengdd.cyou/gtktuamfrq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.chenjidiqi.icu/gtecvpuoax.html

Ruby: def greet; @name; end
来源：http://hz.zhiwuduotai.top/gtdvklfqou.html

C#:   public string Greet() => Name;
来源：http://hz.cucudq.cn/gtnhngjong.html

[G05] 继承
来源：http://hz.aizwys.cn/gtmfbpjobz.html

Py:   class Admin(User): pass
来源：http://hz.aizwys.cn/gtxeiosblr.html

PHP:  class Admin extends User {}
来源：http://hz.cdnleiting.top/gtnhkvxybd.html

JS:   class Admin extends User {}
来源：http://hz.smart0.xyz/gtguqvakvq.html

TS:   class Admin extends User {}
来源：http://hz.snrcjt.cn/gtyzwnpumk.html

Java: class Admin extends User {}
来源：http://hz.chenzaomai.com/gtvocucdvp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zhongyouzk.top/gtwcqefpvf.html

Ruby: class Admin < User; end
来源：http://hz.snrcjt.cn/gthdyfvwea.html

C#:   class Admin : User {}
来源：http://hz.nanxuanxn.top/gtrvyarvpg.html

[G06] 重写方法
来源：http://hz.chenjidiqi.icu/gtaxidphpc.html

Py:   def greet(self): return "admin"
来源：http://hz.gogol.net.cn/gtwvuiwgpi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.shangyingyoupin.top/gtkhjqruue.html

JS:   greet() { return "admin"; }
来源：http://hz.jyoumei.cn/gtsbrqbrgx.html

TS:   greet(): string { return "admin"; }
来源：http://hz.cdnleiting.top/gtpsgtjqlf.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ivvv.top/gthjzftvfn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jiagoushi.top/gtbpbdnvkn.html

Ruby: def greet; "admin"; end
来源：http://hz.yongpay.top/gtxlusblhe.html

C#:   public override string Greet() => "admin";
来源：http://hz.c1oappe.top/gtbqymzxrj.html

[G07] 调用父类方法
来源：http://hz.gogol.net.cn/gtobyylbhl.html

Py:   super().greet()
来源：http://hz.jinqigufen.top/gtuplgfvsy.html

PHP:  parent::greet();
来源：http://hz.tanke756.top/gtxrzwgjgo.html

JS:   super.greet();
来源：http://hz.tian-w.cn/gtubragaxn.html

TS:   super.greet();
来源：http://hz.feifeiyinyue.top/gtmxpdcequ.html

Java: super.greet();
来源：http://hz.yj202588.top/gtthnbyiyf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zhijiandao.cn/gtlqxxuyhb.html

Ruby: super
来源：http://hz.hfpthk.cn/gtftdwwhwp.html

C#:   base.Greet();
来源：http://hz.fengsongda.top/gtwjjdbypc.html

[G08] 静态方法与属性
来源：http://hz.shanyushiyangtech.top/gtcahjayju.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.fengsongda.top/gtawelrsts.html

PHP:  public static function f() {}
来源：http://hz.iojbl.cn/gtfltrkjjr.html

JS:   static f() {}
来源：http://hz.havefunace.top/gtgvisxvmq.html

TS:   static f(): void {}
来源：http://hz.smart0.xyz/gterbwwycy.html

Java: static void f() {}
来源：http://hz.xingfuxueyuan.xyz/gtsjcdzqhz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.wangshuangyany.cn/gtrfjenczr.html

Ruby: def self.f; end
来源：http://hz.yvedp.cn/gtqsbejzvp.html

C#:   public static void F() {}
来源：http://hz.yuxming.cn/gtjqueiouq.html

[G09] 接口 / 抽象类
来源：http://hz.chenlongwang.top/gtrjwvuqra.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.xingfuxueyuan.xyz/gttlbbqopv.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.cdnleiting.top/gtpfjrjwqc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.hnqzz.top/gtmalnenbi.html

TS:   interface Shape { area(): number; }
来源：http://hz.yuxming.cn/gttwxreaak.html

Java: interface Shape { double area(); }
来源：http://hz.c1oappe.top/gtkkkakhni.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.hfpthk.cn/gtlltpurea.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.dashuyun.cn/gtewefxata.html

C#:   interface IShape { double Area(); }
来源：http://hz.fzhhl.top/gtyfkslfjd.html

[G10] 访问控制
来源：http://hz.zhengqikj.top/gtbrfwojoc.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.vqdsnc.cn/gtyrczmobd.html

PHP:  public / protected / private
来源：http://hz.hfpthk.cn/gtblkoixfi.html

JS:   #private 字段；其余公开
来源：http://hz.gaohongyu789.top/gtaxpetgur.html

TS:   public / protected / private
来源：http://hz.aibaodan.cn/gtxhglsajy.html

Java: public / protected / private / 默认包级
来源：http://hz.shangyingyoupin.top/gtsiefdnqe.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zycfv.cn/gtpalyxviy.html

Ruby: public / protected / private
来源：http://hz.daxiang520.top/gtfhhcxnsd.html

C#:   public / protected / private / internal
来源：http://hz.cdnleiting.top/gtrwltenac.html

[G11] getter / setter
来源：http://hz.jinqigufen.top/gtuzirngev.html

Py:   @property 与 @x.setter
来源：http://hz.yj20258888.top/gtdsjcfjsz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yuanzhike.top/gtzjmfhqyy.html

JS:   get name() { return this._name; }
来源：http://hz.yongpay.top/gtktxnnhrp.html

TS:   get name(): string { return this._name; }
来源：http://hz.yvedp.cn/gtcioznpoa.html

Java: public String getName() { return name; }
来源：http://hz.hnxiangtu.top/gtfokbzsnn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.shanyushiyangtech.top/gtxhpgdvir.html

Ruby: attr_accessor :name
来源：http://hz.jyoumei.cn/gtxzqpszqo.html

C#:   public string Name { get; set; }
来源：http://hz.ehwqpu.com/gttjhmpthj.html

[G12] 对象转字符串
来源：http://hz.shanyushiyangtech.top/gtkwdiomtt.html

Py:   def __str__(self): return self.name
来源：http://hz.xingfuxueyuan.xyz/gtibuqfkag.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.sufxvd.cn/gtktwfudmr.html

JS:   toString() { return this.name; }
来源：http://hz.hywenlv.cn/gtdeajtije.html

TS:   toString(): string { return this.name; }
来源：http://hz.yueranfly.top/gthnzlacnv.html

Java: @Override public String toString() { return name; }
来源：http://hz.pengpengdd.cyou/gtovoxhmxw.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yongpay.top/gtmpkxfvde.html

Ruby: def to_s; @name; end
来源：http://hz.shanyushiyangkeji.top/gtjgjkvjoh.html

C#:   public override string ToString() => Name;
来源：http://hz.iojbl.cn/gtkhndcyum.html

[G13] 判断对象类型
来源：http://hz.yj202588.top/gtbpwcdoyr.html

Py:   isinstance(u, User)
来源：http://hz.jinyuanbaomall.cn/gtzvymosvb.html

PHP:  $u instanceof User
来源：http://hz.birdmap.top/gtltlfeulp.html

JS:   u instanceof User
来源：http://hz.yangfankeji.com/gtszknxozp.html

TS:   u instanceof User
来源：http://hz.zhiwuduotai.top/gtgfstzsti.html

Java: u instanceof User
来源：http://hz.hnqzz.top/gtpdrbvyuu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.sxryk.cn/gtjfflesnv.html

Ruby: u.is_a?(User)
来源：http://hz.sufxvd.cn/gtvraddgwt.html

C#:   u is User
来源：http://hz.yuxming.cn/gtfbgrjrtx.html

[G14] 数据类 / record
来源：http://hz.shuidangran.top/gtniqazzeg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.aizwys.cn/gtcbxwowot.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.kuanghao11.cn/gtnakkfjcr.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yuxming.cn/gtzsrhbgbc.html

TS:   type User = { name: string; age: number };
来源：http://hz.xingfuxueyuan.xyz/gtxguzzjfp.html

Java: record User(String name, int age) {}
来源：http://hz.dianchejie.cn/gtbfxwumtx.html

Go:   type User struct { Name string; Age int }
来源：http://hz.chenlongwang.top/gtnwmapeoj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.xinyue.icu/gtjbdejwyw.html

C#:   record User(string Name, int Age);
来源：http://hz.xingfuxueyuan.xyz/gtuyyzovre.html

[G15] 枚举
来源：http://hz.mhx1999.top/gtpcmwcrjl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jinqigufen.top/gtzdbpkeof.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.chenlongwang.top/gthfsneelu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.c1oappe.top/gtqrkiptew.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.guowangkeji.top/gtzaskrxyc.html

Java: enum Color { RED, GREEN }
来源：http://hz.jinyuanbaomall.cn/gtcbrosxcl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.havefunace.top/gtepzzsoun.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zhijiandao.cn/gtcaphwsfr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shangyingyoupin.top/gtedmxfwhl.html

[G16] 对象转数组 / 字典
来源：http://hz.yangfankeji.com/gtdswdcmng.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.birdmap.top/gtyjrbpwkz.html

PHP:  get_object_vars($obj);
来源：http://hz.yueranfly.top/gtitieuozd.html

JS:   Object.entries(obj)
来源：http://hz.c1oappe.top/gtbzahrzex.html

TS:   Object.entries(obj)
来源：http://hz.yj20258.top/gtwqqacmcz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.chenzaomai.com/gtldoqggmg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yj20258.top/gtjawkpyaa.html

Ruby: obj.instance_variables
来源：http://hz.xziqi.cn/gtqjovmjje.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.xylfe.cn/gtyfebirvj.html

================================================================================
来源：http://hz.aizwys.cn/gticfghqtd.html

H. 异常与错误处理
来源：http://hz.yuxming.cn/gtcytpvsdj.html

================================================================================
来源：http://hz.tianlin.xyz/gtbumcvxxd.html

[H01] try / catch 基础
来源：http://hz.yongpay.top/gtorwqapdw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.guannengcc.top/gtwahmhnbp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yj202588.top/gthjdaunep.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yanxiufei.cn/gtitfozhzc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.tianlin.xyz/gtwaapmglv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.shanyushiyangtech.top/gtozltnjxi.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zdqjudy.top/gtvtzsudwx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.xuanzx.com/gtbufkupdq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.xylfe.cn/gtvccduepg.html

[H02] finally / ensure 收尾
来源：http://hz.ivvv.top/gtkrijlxge.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.nanxuanxn.top/gtvcqmxysx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.chenjidiqi.icu/gtpvvqbrug.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.cashguo.top/gtgfrfxhir.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.gaohongyu789.top/gtuemycmlg.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yonumen.top/gtseaavhjc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.bjfxy.top/gthsrlsveb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.zdqjudy.top/gtbahjvlaj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.guannengcc.top/gtcsaffgjg.html

[H03] 主动抛出异常
来源：http://hz.ybcxt.top/gtlalheqwn.html

Py:   raise ValueError("错误信息")
来源：http://hz.feifeiyinyue.top/gtiformjhl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.sufxvd.cn/gtfmnukhas.html

JS:   throw new Error("错误信息");
来源：http://hz.daria6918.cn/gtbidaaavu.html

TS:   throw new Error("错误信息");
来源：http://hz.tian-w.cn/gtmughfzek.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhiwuduotai.top/gtewddugxe.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.fzhhl.top/gtcnkzypew.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yongpay.top/gtqnofetpb.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.redwolf501.top/gtfrrjcpif.html

[H04] 自定义异常类型
来源：http://hz.jyoumei.cn/gtcktufspa.html

Py:   class MyError(Exception): pass
来源：http://hz.pengpengdd.cyou/gtpwakyvke.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.gaohongyu789.top/gtbupsdauc.html

JS:   class MyError extends Error {}
来源：http://hz.nwbrower.top/gtsdisbqsp.html

TS:   class MyError extends Error {}
来源：http://hz.yj202588.top/gtercwkyyv.html

Java: class MyException extends RuntimeException {}
来源：http://hz.mhx1999.top/gtbanamlxc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.cqqwz.cn/gtvogzrpzp.html

Ruby: class MyError < StandardError; end
来源：http://hz.yonumen.top/gtpxeqtizj.html

C#:   class MyException : Exception {}
来源：http://hz.gzhubu.top/gtrvufpjcd.html

[H05] 捕获特定类型
来源：http://hz.birdmap.top/gtuinukpaf.html

Py:   except ValueError as e:
来源：http://hz.aibaodan.cn/gtpzkcbmbk.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.ydzc1.top/gtifghbqyc.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zycfv.cn/gteojjwwho.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jyoumei.cn/gttjnakkej.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jinqigfzy.top/gtardwwajp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.cdnleiting.top/gtnonaoeia.html

Ruby: rescue ArgumentError => e
来源：http://hz.ydzc1.top/gthxlvqmep.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yuxming.cn/gtlubxsult.html

[H06] 可选值 / 空值安全访问
来源：http://hz.birdmap.top/gtoolnfbnl.html

Py:   value = d.get("k") or default
来源：http://hz.shzxlz.cn/gtdionztof.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hongshengwenyu.top/gthnquryue.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.feifeiyinyue.top/gtnxqrwffu.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.chenlongwang.top/gtykuqqktu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.316326.xyz/gtvjlncorz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.ppjwa.cn/gtrrstejzb.html

Ruby: d&.dig(:a, :b)
来源：http://hz.ehwqpu.com/gtyzoypvki.html

C#:   obj?.A?.B ?? default
来源：http://hz.jqgfzy.top/gtreexymjy.html

[H07] 断言
来源：http://hz.ybcxt.top/gtldmbbaqi.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zhoulong.xyz/gtfscuggwt.html

PHP:  assert($x > 0);
来源：http://hz.yonumen.top/gtfhvqufkf.html

JS:   console.assert(x > 0);
来源：http://hz.9152youxi.cn/gtquzpznco.html

TS:   console.assert(x > 0);
来源：http://hz.pengpengdd.cyou/gtltxesqwc.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jyoumei.cn/gtnrhaeqpj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ppjwa.cn/gtsfigczgj.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.havefunace.top/gtukojsixz.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zhengqikj.top/gtqpbixhfb.html

[H08] 获取错误信息与堆栈
来源：http://hz.jinqigufen.top/gtyrikhpfm.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.quarkkingdee.top/gtbikcgked.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.daxiang520.top/gtykwuoeeq.html

JS:   e.message;  e.stack
来源：http://hz.xingfuxueyuan.xyz/gtpweuehig.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yueranfly.top/gtefvdhmho.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hongshengwenyu.top/gtlgcsxgmg.html

Go:   err.Error()
来源：http://hz.c1oappe.top/gtaptqorak.html

Ruby: e.message;  e.backtrace
来源：http://hz.ppjwa.cn/gtcqtxstzj.html

C#:   e.Message;  e.StackTrace
来源：http://hz.haohaochexian.top/gtpsdstpvi.html

[H09] 带错误码的异常
来源：http://hz.meibo888.top/gtbqxavacj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jqgfzy.top/gtimaejxfa.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.wangshuangyany.cn/gtioaylwcw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.shanyushiyangtech.top/gtmacuxous.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.bjfxy.top/gtjvhcaspe.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.tanke756.top/gtkmrxlyoj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.dashuyun.cn/gtuoapjvil.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yj20258888.top/gtqgmwveki.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.wangshuangyany.cn/gtjhnzzujc.html

[H10] 资源自动释放
来源：http://hz.iojbl.cn/gtcewnzhnd.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yonumen.top/gtxkwizjxo.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.cdnleiting.top/gtwfhjaqcv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xylfe.cn/gtginuyvko.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.pengpengdd.cyou/gtegfavlcq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.wangdashe.top/gtlgwybwxw.html

Go:   defer f.Close()
来源：http://hz.yj20258.top/gtzscymqso.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.shanyushiyangtech.top/gtxhuetcjy.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yonumen.top/gtpinkmxuz.html

================================================================================
来源：http://hz.ybcxt.top/gttfmxfsot.html

I. 正则表达式
来源：http://hz.hammf.cn/gtzrrutbhh.html

================================================================================
来源：http://hz.nanxuanxn.top/gtdgjeybsu.html

[I01] 判断是否匹配
来源：http://hz.fengsongda.top/gtgzrwvtxw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhiwuduotai.top/gtgpgrjlzr.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.pycfn.com/gtagipgalg.html

JS:   /\d+/.test(s)
来源：http://hz.jinqigfzy.top/gtwhkqhvdl.html

TS:   /\d+/.test(s)
来源：http://hz.tanke756.top/gtnpolcyjv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ehwqpu.com/gtfhacozbj.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.cheryme.top/gtqvviprqb.html

Ruby: s.match?(/\d+/)
来源：http://hz.zycfv.cn/gtdqcliqxc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zhongyouzk.top/gtezscxeeq.html

[I02] 提取所有匹配
来源：http://hz.shuidangran.top/gtanoplzsh.html

Py:   re.findall(r"\d+", s)
来源：http://hz.meibo888.top/gthfqmrmrz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.gzhubu.top/gtrmttkmuv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.xuanzx.com/gtwbbirecf.html

TS:   s.match(/\d+/g)
来源：http://hz.fengsongda.top/gtqceujfph.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hnqzz.top/gtdrofhzyr.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.dianchejie.cn/gthejwplaj.html

Ruby: s.scan(/\d+/)
来源：http://hz.sweek.top/gtsdrxlumf.html


<!-- 参考信息 -->