代发 wailian999

C#:   File.Exists("a.txt")
来源：http://hz.shanyushiyangkeji.top/gttgxztiaz.html

[F06] 删除文件
来源：http://hz.smart0.xyz/gtzoecugjb.html

Py:   os.remove("a.txt")
来源：http://hz.ydzc1.top/gtribdcmxn.html

PHP:  unlink("a.txt");
来源：http://hz.wangdashe.top/gtzozkbgxt.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.sweek.top/gtbnmvizoa.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.pycfn.com/gtjgsybdvj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.shanyushiyangkeji.top/gtqwiaasvk.html

Go:   os.Remove("a.txt")
来源：http://hz.nanxinkj.top/gtrjpwnqmp.html

Ruby: File.delete("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtpwelzljl.html

C#:   File.Delete("a.txt");
来源：http://hz.xuanzx.com/gtadwpclnp.html

[F07] 创建目录（含多级）
来源：http://hz.cashguo.top/gtficctwie.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jqgufenzy.top/gtgduwzlqe.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.feifeiyinyue.top/gtjnidnhvu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.gotoacloud.top/gtoypmjcpc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hfpthk.cn/gtfwqbagys.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jqgfzy.top/gtmzrouwfj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hnqzz.top/gtidmznlro.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.fzhhl.top/gtuytcyqsw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yj20258888.top/gtdzgvglfg.html

[F08] 遍历目录
来源：http://hz.yonumen.top/gtzvnytpsz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.daxiang520.top/gtakozrczt.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yongpay.top/gtoxcbfvbl.html

JS:   fs.readdirSync("dir")
来源：http://hz.gaohongyu789.top/gtdxsfxiny.html

TS:   fs.readdirSync("dir")
来源：http://hz.xuanzx.com/gtznziuxzo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zhongyouzk.top/gtsbkshtnw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.havefunace.top/gtrcdbruve.html

Ruby: Dir.children("dir")
来源：http://hz.chenlongwang.top/gtqrtrntnh.html

C#:   Directory.GetFiles("dir")
来源：http://hz.redwolf501.top/gtztieqzrl.html

[F09] 获取文件大小
来源：http://hz.sysykeji.top/gtxicwahgp.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zdqjudy.top/gthjihlqqh.html

PHP:  filesize("a.txt");
来源：http://hz.52xcode.cn/gtlmospxzx.html

JS:   fs.statSync("a.txt").size
来源：http://hz.hfpthk.cn/gtnoljvwic.html

TS:   fs.statSync("a.txt").size
来源：http://hz.hongshengwenyu.top/gtasdfbtzo.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.shangyingyoupin.top/gtfxbyksgw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.birdmap.top/gtxqgnhuju.html

Ruby: File.size("a.txt")
来源：http://hz.xuetiantiany.cn/gtnflfjqhs.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.gzhubu.top/gtpmbwsmke.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.chenlongwang.top/gtkqjnisxy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.sysykeji.top/gtrdpvrhqz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.chenzaomai.com/gtplhenxmu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.ywan-chungtsiang.top/gttqjwwuki.html

TS:   path.extname("a.txt")
来源：http://hz.jinghuilouyu.cn/gttacrxcpy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.birdmap.top/gtlkdtrlbc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yj20258.top/gtcvqmklza.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.xylfe.cn/gtzxpufvbz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zhongyouzk.top/gtbylpqwop.html

[F11] 复制与移动文件
来源：http://hz.yonumen.top/gttnohjiwh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.shuidangran.top/gtwbeuuzkg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.0kj1m.cn/gtywjttmxn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.aizwys.cn/gtsfieovui.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ivvv.top/gtlyzdbvnv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jqgufenzy.top/gteouqyexk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.dianchejie.cn/gtbxgdfsgc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jqgfzy.top/gtqpooufnw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.pycfn.com/gtzxpjdoxp.html

[F12] CSV 读写
来源：http://hz.wangdashe.top/gtgwukxpxo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.chenlongwang.top/gtlotrdsjl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.haohaochexian.top/gtngpfuplg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zhixingplan.top/gtbyahhgcj.html

TS:   // 同上
来源：http://hz.zhaomingkeji.xyz/gtexknnxik.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.gogol.net.cn/gtmvximire.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.cdnleiting.top/gtrprzgoed.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.gaohongyu789.top/gteqcprjui.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.ehwqpu.com/gttonghexj.html

================================================================================
来源：http://hz.316326.xyz/gtbqfmkhou.html

G. 面向对象
来源：http://hz.jiagoushi.top/gthxyvqldj.html

================================================================================
来源：http://hz.bjfxy.top/gthccioqlm.html

[G01] 定义类
来源：http://hz.zdqjudy.top/gtbclfkijq.html

Py:   class User: pass
来源：http://hz.hnqzz.top/gtlhoqbqqc.html

PHP:  class User {}
来源：http://hz.yongpay.top/gthtyhpshz.html

JS:   class User {}
来源：http://hz.zhixingplan.top/gtevgbqcxe.html

TS:   class User { name: string = ""; }
来源：http://hz.havefunace.top/gtnogvbhyz.html

Java: class User {}
来源：http://hz.tanke756.top/gtgnesxtap.html

Go:   type User struct { Name string }
来源：http://hz.jqgufenzy.top/gtmvdtspzl.html

Ruby: class User; end
来源：http://hz.bjfxy.top/gtlwuuhjwi.html

C#:   class User {}
来源：http://hz.316326.xyz/gtfryeesls.html

[G02] 构造函数
来源：http://hz.zhaomingkeji.xyz/gtzpboyenn.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.sxryk.cn/gtelpvmvpc.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.daxiang520.top/gtqaehqjpn.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yueranfly.top/gtewgotriy.html

TS:   constructor(public name: string) {}
来源：http://hz.jinyuanbaomall.cn/gtqxxppwpe.html

Java: User(String name) { this.name = name; }
来源：http://hz.chenzaomai.com/gtifaaxsxf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zhoulong.xyz/gtnpjqkjms.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.zhengqikj.top/gtoukqtnta.html

C#:   public User(string name) { Name = name; }
来源：http://hz.xuetiantiany.cn/gtvsnwznya.html

[G03] 实例属性
来源：http://hz.chenzaomai.com/gtrhekurzt.html

Py:   self.name = "x"
来源：http://hz.aizwys.cn/gtapswwzio.html

PHP:  public string $name = "x";
来源：http://hz.bjfxy.top/gtqeaajskv.html

JS:   this.name = "x";
来源：http://hz.chenjidiqi.icu/gtlldyduhp.html

TS:   name: string = "x";
来源：http://hz.316326.xyz/gtcqatfssl.html

Java: private String name;
来源：http://hz.316326.xyz/gtchoyedqo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.wangshuangyany.cn/gtgxpglstu.html

Ruby: @name = "x"
来源：http://hz.sweek.top/gtcxxhmrtb.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.gotoacloud.top/gtsydsppxx.html

[G04] 定义方法
来源：http://hz.zhiwuduotai.top/gtgnmkmiza.html

Py:   def greet(self): return self.name
来源：http://hz.nanxinkj.top/gtttfkyuuc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.ybcxt.top/gtwflimnyp.html

JS:   greet() { return this.name; }
来源：http://hz.shanyushiyangkeji.top/gtmsahjtem.html

TS:   greet(): string { return this.name; }
来源：http://hz.52xcode.cn/gttfoajadc.html

Java: String greet() { return name; }
来源：http://hz.ydjk.org.cn/gtzcfhobgi.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yangfankeji.com/gtwqagfswz.html

Ruby: def greet; @name; end
来源：http://hz.hongshengwenyu.top/gtspttuwdq.html

C#:   public string Greet() => Name;
来源：http://hz.sweek.top/gtlovrkvek.html

[G05] 继承
来源：http://hz.gotoacloud.top/gtebljyoej.html

Py:   class Admin(User): pass
来源：http://hz.andypj.xyz/gtswhnkccp.html

PHP:  class Admin extends User {}
来源：http://hz.hysaishi.cn/gtprbspsbw.html

JS:   class Admin extends User {}
来源：http://hz.cqqwz.cn/gtxtsvdnqv.html

TS:   class Admin extends User {}
来源：http://hz.aizwys.cn/gtwfihrcgm.html

Java: class Admin extends User {}
来源：http://hz.shanyushiyangkeji.top/gtzvtintbn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yvedp.cn/gtljkjvkff.html

Ruby: class Admin < User; end
来源：http://hz.yonumen.top/gtvsgaergz.html

C#:   class Admin : User {}
来源：http://hz.hnxiangtu.top/gtcpesouxv.html

[G06] 重写方法
来源：http://hz.tanke756.top/gtrcrrrsnx.html

Py:   def greet(self): return "admin"
来源：http://hz.zhijiandao.cn/gtuzckutgk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.tanke756.top/gtazuvencs.html

JS:   greet() { return "admin"; }
来源：http://hz.sweek.top/gtiybsnbjb.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jqgufenzy.top/gtezgcvgwj.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhoulong.xyz/gtmsrcbeyf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.wangdashe.top/gtjalnoene.html

Ruby: def greet; "admin"; end
来源：http://hz.snrcjt.cn/gtvebtdcsy.html

C#:   public override string Greet() => "admin";
来源：http://hz.chenlongwang.top/gtlghsfrvi.html

[G07] 调用父类方法
来源：http://hz.dashuyun.cn/gtrzqcivqt.html

Py:   super().greet()
来源：http://hz.cucudq.cn/gtrltsfuuq.html

PHP:  parent::greet();
来源：http://hz.9152youxi.cn/gtramtmxse.html

JS:   super.greet();
来源：http://hz.jinghuilouyu.cn/gtfvejysmm.html

TS:   super.greet();
来源：http://hz.chenjidiqi.icu/gtiyvtxlur.html

Java: super.greet();
来源：http://hz.havefunace.top/gtgdimnvqu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.shangyingyoupin.top/gtezxlogjz.html

Ruby: super
来源：http://hz.sufxvd.cn/gtidihkywr.html

C#:   base.Greet();
来源：http://hz.tanke756.top/gtkftlsqpr.html

[G08] 静态方法与属性
来源：http://hz.svipenyu.cn/gtctewikoh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jinqigufen.top/gtmcbiutvy.html

PHP:  public static function f() {}
来源：http://hz.daxiang520.top/gtdfruxmhr.html

JS:   static f() {}
来源：http://hz.yvedp.cn/gtthqwabyf.html

TS:   static f(): void {}
来源：http://hz.hnxiangtu.top/gtuqrgkxgt.html

Java: static void f() {}
来源：http://hz.yvedp.cn/gtegqmciuu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.c1oappe.top/gtnwcuxggr.html

Ruby: def self.f; end
来源：http://hz.pengpengdd.cyou/gtfyecphhn.html

C#:   public static void F() {}
来源：http://hz.xingfuxueyuan.xyz/gtiifutvoe.html

[G09] 接口 / 抽象类
来源：http://hz.hongshengwenyu.top/gtycnbpoja.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.andypj.xyz/gtkhvuxcse.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.xinyue.icu/gtgrzuthws.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.hfpthk.cn/gtdcgfaewj.html

TS:   interface Shape { area(): number; }
来源：http://hz.quarkkingdee.top/gtmmvsdcok.html

Java: interface Shape { double area(); }
来源：http://hz.hnqzz.top/gtwklnhkto.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.aibaodan.cn/gthbvajnrz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.fengsongda.top/gtbrahnaig.html

C#:   interface IShape { double Area(); }
来源：http://hz.andypj.xyz/gtpzlpnrzd.html

[G10] 访问控制
来源：http://hz.xuetiantiany.cn/gtuuwjoymd.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.52xcode.cn/gtbltioevi.html

PHP:  public / protected / private
来源：http://hz.zdqjudy.top/gtzjdupkvo.html

JS:   #private 字段；其余公开
来源：http://hz.ivvv.top/gtervduxxz.html

TS:   public / protected / private
来源：http://hz.yj20258888.top/gtjvavnjuy.html

Java: public / protected / private / 默认包级
来源：http://hz.hongshengwenyu.top/gtxkbdeguc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ybcxt.top/gtajedhrha.html

Ruby: public / protected / private
来源：http://hz.52xcode.cn/gtfafgnpid.html

C#:   public / protected / private / internal
来源：http://hz.redwolf501.top/gtzgjfidtc.html

[G11] getter / setter
来源：http://hz.zhengqikj.top/gtqhwugekn.html

Py:   @property 与 @x.setter
来源：http://hz.zhiwuduotai.top/gtkdjzwdab.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.tianlin.xyz/gtqiolifkn.html

JS:   get name() { return this._name; }
来源：http://hz.jlsjyb.cn/gtyufojbmc.html

TS:   get name(): string { return this._name; }
来源：http://hz.chenlongwang.top/gtafpbgrnh.html

Java: public String getName() { return name; }
来源：http://hz.xylfe.cn/gtxsgrdudq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.aibaodan.cn/gtjnguwxaj.html

Ruby: attr_accessor :name
来源：http://hz.hfpthk.cn/gticnvghuq.html

C#:   public string Name { get; set; }
来源：http://hz.gzhubu.top/gtczjhxytt.html

[G12] 对象转字符串
来源：http://hz.zhoulong.xyz/gtycwvmkjf.html

Py:   def __str__(self): return self.name
来源：http://hz.mhx1999.top/gtuaeoibpq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.nanxuanxn.top/gtxmodrynk.html

JS:   toString() { return this.name; }
来源：http://hz.hywenlv.cn/gtqlvuszum.html

TS:   toString(): string { return this.name; }
来源：http://hz.ivvv.top/gtgmvgjskt.html

Java: @Override public String toString() { return name; }
来源：http://hz.chenzaomai.com/gtwnndnxoc.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhijiandao.cn/gtncswfvmd.html

Ruby: def to_s; @name; end
来源：http://hz.tianlin.xyz/gtnylcnkmk.html

C#:   public override string ToString() => Name;
来源：http://hz.yanxiufei.cn/gtgwgrddab.html

[G13] 判断对象类型
来源：http://hz.xinyue.icu/gthzpksasv.html

Py:   isinstance(u, User)
来源：http://hz.shanyushiyangtech.top/gtiopafznh.html

PHP:  $u instanceof User
来源：http://hz.yj20258888.top/gtjfovzmfe.html

JS:   u instanceof User
来源：http://hz.jinghuilouyu.cn/gtagqusnec.html

TS:   u instanceof User
来源：http://hz.kuanghao11.cn/gtfwjfjdyc.html

Java: u instanceof User
来源：http://hz.sufxvd.cn/gtshlksyea.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.chenzaomai.com/gtdubbnsra.html

Ruby: u.is_a?(User)
来源：http://hz.zhiwuduotai.top/gtzykvpngh.html

C#:   u is User
来源：http://hz.yangfankeji.com/gtugcagunr.html

[G14] 数据类 / record
来源：http://hz.jinqigufen.top/gtqujkpfsa.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.cucudq.cn/gtnnffdbbq.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.havefunace.top/gtvagryzos.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhiwuduotai.top/gtsyyxxwky.html

TS:   type User = { name: string; age: number };
来源：http://hz.nanxinkj.top/gtsqiiakln.html

Java: record User(String name, int age) {}
来源：http://hz.zhoulong.xyz/gtcwgbccos.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jinyuanbaomall.cn/gtmplzgvey.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.ydjk.org.cn/gtlukejfnz.html

C#:   record User(string Name, int Age);
来源：http://hz.xingfuxueyuan.xyz/gtxijzafxf.html

[G15] 枚举
来源：http://hz.guannengcc.top/gtfkyjrpvm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.gzhubu.top/gtprwtrnfw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.bjfxy.top/gteccmphfm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yj20258888.top/gtymrhqxdw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jqgufenzy.top/gtzmrghjth.html

Java: enum Color { RED, GREEN }
来源：http://hz.zdqjudy.top/gtglqoymns.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.haohaochexian.top/gtyosesjyk.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yj20258.top/gtivmdqpmb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.birdmap.top/gtowzwdghi.html

[G16] 对象转数组 / 字典
来源：http://hz.cucudq.cn/gtabzllgzh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.xinyue.icu/gtbconitro.html

PHP:  get_object_vars($obj);
来源：http://hz.hywenlv.cn/gtlvezujsp.html

JS:   Object.entries(obj)
来源：http://hz.hfpthk.cn/gtravmbvqa.html

TS:   Object.entries(obj)
来源：http://hz.guannengcc.top/gtjdgrbtuh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.xuanzx.com/gtnxqijkwk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hongshengwenyu.top/gtavcawdnw.html

Ruby: obj.instance_variables
来源：http://hz.chenzaomai.com/gtzihhcizq.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.nwbrower.top/gtbdrwiaho.html

================================================================================
来源：http://hz.hfpthk.cn/gtcprjxxgn.html

H. 异常与错误处理
来源：http://hz.tianlin.xyz/gtpnyyfmcr.html

================================================================================
来源：http://hz.pycfn.com/gtebatulcb.html

[H01] try / catch 基础
来源：http://hz.tianlin.xyz/gtrqcdrmgi.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.xinyue.icu/gttskulgqd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.gogol.net.cn/gtjzmaeehz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.kuanghao11.cn/gtygotltph.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hysaishi.cn/gtowekhxtv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zhixingplan.top/gthcuimvmc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zhoulong.xyz/gtaptsoxqs.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.fengsongda.top/gtcdrabjcb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.gogol.net.cn/gttczmpubq.html

[H02] finally / ensure 收尾
来源：http://hz.ehwqpu.com/gtesyovqjh.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.9152youxi.cn/gtnhfgttou.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhaomingkeji.xyz/gtuylmvamj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.xuetiantiany.cn/gthrznmuaa.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.vqdsnc.cn/gtsfiyyaer.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.snrcjt.cn/gtgniymnzj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.dianchejie.cn/gtbkqydinm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.tian-w.cn/gtalqmdoem.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hfpthk.cn/gtwpwqgyao.html

[H03] 主动抛出异常
来源：http://hz.ywan-chungtsiang.top/gtoowhraga.html

Py:   raise ValueError("错误信息")
来源：http://hz.jianghu66.top/gtrexzgpse.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yonumen.top/gtxparpbhf.html

JS:   throw new Error("错误信息");
来源：http://hz.quarkkingdee.top/gtkuigvhfk.html

TS:   throw new Error("错误信息");
来源：http://hz.pycfn.com/gtvkjeryxx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.9152youxi.cn/gtfayuzfdj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.ydjk.org.cn/gtdmpjuspy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yangfankeji.com/gtnyskykow.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.hammf.cn/gtufsyzrmz.html

[H04] 自定义异常类型
来源：http://hz.tanke756.top/gtvstcaicm.html

Py:   class MyError(Exception): pass
来源：http://hz.316326.xyz/gtfduxbgpe.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.fzhhl.top/gtrtijuuyh.html

JS:   class MyError extends Error {}
来源：http://hz.svipenyu.cn/gtyvzenpgd.html

TS:   class MyError extends Error {}
来源：http://hz.fzhhl.top/gtuwracjij.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zhiwuduotai.top/gtphqipukp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.shanyushiyangtech.top/gtekllelyu.html

Ruby: class MyError < StandardError; end
来源：http://hz.ivvv.top/gtpvozcndx.html

C#:   class MyException : Exception {}
来源：http://hz.pengpengdd.cyou/gtqknymymx.html

[H05] 捕获特定类型
来源：http://hz.jinghuilouyu.cn/gtxhjabunm.html

Py:   except ValueError as e:
来源：http://hz.pengpengdd.cyou/gtsvvokyrv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jinyuanbaomall.cn/gtlddnjdkc.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.pengpengdd.cyou/gtgrjfbtoc.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.snrcjt.cn/gtolxaflzo.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.bjfxy.top/gtcqyyyadh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.dashuyun.cn/gtvhxinlgj.html

Ruby: rescue ArgumentError => e
来源：http://hz.zhoulong.xyz/gtewgzauuf.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yj20258.top/gtrpilrqep.html

[H06] 可选值 / 空值安全访问
来源：http://hz.cdnleiting.top/gtxqibgoom.html

Py:   value = d.get("k") or default
来源：http://hz.chenjidiqi.icu/gtintrxado.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hfpthk.cn/gteyyhdglh.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yuanzhike.top/gtupgqdnoa.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yj20258888.top/gtdblzquru.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jianghu66.top/gtnrcczelp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.vqdsnc.cn/gtyeucbbkg.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jqgufenzy.top/gtqwnllflz.html

C#:   obj?.A?.B ?? default
来源：http://hz.aizwys.cn/gtcaphhxkk.html

[H07] 断言
来源：http://hz.gaohongyu789.top/gtucofcvot.html

Py:   assert x > 0, "必须为正"
来源：http://hz.chenjidiqi.icu/gtisrwzpkn.html

PHP:  assert($x > 0);
来源：http://hz.birdmap.top/gtrzhfptpx.html

JS:   console.assert(x > 0);
来源：http://hz.aizwys.cn/gthwcacqeq.html

TS:   console.assert(x > 0);
来源：http://hz.aizwys.cn/gttuemiqcw.html

Java: assert x > 0 : "必须为正";
来源：http://hz.cqqwz.cn/gtuldebsij.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.hammf.cn/gthffpkdqb.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.nanxinkj.top/gthvrfawwa.html

C#:   Debug.Assert(x > 0);
来源：http://hz.fzhhl.top/gtnysvyros.html

[H08] 获取错误信息与堆栈
来源：http://hz.cqqwz.cn/gtjoigtshh.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zdqjudy.top/gtzooymvgb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jianghu66.top/gtpdqgfdvq.html

JS:   e.message;  e.stack
来源：http://hz.zhijiandao.cn/gtwbwcdltx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jinqigfzy.top/gtxrjihbnl.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jinyuanbaomall.cn/gtdtosyiyt.html

Go:   err.Error()
来源：http://hz.xylfe.cn/gtuymavtms.html

Ruby: e.message;  e.backtrace
来源：http://hz.jiagoushi.top/gtnnxhpppa.html

C#:   e.Message;  e.StackTrace
来源：http://hz.xuanzx.com/gtcldqybpf.html

[H09] 带错误码的异常
来源：http://hz.sxryk.cn/gtzmhfbdkv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.nwbrower.top/gtnzsduhuk.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jinqigfzy.top/gtcnxlyumb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.c1oappe.top/gtxivoxysk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.shuidangran.top/gtfxjacpam.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.tianlin.xyz/gtzetuyhds.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.sxryk.cn/gtfqpwpcqq.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.ydzc1.top/gtomswuxln.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.chenlongwang.top/gtwkbjqbwm.html

[H10] 资源自动释放
来源：http://hz.feifeiyinyue.top/gtbtmjnlbs.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yj20258888.top/gtdbralyup.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.dashuyun.cn/gticeaaqyy.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hnxiangtu.top/gtsvdpoxno.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shanyushiyangtech.top/gtvotteysf.html


<!-- 参考信息 -->