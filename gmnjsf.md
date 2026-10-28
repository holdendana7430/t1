代发 wailian999

C#:   File.Exists("a.txt")
来源：http://hz.ybcxt.top/gtyinbbwmo.html

[F06] 删除文件
来源：http://hz.jianghu66.top/gtmyrekwyq.html

Py:   os.remove("a.txt")
来源：http://hz.ivvv.top/gtkjiraxxe.html

PHP:  unlink("a.txt");
来源：http://hz.yangfankeji.com/gtqbqpftci.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.tian-w.cn/gthcadlsmc.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yj20258888.top/gthdrecsrv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.ivvv.top/gtczrzgxzj.html

Go:   os.Remove("a.txt")
来源：http://hz.xziqi.cn/gtkwhmsxis.html

Ruby: File.delete("a.txt")
来源：http://hz.hywenlv.cn/gtngssjwjy.html

C#:   File.Delete("a.txt");
来源：http://hz.yanxiufei.cn/gtzwvvhlsj.html

[F07] 创建目录（含多级）
来源：http://hz.cashguo.top/gtjkqxjzcu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.quarkkingdee.top/gtfolcgwrw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.hfpthk.cn/gtiqkuxnrw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jlsjyb.cn/gtqeexlogk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jinyuanbaomall.cn/gthrmiziwl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.nanxinkj.top/gtviydumgy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zhaomingkeji.xyz/gtcrhatiqc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.xylfe.cn/gtnqlhjhpk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yuxming.cn/gthdczdrsj.html

[F08] 遍历目录
来源：http://hz.zhijiandao.cn/gtkxncqkgn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.jianghu66.top/gtgymcgwlq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jqgufenzy.top/gtnepzffvm.html

JS:   fs.readdirSync("dir")
来源：http://hz.pengpengdd.cyou/gtrqqxcsug.html

TS:   fs.readdirSync("dir")
来源：http://hz.shangyingyoupin.top/gtdnxfoipw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.daxiang520.top/gtapcpewtq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.hywenlv.cn/gtyjlrvtra.html

Ruby: Dir.children("dir")
来源：http://hz.yongpay.top/gtgqoniyqv.html

C#:   Directory.GetFiles("dir")
来源：http://hz.cheryme.top/gtwhjkrqzc.html

[F09] 获取文件大小
来源：http://hz.xuanzx.com/gtqvfiwush.html

Py:   os.path.getsize("a.txt")
来源：http://hz.vqdsnc.cn/gtcwmvcvgu.html

PHP:  filesize("a.txt");
来源：http://hz.zhoulong.xyz/gtkxuchcyw.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yj20258.top/gttigfaoxu.html

TS:   fs.statSync("a.txt").size
来源：http://hz.sxryk.cn/gtsixaieez.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.shanyushiyangkeji.top/gtzpgefenp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yanxiufei.cn/gtsfkxfvcp.html

Ruby: File.size("a.txt")
来源：http://hz.vqdsnc.cn/gtlscwbesd.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.chenlongwang.top/gtfnnabbvv.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.0kj1m.cn/gtocxsewxm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.snrcjt.cn/gtbncrlzjb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.c1oappe.top/gtomzhfdye.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.meibo888.top/gtjvmudsqb.html

TS:   path.extname("a.txt")
来源：http://hz.zycfv.cn/gtekkgqbwa.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jianghu66.top/gtmrifgliw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yj202588.top/gtnaxhyoob.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.fzhhl.top/gtjlfeidsd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.cashguo.top/gtmiftwrpq.html

[F11] 复制与移动文件
来源：http://hz.gogol.net.cn/gtpoftzbww.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.cucudq.cn/gthmwysbwv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yonumen.top/gtlddxdoki.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jqgfzy.top/gttfonlxek.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shangyingyoupin.top/gtiwjuqhrm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.ywan-chungtsiang.top/gtqhnoinwj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.shanyushiyangtech.top/gtogfmpsng.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.xuanzx.com/gtppcjmdht.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yonumen.top/gtydokgyaj.html

[F12] CSV 读写
来源：http://hz.feifeiyinyue.top/gtfubgksmt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.ivvv.top/gtnauphdtm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jinqigufen.top/gtwtavcggj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zhoulong.xyz/gthwoxwexq.html

TS:   // 同上
来源：http://hz.cheryme.top/gtlvqqatzh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.tian-w.cn/gtsfufplkd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.nanxuanxn.top/gtpmddqdgn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.hywenlv.cn/gtwziokfnl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.fengsongda.top/gtzrjqtouk.html

================================================================================
来源：http://hz.nanxinkj.top/gtnckotqnh.html

G. 面向对象
来源：http://hz.shuidangran.top/gtijmkmofl.html

================================================================================
来源：http://hz.birdmap.top/gtrrzcjoox.html

[G01] 定义类
来源：http://hz.jqgfzy.top/gtvxquqmmd.html

Py:   class User: pass
来源：http://hz.daria6918.cn/gtwcozxgws.html

PHP:  class User {}
来源：http://hz.yuanzhike.top/gtidxsdrqs.html

JS:   class User {}
来源：http://hz.mhx1999.top/gtkdurvjjk.html

TS:   class User { name: string = ""; }
来源：http://hz.wangshuangyany.cn/gtcqhnultw.html

Java: class User {}
来源：http://hz.svipenyu.cn/gtfbogchts.html

Go:   type User struct { Name string }
来源：http://hz.andypj.xyz/gtfjabyybk.html

Ruby: class User; end
来源：http://hz.ppjwa.cn/gtzjkgfiqn.html

C#:   class User {}
来源：http://hz.hysaishi.cn/gtzglpizsq.html

[G02] 构造函数
来源：http://hz.svipenyu.cn/gtidzdapmv.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.ehwqpu.com/gtcrrdaxus.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ivvv.top/gtpnasktgn.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jlsjyb.cn/gtmtwykcsp.html

TS:   constructor(public name: string) {}
来源：http://hz.ydjk.org.cn/gtczqgtduv.html

Java: User(String name) { this.name = name; }
来源：http://hz.sysykeji.top/gtwnyeksyf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jianghu66.top/gtiukcfmcz.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.shangyingyoupin.top/gtmokgnmtp.html

C#:   public User(string name) { Name = name; }
来源：http://hz.feifeiyinyue.top/gtvivpjxhf.html

[G03] 实例属性
来源：http://hz.dashuyun.cn/gtfvxxqxlb.html

Py:   self.name = "x"
来源：http://hz.ehwqpu.com/gtdtaxfdqd.html

PHP:  public string $name = "x";
来源：http://hz.52xcode.cn/gtqogmhlaj.html

JS:   this.name = "x";
来源：http://hz.yanxiufei.cn/gtdsgrujfw.html

TS:   name: string = "x";
来源：http://hz.pengpengdd.cyou/gtkeylndcp.html

Java: private String name;
来源：http://hz.wangdashe.top/gtkneediig.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.aibaodan.cn/gtjxxqbzin.html

Ruby: @name = "x"
来源：http://hz.yj20258888.top/gtrwqqcsng.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yuxming.cn/gtjueeafci.html

[G04] 定义方法
来源：http://hz.316326.xyz/gtekxlnqxx.html

Py:   def greet(self): return self.name
来源：http://hz.fzhhl.top/gtbaoqiini.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hammf.cn/gtkgiiomhj.html

JS:   greet() { return this.name; }
来源：http://hz.daria6918.cn/gtxmynqtko.html

TS:   greet(): string { return this.name; }
来源：http://hz.yvedp.cn/gtjjgxvjrw.html

Java: String greet() { return name; }
来源：http://hz.mhx1999.top/gtejqkkgzg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.nanxuanxn.top/gtzmzbhffd.html

Ruby: def greet; @name; end
来源：http://hz.cdnleiting.top/gtdpvmacej.html

C#:   public string Greet() => Name;
来源：http://hz.zhaomingkeji.xyz/gtyqgfhrnw.html

[G05] 继承
来源：http://hz.svipenyu.cn/gtazoeqhvr.html

Py:   class Admin(User): pass
来源：http://hz.shuidangran.top/gtarfrfghs.html

PHP:  class Admin extends User {}
来源：http://hz.316326.xyz/gtxmqbqhif.html

JS:   class Admin extends User {}
来源：http://hz.52xcode.cn/gtsyhkneyk.html

TS:   class Admin extends User {}
来源：http://hz.gaohongyu789.top/gtcujxmxrk.html

Java: class Admin extends User {}
来源：http://hz.wangdashe.top/gthivgkjzl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ppjwa.cn/gteqloztqq.html

Ruby: class Admin < User; end
来源：http://hz.chenjidiqi.icu/gtwmztqfop.html

C#:   class Admin : User {}
来源：http://hz.hongshengwenyu.top/gtxvabrckv.html

[G06] 重写方法
来源：http://hz.hnqzz.top/gtbjpejive.html

Py:   def greet(self): return "admin"
来源：http://hz.shuidangran.top/gtlbxlgtxp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ybcxt.top/gtfjbckadn.html

JS:   greet() { return "admin"; }
来源：http://hz.chenjidiqi.icu/gtqxupvtza.html

TS:   greet(): string { return "admin"; }
来源：http://hz.haohaochexian.top/gtdqrpmrwe.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.kuanghao11.cn/gttkxqgyrb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.0kj1m.cn/gtzprpwnqq.html

Ruby: def greet; "admin"; end
来源：http://hz.chenlongwang.top/gtxmszwhkq.html

C#:   public override string Greet() => "admin";
来源：http://hz.sysykeji.top/gtsqierrze.html

[G07] 调用父类方法
来源：http://hz.xingfuxueyuan.xyz/gtcuagumqi.html

Py:   super().greet()
来源：http://hz.havefunace.top/gtwmozkcyp.html

PHP:  parent::greet();
来源：http://hz.zdqjudy.top/gtewlqxyxn.html

JS:   super.greet();
来源：http://hz.jinyuanbaomall.cn/gtmztblhaj.html

TS:   super.greet();
来源：http://hz.iojbl.cn/gtjfyivgxm.html

Java: super.greet();
来源：http://hz.chenzaomai.com/gtxpzzbkyu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.xingfuxueyuan.xyz/gtkqeznmhz.html

Ruby: super
来源：http://hz.cqqwz.cn/gtccdctgpa.html

C#:   base.Greet();
来源：http://hz.snrcjt.cn/gtrzcmvybw.html

[G08] 静态方法与属性
来源：http://hz.aibaodan.cn/gtmhdwheyj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.hammf.cn/gtnmjiykwe.html

PHP:  public static function f() {}
来源：http://hz.guowangkeji.top/gtglodfssp.html

JS:   static f() {}
来源：http://hz.yj20258.top/gtaigfpzqs.html

TS:   static f(): void {}
来源：http://hz.tian-w.cn/gtljkojcfx.html

Java: static void f() {}
来源：http://hz.redwolf501.top/gtxcsseujs.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yuanzhike.top/gtlcqcherm.html

Ruby: def self.f; end
来源：http://hz.jianghu66.top/gtynmtmlll.html

C#:   public static void F() {}
来源：http://hz.sxryk.cn/gtogymvrnb.html

[G09] 接口 / 抽象类
来源：http://hz.jianghu66.top/gtaimwoxex.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.xylfe.cn/gtjdpohcvk.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zycfv.cn/gthwvyoujh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.mhx1999.top/gtibqgzidh.html

TS:   interface Shape { area(): number; }
来源：http://hz.zycfv.cn/gtyvivombe.html

Java: interface Shape { double area(); }
来源：http://hz.yuanzhike.top/gtqwkomhsu.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.hongshengwenyu.top/gtqnococbs.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.xingfuxueyuan.xyz/gtygdkxvnw.html

C#:   interface IShape { double Area(); }
来源：http://hz.sysykeji.top/gtafnwxnji.html

[G10] 访问控制
来源：http://hz.tian-w.cn/gtkqohsyqc.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.cheryme.top/gtrqbaujpy.html

PHP:  public / protected / private
来源：http://hz.sxryk.cn/gtiskizypp.html

JS:   #private 字段；其余公开
来源：http://hz.jiagoushi.top/gtytginiip.html

TS:   public / protected / private
来源：http://hz.jianghu66.top/gtskoyegox.html

Java: public / protected / private / 默认包级
来源：http://hz.cqqwz.cn/gtrduvlqzu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.nanxinkj.top/gtotslsagm.html

Ruby: public / protected / private
来源：http://hz.xuanzx.com/gtebtyekvw.html

C#:   public / protected / private / internal
来源：http://hz.yj20258.top/gtlqbsazqe.html

[G11] getter / setter
来源：http://hz.svipenyu.cn/gtijkpwkaf.html

Py:   @property 与 @x.setter
来源：http://hz.zycfv.cn/gtuipzoeqi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.cheryme.top/gtagwwynop.html

JS:   get name() { return this._name; }
来源：http://hz.bjfxy.top/gtgzrkhtgy.html

TS:   get name(): string { return this._name; }
来源：http://hz.fzhhl.top/gtjdnzfhbq.html

Java: public String getName() { return name; }
来源：http://hz.redwolf501.top/gtfymjpxor.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.hnqzz.top/gtkrfghqwp.html

Ruby: attr_accessor :name
来源：http://hz.zhixingplan.top/gtvtllpkog.html

C#:   public string Name { get; set; }
来源：http://hz.yj202588.top/gtaoyypevf.html

[G12] 对象转字符串
来源：http://hz.ywan-chungtsiang.top/gtzeinwovj.html

Py:   def __str__(self): return self.name
来源：http://hz.xylfe.cn/gtrskmyspg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zhoulong.xyz/gtradxdlxr.html

JS:   toString() { return this.name; }
来源：http://hz.chenjidiqi.icu/gtxcrfijfk.html

TS:   toString(): string { return this.name; }
来源：http://hz.bjfxy.top/gtoxfickyw.html

Java: @Override public String toString() { return name; }
来源：http://hz.svipenyu.cn/gtgccajrfd.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.wangshuangyany.cn/gtgnejftvr.html

Ruby: def to_s; @name; end
来源：http://hz.jqgfzy.top/gtucsllqom.html

C#:   public override string ToString() => Name;
来源：http://hz.316326.xyz/gtggwcvcop.html

[G13] 判断对象类型
来源：http://hz.52xcode.cn/gtyebreeui.html

Py:   isinstance(u, User)
来源：http://hz.nanxuanxn.top/gtlotsfpgt.html

PHP:  $u instanceof User
来源：http://hz.tanke756.top/gtfsmqznef.html

JS:   u instanceof User
来源：http://hz.dianchejie.cn/gtwawsvaqw.html

TS:   u instanceof User
来源：http://hz.quarkkingdee.top/gtdcubmibp.html

Java: u instanceof User
来源：http://hz.hongshengwenyu.top/gtsjbvzcjy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.wangdashe.top/gtftgqettl.html

Ruby: u.is_a?(User)
来源：http://hz.tianlin.xyz/gtqutphxgh.html

C#:   u is User
来源：http://hz.iojbl.cn/gtyewrztzv.html

[G14] 数据类 / record
来源：http://hz.pycfn.com/gtuelzxmxs.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zhengqikj.top/gtvtkiynyr.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.cqqwz.cn/gtbtgydnmz.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yanxiufei.cn/gtbulrwmup.html

TS:   type User = { name: string; age: number };
来源：http://hz.hongshengwenyu.top/gtkjgkjlit.html

Java: record User(String name, int age) {}
来源：http://hz.yj20258.top/gtbvstpjlf.html

Go:   type User struct { Name string; Age int }
来源：http://hz.hnqzz.top/gtnsflaycs.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zhixingplan.top/gtymzjbpue.html

C#:   record User(string Name, int Age);
来源：http://hz.havefunace.top/gtthepulcn.html

[G15] 枚举
来源：http://hz.yanxiufei.cn/gtvzsohuhz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.svipenyu.cn/gtivixkjxw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yj202588.top/gttnongeil.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zhoulong.xyz/gtqchxaibz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ehwqpu.com/gtjhxmuaws.html

Java: enum Color { RED, GREEN }
来源：http://hz.jinqigufen.top/gtdsxqdkvr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jiagoushi.top/gtbqlirvkd.html

Ruby: Color = %i[red green].freeze
来源：http://hz.meibo888.top/gteflxoent.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.guowangkeji.top/gtnpujgcmp.html

[G16] 对象转数组 / 字典
来源：http://hz.iojbl.cn/gtgeocbaao.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yangfankeji.com/gtfuliipke.html

PHP:  get_object_vars($obj);
来源：http://hz.zhixingplan.top/gtqbkhxapu.html

JS:   Object.entries(obj)
来源：http://hz.zhijiandao.cn/gtekpadqpq.html

TS:   Object.entries(obj)
来源：http://hz.jinqigufen.top/gtbfftmvch.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.birdmap.top/gtoxekifee.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.guannengcc.top/gtqvpktxky.html

Ruby: obj.instance_variables
来源：http://hz.hnxiangtu.top/gtdluqpmsc.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.hammf.cn/gttuqmowxf.html

================================================================================
来源：http://hz.yangfankeji.com/gtjihvqzdu.html

H. 异常与错误处理
来源：http://hz.daxiang520.top/gthqdyphxm.html

================================================================================
来源：http://hz.yuxming.cn/gtvyifidgx.html

[H01] try / catch 基础
来源：http://hz.iojbl.cn/gtzvwuentd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.mhx1999.top/gtriarmjdi.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.gzhubu.top/gttfsnxsmm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.hnqzz.top/gtgfgorteh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.ywan-chungtsiang.top/gtstrducpw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.wangdashe.top/gtpauqobom.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.xuanzx.com/gtzbbcpnbu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.fzhhl.top/gttqhnclnn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.ydzc1.top/gtmrmwprfq.html

[H02] finally / ensure 收尾
来源：http://hz.ybcxt.top/gtkabgnryk.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zdqjudy.top/gtnusmsaqv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jlsjyb.cn/gtvoehlmjw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.quarkkingdee.top/gtinyctdza.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.hfpthk.cn/gtaleiltcj.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jiagoushi.top/gteoyfshcn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ybcxt.top/gtxrpzansr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.cheryme.top/gtypvjaaxt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hysaishi.cn/gteukycqkz.html

[H03] 主动抛出异常
来源：http://hz.jlsjyb.cn/gtrpttfpgy.html

Py:   raise ValueError("错误信息")
来源：http://hz.jinghuilouyu.cn/gtzstdeyly.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zhoulong.xyz/gtqnmhydmu.html

JS:   throw new Error("错误信息");
来源：http://hz.nanxinkj.top/gtumqvihoa.html

TS:   throw new Error("错误信息");
来源：http://hz.fengsongda.top/gtogyrnbre.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.tanke756.top/gtecpikkgu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hfpthk.cn/gtzidmacsh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.svipenyu.cn/gtlumxyviv.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.shuidangran.top/gttnnokyzs.html

[H04] 自定义异常类型
来源：http://hz.gotoacloud.top/gtluadvkoh.html

Py:   class MyError(Exception): pass
来源：http://hz.haohaochexian.top/gtomzfwllt.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.nwbrower.top/gtpzqnwyyp.html

JS:   class MyError extends Error {}
来源：http://hz.zycfv.cn/gteacprnvh.html

TS:   class MyError extends Error {}
来源：http://hz.yonumen.top/gtdnhtogie.html

Java: class MyException extends RuntimeException {}
来源：http://hz.hammf.cn/gtqxzuivsq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jlsjyb.cn/gtailwkznl.html

Ruby: class MyError < StandardError; end
来源：http://hz.cashguo.top/gttvsofrfm.html

C#:   class MyException : Exception {}
来源：http://hz.cucudq.cn/gtimfowdhq.html

[H05] 捕获特定类型
来源：http://hz.tianlin.xyz/gtzoghixrg.html

Py:   except ValueError as e:
来源：http://hz.chenlongwang.top/gtyphvpqac.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.snrcjt.cn/gtyyhvyofq.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.chenzaomai.com/gtallazrmp.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.ivvv.top/gtgwtjwunv.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.0kj1m.cn/gttvnjqmxq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hfpthk.cn/gtlxadkvli.html

Ruby: rescue ArgumentError => e
来源：http://hz.yj202588.top/gtpglvaocq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yonumen.top/gtxeiqyxgl.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zhaomingkeji.xyz/gtsqwiathi.html

Py:   value = d.get("k") or default
来源：http://hz.cdnleiting.top/gtxmwvjbcr.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hysaishi.cn/gtorfknkyk.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jinqigfzy.top/gtjbiwofad.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zhoulong.xyz/gtfpisbrwn.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.cheryme.top/gtegwqmeme.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.birdmap.top/gtzjowoohl.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yvedp.cn/gtwqhlhnaw.html

C#:   obj?.A?.B ?? default
来源：http://hz.tanke756.top/gtpvbvozib.html

[H07] 断言
来源：http://hz.ppjwa.cn/gtnmjanmmt.html

Py:   assert x > 0, "必须为正"
来源：http://hz.sufxvd.cn/gttfaflgxl.html

PHP:  assert($x > 0);
来源：http://hz.fengsongda.top/gtdryzmpys.html

JS:   console.assert(x > 0);
来源：http://hz.sysykeji.top/gtdwdiojpp.html

TS:   console.assert(x > 0);
来源：http://hz.sweek.top/gtwervoics.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yueranfly.top/gtvgcvphzk.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jyoumei.cn/gtcnpploty.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hnxiangtu.top/gtpgxdqcom.html

C#:   Debug.Assert(x > 0);
来源：http://hz.hammf.cn/gtrkcjxafx.html

[H08] 获取错误信息与堆栈
来源：http://hz.fengsongda.top/gtlhmxgswb.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zycfv.cn/gtbxuthqhc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.havefunace.top/gtfbkuxlfx.html

JS:   e.message;  e.stack
来源：http://hz.andypj.xyz/gtnbrurzwt.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.cheryme.top/gtvgoztdjq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jinqigfzy.top/gtoyfvvlxe.html

Go:   err.Error()
来源：http://hz.chenjidiqi.icu/gtkujtplfs.html

Ruby: e.message;  e.backtrace
来源：http://hz.xingfuxueyuan.xyz/gtcivbimlh.html

C#:   e.Message;  e.StackTrace
来源：http://hz.vqdsnc.cn/gtsgzvugmd.html

[H09] 带错误码的异常
来源：http://hz.ydzc1.top/gtotzoqdbp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.gaohongyu789.top/gtdoqrrznq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.chenzaomai.com/gtqmggzghs.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.xingfuxueyuan.xyz/gtepuritcq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.sweek.top/gtuybybawk.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.daria6918.cn/gtjxntcbch.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zhengqikj.top/gtqasarqqs.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yvedp.cn/gtpsbidhtn.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jianghu66.top/gtmzsdkfxl.html

[H10] 资源自动释放
来源：http://hz.guannengcc.top/gtvesdwalk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.aibaodan.cn/gtojgrrfwv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ywan-chungtsiang.top/gtqoucifjk.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xuetiantiany.cn/gtgetunqfz.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.pengpengdd.cyou/gtzjhudvwq.html


<!-- 参考信息 -->