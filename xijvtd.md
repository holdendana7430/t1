代发 wailian999

C#:   File.Exists("a.txt")
来源：http://hz.fzhhl.top/gtwcrrqljg.html

[F06] 删除文件
来源：http://hz.jqgufenzy.top/gtgravdqig.html

Py:   os.remove("a.txt")
来源：http://hz.feifeiyinyue.top/gttuclaavs.html

PHP:  unlink("a.txt");
来源：http://hz.jinghuilouyu.cn/gtqklijgae.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.feifeiyinyue.top/gtrtnlbekv.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hammf.cn/gtoeszuglo.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhixingplan.top/gtgfonjjdd.html

Go:   os.Remove("a.txt")
来源：http://hz.316326.xyz/gtmqgvdlaa.html

Ruby: File.delete("a.txt")
来源：http://hz.yuanzhike.top/gtmvrnbsfi.html

C#:   File.Delete("a.txt");
来源：http://hz.zhiwuduotai.top/gtwqxccuwr.html

[F07] 创建目录（含多级）
来源：http://hz.ydjk.org.cn/gtozzbcded.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.birdmap.top/gtyhfmqzih.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.chenjidiqi.icu/gtdldrdptw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jianghu66.top/gtfjnpvbpb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yvedp.cn/gtrmrqupjg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.havefunace.top/gtqxnhfhkt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yangfankeji.com/gtcyjwpdeb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.ehwqpu.com/gtvkfprysw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.wangshuangyany.cn/gtsjhpahay.html

[F08] 遍历目录
来源：http://hz.zdqjudy.top/gtqmdpmhvy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.ybcxt.top/gtokybfysr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.sysykeji.top/gtzcpkcjac.html

JS:   fs.readdirSync("dir")
来源：http://hz.daxiang520.top/gthxgbovko.html

TS:   fs.readdirSync("dir")
来源：http://hz.vqdsnc.cn/gtdbfljjrz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yuxming.cn/gtnhvmzcmn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.guannengcc.top/gtptakgqxm.html

Ruby: Dir.children("dir")
来源：http://hz.9152youxi.cn/gtdcpkaqss.html

C#:   Directory.GetFiles("dir")
来源：http://hz.cqqwz.cn/gtzvodmziv.html

[F09] 获取文件大小
来源：http://hz.ivvv.top/gtkflabxzh.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zhengqikj.top/gtxftevdjp.html

PHP:  filesize("a.txt");
来源：http://hz.zhengqikj.top/gtkdqyzywk.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yvedp.cn/gtbnqfhevo.html

TS:   fs.statSync("a.txt").size
来源：http://hz.cucudq.cn/gtxpmcbzky.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.shanyushiyangtech.top/gtcjzgkfvw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yuxming.cn/gtsdiylgcu.html

Ruby: File.size("a.txt")
来源：http://hz.ppjwa.cn/gttgfjvocn.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.ehwqpu.com/gtbtyhjock.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.gzhubu.top/gteshipsuo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.shuidangran.top/gtattosuyo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jianghu66.top/gtakqvjuhm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jlsjyb.cn/gtwureeebu.html

TS:   path.extname("a.txt")
来源：http://hz.daria6918.cn/gtymcjqtzb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.ivvv.top/gtyvtvzmtc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.gotoacloud.top/gtzwyfzufe.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.xylfe.cn/gtyacvsisg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yanxiufei.cn/gtvlsqumkz.html

[F11] 复制与移动文件
来源：http://hz.ivvv.top/gtvgjninvj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zycfv.cn/gthceialvl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.gaohongyu789.top/gtyhitswma.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.316326.xyz/gtgcwdutqt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hnxiangtu.top/gtzvupyyey.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.wangdashe.top/gtuxeklttb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.ydjk.org.cn/gtwjijnlqd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.aizwys.cn/gtazbvgaug.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.gogol.net.cn/gtqpfiraqa.html

[F12] CSV 读写
来源：http://hz.jinghuilouyu.cn/gthptuowmt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.ydzc1.top/gtnlhifklo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.0kj1m.cn/gtesqcqnon.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.aibaodan.cn/gtcparakxr.html

TS:   // 同上
来源：http://hz.jqgufenzy.top/gtgyvtdxwk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.sufxvd.cn/gtkaixiijb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jinqigufen.top/gtpdhdlsdv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zhijiandao.cn/gtgwzkluhq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.sxryk.cn/gtkxeuvctj.html

================================================================================
来源：http://hz.sweek.top/gtbozawyjr.html

G. 面向对象
来源：http://hz.chenzaomai.com/gtufdewjri.html

================================================================================
来源：http://hz.jinqigufen.top/gtdtruacgd.html

[G01] 定义类
来源：http://hz.hysaishi.cn/gtdprgnsap.html

Py:   class User: pass
来源：http://hz.hywenlv.cn/gtatbtxkzk.html

PHP:  class User {}
来源：http://hz.tian-w.cn/gtbsygssnx.html

JS:   class User {}
来源：http://hz.daxiang520.top/gtwzqwihvf.html

TS:   class User { name: string = ""; }
来源：http://hz.hnqzz.top/gtuvxdbcjm.html

Java: class User {}
来源：http://hz.yj202588.top/gtdlhydkod.html

Go:   type User struct { Name string }
来源：http://hz.yonumen.top/gtgwrzcrso.html

Ruby: class User; end
来源：http://hz.aizwys.cn/gtuktjnzmg.html

C#:   class User {}
来源：http://hz.yj202588.top/gthopozgsy.html

[G02] 构造函数
来源：http://hz.hysaishi.cn/gtsryalutq.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.redwolf501.top/gtikukeywk.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yj202588.top/gtiisjuztr.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhaomingkeji.xyz/gtzhiqpkrj.html

TS:   constructor(public name: string) {}
来源：http://hz.shanyushiyangkeji.top/gtnwgekfkd.html

Java: User(String name) { this.name = name; }
来源：http://hz.zdqjudy.top/gtpigymvwa.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yongpay.top/gtzuupqxki.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.ybcxt.top/gtetriviac.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jinghuilouyu.cn/gtqdvwezvk.html

[G03] 实例属性
来源：http://hz.jianghu66.top/gtiqmeocqb.html

Py:   self.name = "x"
来源：http://hz.ydjk.org.cn/gtujfjdbss.html

PHP:  public string $name = "x";
来源：http://hz.guowangkeji.top/gtjpsjwkpm.html

JS:   this.name = "x";
来源：http://hz.haohaochexian.top/gtsmwghvig.html

TS:   name: string = "x";
来源：http://hz.52xcode.cn/gtnlbauqhz.html

Java: private String name;
来源：http://hz.gaohongyu789.top/gtckfiitqo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.guannengcc.top/gtngyshhpd.html

Ruby: @name = "x"
来源：http://hz.ybcxt.top/gtlzzatqdm.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.sweek.top/gtvffwxxdw.html

[G04] 定义方法
来源：http://hz.guannengcc.top/gtchjsiwry.html

Py:   def greet(self): return self.name
来源：http://hz.ivvv.top/gtsljwqpvu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.andypj.xyz/gtgnplhftt.html

JS:   greet() { return this.name; }
来源：http://hz.yuanzhike.top/gtxiaugvsa.html

TS:   greet(): string { return this.name; }
来源：http://hz.nwbrower.top/gtfuooykrm.html

Java: String greet() { return name; }
来源：http://hz.hammf.cn/gtmaanvezz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.smart0.xyz/gtgfzbmjcw.html

Ruby: def greet; @name; end
来源：http://hz.andypj.xyz/gtsmkgayzy.html

C#:   public string Greet() => Name;
来源：http://hz.pycfn.com/gtywrygmim.html

[G05] 继承
来源：http://hz.hnxiangtu.top/gtimzywlpo.html

Py:   class Admin(User): pass
来源：http://hz.zhengqikj.top/gtytvquchc.html

PHP:  class Admin extends User {}
来源：http://hz.shzxlz.cn/gtzudpvumr.html

JS:   class Admin extends User {}
来源：http://hz.shzxlz.cn/gtjsmwtext.html

TS:   class Admin extends User {}
来源：http://hz.sweek.top/gtbwhsijzq.html

Java: class Admin extends User {}
来源：http://hz.bjfxy.top/gtlbpdisnc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hywenlv.cn/gtpvbnmfav.html

Ruby: class Admin < User; end
来源：http://hz.gotoacloud.top/gtdqlwgydg.html

C#:   class Admin : User {}
来源：http://hz.yanxiufei.cn/gttjtaours.html

[G06] 重写方法
来源：http://hz.havefunace.top/gtuetqijus.html

Py:   def greet(self): return "admin"
来源：http://hz.gotoacloud.top/gtrbiwnmas.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.xylfe.cn/gtvhtsuyjt.html

JS:   greet() { return "admin"; }
来源：http://hz.svipenyu.cn/gtngwzthto.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jlsjyb.cn/gtpxbdftzy.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jinqigfzy.top/gtruawtfsv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.daxiang520.top/gtaiprwlfi.html

Ruby: def greet; "admin"; end
来源：http://hz.pycfn.com/gtklacfncb.html

C#:   public override string Greet() => "admin";
来源：http://hz.shanyushiyangtech.top/gtrfyvwlhj.html

[G07] 调用父类方法
来源：http://hz.nanxuanxn.top/gtripewuom.html

Py:   super().greet()
来源：http://hz.jqgfzy.top/gtkxkcabpc.html

PHP:  parent::greet();
来源：http://hz.xinyue.icu/gtnsdnqlwi.html

JS:   super.greet();
来源：http://hz.hysaishi.cn/gtmbyaobrd.html

TS:   super.greet();
来源：http://hz.andypj.xyz/gtaeuertll.html

Java: super.greet();
来源：http://hz.guannengcc.top/gtvzptswqx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.dianchejie.cn/gtshkbmtxu.html

Ruby: super
来源：http://hz.yueranfly.top/gtzrkoulpk.html

C#:   base.Greet();
来源：http://hz.hnqzz.top/gtncsidikr.html

[G08] 静态方法与属性
来源：http://hz.smart0.xyz/gtcyauogdi.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.xinyue.icu/gtvxxfcxkp.html

PHP:  public static function f() {}
来源：http://hz.yj20258888.top/gtizugaclz.html

JS:   static f() {}
来源：http://hz.shangyingyoupin.top/gteubuuoro.html

TS:   static f(): void {}
来源：http://hz.sysykeji.top/gtqplqylmp.html

Java: static void f() {}
来源：http://hz.xinyue.icu/gtbeyomlou.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.xziqi.cn/gtcolzkrfv.html

Ruby: def self.f; end
来源：http://hz.aizwys.cn/gthuqindlg.html

C#:   public static void F() {}
来源：http://hz.yuxming.cn/gtmwwbqyjm.html

[G09] 接口 / 抽象类
来源：http://hz.gogol.net.cn/gtflcsoqxv.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.xziqi.cn/gtzqittinx.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.andypj.xyz/gtjfznhyni.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.kuanghao11.cn/gtdyuabexu.html

TS:   interface Shape { area(): number; }
来源：http://hz.xziqi.cn/gtjrooqitu.html

Java: interface Shape { double area(); }
来源：http://hz.wangdashe.top/gtphjpyhyp.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jianghu66.top/gtncqoiheb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.haohaochexian.top/gtsscyzqyy.html

C#:   interface IShape { double Area(); }
来源：http://hz.hfpthk.cn/gtbuyhkmgv.html

[G10] 访问控制
来源：http://hz.yj20258888.top/gtgexpmjla.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.sweek.top/gtyigkirot.html

PHP:  public / protected / private
来源：http://hz.ehwqpu.com/gthzcnfltp.html

JS:   #private 字段；其余公开
来源：http://hz.zhixingplan.top/gtvmfwdfzn.html

TS:   public / protected / private
来源：http://hz.316326.xyz/gtjgdhelfh.html

Java: public / protected / private / 默认包级
来源：http://hz.haohaochexian.top/gtxfenrhxt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.aizwys.cn/gtevzmljna.html

Ruby: public / protected / private
来源：http://hz.cashguo.top/gtfrwlpqow.html

C#:   public / protected / private / internal
来源：http://hz.nanxinkj.top/gtyejlpfpa.html

[G11] getter / setter
来源：http://hz.hfpthk.cn/gtowyucvoc.html

Py:   @property 与 @x.setter
来源：http://hz.fzhhl.top/gtvlamkkhk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.9152youxi.cn/gtwwqzimhq.html

JS:   get name() { return this._name; }
来源：http://hz.sweek.top/gtjmenchvi.html

TS:   get name(): string { return this._name; }
来源：http://hz.ydjk.org.cn/gtepuzwqal.html

Java: public String getName() { return name; }
来源：http://hz.jqgufenzy.top/gtvikqxlpf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.shuidangran.top/gtpkokgnpi.html

Ruby: attr_accessor :name
来源：http://hz.yanxiufei.cn/gtcqgmrxyf.html

C#:   public string Name { get; set; }
来源：http://hz.jyoumei.cn/gtrfmdyarv.html

[G12] 对象转字符串
来源：http://hz.dashuyun.cn/gtsathyxos.html

Py:   def __str__(self): return self.name
来源：http://hz.jqgfzy.top/gtciqpnjge.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zhongyouzk.top/gtmcctuwdq.html

JS:   toString() { return this.name; }
来源：http://hz.jiagoushi.top/gtxvcdjvae.html

TS:   toString(): string { return this.name; }
来源：http://hz.jinyuanbaomall.cn/gtxdndgbfa.html

Java: @Override public String toString() { return name; }
来源：http://hz.xingfuxueyuan.xyz/gtxtwkicwn.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zycfv.cn/gtrykgfurp.html

Ruby: def to_s; @name; end
来源：http://hz.yj20258888.top/gtyemcqese.html

C#:   public override string ToString() => Name;
来源：http://hz.zhengqikj.top/gtkksneaqx.html

[G13] 判断对象类型
来源：http://hz.guowangkeji.top/gtsndxnomn.html

Py:   isinstance(u, User)
来源：http://hz.smart0.xyz/gtufmsqdee.html

PHP:  $u instanceof User
来源：http://hz.chenzaomai.com/gtpohnwmwn.html

JS:   u instanceof User
来源：http://hz.haohaochexian.top/gtltmtdshu.html

TS:   u instanceof User
来源：http://hz.svipenyu.cn/gtzsmthjwj.html

Java: u instanceof User
来源：http://hz.ydjk.org.cn/gtuhvsvcsj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zhijiandao.cn/gtuzdehmuk.html

Ruby: u.is_a?(User)
来源：http://hz.xuanzx.com/gtfgndhbuz.html

C#:   u is User
来源：http://hz.yuanzhike.top/gthulxgxkg.html

[G14] 数据类 / record
来源：http://hz.fzhhl.top/gtbmpexwtu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.vqdsnc.cn/gtlamnrtcq.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jinghuilouyu.cn/gtewpygnrm.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.tian-w.cn/gtvydbhyun.html

TS:   type User = { name: string; age: number };
来源：http://hz.chenjidiqi.icu/gtfolbesjd.html

Java: record User(String name, int age) {}
来源：http://hz.jyoumei.cn/gtccsjpxtj.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zhongyouzk.top/gtlgzceceo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.ywan-chungtsiang.top/gtdscaqfkf.html

C#:   record User(string Name, int Age);
来源：http://hz.nanxinkj.top/gtsbbjnyya.html

[G15] 枚举
来源：http://hz.jiagoushi.top/gtuxatajpo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yangfankeji.com/gtcglaujeg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ehwqpu.com/gtwvcpgqpc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.xinyue.icu/gtvupnftdk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.fzhhl.top/gtqdwfgqet.html

Java: enum Color { RED, GREEN }
来源：http://hz.fzhhl.top/gthjekasuj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.xziqi.cn/gtefcdozwx.html

Ruby: Color = %i[red green].freeze
来源：http://hz.cqqwz.cn/gtsxmbdiqm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.chenjidiqi.icu/gtbepsqjvp.html

[G16] 对象转数组 / 字典
来源：http://hz.shzxlz.cn/gtgmpyrbgu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.ehwqpu.com/gtjgvckqol.html

PHP:  get_object_vars($obj);
来源：http://hz.fengsongda.top/gtkgdczcbn.html

JS:   Object.entries(obj)
来源：http://hz.quarkkingdee.top/gtrxofvcvo.html

TS:   Object.entries(obj)
来源：http://hz.jlsjyb.cn/gtgyprfmaf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.cucudq.cn/gtfmntsshq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jinqigfzy.top/gttqrodult.html

Ruby: obj.instance_variables
来源：http://hz.zhixingplan.top/gtiwsuiwao.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.xingfuxueyuan.xyz/gtyfxntatp.html

================================================================================
来源：http://hz.tian-w.cn/gtgzxqqiff.html

H. 异常与错误处理
来源：http://hz.shuidangran.top/gtkrtmpdif.html

================================================================================
来源：http://hz.kuanghao11.cn/gtaalhvzvg.html

[H01] try / catch 基础
来源：http://hz.yj202588.top/gttdwlurwq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yanxiufei.cn/gtucswtemf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.smart0.xyz/gtjagsbkoq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.sxryk.cn/gtpahhyatz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.shanyushiyangkeji.top/gtfbkqtbqd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ppjwa.cn/gtpzairrkq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jyoumei.cn/gtrvagvqkf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yj20258888.top/gtbrjqfokj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.hnqzz.top/gtkiocamyt.html

[H02] finally / ensure 收尾
来源：http://hz.jiagoushi.top/gthcinizfb.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.smart0.xyz/gtifceazvd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.kuanghao11.cn/gtedrpqeub.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangkeji.top/gtzkacabyz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.cqqwz.cn/gtttoawbrb.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhongyouzk.top/gtswyznene.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.kuanghao11.cn/gtrzcgpseo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yvedp.cn/gtaynghwlx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.sufxvd.cn/gtykwxsses.html

[H03] 主动抛出异常
来源：http://hz.yuxming.cn/gtxepltvcx.html

Py:   raise ValueError("错误信息")
来源：http://hz.jlsjyb.cn/gtsugbucut.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.smart0.xyz/gtmgfhagoq.html

JS:   throw new Error("错误信息");
来源：http://hz.svipenyu.cn/gtcaymatxx.html

TS:   throw new Error("错误信息");
来源：http://hz.jinqigufen.top/gtfknettij.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yuxming.cn/gtxrdryctm.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.52xcode.cn/gtswqweokp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.sxryk.cn/gtpcjatfyj.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.aizwys.cn/gtuhhzqzgp.html

[H04] 自定义异常类型
来源：http://hz.andypj.xyz/gttayrcudq.html

Py:   class MyError(Exception): pass
来源：http://hz.zhaomingkeji.xyz/gtcryzlwuu.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.52xcode.cn/gtmxcxnfxc.html

JS:   class MyError extends Error {}
来源：http://hz.guannengcc.top/gttrrpeufk.html

TS:   class MyError extends Error {}
来源：http://hz.andypj.xyz/gtudzoqimw.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jqgfzy.top/gtvskulvto.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.nanxuanxn.top/gtypbfhxpq.html

Ruby: class MyError < StandardError; end
来源：http://hz.cucudq.cn/gtyskdzkgo.html

C#:   class MyException : Exception {}
来源：http://hz.zhongyouzk.top/gtijkbaqis.html

[H05] 捕获特定类型
来源：http://hz.52xcode.cn/gtosnmbyqo.html

Py:   except ValueError as e:
来源：http://hz.yuanzhike.top/gtirtxcyhy.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.hfpthk.cn/gtwggimnjq.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.snrcjt.cn/gtwufliqwv.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.c1oappe.top/gtpefhzxak.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.ppjwa.cn/gtjovgokcn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zdqjudy.top/gtbnzksitv.html

Ruby: rescue ArgumentError => e
来源：http://hz.jianghu66.top/gtfyqintqo.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.9152youxi.cn/gtlynnjiij.html

[H06] 可选值 / 空值安全访问
来源：http://hz.gogol.net.cn/gtfnrjkkxa.html

Py:   value = d.get("k") or default
来源：http://hz.jyoumei.cn/gtnhmitwsa.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.nwbrower.top/gtmavzimej.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.sysykeji.top/gtsjrokwdw.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jinghuilouyu.cn/gtqhswaypb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.meibo888.top/gtmgddfrso.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.tianlin.xyz/gtklrxjopq.html

Ruby: d&.dig(:a, :b)
来源：http://hz.daria6918.cn/gtdmfdbixj.html

C#:   obj?.A?.B ?? default
来源：http://hz.shanyushiyangkeji.top/gtahktjlop.html

[H07] 断言
来源：http://hz.0kj1m.cn/gtstlerljk.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yuxming.cn/gtezvahdvq.html

PHP:  assert($x > 0);
来源：http://hz.tianlin.xyz/gtfbafomkl.html

JS:   console.assert(x > 0);
来源：http://hz.nanxinkj.top/gtofvjjzhz.html

TS:   console.assert(x > 0);
来源：http://hz.jinyuanbaomall.cn/gtbiwdwksy.html

Java: assert x > 0 : "必须为正";
来源：http://hz.xziqi.cn/gtlmsvoafd.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.haohaochexian.top/gtyzfyyytq.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.pengpengdd.cyou/gtwmdsyklj.html

C#:   Debug.Assert(x > 0);
来源：http://hz.ehwqpu.com/gtclifqecd.html

[H08] 获取错误信息与堆栈
来源：http://hz.jyoumei.cn/gteatculof.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yongpay.top/gtriemdzgm.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.haohaochexian.top/gteipbadga.html

JS:   e.message;  e.stack
来源：http://hz.hnxiangtu.top/gteemvgukq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.guowangkeji.top/gtwmglgcrn.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.mhx1999.top/gtsvjfmwvb.html

Go:   err.Error()
来源：http://hz.jqgufenzy.top/gtbexmehgr.html

Ruby: e.message;  e.backtrace
来源：http://hz.cheryme.top/gtcxjtoini.html

C#:   e.Message;  e.StackTrace
来源：http://hz.hnqzz.top/gtssdvbcqw.html

[H09] 带错误码的异常
来源：http://hz.fzhhl.top/gthzebvcrk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.ybcxt.top/gtrblsomsp.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.shanyushiyangtech.top/gtsqraqntl.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.gogol.net.cn/gtidhagdol.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.cdnleiting.top/gtcfizzjhk.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yanxiufei.cn/gtebrlowuq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.tanke756.top/gtpzwonvjx.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.redwolf501.top/gtpqpqzyqq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.snrcjt.cn/gtbdeglldz.html

[H10] 资源自动释放
来源：http://hz.c1oappe.top/gtozuczvct.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.havefunace.top/gtqhjojopk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.dianchejie.cn/gtplsbitff.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.dashuyun.cn/gtdyzuskat.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.aizwys.cn/gtcdogfuey.html


<!-- 参考信息 -->