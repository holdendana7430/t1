代发 wailian999

Ruby: File.delete("a.txt")
来源：http://hz.hywenlv.cn/gtjicdlaze.html

C#:   File.Delete("a.txt");
来源：http://hz.ydzc1.top/gtqeuljmlt.html

[F07] 创建目录（含多级）
来源：http://hz.yuanzhike.top/gtqaunzoou.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.birdmap.top/gtcwnavtun.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zhiwuduotai.top/gttlcxjcnv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.svipenyu.cn/gtpocpresk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hammf.cn/gtwrsdcvwj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.chenjidiqi.icu/gtokdauybo.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.tian-w.cn/gtjnzamldw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.ywan-chungtsiang.top/gtlsliasns.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.tanke756.top/gtaodovjhw.html

[F08] 遍历目录
来源：http://hz.chenjidiqi.icu/gtmqswpatt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.kuanghao11.cn/gtwdqbqzgc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.cheryme.top/gtjmtzvzyj.html

JS:   fs.readdirSync("dir")
来源：http://hz.guannengcc.top/gtruqqlyry.html

TS:   fs.readdirSync("dir")
来源：http://hz.aibaodan.cn/gtumthfveg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.9152youxi.cn/gtniikuhex.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.chenjidiqi.icu/gtxepmflko.html

Ruby: Dir.children("dir")
来源：http://hz.pycfn.com/gtzsandiwd.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jinyuanbaomall.cn/gtoktgbgoc.html

[F09] 获取文件大小
来源：http://hz.tian-w.cn/gticcneqkg.html

Py:   os.path.getsize("a.txt")
来源：http://hz.cashguo.top/gteklhwoez.html

PHP:  filesize("a.txt");
来源：http://hz.iojbl.cn/gttwvupugf.html

JS:   fs.statSync("a.txt").size
来源：http://hz.meibo888.top/gtqxtpmqvg.html

TS:   fs.statSync("a.txt").size
来源：http://hz.havefunace.top/gtgjlipfva.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zycfv.cn/gtclgemjvo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zycfv.cn/gterseaphn.html

Ruby: File.size("a.txt")
来源：http://hz.hysaishi.cn/gtuikirvra.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.316326.xyz/gtaustrjlt.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yuanzhike.top/gtovwpgcdb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.hysaishi.cn/gtvuobvrgl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.daxiang520.top/gtssxrjthd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.ehwqpu.com/gtfaqzdkkq.html

TS:   path.extname("a.txt")
来源：http://hz.cheryme.top/gttljijlye.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhongyouzk.top/gtsolkfnpr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zhongyouzk.top/gtalxpeogz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.kuanghao11.cn/gturudmrwd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.cdnleiting.top/gthwmepupu.html

[F11] 复制与移动文件
来源：http://hz.tianlin.xyz/gtmnqtppxg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.hfpthk.cn/gtgxeiroaw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.ywan-chungtsiang.top/gtbqcunfjz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ybcxt.top/gtrngekcie.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.snrcjt.cn/gtmgwfresq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.gogol.net.cn/gttdfgknen.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.bjfxy.top/gthvleqvnn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.pengpengdd.cyou/gtigsmyjwg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yj202588.top/gtchejxpvf.html

[F12] CSV 读写
来源：http://hz.guannengcc.top/gtnhefqurs.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.chenzaomai.com/gtkdpodmna.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.ydjk.org.cn/gtqleyegdo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yj20258888.top/gtxovfpmky.html

TS:   // 同上
来源：http://hz.jinghuilouyu.cn/gtabvpeyjq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.52xcode.cn/gtvqxsugut.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.pengpengdd.cyou/gteuzlztzm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.shanyushiyangtech.top/gtqroeilmv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.chenzaomai.com/gtelwtmpze.html

================================================================================
来源：http://hz.zhongyouzk.top/gtpxebsemk.html

G. 面向对象
来源：http://hz.guowangkeji.top/gtrzvnyufu.html

================================================================================
来源：http://hz.chenlongwang.top/gtqgnqrgyx.html

[G01] 定义类
来源：http://hz.jinyuanbaomall.cn/gtdhybkaft.html

Py:   class User: pass
来源：http://hz.jyoumei.cn/gtkbrjkrbr.html

PHP:  class User {}
来源：http://hz.c1oappe.top/gtrzsfpuwn.html

JS:   class User {}
来源：http://hz.zhaomingkeji.xyz/gtugsqucwq.html

TS:   class User { name: string = ""; }
来源：http://hz.jianghu66.top/gtvmlbyzrx.html

Java: class User {}
来源：http://hz.c1oappe.top/gthghzuhjt.html

Go:   type User struct { Name string }
来源：http://hz.fzhhl.top/gtvoqwlvgv.html

Ruby: class User; end
来源：http://hz.0kj1m.cn/gtpiwgndms.html

C#:   class User {}
来源：http://hz.daxiang520.top/gtqhyqrgqg.html

[G02] 构造函数
来源：http://hz.gogol.net.cn/gtwecoreiy.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.gogol.net.cn/gtngudwyur.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.pycfn.com/gttmnosypa.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.shanyushiyangtech.top/gtyjzwjzok.html

TS:   constructor(public name: string) {}
来源：http://hz.jinqigfzy.top/gtmhswinbh.html

Java: User(String name) { this.name = name; }
来源：http://hz.xziqi.cn/gtavkqmrdh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.cdnleiting.top/gtmjdiamkh.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.hywenlv.cn/gtivbgoyyz.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jqgufenzy.top/gtzphatqqy.html

[G03] 实例属性
来源：http://hz.feifeiyinyue.top/gtdbxyxjrk.html

Py:   self.name = "x"
来源：http://hz.svipenyu.cn/gtzsrueovm.html

PHP:  public string $name = "x";
来源：http://hz.xinyue.icu/gtrngcdbuz.html

JS:   this.name = "x";
来源：http://hz.jinghuilouyu.cn/gtygpznlxt.html

TS:   name: string = "x";
来源：http://hz.quarkkingdee.top/gtnyshryhc.html

Java: private String name;
来源：http://hz.zycfv.cn/gtcrwnotvg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yuxming.cn/gtgdhtvotg.html

Ruby: @name = "x"
来源：http://hz.ppjwa.cn/gtxgwjgxmt.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yanxiufei.cn/gteewtybvf.html

[G04] 定义方法
来源：http://hz.birdmap.top/gtfiyeddqq.html

Py:   def greet(self): return self.name
来源：http://hz.guowangkeji.top/gtjhnranwh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jqgufenzy.top/gtrkfytolc.html

JS:   greet() { return this.name; }
来源：http://hz.nwbrower.top/gtbimodsab.html

TS:   greet(): string { return this.name; }
来源：http://hz.ivvv.top/gthxsiohkk.html

Java: String greet() { return name; }
来源：http://hz.9152youxi.cn/gtqyshmoxn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.feifeiyinyue.top/gtukfhabft.html

Ruby: def greet; @name; end
来源：http://hz.mhx1999.top/gtjmgrpdrp.html

C#:   public string Greet() => Name;
来源：http://hz.xylfe.cn/gtdbnxxxsl.html

[G05] 继承
来源：http://hz.cucudq.cn/gtycnclhem.html

Py:   class Admin(User): pass
来源：http://hz.zhongyouzk.top/gtfkjkgldm.html

PHP:  class Admin extends User {}
来源：http://hz.hfpthk.cn/gtispavtod.html

JS:   class Admin extends User {}
来源：http://hz.ehwqpu.com/gtklztmmiw.html

TS:   class Admin extends User {}
来源：http://hz.yj20258888.top/gtmjtsidey.html

Java: class Admin extends User {}
来源：http://hz.yueranfly.top/gtbevihici.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yuanzhike.top/gthxpoeovr.html

Ruby: class Admin < User; end
来源：http://hz.fengsongda.top/gtmscicfvu.html

C#:   class Admin : User {}
来源：http://hz.cqqwz.cn/gtjqjfgnwh.html

[G06] 重写方法
来源：http://hz.hnqzz.top/gtnglzodlf.html

Py:   def greet(self): return "admin"
来源：http://hz.jqgufenzy.top/gthwcvoeev.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.vqdsnc.cn/gtgvvtxqjk.html

JS:   greet() { return "admin"; }
来源：http://hz.gogol.net.cn/gthgcioqcq.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jinghuilouyu.cn/gtqgkthime.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.pycfn.com/gtlnsujasz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.ywan-chungtsiang.top/gtmzxnyjtw.html

Ruby: def greet; "admin"; end
来源：http://hz.pengpengdd.cyou/gtlmfqipto.html

C#:   public override string Greet() => "admin";
来源：http://hz.chenlongwang.top/gtfvvzuatw.html

[G07] 调用父类方法
来源：http://hz.xuanzx.com/gtrssmbgak.html

Py:   super().greet()
来源：http://hz.hfpthk.cn/gttiiiwiog.html

PHP:  parent::greet();
来源：http://hz.zhixingplan.top/gtxnrmvpra.html

JS:   super.greet();
来源：http://hz.yvedp.cn/gtlzxddvwt.html

TS:   super.greet();
来源：http://hz.daria6918.cn/gtobxunrlh.html

Java: super.greet();
来源：http://hz.yanxiufei.cn/gtseewiiwz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.sxryk.cn/gtnpkehymf.html

Ruby: super
来源：http://hz.nwbrower.top/gtgtmhirzq.html

C#:   base.Greet();
来源：http://hz.aibaodan.cn/gtpvwwrylh.html

[G08] 静态方法与属性
来源：http://hz.ivvv.top/gtgsmuwsie.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yanxiufei.cn/gtgzuqbjnj.html

PHP:  public static function f() {}
来源：http://hz.chenzaomai.com/gtbfdlmczr.html

JS:   static f() {}
来源：http://hz.guowangkeji.top/gtymapxsej.html

TS:   static f(): void {}
来源：http://hz.yj202588.top/gttqdnrdgh.html

Java: static void f() {}
来源：http://hz.nanxinkj.top/gtumdkfbrh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.daxiang520.top/gtpdblsxpq.html

Ruby: def self.f; end
来源：http://hz.bjfxy.top/gtqqrqqqot.html

C#:   public static void F() {}
来源：http://hz.xylfe.cn/gtqvgaaubw.html

[G09] 接口 / 抽象类
来源：http://hz.316326.xyz/gthhoopwcc.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yj20258888.top/gtgbkfkejt.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.pycfn.com/gtxpmiaugs.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.dashuyun.cn/gtmsqaotdp.html

TS:   interface Shape { area(): number; }
来源：http://hz.yongpay.top/gtitsvcuel.html

Java: interface Shape { double area(); }
来源：http://hz.c1oappe.top/gtccpqlsrq.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.redwolf501.top/gthwbebemg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.316326.xyz/gthztylzca.html

C#:   interface IShape { double Area(); }
来源：http://hz.shangyingyoupin.top/gtdfbqxmpq.html

[G10] 访问控制
来源：http://hz.nanxuanxn.top/gtmlgtbphf.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.daxiang520.top/gtwwtthquq.html

PHP:  public / protected / private
来源：http://hz.316326.xyz/gtejacmcwv.html

JS:   #private 字段；其余公开
来源：http://hz.sysykeji.top/gtuqtlcyta.html

TS:   public / protected / private
来源：http://hz.havefunace.top/gtehpgcgzl.html

Java: public / protected / private / 默认包级
来源：http://hz.zhengqikj.top/gtpbjkyusy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jlsjyb.cn/gtxzcgtqqx.html

Ruby: public / protected / private
来源：http://hz.ydzc1.top/gtsnwwcbpr.html

C#:   public / protected / private / internal
来源：http://hz.wangdashe.top/gthobblhjw.html

[G11] getter / setter
来源：http://hz.kuanghao11.cn/gtthpbosch.html

Py:   @property 与 @x.setter
来源：http://hz.bjfxy.top/gtlywelsxw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jyoumei.cn/gtvcushhoe.html

JS:   get name() { return this._name; }
来源：http://hz.jianghu66.top/gttdxleqap.html

TS:   get name(): string { return this._name; }
来源：http://hz.cheryme.top/gttmgvukxg.html

Java: public String getName() { return name; }
来源：http://hz.ywan-chungtsiang.top/gtykjvyrjk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.birdmap.top/gtjluljwjj.html

Ruby: attr_accessor :name
来源：http://hz.kuanghao11.cn/gtfksdysul.html

C#:   public string Name { get; set; }
来源：http://hz.yj20258.top/gtomziixim.html

[G12] 对象转字符串
来源：http://hz.jinyuanbaomall.cn/gturexemax.html

Py:   def __str__(self): return self.name
来源：http://hz.jinqigufen.top/gtimrebdux.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.wangdashe.top/gtczzawaxw.html

JS:   toString() { return this.name; }
来源：http://hz.ppjwa.cn/gtgbhtpzzt.html

TS:   toString(): string { return this.name; }
来源：http://hz.chenjidiqi.icu/gtzfxutoho.html

Java: @Override public String toString() { return name; }
来源：http://hz.yj20258888.top/gtdnezvfql.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhengqikj.top/gtxwygqqmf.html

Ruby: def to_s; @name; end
来源：http://hz.316326.xyz/gtlovderxz.html

C#:   public override string ToString() => Name;
来源：http://hz.snrcjt.cn/gtyitotnju.html

[G13] 判断对象类型
来源：http://hz.jyoumei.cn/gtclcayscl.html

Py:   isinstance(u, User)
来源：http://hz.redwolf501.top/gtmelywyav.html

PHP:  $u instanceof User
来源：http://hz.havefunace.top/gttdhljtwq.html

JS:   u instanceof User
来源：http://hz.gzhubu.top/gtqyhjdouv.html

TS:   u instanceof User
来源：http://hz.iojbl.cn/gtcrnwuive.html

Java: u instanceof User
来源：http://hz.xuetiantiany.cn/gtnlcvptrf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jinqigfzy.top/gticpvvqjh.html

Ruby: u.is_a?(User)
来源：http://hz.0kj1m.cn/gtajsakzvs.html

C#:   u is User
来源：http://hz.shanyushiyangkeji.top/gtwgjcaupw.html

[G14] 数据类 / record
来源：http://hz.guannengcc.top/gtlnjdtvso.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.sysykeji.top/gtlfmtzrum.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.ydzc1.top/gtzcfwhjex.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhiwuduotai.top/gtmndaikox.html

TS:   type User = { name: string; age: number };
来源：http://hz.jinqigufen.top/gtlxefhbql.html

Java: record User(String name, int age) {}
来源：http://hz.guowangkeji.top/gtpyjpwjlu.html

Go:   type User struct { Name string; Age int }
来源：http://hz.cqqwz.cn/gtjtonxgnl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jinqigfzy.top/gtufyoxvte.html

C#:   record User(string Name, int Age);
来源：http://hz.gaohongyu789.top/gtcgbqbdzk.html

[G15] 枚举
来源：http://hz.gogol.net.cn/gtvkcclttn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.ppjwa.cn/gtdfhlngzh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.cashguo.top/gtppwqlsxi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jqgufenzy.top/gtxdwuphtd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.mhx1999.top/gtpppadaxf.html

Java: enum Color { RED, GREEN }
来源：http://hz.yj202588.top/gtxvgabtpm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.guannengcc.top/gtkpjxfudh.html

Ruby: Color = %i[red green].freeze
来源：http://hz.feifeiyinyue.top/gtftvvperw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.dianchejie.cn/gtpkydpmck.html

[G16] 对象转数组 / 字典
来源：http://hz.shangyingyoupin.top/gtdxiglcrm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jyoumei.cn/gtqhslrtmo.html

PHP:  get_object_vars($obj);
来源：http://hz.hysaishi.cn/gtkeltcmyn.html

JS:   Object.entries(obj)
来源：http://hz.xingfuxueyuan.xyz/gtmoxgmggm.html

TS:   Object.entries(obj)
来源：http://hz.guowangkeji.top/gtqihdkryx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhoulong.xyz/gtgdxurspi.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yueranfly.top/gtwhbmtzfs.html

Ruby: obj.instance_variables
来源：http://hz.aizwys.cn/gtooavvvji.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yueranfly.top/gtpyxoxsrl.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtsxdmioxp.html

H. 异常与错误处理
来源：http://hz.cqqwz.cn/gtwuqicsiw.html

================================================================================
来源：http://hz.hfpthk.cn/gtstsysolh.html

[H01] try / catch 基础
来源：http://hz.ybcxt.top/gtpoulqctg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.gotoacloud.top/gtypvogpfz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yanxiufei.cn/gtfttmsmnd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jinghuilouyu.cn/gtoqxjgdci.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.iojbl.cn/gtuaxamyva.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.9152youxi.cn/gtcqcvmhys.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.nanxinkj.top/gtuxphoten.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jinghuilouyu.cn/gtsdrptfad.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.mhx1999.top/gtjzuqbpjp.html

[H02] finally / ensure 收尾
来源：http://hz.fengsongda.top/gtgjclcmur.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yonumen.top/gtbtackjbl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.gaohongyu789.top/gtnwwhzjpv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.tianlin.xyz/gtmwotrvdm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhiwuduotai.top/gtlmmdcawe.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhengqikj.top/gtcihvqcdq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zhongyouzk.top/gtfikowmcv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.zhaomingkeji.xyz/gtqmlvjqda.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.xingfuxueyuan.xyz/gtpopuvsln.html

[H03] 主动抛出异常
来源：http://hz.shanyushiyangkeji.top/gtxzsbahvi.html

Py:   raise ValueError("错误信息")
来源：http://hz.jinghuilouyu.cn/gtcssctfes.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.wangshuangyany.cn/gtefjsypiy.html

JS:   throw new Error("错误信息");
来源：http://hz.jianghu66.top/gtsojxmokb.html

TS:   throw new Error("错误信息");
来源：http://hz.zdqjudy.top/gtyqlzhqzj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhongyouzk.top/gtdhbaaohn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yanxiufei.cn/gtgexcdcub.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.cqqwz.cn/gtnwpucruh.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.0kj1m.cn/gtkmbyzwkd.html

[H04] 自定义异常类型
来源：http://hz.hammf.cn/gthrxvzrqd.html

Py:   class MyError(Exception): pass
来源：http://hz.chenjidiqi.icu/gtjytecvas.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jqgfzy.top/gtqmxqzoqh.html

JS:   class MyError extends Error {}
来源：http://hz.sxryk.cn/gtvojjtuao.html

TS:   class MyError extends Error {}
来源：http://hz.meibo888.top/gtvrfuoxud.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jyoumei.cn/gtlorwyqvw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.cashguo.top/gtnslirbkn.html

Ruby: class MyError < StandardError; end
来源：http://hz.hnqzz.top/gtsucpzfjw.html

C#:   class MyException : Exception {}
来源：http://hz.ivvv.top/gtritpjmer.html

[H05] 捕获特定类型
来源：http://hz.guowangkeji.top/gtmqlsxzgi.html

Py:   except ValueError as e:
来源：http://hz.daria6918.cn/gteevwggon.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.52xcode.cn/gttpueulrl.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yuxming.cn/gtvfvnkwdc.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.c1oappe.top/gtfgzdoiyw.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.dashuyun.cn/gtlhhqiida.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yangfankeji.com/gtzhfuevhl.html

Ruby: rescue ArgumentError => e
来源：http://hz.xziqi.cn/gtxcfypxyq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.ppjwa.cn/gthrpnyxsf.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yangfankeji.com/gtiujurbih.html

Py:   value = d.get("k") or default
来源：http://hz.redwolf501.top/gtykqbukqe.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.sweek.top/gtkniwwsnz.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.shanyushiyangtech.top/gtqfglibev.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jiagoushi.top/gtzkgajnqo.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.shangyingyoupin.top/gtgnqfmftc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.aibaodan.cn/gtbhlxcuez.html

Ruby: d&.dig(:a, :b)
来源：http://hz.chenjidiqi.icu/gtmtpraatz.html

C#:   obj?.A?.B ?? default
来源：http://hz.meibo888.top/gtrvyvjndf.html

[H07] 断言
来源：http://hz.aibaodan.cn/gtzgrnucry.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yj20258.top/gtfxvpbpfp.html

PHP:  assert($x > 0);
来源：http://hz.wangdashe.top/gtlcgquvgj.html

JS:   console.assert(x > 0);
来源：http://hz.cdnleiting.top/gtfffromvh.html

TS:   console.assert(x > 0);
来源：http://hz.redwolf501.top/gttqonjjut.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jianghu66.top/gttlckrwhr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.quarkkingdee.top/gtmmqrmfif.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.haohaochexian.top/gtqmsccktm.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zhiwuduotai.top/gtzevuspbi.html

[H08] 获取错误信息与堆栈
来源：http://hz.feifeiyinyue.top/gtalgrzdvs.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.pycfn.com/gtdtvkmtna.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.aibaodan.cn/gtmqlkiidg.html

JS:   e.message;  e.stack
来源：http://hz.cashguo.top/gtuxlnaldg.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.gotoacloud.top/gtdewgwvdf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.mhx1999.top/gtuqufkuoz.html

Go:   err.Error()
来源：http://hz.nanxinkj.top/gtqkrgpzdf.html

Ruby: e.message;  e.backtrace
来源：http://hz.tianlin.xyz/gtvybspkiy.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhixingplan.top/gtlthydcgh.html

[H09] 带错误码的异常
来源：http://hz.0kj1m.cn/gtkudqlvtc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.wangshuangyany.cn/gtgmjgvyhr.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jinyuanbaomall.cn/gtkzvzwwip.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.c1oappe.top/gtehoqaigb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.c1oappe.top/gtmvwajovs.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.shanyushiyangtech.top/gtvcakhota.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jinyuanbaomall.cn/gtuhfptmes.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.ydjk.org.cn/gtbcsfvahn.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.xinyue.icu/gtccklrlsy.html

[H10] 资源自动释放
来源：http://hz.shuidangran.top/gtxkfuytbg.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zhongyouzk.top/gtlcophien.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yanxiufei.cn/gtvnklkzhj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.andypj.xyz/gteuubrkrg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shanyushiyangtech.top/gtvxcpjifg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jiagoushi.top/gtzlfrvmyg.html

Go:   defer f.Close()
来源：http://hz.kuanghao11.cn/gtguzpdmqp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.tianlin.xyz/gtcqwyxvns.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.shanyushiyangtech.top/gtkgqdxumq.html

================================================================================
来源：http://hz.sufxvd.cn/gtkkhcwqcf.html

I. 正则表达式
来源：http://hz.redwolf501.top/gtldqfafgq.html

================================================================================
来源：http://hz.birdmap.top/gtfqzrtomg.html

[I01] 判断是否匹配
来源：http://hz.yj202588.top/gtfpltnbzp.html


<!-- 参考信息 -->