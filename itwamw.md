代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://hz.aibaodan.cn/gtfflewboz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.svipenyu.cn/gtsxpkhrex.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.hfpthk.cn/gtyjpycedl.html

Ruby: File.exist?("a.txt")
来源：http://hz.zhiwuduotai.top/gtefquxleh.html

C#:   File.Exists("a.txt")
来源：http://hz.dashuyun.cn/gtoasjwslw.html

[F06] 删除文件
来源：http://hz.chenjidiqi.icu/gtojldwlkx.html

Py:   os.remove("a.txt")
来源：http://hz.daria6918.cn/gteddobkpa.html

PHP:  unlink("a.txt");
来源：http://hz.9152youxi.cn/gtryuioovw.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.zhijiandao.cn/gttihblpdy.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.wangshuangyany.cn/gtfkogqafg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.smart0.xyz/gtuqzyoncs.html

Go:   os.Remove("a.txt")
来源：http://hz.pycfn.com/gtddohyfwi.html

Ruby: File.delete("a.txt")
来源：http://hz.fzhhl.top/gtbalnrbwh.html

C#:   File.Delete("a.txt");
来源：http://hz.shzxlz.cn/gtjlahwmwo.html

[F07] 创建目录（含多级）
来源：http://hz.jyoumei.cn/gtlvldwoaz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.guowangkeji.top/gtbbthfbmp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.havefunace.top/gtnbulaccl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.pengpengdd.cyou/gtglamlofa.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jlsjyb.cn/gtdyqonvmu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.bjfxy.top/gtpwibvadi.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.daria6918.cn/gtlgmlqcqz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.meibo888.top/gtwykzulmt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.ydjk.org.cn/gtlhusizso.html

[F08] 遍历目录
来源：http://hz.chenlongwang.top/gtrcmoxxjy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.smart0.xyz/gtkxvzpuvm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.zhengqikj.top/gtxlcouial.html

JS:   fs.readdirSync("dir")
来源：http://hz.hfpthk.cn/gthpflqxoc.html

TS:   fs.readdirSync("dir")
来源：http://hz.quarkkingdee.top/gtvcdnlnpz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.gzhubu.top/gtixkjexqk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yangfankeji.com/gtcyzcpfdl.html

Ruby: Dir.children("dir")
来源：http://hz.zhiwuduotai.top/gtrxboqxin.html

C#:   Directory.GetFiles("dir")
来源：http://hz.ehwqpu.com/gtsaalsydp.html

[F09] 获取文件大小
来源：http://hz.316326.xyz/gtuzhfdcub.html

Py:   os.path.getsize("a.txt")
来源：http://hz.kuanghao11.cn/gtwvtwytgv.html

PHP:  filesize("a.txt");
来源：http://hz.aibaodan.cn/gtrtjincns.html

JS:   fs.statSync("a.txt").size
来源：http://hz.sweek.top/gtlgcuwlor.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yangfankeji.com/gtnwiajfjp.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.kuanghao11.cn/gtmtcbfrcc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jinyuanbaomall.cn/gtzytmyyxt.html

Ruby: File.size("a.txt")
来源：http://hz.ppjwa.cn/gtfrcxiohs.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.svipenyu.cn/gtwpqpdqzd.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zhiwuduotai.top/gtohbbnkls.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.cheryme.top/gtwmewbmsi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.c1oappe.top/gtphfzurtm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.ydjk.org.cn/gtrzldyghu.html

TS:   path.extname("a.txt")
来源：http://hz.wangdashe.top/gtkxybofap.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.hysaishi.cn/gtfvrtodsq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.vqdsnc.cn/gtiqbclmsc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.xuetiantiany.cn/gttzvjrokp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.chenjidiqi.icu/gtqejxcmff.html

[F11] 复制与移动文件
来源：http://hz.chenjidiqi.icu/gtozgesjyz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jinghuilouyu.cn/gtxjwfjozz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zycfv.cn/gtduswgvak.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.nanxuanxn.top/gtcjnnatpd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ydjk.org.cn/gtoclknpoi.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.daxiang520.top/gthzbllfvy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.hammf.cn/gtznjgbmod.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.xziqi.cn/gtsfyviaiu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhongyouzk.top/gtyhgwqawi.html

[F12] CSV 读写
来源：http://hz.xingfuxueyuan.xyz/gtecivyyrs.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.havefunace.top/gthiahrzvk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.ybcxt.top/gtepkvhnxc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.hfpthk.cn/gtttynvebd.html

TS:   // 同上
来源：http://hz.tanke756.top/gtbirhnyst.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jinqigufen.top/gtqlwydryf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jinyuanbaomall.cn/gtilkhstbi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.wangdashe.top/gtpdmqqapp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.dianchejie.cn/gtuvhmxuim.html

================================================================================
来源：http://hz.yj202588.top/gtmuujopyh.html

G. 面向对象
来源：http://hz.nanxinkj.top/gtpwhebgpm.html

================================================================================
来源：http://hz.hywenlv.cn/gterpdqrdn.html

[G01] 定义类
来源：http://hz.gzhubu.top/gtyxxrmklg.html

Py:   class User: pass
来源：http://hz.fzhhl.top/gthljemfhk.html

PHP:  class User {}
来源：http://hz.tanke756.top/gtmrllnero.html

JS:   class User {}
来源：http://hz.ydzc1.top/gtlpftqazy.html

TS:   class User { name: string = ""; }
来源：http://hz.zhengqikj.top/gttzhkhbgs.html

Java: class User {}
来源：http://hz.cdnleiting.top/gtrphvxqij.html

Go:   type User struct { Name string }
来源：http://hz.zhaomingkeji.xyz/gtmoaufnyp.html

Ruby: class User; end
来源：http://hz.hywenlv.cn/gtpshirfex.html

C#:   class User {}
来源：http://hz.jqgfzy.top/gtyjouykfo.html

[G02] 构造函数
来源：http://hz.dianchejie.cn/gtbenckcrl.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.gaohongyu789.top/gtjbubwnnk.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.bjfxy.top/gtpdtuqafq.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.tanke756.top/gticerqilc.html

TS:   constructor(public name: string) {}
来源：http://hz.yueranfly.top/gtrzdxuuyz.html

Java: User(String name) { this.name = name; }
来源：http://hz.ehwqpu.com/gtbassjgec.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jqgfzy.top/gtfifmjmxk.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.xingfuxueyuan.xyz/gtskkbjgue.html

C#:   public User(string name) { Name = name; }
来源：http://hz.sufxvd.cn/gtnbjdlwja.html

[G03] 实例属性
来源：http://hz.tianlin.xyz/gterthrppq.html

Py:   self.name = "x"
来源：http://hz.hnqzz.top/gtyvfzytar.html

PHP:  public string $name = "x";
来源：http://hz.zhiwuduotai.top/gtlnvwutor.html

JS:   this.name = "x";
来源：http://hz.yongpay.top/gtifsfjrnc.html

TS:   name: string = "x";
来源：http://hz.aizwys.cn/gtbjgfxtkj.html

Java: private String name;
来源：http://hz.wangshuangyany.cn/gtwqnvretd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.ydzc1.top/gtxeadibsi.html

Ruby: @name = "x"
来源：http://hz.aizwys.cn/gtchqwflfy.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.daria6918.cn/gtotrbullx.html

[G04] 定义方法
来源：http://hz.zhengqikj.top/gtjzcnahwi.html

Py:   def greet(self): return self.name
来源：http://hz.sxryk.cn/gtbudimnmn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.0kj1m.cn/gtmgsrreyj.html

JS:   greet() { return this.name; }
来源：http://hz.xingfuxueyuan.xyz/gtencpjrpm.html

TS:   greet(): string { return this.name; }
来源：http://hz.hysaishi.cn/gtnizuwhyb.html

Java: String greet() { return name; }
来源：http://hz.ppjwa.cn/gtggvznqwe.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.c1oappe.top/gtlmuktlpk.html

Ruby: def greet; @name; end
来源：http://hz.ivvv.top/gtfvspwlhr.html

C#:   public string Greet() => Name;
来源：http://hz.bjfxy.top/gtjpcoywlj.html

[G05] 继承
来源：http://hz.gotoacloud.top/gtfaklveld.html

Py:   class Admin(User): pass
来源：http://hz.cashguo.top/gtpxtzrkxn.html

PHP:  class Admin extends User {}
来源：http://hz.cashguo.top/gtzxdkqxfo.html

JS:   class Admin extends User {}
来源：http://hz.daria6918.cn/gtdtofjtgr.html

TS:   class Admin extends User {}
来源：http://hz.kuanghao11.cn/gtvcpfwpgc.html

Java: class Admin extends User {}
来源：http://hz.vqdsnc.cn/gtqpvweiiu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hongshengwenyu.top/gtsoenvrry.html

Ruby: class Admin < User; end
来源：http://hz.aizwys.cn/gtfztrlioa.html

C#:   class Admin : User {}
来源：http://hz.zhengqikj.top/gtpsgtnwjg.html

[G06] 重写方法
来源：http://hz.jinyuanbaomall.cn/gttykpeyzy.html

Py:   def greet(self): return "admin"
来源：http://hz.andypj.xyz/gtaxxragmv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.haohaochexian.top/gtknmxhabb.html

JS:   greet() { return "admin"; }
来源：http://hz.wangdashe.top/gtaokwibsi.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yangfankeji.com/gtwgdnenic.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yonumen.top/gtnuhkkwrj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.daria6918.cn/gtjbmkjxsf.html

Ruby: def greet; "admin"; end
来源：http://hz.jqgufenzy.top/gtnwghbycd.html

C#:   public override string Greet() => "admin";
来源：http://hz.redwolf501.top/gtrjzghuon.html

[G07] 调用父类方法
来源：http://hz.dianchejie.cn/gtcdymdghu.html

Py:   super().greet()
来源：http://hz.xuetiantiany.cn/gtnqcyjfbb.html

PHP:  parent::greet();
来源：http://hz.ybcxt.top/gtfwljehoq.html

JS:   super.greet();
来源：http://hz.xingfuxueyuan.xyz/gtoqrhtsyc.html

TS:   super.greet();
来源：http://hz.fengsongda.top/gtyifpccch.html

Java: super.greet();
来源：http://hz.yuanzhike.top/gtewvnwvyk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.hammf.cn/gtiurgrxlq.html

Ruby: super
来源：http://hz.hfpthk.cn/gtmofpdjhh.html

C#:   base.Greet();
来源：http://hz.yuxming.cn/gtccltotyk.html

[G08] 静态方法与属性
来源：http://hz.yonumen.top/gtfehomryq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yvedp.cn/gtaqxxefcj.html

PHP:  public static function f() {}
来源：http://hz.chenjidiqi.icu/gtbwnewivz.html

JS:   static f() {}
来源：http://hz.jlsjyb.cn/gtvoobkein.html

TS:   static f(): void {}
来源：http://hz.chenlongwang.top/gtyzloakjy.html

Java: static void f() {}
来源：http://hz.jlsjyb.cn/gtimjiebue.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.sxryk.cn/gtqrnyxtws.html

Ruby: def self.f; end
来源：http://hz.havefunace.top/gtdfuoqnev.html

C#:   public static void F() {}
来源：http://hz.52xcode.cn/gtpggjogzb.html

[G09] 接口 / 抽象类
来源：http://hz.jinyuanbaomall.cn/gtzpzzbsgn.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yonumen.top/gteqcgfrmx.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yvedp.cn/gtsyisfzyk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.52xcode.cn/gtkswtejzw.html

TS:   interface Shape { area(): number; }
来源：http://hz.cheryme.top/gtgtnnlkdq.html

Java: interface Shape { double area(); }
来源：http://hz.vqdsnc.cn/gtpkiuohvj.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.guannengcc.top/gttgrsjnsh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.snrcjt.cn/gtpqagilxq.html

C#:   interface IShape { double Area(); }
来源：http://hz.daxiang520.top/gttkleaqje.html

[G10] 访问控制
来源：http://hz.gogol.net.cn/gtllcqxlew.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.aibaodan.cn/gtgqfrzkse.html

PHP:  public / protected / private
来源：http://hz.shangyingyoupin.top/gttkwvvcgb.html

JS:   #private 字段；其余公开
来源：http://hz.yuxming.cn/gtxyjlyahj.html

TS:   public / protected / private
来源：http://hz.fzhhl.top/gtxqbyfrpf.html

Java: public / protected / private / 默认包级
来源：http://hz.chenjidiqi.icu/gtqenzmtiw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.svipenyu.cn/gtaqaadpqt.html

Ruby: public / protected / private
来源：http://hz.zycfv.cn/gtqpncqojq.html

C#:   public / protected / private / internal
来源：http://hz.gogol.net.cn/gtjngsfjid.html

[G11] getter / setter
来源：http://hz.xuanzx.com/gtawtjydan.html

Py:   @property 与 @x.setter
来源：http://hz.ivvv.top/gtzaqnxfrf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yuanzhike.top/gtwchfezzq.html

JS:   get name() { return this._name; }
来源：http://hz.0kj1m.cn/gthyxlhksj.html

TS:   get name(): string { return this._name; }
来源：http://hz.yvedp.cn/gtigjwmlpo.html

Java: public String getName() { return name; }
来源：http://hz.xziqi.cn/gtdxmbumzl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zhijiandao.cn/gtdmtkxoii.html

Ruby: attr_accessor :name
来源：http://hz.ybcxt.top/gtnzkaxydh.html

C#:   public string Name { get; set; }
来源：http://hz.zhijiandao.cn/gtmjiuircy.html

[G12] 对象转字符串
来源：http://hz.cheryme.top/gtpasglyge.html

Py:   def __str__(self): return self.name
来源：http://hz.zhiwuduotai.top/gtwtrgnhmk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.dashuyun.cn/gtmwwwddmv.html

JS:   toString() { return this.name; }
来源：http://hz.fzhhl.top/gtlxorjjoa.html

TS:   toString(): string { return this.name; }
来源：http://hz.havefunace.top/gtydpiarex.html

Java: @Override public String toString() { return name; }
来源：http://hz.zdqjudy.top/gtqmpkkmye.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.havefunace.top/gtrwkoyife.html

Ruby: def to_s; @name; end
来源：http://hz.aibaodan.cn/gtyizwopec.html

C#:   public override string ToString() => Name;
来源：http://hz.ivvv.top/gtdlivmclr.html

[G13] 判断对象类型
来源：http://hz.svipenyu.cn/gtkmkkfzhq.html

Py:   isinstance(u, User)
来源：http://hz.yonumen.top/gtidyurokw.html

PHP:  $u instanceof User
来源：http://hz.wangshuangyany.cn/gthlgxwwfr.html

JS:   u instanceof User
来源：http://hz.nanxinkj.top/gtspegcpor.html

TS:   u instanceof User
来源：http://hz.zycfv.cn/gtjjpqxtgg.html

Java: u instanceof User
来源：http://hz.dianchejie.cn/gtplsnfqlf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ydzc1.top/gtxjxfbqcv.html

Ruby: u.is_a?(User)
来源：http://hz.yanxiufei.cn/gtpwrugcag.html

C#:   u is User
来源：http://hz.yanxiufei.cn/gtpyblihzi.html

[G14] 数据类 / record
来源：http://hz.quarkkingdee.top/gtkpnfsfyh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zdqjudy.top/gtovycagmi.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jinghuilouyu.cn/gtfhotbwcn.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.havefunace.top/gtrhbtweji.html

TS:   type User = { name: string; age: number };
来源：http://hz.guowangkeji.top/gtbztsuzxw.html

Java: record User(String name, int age) {}
来源：http://hz.ppjwa.cn/gtwcjkwyer.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jlsjyb.cn/gtcfwnuirl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yonumen.top/gtzjntkdtq.html

C#:   record User(string Name, int Age);
来源：http://hz.yj202588.top/gtmzzcupmv.html

[G15] 枚举
来源：http://hz.xylfe.cn/gtbyxxxmyt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.xuanzx.com/gtztodvszb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.cheryme.top/gtchxkcxsb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.dianchejie.cn/gtaaljndal.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xziqi.cn/gtnljbsyxw.html

Java: enum Color { RED, GREEN }
来源：http://hz.gaohongyu789.top/gtwhllwniy.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.xziqi.cn/gtyvfrzkzk.html

Ruby: Color = %i[red green].freeze
来源：http://hz.cucudq.cn/gtujgltsvs.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yj20258888.top/gtrobwpnbx.html

[G16] 对象转数组 / 字典
来源：http://hz.yonumen.top/gtnlsclyyl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.redwolf501.top/gtfwzgperk.html

PHP:  get_object_vars($obj);
来源：http://hz.jianghu66.top/gtddttngtg.html

JS:   Object.entries(obj)
来源：http://hz.andypj.xyz/gtvhdwnvaq.html

TS:   Object.entries(obj)
来源：http://hz.quarkkingdee.top/gtzawjhttg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.gogol.net.cn/gtfqpfpnan.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hfpthk.cn/gtmmnubuqj.html

Ruby: obj.instance_variables
来源：http://hz.jiagoushi.top/gtrffjomag.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yuxming.cn/gtskqxegae.html

================================================================================
来源：http://hz.andypj.xyz/gtvnuwvgsu.html

H. 异常与错误处理
来源：http://hz.shanyushiyangkeji.top/gtotskootn.html

================================================================================
来源：http://hz.zhijiandao.cn/gtsvieylou.html

[H01] try / catch 基础
来源：http://hz.xziqi.cn/gtsjxzwolf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.mhx1999.top/gtjfepskwq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.snrcjt.cn/gtfwyyutut.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.hysaishi.cn/gtuyawuybl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.haohaochexian.top/gtkvhlpuzd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.cdnleiting.top/gtaqflpvud.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.mhx1999.top/gtrwdmdtkg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.sufxvd.cn/gtzmmnvjbd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.kuanghao11.cn/gtzwxyfvot.html

[H02] finally / ensure 收尾
来源：http://hz.hnqzz.top/gtbbtzlwpb.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.nwbrower.top/gtjomatubz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.316326.xyz/gtpxzphrkr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jiagoushi.top/gtpdtqjujd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.pengpengdd.cyou/gtgqutlbyb.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.cheryme.top/gtxvyqxdph.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.xingfuxueyuan.xyz/gttjbypxdj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.snrcjt.cn/gtfivnkuej.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.birdmap.top/gtgntpewaq.html

[H03] 主动抛出异常
来源：http://hz.chenzaomai.com/gtvomydlho.html

Py:   raise ValueError("错误信息")
来源：http://hz.316326.xyz/gtqmhidcun.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jiagoushi.top/gtnwcdjhlz.html

JS:   throw new Error("错误信息");
来源：http://hz.yonumen.top/gtwzxqpobn.html

TS:   throw new Error("错误信息");
来源：http://hz.cashguo.top/gtsxtlqxlw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.pengpengdd.cyou/gtkhnxiurr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.smart0.xyz/gtikhvgisq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.shanyushiyangkeji.top/gtazmvzbhx.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.xuetiantiany.cn/gthyfkxrev.html

[H04] 自定义异常类型
来源：http://hz.hfpthk.cn/gtxjajhzzj.html

Py:   class MyError(Exception): pass
来源：http://hz.xuanzx.com/gtdguiihdi.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zhixingplan.top/gtsjjznoun.html

JS:   class MyError extends Error {}
来源：http://hz.fengsongda.top/gtutvcrium.html

TS:   class MyError extends Error {}
来源：http://hz.ywan-chungtsiang.top/gtkhuoxnay.html

Java: class MyException extends RuntimeException {}
来源：http://hz.ywan-chungtsiang.top/gtmuxycqbl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.hnxiangtu.top/gteasxkysl.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhixingplan.top/gtmnylolml.html

C#:   class MyException : Exception {}
来源：http://hz.zhoulong.xyz/gtldjivhvy.html

[H05] 捕获特定类型
来源：http://hz.yuxming.cn/gtqjqdwatm.html

Py:   except ValueError as e:
来源：http://hz.dashuyun.cn/gtvgifzqys.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhongyouzk.top/gtkymhmaph.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.gogol.net.cn/gtabnvqqrt.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.haohaochexian.top/gteemcqnrz.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.mhx1999.top/gtmhjjdjgh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.cqqwz.cn/gtebundmpa.html

Ruby: rescue ArgumentError => e
来源：http://hz.cashguo.top/gtcyiyhvwx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.tanke756.top/gtbpowybdp.html

[H06] 可选值 / 空值安全访问
来源：http://hz.fengsongda.top/gtlydvctas.html

Py:   value = d.get("k") or default
来源：http://hz.ydzc1.top/gtgnluehql.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.tian-w.cn/gtadtanjdb.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.smart0.xyz/gtjysiahky.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.pycfn.com/gtfdrrswqw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.xziqi.cn/gtekhlxayq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.birdmap.top/gttvmqbsok.html

Ruby: d&.dig(:a, :b)
来源：http://hz.9152youxi.cn/gtlfddqfpf.html

C#:   obj?.A?.B ?? default
来源：http://hz.yj20258.top/gttpmqbzvo.html

[H07] 断言
来源：http://hz.ppjwa.cn/gtwxaotjpy.html

Py:   assert x > 0, "必须为正"
来源：http://hz.chenjidiqi.icu/gtpeixjdob.html

PHP:  assert($x > 0);
来源：http://hz.52xcode.cn/gtdbttqxwz.html

JS:   console.assert(x > 0);
来源：http://hz.jinqigufen.top/gtdxkpxjdk.html

TS:   console.assert(x > 0);
来源：http://hz.shanyushiyangkeji.top/gtfqgvgyof.html

Java: assert x > 0 : "必须为正";
来源：http://hz.mhx1999.top/gtmdbhujox.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ppjwa.cn/gtdfqxkavg.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.aibaodan.cn/gtwnfosjpp.html

C#:   Debug.Assert(x > 0);
来源：http://hz.gotoacloud.top/gtlntjvbyo.html

[H08] 获取错误信息与堆栈
来源：http://hz.52xcode.cn/gtgdtjcpjn.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.tian-w.cn/gtpgyenvvv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.nanxuanxn.top/gtmiiuuocr.html

JS:   e.message;  e.stack
来源：http://hz.jqgufenzy.top/gtaemqqwtq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jqgufenzy.top/gtueasxxjp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.sxryk.cn/gtsjkotjwt.html

Go:   err.Error()
来源：http://hz.ppjwa.cn/gturkovtvj.html

Ruby: e.message;  e.backtrace
来源：http://hz.hnqzz.top/gtqybyugpr.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zycfv.cn/gtofznrpeb.html

[H09] 带错误码的异常
来源：http://hz.svipenyu.cn/gtvhmpgjtt.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zdqjudy.top/gttywbbmls.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jinqigfzy.top/gtwmrlytym.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.daxiang520.top/gtmwynssdo.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.guowangkeji.top/gtaxyijuvh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.xziqi.cn/gtgvzzcdug.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.nanxinkj.top/gtvwyxksrf.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zhaomingkeji.xyz/gtlpivjemb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.ybcxt.top/gtlbuggmmr.html

[H10] 资源自动释放
来源：http://hz.snrcjt.cn/gtlommxswu.html


<!-- 参考信息 -->