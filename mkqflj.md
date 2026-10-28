代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.nanxinkj.top/gtqaqxszje.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hammf.cn/gtiapczody.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.sufxvd.cn/gtreplyzro.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.shangyingyoupin.top/gtnsleuond.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.daria6918.cn/gtvmzpismb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zhaomingkeji.xyz/gtcjpihqam.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.feifeiyinyue.top/gtnkuaantc.html

[F08] 遍历目录
来源：http://hz.yangfankeji.com/gtvcamgfag.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.gzhubu.top/gtumjufsew.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jinyuanbaomall.cn/gtcrzgwfja.html

JS:   fs.readdirSync("dir")
来源：http://hz.hnxiangtu.top/gtlkgskrkk.html

TS:   fs.readdirSync("dir")
来源：http://hz.redwolf501.top/gteknylzwt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jiagoushi.top/gttrxysejd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.cheryme.top/gtaceyjvlk.html

Ruby: Dir.children("dir")
来源：http://hz.gaohongyu789.top/gtdmjyaavh.html

C#:   Directory.GetFiles("dir")
来源：http://hz.xylfe.cn/gtatfsfgub.html

[F09] 获取文件大小
来源：http://hz.sweek.top/gtxqvguusp.html

Py:   os.path.getsize("a.txt")
来源：http://hz.gzhubu.top/gtmlkmhbby.html

PHP:  filesize("a.txt");
来源：http://hz.jiagoushi.top/gthtjsbwig.html

JS:   fs.statSync("a.txt").size
来源：http://hz.cqqwz.cn/gtcddpvzxn.html

TS:   fs.statSync("a.txt").size
来源：http://hz.ywan-chungtsiang.top/gteopfwyil.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.pycfn.com/gtufalukws.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.birdmap.top/gtkzldpvvd.html

Ruby: File.size("a.txt")
来源：http://hz.wangshuangyany.cn/gttvkorhar.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.hnqzz.top/gtqccpmcdo.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jinqigfzy.top/gtxpqxbzyf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.tanke756.top/gtlznffipo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zhijiandao.cn/gtlsixxeqj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jianghu66.top/gtqiakhihq.html

TS:   path.extname("a.txt")
来源：http://hz.tian-w.cn/gtmtozpszk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.iojbl.cn/gtrniwwbjo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.birdmap.top/gtpdkxijnb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.feifeiyinyue.top/gtcjnfwpfy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.shanyushiyangtech.top/gtnxqebxug.html

[F11] 复制与移动文件
来源：http://hz.pycfn.com/gtvpuuubvq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.nanxuanxn.top/gtcmmmsbxk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.guowangkeji.top/gtlpvedfme.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yuanzhike.top/gtgjtxqpiu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ywan-chungtsiang.top/gtwmkqxsmz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jyoumei.cn/gtxutlfbcl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.pycfn.com/gtoebgxdup.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yuanzhike.top/gtamzlyqvc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.hnqzz.top/gtsilzacfg.html

[F12] CSV 读写
来源：http://hz.cdnleiting.top/gtvoqzqmmd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jqgfzy.top/gttctpkawr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hnqzz.top/gtqwonlztx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.feifeiyinyue.top/gtbdhvilju.html

TS:   // 同上
来源：http://hz.shanyushiyangkeji.top/gtnmbyvajc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.hysaishi.cn/gtspkevelx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.haohaochexian.top/gtbvyovqsh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zhengqikj.top/gtwuhezoux.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.cucudq.cn/gtenwvgotz.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtjpoomili.html

G. 面向对象
来源：http://hz.ydjk.org.cn/gtfkxsvfpq.html

================================================================================
来源：http://hz.birdmap.top/gthklaruaw.html

[G01] 定义类
来源：http://hz.gogol.net.cn/gtfujcidye.html

Py:   class User: pass
来源：http://hz.yonumen.top/gtdzsowgqs.html

PHP:  class User {}
来源：http://hz.jinyuanbaomall.cn/gtxyvndvqs.html

JS:   class User {}
来源：http://hz.snrcjt.cn/gtvochkzlu.html

TS:   class User { name: string = ""; }
来源：http://hz.jlsjyb.cn/gtqthjzaka.html

Java: class User {}
来源：http://hz.yueranfly.top/gtvbfywuai.html

Go:   type User struct { Name string }
来源：http://hz.c1oappe.top/gtxwnytpem.html

Ruby: class User; end
来源：http://hz.zhengqikj.top/gtxltcoyrf.html

C#:   class User {}
来源：http://hz.cheryme.top/gtobhffxbk.html

[G02] 构造函数
来源：http://hz.feifeiyinyue.top/gtbmngleao.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhijiandao.cn/gtzmxgmjmb.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.snrcjt.cn/gtgagfjorn.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jyoumei.cn/gtiwdhawsq.html

TS:   constructor(public name: string) {}
来源：http://hz.smart0.xyz/gtybpjdmsy.html

Java: User(String name) { this.name = name; }
来源：http://hz.ppjwa.cn/gtulpjwuzp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.feifeiyinyue.top/gtzxlrapct.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.52xcode.cn/gtmtvajczv.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jqgufenzy.top/gtibijorcx.html

[G03] 实例属性
来源：http://hz.zhongyouzk.top/gtbgpdkzhv.html

Py:   self.name = "x"
来源：http://hz.xylfe.cn/gtyvvsgvev.html

PHP:  public string $name = "x";
来源：http://hz.xingfuxueyuan.xyz/gtptcgtewk.html

JS:   this.name = "x";
来源：http://hz.cashguo.top/gtvkndpomv.html

TS:   name: string = "x";
来源：http://hz.fzhhl.top/gtnhrjbbbo.html

Java: private String name;
来源：http://hz.cdnleiting.top/gtcivcdhvb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zdqjudy.top/gtgnjfxbjq.html

Ruby: @name = "x"
来源：http://hz.cqqwz.cn/gtltepybfn.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.nanxuanxn.top/gtrzheurlp.html

[G04] 定义方法
来源：http://hz.tian-w.cn/gtdnvtcfem.html

Py:   def greet(self): return self.name
来源：http://hz.fzhhl.top/gtgybxpwsg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yj20258.top/gtnztrmqxe.html

JS:   greet() { return this.name; }
来源：http://hz.shanyushiyangtech.top/gtmaarenvm.html

TS:   greet(): string { return this.name; }
来源：http://hz.cqqwz.cn/gtjpwkweyb.html

Java: String greet() { return name; }
来源：http://hz.ydjk.org.cn/gtobamdnnp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.316326.xyz/gttefhbgme.html

Ruby: def greet; @name; end
来源：http://hz.hongshengwenyu.top/gtxvsetfhk.html

C#:   public string Greet() => Name;
来源：http://hz.yj202588.top/gtoyxoyhiw.html

[G05] 继承
来源：http://hz.redwolf501.top/gtzpcaensu.html

Py:   class Admin(User): pass
来源：http://hz.havefunace.top/gtybeyijqb.html

PHP:  class Admin extends User {}
来源：http://hz.meibo888.top/gtrvvohbxa.html

JS:   class Admin extends User {}
来源：http://hz.shanyushiyangtech.top/gtpunyujkg.html

TS:   class Admin extends User {}
来源：http://hz.yangfankeji.com/gtgfniogox.html

Java: class Admin extends User {}
来源：http://hz.gzhubu.top/gtavgdglza.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.gzhubu.top/gtbqoyunyx.html

Ruby: class Admin < User; end
来源：http://hz.shanyushiyangkeji.top/gtzsnkoxej.html

C#:   class Admin : User {}
来源：http://hz.9152youxi.cn/gteibrutso.html

[G06] 重写方法
来源：http://hz.cdnleiting.top/gtclbhuair.html

Py:   def greet(self): return "admin"
来源：http://hz.hnqzz.top/gtlfytievp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.hammf.cn/gtlcrmhzyc.html

JS:   greet() { return "admin"; }
来源：http://hz.hnqzz.top/gtukehzwnq.html

TS:   greet(): string { return "admin"; }
来源：http://hz.havefunace.top/gtkmugzbpw.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.daxiang520.top/gtmnlvgsoi.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jinqigufen.top/gteyuintcx.html

Ruby: def greet; "admin"; end
来源：http://hz.smart0.xyz/gtjxvqacvx.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhiwuduotai.top/gtcwdsqyel.html

[G07] 调用父类方法
来源：http://hz.9152youxi.cn/gtazksvfry.html

Py:   super().greet()
来源：http://hz.hfpthk.cn/gtlbatqmql.html

PHP:  parent::greet();
来源：http://hz.hywenlv.cn/gtfpsnuuco.html

JS:   super.greet();
来源：http://hz.zhoulong.xyz/gtlsikbqvq.html

TS:   super.greet();
来源：http://hz.shzxlz.cn/gtvdvmqqed.html

Java: super.greet();
来源：http://hz.guowangkeji.top/gtpdmipgok.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.xinyue.icu/gtxsbdfsol.html

Ruby: super
来源：http://hz.cucudq.cn/gtzzcdlejq.html

C#:   base.Greet();
来源：http://hz.yueranfly.top/gtcpzsbwke.html

[G08] 静态方法与属性
来源：http://hz.guannengcc.top/gtfzrjcmkm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.guannengcc.top/gtgiyojeye.html

PHP:  public static function f() {}
来源：http://hz.yongpay.top/gtydbujmdf.html

JS:   static f() {}
来源：http://hz.52xcode.cn/gtvwbfsvot.html

TS:   static f(): void {}
来源：http://hz.kuanghao11.cn/gtgwrhbbzz.html

Java: static void f() {}
来源：http://hz.wangshuangyany.cn/gturuecuff.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhixingplan.top/gtcoovtpdz.html

Ruby: def self.f; end
来源：http://hz.sweek.top/gtszuvsfjk.html

C#:   public static void F() {}
来源：http://hz.aibaodan.cn/gtzdfqifle.html

[G09] 接口 / 抽象类
来源：http://hz.chenjidiqi.icu/gtnzhnznfx.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.smart0.xyz/gtnabproww.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.cashguo.top/gtprukxweb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.daria6918.cn/gtltxwqdwj.html

TS:   interface Shape { area(): number; }
来源：http://hz.fengsongda.top/gtoffqwkxm.html

Java: interface Shape { double area(); }
来源：http://hz.cdnleiting.top/gtfpdfbjvt.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.snrcjt.cn/gtkfrpmtyn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zdqjudy.top/gtmhsbwkmy.html

C#:   interface IShape { double Area(); }
来源：http://hz.tanke756.top/gtjwoqgfir.html

[G10] 访问控制
来源：http://hz.jqgfzy.top/gtdhtnwjvb.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.ywan-chungtsiang.top/gtlchxnuwx.html

PHP:  public / protected / private
来源：http://hz.snrcjt.cn/gtaxlnbjmd.html

JS:   #private 字段；其余公开
来源：http://hz.guannengcc.top/gtyktjmibb.html

TS:   public / protected / private
来源：http://hz.gogol.net.cn/gttgrxzavl.html

Java: public / protected / private / 默认包级
来源：http://hz.tanke756.top/gtlquooozi.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.xinyue.icu/gtuyvoytcy.html

Ruby: public / protected / private
来源：http://hz.wangdashe.top/gttjegtaww.html

C#:   public / protected / private / internal
来源：http://hz.havefunace.top/gtmfruuosl.html

[G11] getter / setter
来源：http://hz.yuxming.cn/gtvqdxqost.html

Py:   @property 与 @x.setter
来源：http://hz.yuxming.cn/gtnswmherx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.xuanzx.com/gtpegvpnbn.html

JS:   get name() { return this._name; }
来源：http://hz.gogol.net.cn/gtcqqadiqs.html

TS:   get name(): string { return this._name; }
来源：http://hz.zycfv.cn/gtbayrppyf.html

Java: public String getName() { return name; }
来源：http://hz.sufxvd.cn/gtqucquuyb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.hfpthk.cn/gtlqyuyfct.html

Ruby: attr_accessor :name
来源：http://hz.aizwys.cn/gtusrddpie.html

C#:   public string Name { get; set; }
来源：http://hz.yj202588.top/gtxosexbpg.html

[G12] 对象转字符串
来源：http://hz.aizwys.cn/gtzknbekdh.html

Py:   def __str__(self): return self.name
来源：http://hz.fengsongda.top/gttriwyqax.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ybcxt.top/gtkrjilxbg.html

JS:   toString() { return this.name; }
来源：http://hz.shuidangran.top/gtdfhjhvdv.html

TS:   toString(): string { return this.name; }
来源：http://hz.316326.xyz/gtqcisybpv.html

Java: @Override public String toString() { return name; }
来源：http://hz.sufxvd.cn/gtrnxdzajs.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhaomingkeji.xyz/gtggdxenva.html

Ruby: def to_s; @name; end
来源：http://hz.hnqzz.top/gtdfyrptio.html

C#:   public override string ToString() => Name;
来源：http://hz.ywan-chungtsiang.top/gtdltzedhk.html

[G13] 判断对象类型
来源：http://hz.gaohongyu789.top/gtixxgbqqw.html

Py:   isinstance(u, User)
来源：http://hz.tanke756.top/gtglffoctk.html

PHP:  $u instanceof User
来源：http://hz.mhx1999.top/gtzlzfwejf.html

JS:   u instanceof User
来源：http://hz.cucudq.cn/gtexcwzmau.html

TS:   u instanceof User
来源：http://hz.yangfankeji.com/gtmxjvblqm.html

Java: u instanceof User
来源：http://hz.cqqwz.cn/gtljxlytyp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jyoumei.cn/gtqtskilor.html

Ruby: u.is_a?(User)
来源：http://hz.jinyuanbaomall.cn/gtbfcpmuhp.html

C#:   u is User
来源：http://hz.bjfxy.top/gtdxemxjno.html

[G14] 数据类 / record
来源：http://hz.ppjwa.cn/gtomufgced.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.hnqzz.top/gtessnajtc.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yueranfly.top/gtmhsrvumo.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.fengsongda.top/gtbrtzgvnu.html

TS:   type User = { name: string; age: number };
来源：http://hz.xinyue.icu/gtprvcfsxh.html

Java: record User(String name, int age) {}
来源：http://hz.birdmap.top/gtsfsplgok.html

Go:   type User struct { Name string; Age int }
来源：http://hz.xylfe.cn/gtkoqqyijc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yongpay.top/gtpyhsfyif.html

C#:   record User(string Name, int Age);
来源：http://hz.snrcjt.cn/gtyepjsidp.html

[G15] 枚举
来源：http://hz.cucudq.cn/gtfptmwqdr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zhoulong.xyz/gtvrtafgka.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.xuetiantiany.cn/gtiywttjrg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.aibaodan.cn/gtftqrkgqy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.havefunace.top/gtkpfpgzxl.html

Java: enum Color { RED, GREEN }
来源：http://hz.mhx1999.top/gtfegmtrjc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yuxming.cn/gtoyufpewz.html

Ruby: Color = %i[red green].freeze
来源：http://hz.dashuyun.cn/gtyokmjmjf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cucudq.cn/gtvzjlnqis.html

[G16] 对象转数组 / 字典
来源：http://hz.sweek.top/gtihfdisxc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.hammf.cn/gtyznxxizv.html

PHP:  get_object_vars($obj);
来源：http://hz.jqgfzy.top/gtyujfykse.html

JS:   Object.entries(obj)
来源：http://hz.shzxlz.cn/gtfnszwtkq.html

TS:   Object.entries(obj)
来源：http://hz.52xcode.cn/gthklrbsrk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.vqdsnc.cn/gtavhghxlm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.chenjidiqi.icu/gtpbchqing.html

Ruby: obj.instance_variables
来源：http://hz.dianchejie.cn/gtbqoznduh.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.chenzaomai.com/gtmcznfves.html

================================================================================
来源：http://hz.daria6918.cn/gtztexivko.html

H. 异常与错误处理
来源：http://hz.cdnleiting.top/gtekvfmrmn.html

================================================================================
来源：http://hz.hysaishi.cn/gtkwglemzl.html

[H01] try / catch 基础
来源：http://hz.jinyuanbaomall.cn/gthortvxbe.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.cqqwz.cn/gtlqbvwrdg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.guowangkeji.top/gtxfctmgbd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.gotoacloud.top/gtdeaypzvf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.wangshuangyany.cn/gtmbyxbltb.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ydjk.org.cn/gtteabbntd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jinqigfzy.top/gtabwgetuy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.wangdashe.top/gtetufpmvs.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jqgfzy.top/gtolidwpvq.html

[H02] finally / ensure 收尾
来源：http://hz.yj20258888.top/gterrocvkd.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.dashuyun.cn/gtzadmfkwu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jinqigufen.top/gtcwetitvk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hysaishi.cn/gtjzniafkj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.hysaishi.cn/gtwpnqebyv.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.haohaochexian.top/gtyfrpgvcu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.mhx1999.top/gtofdthabn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.zhoulong.xyz/gtgpkwkavo.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zhengqikj.top/gtcpfejaoe.html

[H03] 主动抛出异常
来源：http://hz.bjfxy.top/gtodsyvpfr.html

Py:   raise ValueError("错误信息")
来源：http://hz.wangshuangyany.cn/gtjgtayavm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.shangyingyoupin.top/gtawytxpvo.html

JS:   throw new Error("错误信息");
来源：http://hz.cheryme.top/gtdeqbhthi.html

TS:   throw new Error("错误信息");
来源：http://hz.wangdashe.top/gtwcjjwidn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.guowangkeji.top/gtsizsakcw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.gzhubu.top/gtddupzrea.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.guowangkeji.top/gtwuwcsllk.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.shanyushiyangtech.top/gtjbohujwv.html

[H04] 自定义异常类型
来源：http://hz.pengpengdd.cyou/gtynnlzefh.html

Py:   class MyError(Exception): pass
来源：http://hz.jqgfzy.top/gthbabxucr.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.andypj.xyz/gtsyudkeyo.html

JS:   class MyError extends Error {}
来源：http://hz.cdnleiting.top/gtwhwntcmd.html

TS:   class MyError extends Error {}
来源：http://hz.zhengqikj.top/gtzgwoiqob.html

Java: class MyException extends RuntimeException {}
来源：http://hz.daria6918.cn/gtfuakaezw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.haohaochexian.top/gteaabpgkn.html

Ruby: class MyError < StandardError; end
来源：http://hz.ehwqpu.com/gtmhgbotcr.html

C#:   class MyException : Exception {}
来源：http://hz.yuxming.cn/gtarvquppa.html

[H05] 捕获特定类型
来源：http://hz.52xcode.cn/gtmdjemqfc.html

Py:   except ValueError as e:
来源：http://hz.ywan-chungtsiang.top/gtabmkeiem.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.aibaodan.cn/gtbsejbdve.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.aizwys.cn/gtcwkflwpz.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.fzhhl.top/gtjpatmcrs.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.9152youxi.cn/gtjxsxznsi.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zhengqikj.top/gtsgzjbzme.html

Ruby: rescue ArgumentError => e
来源：http://hz.aizwys.cn/gteeikzmta.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jianghu66.top/gtgrcsjgyc.html

[H06] 可选值 / 空值安全访问
来源：http://hz.aibaodan.cn/gtlxillulk.html

Py:   value = d.get("k") or default
来源：http://hz.xziqi.cn/gtkijnakef.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.redwolf501.top/gthditgudh.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.fzhhl.top/gtrdrgjbih.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.cqqwz.cn/gtkyibidsz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.sysykeji.top/gthiwmmslc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.sxryk.cn/gtpmmeekil.html

Ruby: d&.dig(:a, :b)
来源：http://hz.hongshengwenyu.top/gtbrzucfyx.html

C#:   obj?.A?.B ?? default
来源：http://hz.jianghu66.top/gtmifvjjrv.html

[H07] 断言
来源：http://hz.zycfv.cn/gtoqoejwpb.html

Py:   assert x > 0, "必须为正"
来源：http://hz.ydzc1.top/gtnbgqejju.html

PHP:  assert($x > 0);
来源：http://hz.zhixingplan.top/gtctaeimhh.html

JS:   console.assert(x > 0);
来源：http://hz.jinqigfzy.top/gtpqdxezjw.html

TS:   console.assert(x > 0);
来源：http://hz.hammf.cn/gtympzmscf.html

Java: assert x > 0 : "必须为正";
来源：http://hz.fengsongda.top/gtojbchtlc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.nwbrower.top/gtimsdadps.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.c1oappe.top/gtuzxcvasj.html

C#:   Debug.Assert(x > 0);
来源：http://hz.feifeiyinyue.top/gtmeqdhnfx.html

[H08] 获取错误信息与堆栈
来源：http://hz.dashuyun.cn/gtbgvzdnbb.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.gotoacloud.top/gtusdtedma.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.ivvv.top/gtbrvrrvww.html

JS:   e.message;  e.stack
来源：http://hz.sxryk.cn/gtzfkxlxrf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.nwbrower.top/gtsfcdnrbi.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.xuetiantiany.cn/gttxqdjiss.html

Go:   err.Error()
来源：http://hz.yongpay.top/gttwvgdgjs.html

Ruby: e.message;  e.backtrace
来源：http://hz.chenlongwang.top/gtneooverw.html

C#:   e.Message;  e.StackTrace
来源：http://hz.gotoacloud.top/gthwlnqqbz.html

[H09] 带错误码的异常
来源：http://hz.redwolf501.top/gtpsqwaxks.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jiagoushi.top/gtiaphmehe.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.cucudq.cn/gtdmmokcpg.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.andypj.xyz/gtnqrevhsn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jinyuanbaomall.cn/gtefgaeypr.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.xylfe.cn/gtdittquwb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.tianlin.xyz/gtpnmbiewj.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.quarkkingdee.top/gtsvvlssod.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.pycfn.com/gtnrcqkbve.html

[H10] 资源自动释放
来源：http://hz.chenzaomai.com/gtnfiqwwht.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.hysaishi.cn/gtfxzytjxn.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.hnxiangtu.top/gtltmxsxmd.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.aibaodan.cn/gtehoemoif.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.fzhhl.top/gtpbojqdkc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.aibaodan.cn/gtofgzbivj.html

Go:   defer f.Close()
来源：http://hz.gogol.net.cn/gthzdqjipf.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.vqdsnc.cn/gtvlyzqxiy.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yvedp.cn/gttylmlmwz.html

================================================================================
来源：http://hz.52xcode.cn/gtypuoejdm.html

I. 正则表达式
来源：http://hz.zhoulong.xyz/gtfmnhhwhy.html

================================================================================
来源：http://hz.ivvv.top/gtxrdxdudd.html

[I01] 判断是否匹配
来源：http://hz.jianghu66.top/gttzheeulo.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.sxryk.cn/gtrceggdgu.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yvedp.cn/gteqhrnnpv.html

JS:   /\d+/.test(s)
来源：http://hz.yuanzhike.top/gttosegyyw.html

TS:   /\d+/.test(s)
来源：http://hz.xylfe.cn/gtpsbfvleh.html


<!-- 参考信息 -->