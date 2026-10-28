代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://hz.ppjwa.cn/gtkeowsaqe.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.gogol.net.cn/gtsyxrsdzj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.sweek.top/gtrhgwhsae.html

Ruby: File.exist?("a.txt")
来源：http://hz.chenlongwang.top/gtljaoenqj.html

C#:   File.Exists("a.txt")
来源：http://hz.shanyushiyangtech.top/gtadzhedhf.html

[F06] 删除文件
来源：http://hz.ivvv.top/gtdxzyuuka.html

Py:   os.remove("a.txt")
来源：http://hz.guowangkeji.top/gtxxlqtayi.html

PHP:  unlink("a.txt");
来源：http://hz.andypj.xyz/gtwdfhpvat.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.nanxuanxn.top/gtvhktwvyb.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.fzhhl.top/gtboevhvth.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.fzhhl.top/gtglvohzfb.html

Go:   os.Remove("a.txt")
来源：http://hz.dianchejie.cn/gtkrvqnhud.html

Ruby: File.delete("a.txt")
来源：http://hz.snrcjt.cn/gtoyzzxhri.html

C#:   File.Delete("a.txt");
来源：http://hz.yj20258.top/gthktxwtpg.html

[F07] 创建目录（含多级）
来源：http://hz.vqdsnc.cn/gtoefjrqix.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.mhx1999.top/gtlxisajki.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.9152youxi.cn/gtegppbtdu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ivvv.top/gtrixszvsw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.nanxinkj.top/gtexcekmwn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.zhoulong.xyz/gtazxxfpyh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.ydjk.org.cn/gtqsqaiquz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yuanzhike.top/gtwgozoumj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.hammf.cn/gtdwboohmw.html

[F08] 遍历目录
来源：http://hz.gzhubu.top/gtpqnddavm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.shangyingyoupin.top/gtojitbhne.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.shangyingyoupin.top/gtxbydnkhx.html

JS:   fs.readdirSync("dir")
来源：http://hz.shanyushiyangkeji.top/gtgdltxkrt.html

TS:   fs.readdirSync("dir")
来源：http://hz.ydjk.org.cn/gtmrqrtmom.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.sxryk.cn/gtriznyyrt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yueranfly.top/gtiiwasubj.html

Ruby: Dir.children("dir")
来源：http://hz.fzhhl.top/gtzkeeuupw.html

C#:   Directory.GetFiles("dir")
来源：http://hz.pengpengdd.cyou/gtiehsohlo.html

[F09] 获取文件大小
来源：http://hz.fengsongda.top/gtypxphfqp.html

Py:   os.path.getsize("a.txt")
来源：http://hz.xylfe.cn/gtovskhllz.html

PHP:  filesize("a.txt");
来源：http://hz.redwolf501.top/gtzqhdqdso.html

JS:   fs.statSync("a.txt").size
来源：http://hz.sysykeji.top/gtlvlwxgbp.html

TS:   fs.statSync("a.txt").size
来源：http://hz.havefunace.top/gtclkqubma.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.aibaodan.cn/gtqpzdlqzo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.bjfxy.top/gtemuhqjbo.html

Ruby: File.size("a.txt")
来源：http://hz.quarkkingdee.top/gtlyuxhtxp.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.nanxuanxn.top/gtuxojthdk.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.ivvv.top/gtwyvvotoy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zycfv.cn/gtfhfxelgg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jinqigufen.top/gtpgktyfoz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.iojbl.cn/gthhqjabwb.html

TS:   path.extname("a.txt")
来源：http://hz.hnxiangtu.top/gtphqjjaox.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.snrcjt.cn/gtrebmxkqb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.dashuyun.cn/gtbadxsble.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.hywenlv.cn/gtlvfreuxp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.ivvv.top/gtkrjujigr.html

[F11] 复制与移动文件
来源：http://hz.redwolf501.top/gtpnanpzel.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.cheryme.top/gtbtxcjvkk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.sweek.top/gtqpylrzta.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhongyouzk.top/gtuxbavnpn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.vqdsnc.cn/gtruevbkhh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.andypj.xyz/gtrawslxfo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jyoumei.cn/gtsdarzixz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.sysykeji.top/gtpgqpesjk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.vqdsnc.cn/gtgdoenaeh.html

[F12] CSV 读写
来源：http://hz.zhiwuduotai.top/gtvvpqtdid.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.shanyushiyangkeji.top/gtsxkikrwi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.aizwys.cn/gtsegjdwdj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.aibaodan.cn/gtojnfomqx.html

TS:   // 同上
来源：http://hz.pycfn.com/gtbapuodud.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ybcxt.top/gtkrtvnyrb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.tian-w.cn/gtswzzebmy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.tian-w.cn/gtlrcaagry.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.c1oappe.top/gtbauxfrsk.html

================================================================================
来源：http://hz.hammf.cn/gtgmnjxjfh.html

G. 面向对象
来源：http://hz.52xcode.cn/gtksnexrhd.html

================================================================================
来源：http://hz.hysaishi.cn/gtepaqnzns.html

[G01] 定义类
来源：http://hz.hywenlv.cn/gtfqgfluua.html

Py:   class User: pass
来源：http://hz.xuetiantiany.cn/gtilartwyl.html

PHP:  class User {}
来源：http://hz.tanke756.top/gtxkaagexl.html

JS:   class User {}
来源：http://hz.aizwys.cn/gtvwkptauj.html

TS:   class User { name: string = ""; }
来源：http://hz.xuetiantiany.cn/gtdqzqoevz.html

Java: class User {}
来源：http://hz.redwolf501.top/gtxgdnhrlt.html

Go:   type User struct { Name string }
来源：http://hz.316326.xyz/gtkxvbeqxu.html

Ruby: class User; end
来源：http://hz.iojbl.cn/gtfnhpywia.html

C#:   class User {}
来源：http://hz.jlsjyb.cn/gtvpyekxkk.html

[G02] 构造函数
来源：http://hz.jinqigfzy.top/gtaxkioarv.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.vqdsnc.cn/gtzhijqhkc.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yvedp.cn/gtnihzltlt.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.wangshuangyany.cn/gtiwplmfcz.html

TS:   constructor(public name: string) {}
来源：http://hz.xingfuxueyuan.xyz/gtcqxhvcgz.html

Java: User(String name) { this.name = name; }
来源：http://hz.gogol.net.cn/gtmxbabmbb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yueranfly.top/gtbumqvwcf.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.hongshengwenyu.top/gtwfpufint.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jinghuilouyu.cn/gtucbsxtuz.html

[G03] 实例属性
来源：http://hz.jqgufenzy.top/gtsuvidgcm.html

Py:   self.name = "x"
来源：http://hz.cdnleiting.top/gtszfkpzqi.html

PHP:  public string $name = "x";
来源：http://hz.jinqigfzy.top/gtpcwtuaob.html

JS:   this.name = "x";
来源：http://hz.yangfankeji.com/gtxxhfkocg.html

TS:   name: string = "x";
来源：http://hz.xylfe.cn/gtvhrkghny.html

Java: private String name;
来源：http://hz.hnxiangtu.top/gtvpucttfa.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.sysykeji.top/gtkrzhqlzh.html

Ruby: @name = "x"
来源：http://hz.fzhhl.top/gtpkpwxham.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.tianlin.xyz/gtoctoixfk.html

[G04] 定义方法
来源：http://hz.shangyingyoupin.top/gtmrozeobl.html

Py:   def greet(self): return self.name
来源：http://hz.xylfe.cn/gtftiwhcsf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.haohaochexian.top/gtrjsakbte.html

JS:   greet() { return this.name; }
来源：http://hz.fengsongda.top/gtfrsnxslz.html

TS:   greet(): string { return this.name; }
来源：http://hz.hfpthk.cn/gtxdkicqpr.html

Java: String greet() { return name; }
来源：http://hz.52xcode.cn/gtcgtqevtu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ydzc1.top/gtnlawxwpx.html

Ruby: def greet; @name; end
来源：http://hz.feifeiyinyue.top/gtxjdtrpkj.html

C#:   public string Greet() => Name;
来源：http://hz.hnqzz.top/gttlfssgoo.html

[G05] 继承
来源：http://hz.shangyingyoupin.top/gtrtadewpo.html

Py:   class Admin(User): pass
来源：http://hz.9152youxi.cn/gtnfukolvk.html

PHP:  class Admin extends User {}
来源：http://hz.hywenlv.cn/gtrjizyrjp.html

JS:   class Admin extends User {}
来源：http://hz.jinyuanbaomall.cn/gtqaewmftk.html

TS:   class Admin extends User {}
来源：http://hz.sxryk.cn/gtysehfdsy.html

Java: class Admin extends User {}
来源：http://hz.shuidangran.top/gtncwwspun.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.dianchejie.cn/gtronjjwct.html

Ruby: class Admin < User; end
来源：http://hz.jqgfzy.top/gtpnrrycgq.html

C#:   class Admin : User {}
来源：http://hz.mhx1999.top/gteshdecft.html

[G06] 重写方法
来源：http://hz.0kj1m.cn/gtzkmtmdiv.html

Py:   def greet(self): return "admin"
来源：http://hz.xinyue.icu/gtoexiunie.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.sysykeji.top/gteqdhctky.html

JS:   greet() { return "admin"; }
来源：http://hz.sysykeji.top/gtrqmrlyuv.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zhoulong.xyz/gtljpyyzll.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.tianlin.xyz/gtcoldslmr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.nanxinkj.top/gtkdmsujcj.html

Ruby: def greet; "admin"; end
来源：http://hz.aibaodan.cn/gtaanzxhcp.html

C#:   public override string Greet() => "admin";
来源：http://hz.hywenlv.cn/gtfptdrkdy.html

[G07] 调用父类方法
来源：http://hz.bjfxy.top/gtnhpajwpw.html

Py:   super().greet()
来源：http://hz.jinqigfzy.top/gtkzwwavnd.html

PHP:  parent::greet();
来源：http://hz.ybcxt.top/gtmsifiqzx.html

JS:   super.greet();
来源：http://hz.nanxinkj.top/gtszmggkcy.html

TS:   super.greet();
来源：http://hz.jinyuanbaomall.cn/gtbwrkaonn.html

Java: super.greet();
来源：http://hz.52xcode.cn/gtprlyawjm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.xylfe.cn/gtsgpyjjjf.html

Ruby: super
来源：http://hz.zhoulong.xyz/gtjldrpimt.html

C#:   base.Greet();
来源：http://hz.smart0.xyz/gtotacskcx.html

[G08] 静态方法与属性
来源：http://hz.feifeiyinyue.top/gtookvywxz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.52xcode.cn/gtezwswjhw.html

PHP:  public static function f() {}
来源：http://hz.pycfn.com/gtdskcewkx.html

JS:   static f() {}
来源：http://hz.daria6918.cn/gtrxdzvytw.html

TS:   static f(): void {}
来源：http://hz.cdnleiting.top/gtqlnqmibh.html

Java: static void f() {}
来源：http://hz.shangyingyoupin.top/gtzzfovhad.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.nanxuanxn.top/gtmnkrxvhh.html

Ruby: def self.f; end
来源：http://hz.hysaishi.cn/gtbgefjexw.html

C#:   public static void F() {}
来源：http://hz.yj20258888.top/gtmndvmqtb.html

[G09] 接口 / 抽象类
来源：http://hz.feifeiyinyue.top/gtkugryyen.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.hnxiangtu.top/gtqfzykgiz.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yuanzhike.top/gtvousouxp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.smart0.xyz/gtojwzoojg.html

TS:   interface Shape { area(): number; }
来源：http://hz.shzxlz.cn/gtaixjgvzh.html

Java: interface Shape { double area(); }
来源：http://hz.jyoumei.cn/gtsxuximqr.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.shangyingyoupin.top/gtxvdezmev.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.guowangkeji.top/gtjlbxehvq.html

C#:   interface IShape { double Area(); }
来源：http://hz.wangshuangyany.cn/gtxoxfdmvu.html

[G10] 访问控制
来源：http://hz.0kj1m.cn/gtcrpbqigx.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.sweek.top/gtgdgflpxc.html

PHP:  public / protected / private
来源：http://hz.sysykeji.top/gtadknivmc.html

JS:   #private 字段；其余公开
来源：http://hz.gaohongyu789.top/gtycesxpho.html

TS:   public / protected / private
来源：http://hz.shuidangran.top/gtnpcnpibe.html

Java: public / protected / private / 默认包级
来源：http://hz.yangfankeji.com/gtdmbamgbd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jinghuilouyu.cn/gtfhfajtwy.html

Ruby: public / protected / private
来源：http://hz.chenlongwang.top/gtmlvtzhav.html

C#:   public / protected / private / internal
来源：http://hz.shanyushiyangtech.top/gtzvkxvwut.html

[G11] getter / setter
来源：http://hz.zhengqikj.top/gtazkdiypk.html

Py:   @property 与 @x.setter
来源：http://hz.vqdsnc.cn/gtkvdwzfxh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.hnqzz.top/gtwenyfeyi.html

JS:   get name() { return this._name; }
来源：http://hz.jianghu66.top/gtiznakpjc.html

TS:   get name(): string { return this._name; }
来源：http://hz.wangshuangyany.cn/gtaoudipqa.html

Java: public String getName() { return name; }
来源：http://hz.meibo888.top/gtrfsxsiru.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.guannengcc.top/gtucmnflbd.html

Ruby: attr_accessor :name
来源：http://hz.yongpay.top/gtcizrdftp.html

C#:   public string Name { get; set; }
来源：http://hz.zhoulong.xyz/gtwfoylmlq.html

[G12] 对象转字符串
来源：http://hz.yj20258888.top/gtljmsbmew.html

Py:   def __str__(self): return self.name
来源：http://hz.wangshuangyany.cn/gtekdjgams.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.fzhhl.top/gtxckhttak.html

JS:   toString() { return this.name; }
来源：http://hz.cqqwz.cn/gtphntvdhz.html

TS:   toString(): string { return this.name; }
来源：http://hz.haohaochexian.top/gtbwmtghfo.html

Java: @Override public String toString() { return name; }
来源：http://hz.yuanzhike.top/gtpwumzfnx.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.hfpthk.cn/gtddpphkbz.html

Ruby: def to_s; @name; end
来源：http://hz.pengpengdd.cyou/gtfyetesqz.html

C#:   public override string ToString() => Name;
来源：http://hz.yj20258.top/gttuwvqidn.html

[G13] 判断对象类型
来源：http://hz.shzxlz.cn/gtvtjtdxbe.html

Py:   isinstance(u, User)
来源：http://hz.fzhhl.top/gtjotaykbr.html

PHP:  $u instanceof User
来源：http://hz.mhx1999.top/gtylhabynl.html

JS:   u instanceof User
来源：http://hz.zdqjudy.top/gtsurkpcsw.html

TS:   u instanceof User
来源：http://hz.shanyushiyangkeji.top/gtsxwnrica.html

Java: u instanceof User
来源：http://hz.meibo888.top/gtlbvwzljj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zycfv.cn/gttrfezqet.html

Ruby: u.is_a?(User)
来源：http://hz.shangyingyoupin.top/gtioctcvbv.html

C#:   u is User
来源：http://hz.yueranfly.top/gtfmkbacbv.html

[G14] 数据类 / record
来源：http://hz.cqqwz.cn/gtsrxkidwf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yongpay.top/gtbzjdbwys.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.wangdashe.top/gtjyirawmo.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.xingfuxueyuan.xyz/gtlcjlrsma.html

TS:   type User = { name: string; age: number };
来源：http://hz.hywenlv.cn/gtmfexwqqo.html

Java: record User(String name, int age) {}
来源：http://hz.feifeiyinyue.top/gtrpwahjho.html

Go:   type User struct { Name string; Age int }
来源：http://hz.nanxuanxn.top/gttdvzdorq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yonumen.top/gtfonrwxxs.html

C#:   record User(string Name, int Age);
来源：http://hz.gogol.net.cn/gthfzxjpwa.html

[G15] 枚举
来源：http://hz.smart0.xyz/gtjidmxzyu.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zycfv.cn/gtuwiiwwci.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.gaohongyu789.top/gtqluirhja.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hnqzz.top/gtugnezjaz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yangfankeji.com/gtglveqcku.html

Java: enum Color { RED, GREEN }
来源：http://hz.yonumen.top/gturdkphap.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.gaohongyu789.top/gtwhvrzfrf.html

Ruby: Color = %i[red green].freeze
来源：http://hz.guannengcc.top/gtcnmqjbal.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.chenjidiqi.icu/gtisngcfmt.html

[G16] 对象转数组 / 字典
来源：http://hz.birdmap.top/gtdeohektj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jinqigufen.top/gtyzwpxogw.html

PHP:  get_object_vars($obj);
来源：http://hz.zhoulong.xyz/gtywcbtyfn.html

JS:   Object.entries(obj)
来源：http://hz.ydzc1.top/gtvxzlnfhl.html

TS:   Object.entries(obj)
来源：http://hz.xziqi.cn/gtdmsxvury.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hysaishi.cn/gtzkvyffsd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.xinyue.icu/gtrqssnpvt.html

Ruby: obj.instance_variables
来源：http://hz.yuxming.cn/gtlbiowpnx.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.sweek.top/gtegalapgf.html

================================================================================
来源：http://hz.shzxlz.cn/gtzxqgsvqv.html

H. 异常与错误处理
来源：http://hz.wangshuangyany.cn/gtfongjmxq.html

================================================================================
来源：http://hz.xinyue.icu/gtpgxxbtsy.html

[H01] try / catch 基础
来源：http://hz.gotoacloud.top/gtlfqkbyop.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.nwbrower.top/gtqrliaffb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.chenjidiqi.icu/gtrcpjxrwy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jqgfzy.top/gtwwoxpekx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zhixingplan.top/gtnivccipg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.hammf.cn/gttdjxadur.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.tanke756.top/gtybnmqkuo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.tian-w.cn/gtsyzwvvoi.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yj20258888.top/gtazcujazd.html

[H02] finally / ensure 收尾
来源：http://hz.cdnleiting.top/gtepoqgbrk.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.meibo888.top/gtveubdkqm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.0kj1m.cn/gtpuhsmzlu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.wangshuangyany.cn/gtzqhcvioy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jlsjyb.cn/gteerioeji.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.cashguo.top/gtyuvkiggt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.havefunace.top/gtchoesncy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.shanyushiyangkeji.top/gtswxxmivk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.gotoacloud.top/gtgyyrmiwc.html

[H03] 主动抛出异常
来源：http://hz.ppjwa.cn/gtndptowmn.html

Py:   raise ValueError("错误信息")
来源：http://hz.zhongyouzk.top/gtiovmwiaw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.shanyushiyangtech.top/gttmbjlcnf.html

JS:   throw new Error("错误信息");
来源：http://hz.xuetiantiany.cn/gtcruvxwfs.html

TS:   throw new Error("错误信息");
来源：http://hz.yj20258888.top/gtmyhstpnh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jianghu66.top/gtxwsznxwr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.ywan-chungtsiang.top/gttsbqcqdq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zhongyouzk.top/gtjfjknlwa.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.pengpengdd.cyou/gtbqoidykg.html

[H04] 自定义异常类型
来源：http://hz.daxiang520.top/gtxhwelhno.html

Py:   class MyError(Exception): pass
来源：http://hz.jqgufenzy.top/gtsnpwbtsc.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.bjfxy.top/gtsbniwrhw.html

JS:   class MyError extends Error {}
来源：http://hz.yj202588.top/gtdhtukrap.html

TS:   class MyError extends Error {}
来源：http://hz.xylfe.cn/gtnasbottx.html

Java: class MyException extends RuntimeException {}
来源：http://hz.hysaishi.cn/gtqsvbgruu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yuxming.cn/gtkfyekoxx.html

Ruby: class MyError < StandardError; end
来源：http://hz.havefunace.top/gtzejfkuub.html

C#:   class MyException : Exception {}
来源：http://hz.hywenlv.cn/gtwubvygov.html

[H05] 捕获特定类型
来源：http://hz.zhengqikj.top/gtboxvubgg.html

Py:   except ValueError as e:
来源：http://hz.shanyushiyangkeji.top/gtuzlblafx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.9152youxi.cn/gtkkqzhsuz.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jyoumei.cn/gtxxqpgjcc.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jyoumei.cn/gtakjtkvbd.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.xuetiantiany.cn/gtmsjjxbfj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zhijiandao.cn/gtixypkaan.html

Ruby: rescue ArgumentError => e
来源：http://hz.yanxiufei.cn/gtggfblbaz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hongshengwenyu.top/gttghsfgby.html

[H06] 可选值 / 空值安全访问
来源：http://hz.fengsongda.top/gtixwfmdet.html

Py:   value = d.get("k") or default
来源：http://hz.quarkkingdee.top/gtjkuuyesf.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.quarkkingdee.top/gtjongsrxa.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.aizwys.cn/gtldnjmzmi.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zhaomingkeji.xyz/gtwpppvjwm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.vqdsnc.cn/gtktitneji.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.shanyushiyangtech.top/gtksoyoihv.html

Ruby: d&.dig(:a, :b)
来源：http://hz.xziqi.cn/gttikpufkd.html

C#:   obj?.A?.B ?? default
来源：http://hz.hnqzz.top/gtruwwdftw.html

[H07] 断言
来源：http://hz.xylfe.cn/gtdtetwfij.html

Py:   assert x > 0, "必须为正"
来源：http://hz.hysaishi.cn/gtazaxvuwh.html

PHP:  assert($x > 0);
来源：http://hz.dianchejie.cn/gtdxypeyjz.html

JS:   console.assert(x > 0);
来源：http://hz.iojbl.cn/gtdqzyjnuk.html

TS:   console.assert(x > 0);
来源：http://hz.yj202588.top/gtpnpsykgh.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jyoumei.cn/gtxrfgawup.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.quarkkingdee.top/gtotkgavxa.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.sxryk.cn/gtsduwyzhb.html

C#:   Debug.Assert(x > 0);
来源：http://hz.chenjidiqi.icu/gtbjefunou.html

[H08] 获取错误信息与堆栈
来源：http://hz.snrcjt.cn/gtgariplao.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.chenzaomai.com/gttonugisa.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zhoulong.xyz/gtfymfwnch.html

JS:   e.message;  e.stack
来源：http://hz.cashguo.top/gtobjxjcod.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yonumen.top/gtlzavawbo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhijiandao.cn/gtyvuquqkj.html

Go:   err.Error()
来源：http://hz.cheryme.top/gteexpedva.html

Ruby: e.message;  e.backtrace
来源：http://hz.zhaomingkeji.xyz/gtbeithhdm.html

C#:   e.Message;  e.StackTrace
来源：http://hz.cucudq.cn/gtpctvfrbt.html

[H09] 带错误码的异常
来源：http://hz.dashuyun.cn/gtlkcseirn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.ydzc1.top/gtzjjlmbbd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.xuetiantiany.cn/gtxayizdkx.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zdqjudy.top/gtcjmqdiev.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.0kj1m.cn/gtzamyvduu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.andypj.xyz/gtiilkhyir.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.haohaochexian.top/gtqjnktdoz.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.mhx1999.top/gtkmjsvlop.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhengqikj.top/gtlipjwsct.html

[H10] 资源自动释放
来源：http://hz.chenzaomai.com/gtujinmkbc.html


<!-- 参考信息 -->