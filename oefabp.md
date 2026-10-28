代发 wailian999

C#:   File.Exists("a.txt")
来源：http://hz.yuanzhike.top/gtuxewszot.html

[F06] 删除文件
来源：http://hz.birdmap.top/gtistjbabd.html

Py:   os.remove("a.txt")
来源：http://hz.nanxinkj.top/gtmmsqjjok.html

PHP:  unlink("a.txt");
来源：http://hz.ydjk.org.cn/gtwtrwkdvr.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.wangdashe.top/gtqvthilpe.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yanxiufei.cn/gtgfyhkvpz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yj20258.top/gtnhwxbkfn.html

Go:   os.Remove("a.txt")
来源：http://hz.shanyushiyangtech.top/gtrowmzpuu.html

Ruby: File.delete("a.txt")
来源：http://hz.haohaochexian.top/gtpllievxm.html

C#:   File.Delete("a.txt");
来源：http://hz.yj20258888.top/gtpnfgwpwn.html

[F07] 创建目录（含多级）
来源：http://hz.sxryk.cn/gtsdunxbzw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yj202588.top/gtiefcnigi.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.cheryme.top/gtczdnrirm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.dashuyun.cn/gtjmdtkzge.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cheryme.top/gtizmvtsmj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yueranfly.top/gtialrswzj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.wangdashe.top/gtsvbhsbnw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yanxiufei.cn/gtnqvdnbpq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.sxryk.cn/gtqbiwiivs.html

[F08] 遍历目录
来源：http://hz.yvedp.cn/gtmemqukvl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.sweek.top/gtgghvglyj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.ybcxt.top/gtpkmkmrcm.html

JS:   fs.readdirSync("dir")
来源：http://hz.quarkkingdee.top/gtoyilmusg.html

TS:   fs.readdirSync("dir")
来源：http://hz.tian-w.cn/gtwxxreeoa.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.wangshuangyany.cn/gtundtcrwh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.wangshuangyany.cn/gtdjdkmxiu.html

Ruby: Dir.children("dir")
来源：http://hz.zhixingplan.top/gtnbojryqw.html

C#:   Directory.GetFiles("dir")
来源：http://hz.wangdashe.top/gtkflkpzvi.html

[F09] 获取文件大小
来源：http://hz.jianghu66.top/gtvxthcqsh.html

Py:   os.path.getsize("a.txt")
来源：http://hz.birdmap.top/gtzzcknjhk.html

PHP:  filesize("a.txt");
来源：http://hz.zhixingplan.top/gtuvscmytr.html

JS:   fs.statSync("a.txt").size
来源：http://hz.xuetiantiany.cn/gttvwwukpo.html

TS:   fs.statSync("a.txt").size
来源：http://hz.ydjk.org.cn/gtsqaukkxq.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.kuanghao11.cn/gthwipqhoc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jinghuilouyu.cn/gthfppftxt.html

Ruby: File.size("a.txt")
来源：http://hz.smart0.xyz/gtovfhgref.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.pycfn.com/gtofgdkagl.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hnqzz.top/gtcffpmlct.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.pengpengdd.cyou/gtqifaqzmp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yvedp.cn/gtuadhkxrw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yonumen.top/gtbdfwbtmp.html

TS:   path.extname("a.txt")
来源：http://hz.mhx1999.top/gtjtsgxlee.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jiagoushi.top/gtwlcdvfqi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zhaomingkeji.xyz/gthtfpycmn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.shangyingyoupin.top/gtoiosiclu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jinqigfzy.top/gtvxxytlgq.html

[F11] 复制与移动文件
来源：http://hz.mhx1999.top/gtdirmsggg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.chenzaomai.com/gtbtjwewxl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.aibaodan.cn/gtdunybmhq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yuxming.cn/gtzmdzqvfs.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jianghu66.top/gtnnkmxjwn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zhengqikj.top/gtumattpgh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.xuetiantiany.cn/gtuwevwsuv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.andypj.xyz/gtbrbjllti.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.gzhubu.top/gtstymxpvj.html

[F12] CSV 读写
来源：http://hz.gotoacloud.top/gtexztjmnn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.pengpengdd.cyou/gtdjtqrypn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hammf.cn/gtyqegtkcp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.xylfe.cn/gtwqtfvwtf.html

TS:   // 同上
来源：http://hz.cqqwz.cn/gtrfzvclji.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.svipenyu.cn/gtbvmuafei.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.shanyushiyangkeji.top/gtacprpzms.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yuxming.cn/gtqvmdhgho.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.gzhubu.top/gtyhpvlihk.html

================================================================================
来源：http://hz.wangdashe.top/gtnxawepgn.html

G. 面向对象
来源：http://hz.shzxlz.cn/gtyfbnmeqi.html

================================================================================
来源：http://hz.daria6918.cn/gtrqzrdxun.html

[G01] 定义类
来源：http://hz.zdqjudy.top/gtjmteapiu.html

Py:   class User: pass
来源：http://hz.snrcjt.cn/gtksopykce.html

PHP:  class User {}
来源：http://hz.52xcode.cn/gtespkjfil.html

JS:   class User {}
来源：http://hz.xylfe.cn/gtzhhdtkrr.html

TS:   class User { name: string = ""; }
来源：http://hz.xziqi.cn/gtaqilcgys.html

Java: class User {}
来源：http://hz.hongshengwenyu.top/gtajnkrwnm.html

Go:   type User struct { Name string }
来源：http://hz.cheryme.top/gtsbifvuqb.html

Ruby: class User; end
来源：http://hz.xuetiantiany.cn/gtizzfkwje.html

C#:   class User {}
来源：http://hz.shanyushiyangkeji.top/gtnzbzfryj.html

[G02] 构造函数
来源：http://hz.yonumen.top/gtbdqbjkhe.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.birdmap.top/gtltbqburx.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.snrcjt.cn/gtqcroppgi.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.cucudq.cn/gtnsmpiwny.html

TS:   constructor(public name: string) {}
来源：http://hz.ydzc1.top/gtgteeurnk.html

Java: User(String name) { this.name = name; }
来源：http://hz.ppjwa.cn/gtijyfecok.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yanxiufei.cn/gtjdylldxs.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.aibaodan.cn/gtixjdvack.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zycfv.cn/gtjbrznuub.html

[G03] 实例属性
来源：http://hz.sweek.top/gtpkxtehga.html

Py:   self.name = "x"
来源：http://hz.jinghuilouyu.cn/gttcfkqfqv.html

PHP:  public string $name = "x";
来源：http://hz.xuetiantiany.cn/gtgoeszvgs.html

JS:   this.name = "x";
来源：http://hz.shangyingyoupin.top/gtfviwqoad.html

TS:   name: string = "x";
来源：http://hz.c1oappe.top/gtaotrwhyw.html

Java: private String name;
来源：http://hz.hammf.cn/gthpphhipb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.cashguo.top/gtkbsnvcvj.html

Ruby: @name = "x"
来源：http://hz.yj20258.top/gtzdpxjdpm.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.dashuyun.cn/gtpuptweln.html

[G04] 定义方法
来源：http://hz.zhixingplan.top/gtlvlvbsoq.html

Py:   def greet(self): return self.name
来源：http://hz.tanke756.top/gtregmpboq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.ydjk.org.cn/gtvammonny.html

JS:   greet() { return this.name; }
来源：http://hz.jinghuilouyu.cn/gtodkcvtfm.html

TS:   greet(): string { return this.name; }
来源：http://hz.jinghuilouyu.cn/gtnfqqfjgv.html

Java: String greet() { return name; }
来源：http://hz.ehwqpu.com/gtbuurelix.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.daria6918.cn/gttcacklsc.html

Ruby: def greet; @name; end
来源：http://hz.bjfxy.top/gtpewhnwch.html

C#:   public string Greet() => Name;
来源：http://hz.yanxiufei.cn/gtnetdxeuw.html

[G05] 继承
来源：http://hz.zhijiandao.cn/gtmsgbrwzy.html

Py:   class Admin(User): pass
来源：http://hz.nwbrower.top/gtxrjdljqz.html

PHP:  class Admin extends User {}
来源：http://hz.shangyingyoupin.top/gtlpdhntco.html

JS:   class Admin extends User {}
来源：http://hz.ydjk.org.cn/gtyiejxbuf.html

TS:   class Admin extends User {}
来源：http://hz.tanke756.top/gtugblrnep.html

Java: class Admin extends User {}
来源：http://hz.yanxiufei.cn/gtdljgwwuv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.tanke756.top/gtslrwcgan.html

Ruby: class Admin < User; end
来源：http://hz.chenzaomai.com/gtchzycxzq.html

C#:   class Admin : User {}
来源：http://hz.jiagoushi.top/gtkgrbhaom.html

[G06] 重写方法
来源：http://hz.gaohongyu789.top/gtipowbxue.html

Py:   def greet(self): return "admin"
来源：http://hz.xziqi.cn/gtadxnbfoz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.guannengcc.top/gtriknxhyn.html

JS:   greet() { return "admin"; }
来源：http://hz.zhijiandao.cn/gtyiemcxsm.html

TS:   greet(): string { return "admin"; }
来源：http://hz.9152youxi.cn/gtfceygnnu.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jinqigfzy.top/gtvvdgdvbk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.guannengcc.top/gtpnsaexfz.html

Ruby: def greet; "admin"; end
来源：http://hz.shangyingyoupin.top/gtelslszof.html

C#:   public override string Greet() => "admin";
来源：http://hz.fzhhl.top/gtfkalggya.html

[G07] 调用父类方法
来源：http://hz.wangdashe.top/gtxblfsafj.html

Py:   super().greet()
来源：http://hz.aizwys.cn/gtyuohjbwb.html

PHP:  parent::greet();
来源：http://hz.smart0.xyz/gtxsoidzgk.html

JS:   super.greet();
来源：http://hz.daxiang520.top/gtelpbkgat.html

TS:   super.greet();
来源：http://hz.zhongyouzk.top/gtubccqjsi.html

Java: super.greet();
来源：http://hz.shanyushiyangtech.top/gtbodsqurg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.316326.xyz/gthnlryyhh.html

Ruby: super
来源：http://hz.wangdashe.top/gtnsnahyic.html

C#:   base.Greet();
来源：http://hz.jianghu66.top/gtgrqiyxyh.html

[G08] 静态方法与属性
来源：http://hz.haohaochexian.top/gtfuvvooww.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.sxryk.cn/gtegjvwrhz.html

PHP:  public static function f() {}
来源：http://hz.xinyue.icu/gtenjdefrh.html

JS:   static f() {}
来源：http://hz.snrcjt.cn/gtmxzilovs.html

TS:   static f(): void {}
来源：http://hz.zhaomingkeji.xyz/gtahkljdpx.html

Java: static void f() {}
来源：http://hz.zhengqikj.top/gthuqkmiwh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhixingplan.top/gtigtrelsq.html

Ruby: def self.f; end
来源：http://hz.zycfv.cn/gthjjoqxnq.html

C#:   public static void F() {}
来源：http://hz.yj20258.top/gtycxglitu.html

[G09] 接口 / 抽象类
来源：http://hz.cheryme.top/gtuyaarssw.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.dianchejie.cn/gtsmyunlbi.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yuxming.cn/gtdynpuvnr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.xingfuxueyuan.xyz/gtyzwdxrzb.html

TS:   interface Shape { area(): number; }
来源：http://hz.gogol.net.cn/gtkhdaskxj.html

Java: interface Shape { double area(); }
来源：http://hz.nanxuanxn.top/gtguqzrohv.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.havefunace.top/gtcywruksf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.sxryk.cn/gtalanxrqe.html

C#:   interface IShape { double Area(); }
来源：http://hz.tian-w.cn/gtrsltmcvf.html

[G10] 访问控制
来源：http://hz.fengsongda.top/gtzwdmatpj.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.kuanghao11.cn/gttntqvmqu.html

PHP:  public / protected / private
来源：http://hz.jinghuilouyu.cn/gtazkptxkd.html

JS:   #private 字段；其余公开
来源：http://hz.yj202588.top/gtbszrkvad.html

TS:   public / protected / private
来源：http://hz.guannengcc.top/gtzwpqncqx.html

Java: public / protected / private / 默认包级
来源：http://hz.jianghu66.top/gtfwsibsrx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yj20258888.top/gtajcrysbn.html

Ruby: public / protected / private
来源：http://hz.yongpay.top/gtfdohhuuj.html

C#:   public / protected / private / internal
来源：http://hz.c1oappe.top/gturpqlswz.html

[G11] getter / setter
来源：http://hz.zhoulong.xyz/gtzthgawxd.html

Py:   @property 与 @x.setter
来源：http://hz.snrcjt.cn/gtddgabkhc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zdqjudy.top/gtybocqeyp.html

JS:   get name() { return this._name; }
来源：http://hz.gotoacloud.top/gtstsbpprn.html

TS:   get name(): string { return this._name; }
来源：http://hz.wangdashe.top/gtjoetqquy.html

Java: public String getName() { return name; }
来源：http://hz.shanyushiyangtech.top/gtmcmaquyi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.chenjidiqi.icu/gtzjyrxezg.html

Ruby: attr_accessor :name
来源：http://hz.hfpthk.cn/gtirbahhph.html

C#:   public string Name { get; set; }
来源：http://hz.zhengqikj.top/gtsadkegay.html

[G12] 对象转字符串
来源：http://hz.316326.xyz/gthwugjjvr.html

Py:   def __str__(self): return self.name
来源：http://hz.xylfe.cn/gtwojiudem.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.aizwys.cn/gtucvusniy.html

JS:   toString() { return this.name; }
来源：http://hz.iojbl.cn/gtqcatpikg.html

TS:   toString(): string { return this.name; }
来源：http://hz.jianghu66.top/gtgvzhrnfq.html

Java: @Override public String toString() { return name; }
来源：http://hz.shanyushiyangkeji.top/gtbvihidtr.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.xuanzx.com/gtszwtwfkv.html

Ruby: def to_s; @name; end
来源：http://hz.cheryme.top/gtgkedsydp.html

C#:   public override string ToString() => Name;
来源：http://hz.snrcjt.cn/gtiydtblfc.html

[G13] 判断对象类型
来源：http://hz.xinyue.icu/gtdrijuuzf.html

Py:   isinstance(u, User)
来源：http://hz.gotoacloud.top/gtvbaudnwv.html

PHP:  $u instanceof User
来源：http://hz.mhx1999.top/gtwxwzqjqz.html

JS:   u instanceof User
来源：http://hz.xuanzx.com/gtlxrvehmu.html

TS:   u instanceof User
来源：http://hz.gaohongyu789.top/gtkvrezmwb.html

Java: u instanceof User
来源：http://hz.gaohongyu789.top/gtrjaopqhx.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jinghuilouyu.cn/gtmyhaemxh.html

Ruby: u.is_a?(User)
来源：http://hz.tianlin.xyz/gtszwmqipt.html

C#:   u is User
来源：http://hz.zhixingplan.top/gtoipvcqhl.html

[G14] 数据类 / record
来源：http://hz.gotoacloud.top/gthruanord.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.havefunace.top/gtwujidchc.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zhongyouzk.top/gtgujfnhiq.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jyoumei.cn/gtuqkosixo.html

TS:   type User = { name: string; age: number };
来源：http://hz.xingfuxueyuan.xyz/gtlwveourc.html

Java: record User(String name, int age) {}
来源：http://hz.nwbrower.top/gtxjuoymlf.html

Go:   type User struct { Name string; Age int }
来源：http://hz.tian-w.cn/gtssgbhiob.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.shanyushiyangkeji.top/gtbenyditl.html

C#:   record User(string Name, int Age);
来源：http://hz.zhongyouzk.top/gtbgzhvpfq.html

[G15] 枚举
来源：http://hz.jqgufenzy.top/gtxnlzvimp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zhoulong.xyz/gtzjcbvyyq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.316326.xyz/gtokbfqcqm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.redwolf501.top/gtfvbttnkr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.0kj1m.cn/gttifkiqgk.html

Java: enum Color { RED, GREEN }
来源：http://hz.redwolf501.top/gttzsetwin.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jqgufenzy.top/gtddxpaopf.html

Ruby: Color = %i[red green].freeze
来源：http://hz.cdnleiting.top/gttqcdhxth.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.havefunace.top/gthvjycszd.html

[G16] 对象转数组 / 字典
来源：http://hz.zhiwuduotai.top/gtjcvsufue.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhixingplan.top/gtpdeslorx.html

PHP:  get_object_vars($obj);
来源：http://hz.feifeiyinyue.top/gtvgbjugoz.html

JS:   Object.entries(obj)
来源：http://hz.c1oappe.top/gtzuogojio.html

TS:   Object.entries(obj)
来源：http://hz.gotoacloud.top/gtpsrayecq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yangfankeji.com/gtlxyvzkfm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.cdnleiting.top/gtdismsgph.html

Ruby: obj.instance_variables
来源：http://hz.yangfankeji.com/gtjbydzjst.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.daria6918.cn/gtqptrbzdl.html

================================================================================
来源：http://hz.zhengqikj.top/gtmckkpost.html

H. 异常与错误处理
来源：http://hz.ydjk.org.cn/gtjjjsyeee.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtafmyrmdv.html

[H01] try / catch 基础
来源：http://hz.yueranfly.top/gtmejkerub.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jqgfzy.top/gtybbgasms.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.iojbl.cn/gtjiqrqnnb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.hysaishi.cn/gtkwwrmcny.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.shzxlz.cn/gtesoaemyu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.snrcjt.cn/gtcwykjygb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.smart0.xyz/gtmzcjdcgz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.fengsongda.top/gtqyzoefxt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.hysaishi.cn/gttqwgbphj.html

[H02] finally / ensure 收尾
来源：http://hz.yj20258888.top/gtvbxxosaf.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yj20258.top/gtpycnjdld.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhoulong.xyz/gteeourhhd.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jinqigfzy.top/gtaiukfxnw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.52xcode.cn/gtvnzvkyma.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jqgufenzy.top/gtpnytjzcf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ppjwa.cn/gthjhfknbd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.9152youxi.cn/gtzhofflcn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.aibaodan.cn/gtmsgqswqc.html

[H03] 主动抛出异常
来源：http://hz.zhoulong.xyz/gtrgqimuij.html

Py:   raise ValueError("错误信息")
来源：http://hz.svipenyu.cn/gttvdsymgg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yj20258.top/gtsllcobcq.html

JS:   throw new Error("错误信息");
来源：http://hz.jqgufenzy.top/gtudrqjpru.html

TS:   throw new Error("错误信息");
来源：http://hz.zdqjudy.top/gtsknmrzum.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.c1oappe.top/gtbscaiamz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yangfankeji.com/gtalmiszit.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zhengqikj.top/gtyxgvrmky.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yuxming.cn/gtiapbfsew.html

[H04] 自定义异常类型
来源：http://hz.feifeiyinyue.top/gtpyhihqcp.html

Py:   class MyError(Exception): pass
来源：http://hz.chenlongwang.top/gtmzdmvrsr.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.ywan-chungtsiang.top/gtxhhanfgm.html

JS:   class MyError extends Error {}
来源：http://hz.quarkkingdee.top/gtchblpqdj.html

TS:   class MyError extends Error {}
来源：http://hz.0kj1m.cn/gtnribrrzm.html

Java: class MyException extends RuntimeException {}
来源：http://hz.hnxiangtu.top/gtwklhqabx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.daxiang520.top/gtalarqthh.html

Ruby: class MyError < StandardError; end
来源：http://hz.gzhubu.top/gttnuzqkzp.html

C#:   class MyException : Exception {}
来源：http://hz.c1oappe.top/gtgouezmiz.html

[H05] 捕获特定类型
来源：http://hz.ydjk.org.cn/gtyzzcnnvx.html

Py:   except ValueError as e:
来源：http://hz.tanke756.top/gttrrjdnlg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.shanyushiyangkeji.top/gtnihasnin.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zhongyouzk.top/gtbxrvlfkv.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhoulong.xyz/gtseoaeikj.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.xylfe.cn/gteqkpkxkx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.shanyushiyangkeji.top/gtpbcpebrr.html

Ruby: rescue ArgumentError => e
来源：http://hz.0kj1m.cn/gtrltzbjxc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.shuidangran.top/gtufruadjc.html

[H06] 可选值 / 空值安全访问
来源：http://hz.ybcxt.top/gtjckigbci.html

Py:   value = d.get("k") or default
来源：http://hz.kuanghao11.cn/gtuvimvqui.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hnxiangtu.top/gtiqvemfkg.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.xylfe.cn/gtphqyesff.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.nanxuanxn.top/gtoqncpszf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.shangyingyoupin.top/gtswtkrvtl.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.birdmap.top/gtanyjrwll.html

Ruby: d&.dig(:a, :b)
来源：http://hz.9152youxi.cn/gtfwgkzdak.html

C#:   obj?.A?.B ?? default
来源：http://hz.pengpengdd.cyou/gtwpxidyji.html

[H07] 断言
来源：http://hz.shanyushiyangkeji.top/gtppoywgxv.html

Py:   assert x > 0, "必须为正"
来源：http://hz.ywan-chungtsiang.top/gtswmjcbmm.html

PHP:  assert($x > 0);
来源：http://hz.svipenyu.cn/gtxezkelyn.html

JS:   console.assert(x > 0);
来源：http://hz.fengsongda.top/gthqtbkuxr.html

TS:   console.assert(x > 0);
来源：http://hz.gzhubu.top/gtaytmmoir.html

Java: assert x > 0 : "必须为正";
来源：http://hz.dashuyun.cn/gtqvbelnco.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yanxiufei.cn/gtjxxqjgaa.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.feifeiyinyue.top/gtifcecnrt.html

C#:   Debug.Assert(x > 0);
来源：http://hz.snrcjt.cn/gtqctyueke.html

[H08] 获取错误信息与堆栈
来源：http://hz.pycfn.com/gteuxckabk.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.pycfn.com/gtrcscaiuu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yuanzhike.top/gtxrxpdiqq.html

JS:   e.message;  e.stack
来源：http://hz.feifeiyinyue.top/gtyxtnuwlc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.ehwqpu.com/gtwilusjvc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.chenjidiqi.icu/gtjsifkldn.html

Go:   err.Error()
来源：http://hz.fengsongda.top/gthulnvcwu.html

Ruby: e.message;  e.backtrace
来源：http://hz.nwbrower.top/gtoeqegvab.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jinyuanbaomall.cn/gtrymjunhe.html

[H09] 带错误码的异常
来源：http://hz.sufxvd.cn/gtkwugwuke.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yanxiufei.cn/gtwfjkipte.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.xingfuxueyuan.xyz/gtgrfdwhel.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.ydzc1.top/gtjanczfwb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.guannengcc.top/gtvnpicorf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.shuidangran.top/gtxtgnkrwc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.xziqi.cn/gtodzkphhm.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.dashuyun.cn/gtmdvvfqsr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhixingplan.top/gtodeqqjle.html

[H10] 资源自动释放
来源：http://hz.jianghu66.top/gtvjxiykgv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.hnxiangtu.top/gtmksvmfow.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.tanke756.top/gtvuwkztem.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.guannengcc.top/gtkunhfdaq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.9152youxi.cn/gtzevnshsz.html


<!-- 参考信息 -->