代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://hz.sysykeji.top/gtqjwsgtvi.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yvedp.cn/gttcfhhuge.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhoulong.xyz/gtninipqjc.html

Go:   os.Remove("a.txt")
来源：http://hz.chenjidiqi.icu/gtdowpdxxi.html

Ruby: File.delete("a.txt")
来源：http://hz.fzhhl.top/gtdudcpwxg.html

C#:   File.Delete("a.txt");
来源：http://hz.aizwys.cn/gtqrtqbtai.html

[F07] 创建目录（含多级）
来源：http://hz.birdmap.top/gtgwfkcquw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jiagoushi.top/gthslcduly.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.meibo888.top/gtdiufbejx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.guannengcc.top/gtzyihuuol.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.bjfxy.top/gtcdukjpty.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.mhx1999.top/gtsqespmsa.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hnqzz.top/gtgcgduerd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.fengsongda.top/gthyrorhcw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.mhx1999.top/gtpytmpvby.html

[F08] 遍历目录
来源：http://hz.hammf.cn/gttnmtvjqi.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.chenjidiqi.icu/gtjnnzpvfg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yueranfly.top/gtnwntudgb.html

JS:   fs.readdirSync("dir")
来源：http://hz.xingfuxueyuan.xyz/gtdlxcixdp.html

TS:   fs.readdirSync("dir")
来源：http://hz.hnxiangtu.top/gtynfrzhdk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.ywan-chungtsiang.top/gtwkxampxy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.haohaochexian.top/gtkrcquald.html

Ruby: Dir.children("dir")
来源：http://hz.kuanghao11.cn/gtactgzsqr.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jqgufenzy.top/gtrosotnsg.html

[F09] 获取文件大小
来源：http://hz.cucudq.cn/gthqchuraq.html

Py:   os.path.getsize("a.txt")
来源：http://hz.sufxvd.cn/gtctmhzjia.html

PHP:  filesize("a.txt");
来源：http://hz.quarkkingdee.top/gtdgirvshm.html

JS:   fs.statSync("a.txt").size
来源：http://hz.andypj.xyz/gtrrgpxtjr.html

TS:   fs.statSync("a.txt").size
来源：http://hz.aizwys.cn/gtjkbfcpcu.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.aizwys.cn/gtbqrlnysr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yonumen.top/gtvximbdxd.html

Ruby: File.size("a.txt")
来源：http://hz.xuetiantiany.cn/gtvtnfjlly.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jinyuanbaomall.cn/gtubnuwswo.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.svipenyu.cn/gtrcqhgfpa.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.sysykeji.top/gtezbcmury.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zhoulong.xyz/gtankqimww.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.sweek.top/gthpueejjn.html

TS:   path.extname("a.txt")
来源：http://hz.hongshengwenyu.top/gtizwatmjy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.hnxiangtu.top/gtvynkhpij.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.shanyushiyangkeji.top/gtouxkpplj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhengqikj.top/gthemseqms.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.cucudq.cn/gtmtcfwzwv.html

[F11] 复制与移动文件
来源：http://hz.zhiwuduotai.top/gtjcamledc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yvedp.cn/gthhsbmjxb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.xuanzx.com/gtuzbstiji.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.fzhhl.top/gtncwwovwe.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cashguo.top/gtnbjzxofl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.svipenyu.cn/gtrclztdsw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.cheryme.top/gtoyqqwlgo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.meibo888.top/gtrmcajmmm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ywan-chungtsiang.top/gtfsmseurf.html

[F12] CSV 读写
来源：http://hz.ybcxt.top/gtgqakmjdo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.meibo888.top/gtjvcrybhr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jinghuilouyu.cn/gticvpfpir.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yj202588.top/gtldfermij.html

TS:   // 同上
来源：http://hz.zhixingplan.top/gtdgbfrdzl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yj20258.top/gtodfgbdyd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yj20258.top/gtbvurjkpz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jyoumei.cn/gtcqamgvqe.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yonumen.top/gtwexvbgoa.html

================================================================================
来源：http://hz.xuanzx.com/gtukynyyfx.html

G. 面向对象
来源：http://hz.jqgfzy.top/gtbmxpgghb.html

================================================================================
来源：http://hz.yuxming.cn/gtsifkwffi.html

[G01] 定义类
来源：http://hz.gaohongyu789.top/gtivblzahj.html

Py:   class User: pass
来源：http://hz.ppjwa.cn/gtqerbmimo.html

PHP:  class User {}
来源：http://hz.nwbrower.top/gtfxzazqry.html

JS:   class User {}
来源：http://hz.nanxuanxn.top/gtsqbvbfjz.html

TS:   class User { name: string = ""; }
来源：http://hz.zhoulong.xyz/gtuubeflfm.html

Java: class User {}
来源：http://hz.fzhhl.top/gtggrldqzk.html

Go:   type User struct { Name string }
来源：http://hz.yonumen.top/gtyxouyzaj.html

Ruby: class User; end
来源：http://hz.shanyushiyangtech.top/gtkxclbvzc.html

C#:   class User {}
来源：http://hz.hongshengwenyu.top/gtithyyaao.html

[G02] 构造函数
来源：http://hz.pycfn.com/gtkctxradh.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.hnqzz.top/gtxyfsfiwf.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.sysykeji.top/gtdggclgiz.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jyoumei.cn/gtiauaymqb.html

TS:   constructor(public name: string) {}
来源：http://hz.sweek.top/gtxqotfzmf.html

Java: User(String name) { this.name = name; }
来源：http://hz.jlsjyb.cn/gtgrjwvkzv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yj20258888.top/gtpmoxkghp.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.pengpengdd.cyou/gtqhyziebh.html

C#:   public User(string name) { Name = name; }
来源：http://hz.bjfxy.top/gtbhahqmvf.html

[G03] 实例属性
来源：http://hz.quarkkingdee.top/gtgpayfscf.html

Py:   self.name = "x"
来源：http://hz.guowangkeji.top/gtjtdjwyzo.html

PHP:  public string $name = "x";
来源：http://hz.shzxlz.cn/gtvrinarnz.html

JS:   this.name = "x";
来源：http://hz.xuetiantiany.cn/gtoqvudamb.html

TS:   name: string = "x";
来源：http://hz.daria6918.cn/gtnmoxaopy.html

Java: private String name;
来源：http://hz.shanyushiyangtech.top/gthglkneiv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zdqjudy.top/gtrobcgeye.html

Ruby: @name = "x"
来源：http://hz.cqqwz.cn/gtdoesujgo.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.meibo888.top/gticgquiyi.html

[G04] 定义方法
来源：http://hz.yuxming.cn/gtlwzrfszw.html

Py:   def greet(self): return self.name
来源：http://hz.iojbl.cn/gtmtetvmxk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.tianlin.xyz/gthoplowje.html

JS:   greet() { return this.name; }
来源：http://hz.pycfn.com/gtdgrjxdmq.html

TS:   greet(): string { return this.name; }
来源：http://hz.jlsjyb.cn/gtucxtpwtf.html

Java: String greet() { return name; }
来源：http://hz.redwolf501.top/gtrqjwxtfw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.chenjidiqi.icu/gtjtsoewjz.html

Ruby: def greet; @name; end
来源：http://hz.zdqjudy.top/gtyrrimcpu.html

C#:   public string Greet() => Name;
来源：http://hz.quarkkingdee.top/gtffyqjjgw.html

[G05] 继承
来源：http://hz.chenlongwang.top/gtnslgpwgb.html

Py:   class Admin(User): pass
来源：http://hz.zhiwuduotai.top/gthxsrpszj.html

PHP:  class Admin extends User {}
来源：http://hz.jlsjyb.cn/gtewxwziff.html

JS:   class Admin extends User {}
来源：http://hz.hammf.cn/gtclyjdeyo.html

TS:   class Admin extends User {}
来源：http://hz.redwolf501.top/gtupxgwhhh.html

Java: class Admin extends User {}
来源：http://hz.gotoacloud.top/gtczhumdhe.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jinghuilouyu.cn/gtridmvxhc.html

Ruby: class Admin < User; end
来源：http://hz.gzhubu.top/gthycxbicx.html

C#:   class Admin : User {}
来源：http://hz.hywenlv.cn/gtqqfescxn.html

[G06] 重写方法
来源：http://hz.ivvv.top/gtuklpjxho.html

Py:   def greet(self): return "admin"
来源：http://hz.meibo888.top/gtbogtwgnr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.wangdashe.top/gtbfnxgfmt.html

JS:   greet() { return "admin"; }
来源：http://hz.svipenyu.cn/gtzmczhkcf.html

TS:   greet(): string { return "admin"; }
来源：http://hz.iojbl.cn/gteuzzmscw.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.kuanghao11.cn/gtqcsvnvne.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.gzhubu.top/gtjhnyajaf.html

Ruby: def greet; "admin"; end
来源：http://hz.gzhubu.top/gttanmonys.html

C#:   public override string Greet() => "admin";
来源：http://hz.wangdashe.top/gtmjnexmvm.html

[G07] 调用父类方法
来源：http://hz.ppjwa.cn/gtizamwric.html

Py:   super().greet()
来源：http://hz.shangyingyoupin.top/gtozgrqvic.html

PHP:  parent::greet();
来源：http://hz.guowangkeji.top/gtysmvfhov.html

JS:   super.greet();
来源：http://hz.shzxlz.cn/gtkxtugjcl.html

TS:   super.greet();
来源：http://hz.fengsongda.top/gtgdhpmxkn.html

Java: super.greet();
来源：http://hz.shangyingyoupin.top/gtdfggejad.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yonumen.top/gtlemhoqql.html

Ruby: super
来源：http://hz.ydjk.org.cn/gttryudwee.html

C#:   base.Greet();
来源：http://hz.feifeiyinyue.top/gtnisobjjb.html

[G08] 静态方法与属性
来源：http://hz.chenjidiqi.icu/gtfrrtovhl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.hnxiangtu.top/gtjbpuhwzw.html

PHP:  public static function f() {}
来源：http://hz.ehwqpu.com/gtaqqzmlpq.html

JS:   static f() {}
来源：http://hz.shuidangran.top/gtyunrvgwk.html

TS:   static f(): void {}
来源：http://hz.redwolf501.top/gtneqdbjgl.html

Java: static void f() {}
来源：http://hz.hywenlv.cn/gtagfcbyck.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhaomingkeji.xyz/gtnbsjmmry.html

Ruby: def self.f; end
来源：http://hz.cdnleiting.top/gtzkpubsoq.html

C#:   public static void F() {}
来源：http://hz.yongpay.top/gtyeoabwpf.html

[G09] 接口 / 抽象类
来源：http://hz.daxiang520.top/gtuebwkmrx.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zhengqikj.top/gtbzvxokyh.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zdqjudy.top/gtiknrsoww.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.nwbrower.top/gtgelkzvat.html

TS:   interface Shape { area(): number; }
来源：http://hz.tanke756.top/gtzrokssoc.html

Java: interface Shape { double area(); }
来源：http://hz.9152youxi.cn/gtgpljwlfo.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.havefunace.top/gtffdahnfe.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yonumen.top/gtwchsowpl.html

C#:   interface IShape { double Area(); }
来源：http://hz.jqgufenzy.top/gtbkovaywn.html

[G10] 访问控制
来源：http://hz.shanyushiyangkeji.top/gtcycvqxwy.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.andypj.xyz/gtiagejqwi.html

PHP:  public / protected / private
来源：http://hz.chenjidiqi.icu/gtuxxuozfw.html

JS:   #private 字段；其余公开
来源：http://hz.xuanzx.com/gtunxlryek.html

TS:   public / protected / private
来源：http://hz.fzhhl.top/gtxibpvsex.html

Java: public / protected / private / 默认包级
来源：http://hz.zhongyouzk.top/gtcigeofwp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.xinyue.icu/gtlhpydotp.html

Ruby: public / protected / private
来源：http://hz.sweek.top/gtjfdswddp.html

C#:   public / protected / private / internal
来源：http://hz.yuanzhike.top/gtplqoogry.html

[G11] getter / setter
来源：http://hz.svipenyu.cn/gtfnodbfip.html

Py:   @property 与 @x.setter
来源：http://hz.gotoacloud.top/gthlcpdfxc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.daxiang520.top/gtaqoatbnr.html

JS:   get name() { return this._name; }
来源：http://hz.sweek.top/gtxmtmzxjo.html

TS:   get name(): string { return this._name; }
来源：http://hz.yj20258.top/gtegfiiopd.html

Java: public String getName() { return name; }
来源：http://hz.jianghu66.top/gtaltxfjhq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.chenjidiqi.icu/gthswzhqji.html

Ruby: attr_accessor :name
来源：http://hz.9152youxi.cn/gturxmdvux.html

C#:   public string Name { get; set; }
来源：http://hz.gaohongyu789.top/gtobyvxioi.html

[G12] 对象转字符串
来源：http://hz.mhx1999.top/gtowoagstp.html

Py:   def __str__(self): return self.name
来源：http://hz.sxryk.cn/gtrssvrpku.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.xziqi.cn/gtfqvhwzrp.html

JS:   toString() { return this.name; }
来源：http://hz.daxiang520.top/gtrkpslehh.html

TS:   toString(): string { return this.name; }
来源：http://hz.meibo888.top/gtokvqdliz.html

Java: @Override public String toString() { return name; }
来源：http://hz.jinghuilouyu.cn/gtktqpppla.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.ybcxt.top/gtyupxbufr.html

Ruby: def to_s; @name; end
来源：http://hz.wangdashe.top/gtkopvbctl.html

C#:   public override string ToString() => Name;
来源：http://hz.wangshuangyany.cn/gtursrdmim.html

[G13] 判断对象类型
来源：http://hz.xinyue.icu/gtiodfbdgd.html

Py:   isinstance(u, User)
来源：http://hz.redwolf501.top/gtpippxgqy.html

PHP:  $u instanceof User
来源：http://hz.dashuyun.cn/gtsvdppbsw.html

JS:   u instanceof User
来源：http://hz.yj202588.top/gttkanafaj.html

TS:   u instanceof User
来源：http://hz.xuanzx.com/gtrdrvntvb.html

Java: u instanceof User
来源：http://hz.dashuyun.cn/gtwbioolzw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.316326.xyz/gttzebqdnz.html

Ruby: u.is_a?(User)
来源：http://hz.ywan-chungtsiang.top/gtgzaunmjd.html

C#:   u is User
来源：http://hz.hywenlv.cn/gtpagcrxtl.html

[G14] 数据类 / record
来源：http://hz.xinyue.icu/gtvvetoxbq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.shzxlz.cn/gtqfldkhfx.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.shanyushiyangkeji.top/gtzpfkadny.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.svipenyu.cn/gtjqpunori.html

TS:   type User = { name: string; age: number };
来源：http://hz.smart0.xyz/gtpmzpjrnj.html

Java: record User(String name, int age) {}
来源：http://hz.fzhhl.top/gtizrcqqfu.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yangfankeji.com/gtkfnndhey.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.birdmap.top/gtiarfxwpf.html

C#:   record User(string Name, int Age);
来源：http://hz.gaohongyu789.top/gthfnrwajf.html

[G15] 枚举
来源：http://hz.wangdashe.top/gtzqhwrgbr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.hfpthk.cn/gtvjcousol.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.feifeiyinyue.top/gtrtbligqp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jinghuilouyu.cn/gtsdnmzrgt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.snrcjt.cn/gtopkpvuvu.html

Java: enum Color { RED, GREEN }
来源：http://hz.guannengcc.top/gtnujgahor.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.9152youxi.cn/gtsjrorcxb.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yueranfly.top/gtocdhvsit.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shangyingyoupin.top/gtbkkqaaft.html

[G16] 对象转数组 / 字典
来源：http://hz.zhaomingkeji.xyz/gtyqbezehm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.tianlin.xyz/gtgzyhzwae.html

PHP:  get_object_vars($obj);
来源：http://hz.nanxuanxn.top/gtmumkgjmp.html

JS:   Object.entries(obj)
来源：http://hz.jinqigufen.top/gtwwdpmeiy.html

TS:   Object.entries(obj)
来源：http://hz.yj20258888.top/gtcfraxywn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.9152youxi.cn/gthkoccmnq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.zhiwuduotai.top/gtprsyjruj.html

Ruby: obj.instance_variables
来源：http://hz.jyoumei.cn/gtavukxejs.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhongyouzk.top/gtidvggdbi.html

================================================================================
来源：http://hz.cqqwz.cn/gtbydkgnos.html

H. 异常与错误处理
来源：http://hz.jlsjyb.cn/gtltotfang.html

================================================================================
来源：http://hz.nanxuanxn.top/gtxpetucav.html

[H01] try / catch 基础
来源：http://hz.pengpengdd.cyou/gtkdtvbomx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.tanke756.top/gtdmbyilij.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yuxming.cn/gtveyezgnw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.meibo888.top/gtgcqkslrx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.daxiang520.top/gtmkmslgkc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jinqigfzy.top/gtouxlumaa.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.birdmap.top/gtzccadjlx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.cashguo.top/gtchgyjvmg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.cdnleiting.top/gtxcchnfoi.html

[H02] finally / ensure 收尾
来源：http://hz.9152youxi.cn/gtfndixjpc.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.feifeiyinyue.top/gtzwebzhsb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.birdmap.top/gtyfpbalat.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yongpay.top/gtettjaryr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yvedp.cn/gtfujdieur.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.iojbl.cn/gtkrbxtkpa.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.wangdashe.top/gtnkrspgku.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.cashguo.top/gtuqgffvvb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yuxming.cn/gtpynctfjn.html

[H03] 主动抛出异常
来源：http://hz.guannengcc.top/gtijbuafhl.html

Py:   raise ValueError("错误信息")
来源：http://hz.vqdsnc.cn/gtbraqweye.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.ybcxt.top/gtmcsejmku.html

JS:   throw new Error("错误信息");
来源：http://hz.jiagoushi.top/gtovqpasdv.html

TS:   throw new Error("错误信息");
来源：http://hz.aibaodan.cn/gtvwtmcevs.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.ppjwa.cn/gtxswhqemt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.chenzaomai.com/gtecjrezyb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.sweek.top/gtixqasjrh.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.aizwys.cn/gtkxlwwfvy.html

[H04] 自定义异常类型
来源：http://hz.yuxming.cn/gtxjvgzkaa.html

Py:   class MyError(Exception): pass
来源：http://hz.dashuyun.cn/gtlcbnykoh.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.fzhhl.top/gtyrjrvvfe.html

JS:   class MyError extends Error {}
来源：http://hz.daria6918.cn/gtkahpnmfv.html

TS:   class MyError extends Error {}
来源：http://hz.jqgufenzy.top/gtrsgdvujd.html

Java: class MyException extends RuntimeException {}
来源：http://hz.chenlongwang.top/gtibgownph.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.guowangkeji.top/gtvnceosyb.html

Ruby: class MyError < StandardError; end
来源：http://hz.redwolf501.top/gtepxkkuul.html

C#:   class MyException : Exception {}
来源：http://hz.sweek.top/gttdpragnd.html

[H05] 捕获特定类型
来源：http://hz.shzxlz.cn/gtynvlxbsy.html

Py:   except ValueError as e:
来源：http://hz.zhaomingkeji.xyz/gtutdknwfi.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yongpay.top/gtikdopfuv.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.tianlin.xyz/gtzkvtyivo.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.haohaochexian.top/gtbehusawg.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.316326.xyz/gtbmrasaal.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.shanyushiyangtech.top/gteljmcpaj.html

Ruby: rescue ArgumentError => e
来源：http://hz.zhoulong.xyz/gtkaenzhkz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jinqigfzy.top/gtkvnzlzkk.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zdqjudy.top/gtjhycwktm.html

Py:   value = d.get("k") or default
来源：http://hz.xziqi.cn/gtwdvwlakl.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.fzhhl.top/gtxntauefu.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zhoulong.xyz/gtvezmuhsv.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.gogol.net.cn/gtljxwgdkg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jqgufenzy.top/gtkcrnxdxv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.316326.xyz/gttarbmsjb.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhaomingkeji.xyz/gtzgmlqmbd.html

C#:   obj?.A?.B ?? default
来源：http://hz.yvedp.cn/gtugbvamyj.html

[H07] 断言
来源：http://hz.dianchejie.cn/gtsbpibqnb.html

Py:   assert x > 0, "必须为正"
来源：http://hz.gogol.net.cn/gtwfhxglda.html

PHP:  assert($x > 0);
来源：http://hz.hfpthk.cn/gttpnkfxuw.html

JS:   console.assert(x > 0);
来源：http://hz.havefunace.top/gtcgbjltnc.html

TS:   console.assert(x > 0);
来源：http://hz.gaohongyu789.top/gtwkpdgwdu.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yj20258888.top/gtebkklyrn.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.xingfuxueyuan.xyz/gtmsaplufq.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jinghuilouyu.cn/gtaktagctz.html

C#:   Debug.Assert(x > 0);
来源：http://hz.andypj.xyz/gtzrsbsaey.html

[H08] 获取错误信息与堆栈
来源：http://hz.zycfv.cn/gtiojccziq.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ppjwa.cn/gtzindhrbo.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.redwolf501.top/gtqnomfwbx.html

JS:   e.message;  e.stack
来源：http://hz.0kj1m.cn/gttddlhktz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.gotoacloud.top/gtijjobxbg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jinqigufen.top/gtoykbwjzp.html

Go:   err.Error()
来源：http://hz.yongpay.top/gtjtigvmkj.html

Ruby: e.message;  e.backtrace
来源：http://hz.shzxlz.cn/gtdbmohgqy.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zdqjudy.top/gtpqvtqfbb.html

[H09] 带错误码的异常
来源：http://hz.nanxinkj.top/gtqxfvliqe.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.xuanzx.com/gterjdtrwq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zhongyouzk.top/gttuqmhuqw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.pycfn.com/gtdxbcpdch.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.feifeiyinyue.top/gtwzbbxxjv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jinqigufen.top/gtzgugndly.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yuxming.cn/gtymdqteqg.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.dashuyun.cn/gtlsvzidoh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.xingfuxueyuan.xyz/gtvgnerzid.html

[H10] 资源自动释放
来源：http://hz.yvedp.cn/gtjcnctgpp.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.52xcode.cn/gttqpnslww.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.hammf.cn/gtkkrdjfzu.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhiwuduotai.top/gtepqafrdf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.dashuyun.cn/gtoldgviue.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jlsjyb.cn/gtnxoblkji.html

Go:   defer f.Close()
来源：http://hz.yueranfly.top/gtwrnhheak.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.tian-w.cn/gthlbqgasc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.havefunace.top/gtowjhvuit.html


<!-- 参考信息 -->