代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://hz.cucudq.cn/gtchpfjgml.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.cucudq.cn/gtvhurhbib.html

PHP:  file_exists("a.txt");
来源：http://hz.svipenyu.cn/gtvkaewspu.html

JS:   fs.existsSync("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtsukuwvzu.html

TS:   fs.existsSync("a.txt")
来源：http://hz.jinghuilouyu.cn/gtmwbuaixv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.quarkkingdee.top/gtvphhpfjx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zhaomingkeji.xyz/gtztdddwtw.html

Ruby: File.exist?("a.txt")
来源：http://hz.gzhubu.top/gtntpdejnu.html

C#:   File.Exists("a.txt")
来源：http://hz.gaohongyu789.top/gtwhvnuvja.html

[F06] 删除文件
来源：http://hz.chenjidiqi.icu/gtywnzfrif.html

Py:   os.remove("a.txt")
来源：http://hz.zhixingplan.top/gtqmxhrrpl.html

PHP:  unlink("a.txt");
来源：http://hz.ehwqpu.com/gtdcmvvmtn.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.guannengcc.top/gtruorupbk.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jinqigfzy.top/gtdbqbfath.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.meibo888.top/gttqbqxloj.html

Go:   os.Remove("a.txt")
来源：http://hz.jqgufenzy.top/gtcitrtipo.html

Ruby: File.delete("a.txt")
来源：http://hz.cheryme.top/gtxtgopvth.html

C#:   File.Delete("a.txt");
来源：http://hz.shuidangran.top/gtdugilpnu.html

[F07] 创建目录（含多级）
来源：http://hz.svipenyu.cn/gtncunhvuz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zhixingplan.top/gtwsnlmaob.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zhixingplan.top/gtlecpklbq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jianghu66.top/gtzpjohigx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.c1oappe.top/gtbtmnpodm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.fengsongda.top/gtzgowyvzv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hysaishi.cn/gtevgcypkt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.redwolf501.top/gtjpjtmujl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jianghu66.top/gtbvwtlsei.html

[F08] 遍历目录
来源：http://hz.sweek.top/gtnrsdinyh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.ywan-chungtsiang.top/gtoignmodu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.hfpthk.cn/gtvxnzqqwu.html

JS:   fs.readdirSync("dir")
来源：http://hz.hongshengwenyu.top/gtwvutwwpv.html

TS:   fs.readdirSync("dir")
来源：http://hz.jlsjyb.cn/gtuuvugdub.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.daria6918.cn/gtemqnpyqa.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zhijiandao.cn/gtxrpvqafk.html

Ruby: Dir.children("dir")
来源：http://hz.gzhubu.top/gtoxvhthfv.html

C#:   Directory.GetFiles("dir")
来源：http://hz.fengsongda.top/gtziljvvfi.html

[F09] 获取文件大小
来源：http://hz.guannengcc.top/gtvfdyrvvg.html

Py:   os.path.getsize("a.txt")
来源：http://hz.dianchejie.cn/gtmyurrysz.html

PHP:  filesize("a.txt");
来源：http://hz.hysaishi.cn/gtyzmolrsm.html

JS:   fs.statSync("a.txt").size
来源：http://hz.nanxuanxn.top/gtfojdiafa.html

TS:   fs.statSync("a.txt").size
来源：http://hz.andypj.xyz/gtlkryxkod.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zhixingplan.top/gtgfrlbqzx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.quarkkingdee.top/gtdkxkyarm.html

Ruby: File.size("a.txt")
来源：http://hz.cucudq.cn/gtwoqxvhoj.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.9152youxi.cn/gtclyjmxjp.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yuxming.cn/gtnovlfljh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.ybcxt.top/gtdtnyrpyv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jinqigfzy.top/gtdsfrzcci.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.0kj1m.cn/gtgiziyqof.html

TS:   path.extname("a.txt")
来源：http://hz.zhengqikj.top/gttwhgdjlk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.meibo888.top/gtsczkrfov.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jqgfzy.top/gtomdlzwnd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jinghuilouyu.cn/gtsyvcbfmu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yangfankeji.com/gtpzeufgvs.html

[F11] 复制与移动文件
来源：http://hz.aizwys.cn/gtuescnhmd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.redwolf501.top/gtrnlzxxkj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.kuanghao11.cn/gtbsmdhxgu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shanyushiyangtech.top/gtnchtmuet.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.daxiang520.top/gtjudbqrkf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yuxming.cn/gtziozlezl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.iojbl.cn/gtjshxlkwz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.kuanghao11.cn/gtrtwocyyy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.nwbrower.top/gtfpotqkko.html

[F12] CSV 读写
来源：http://hz.shuidangran.top/gtotihmwcr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.316326.xyz/gtvdnkwral.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.xuanzx.com/gtjbmgyrvb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.snrcjt.cn/gtirinrwfr.html

TS:   // 同上
来源：http://hz.52xcode.cn/gtptgagnys.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yangfankeji.com/gtrtzkxdgv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhaomingkeji.xyz/gtrtrgohrh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.quarkkingdee.top/gtsyibdglr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.ydzc1.top/gtxjfdkdhb.html

================================================================================
来源：http://hz.nanxinkj.top/gtzqsqnhpl.html

G. 面向对象
来源：http://hz.yj202588.top/gtdoocmzrk.html

================================================================================
来源：http://hz.ppjwa.cn/gtykcjbkhq.html

[G01] 定义类
来源：http://hz.ybcxt.top/gtdljutfzg.html

Py:   class User: pass
来源：http://hz.bjfxy.top/gttrgykxgn.html

PHP:  class User {}
来源：http://hz.ehwqpu.com/gtyiwcvwwp.html

JS:   class User {}
来源：http://hz.dianchejie.cn/gtwdsspzfr.html

TS:   class User { name: string = ""; }
来源：http://hz.daxiang520.top/gtjpwoufti.html

Java: class User {}
来源：http://hz.gaohongyu789.top/gtzwukyrhg.html

Go:   type User struct { Name string }
来源：http://hz.bjfxy.top/gtbnykpphx.html

Ruby: class User; end
来源：http://hz.ivvv.top/gthjuieeew.html

C#:   class User {}
来源：http://hz.hywenlv.cn/gtkfvyvuyb.html

[G02] 构造函数
来源：http://hz.ywan-chungtsiang.top/gtmgsgogit.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yongpay.top/gtmvhsndwr.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jinghuilouyu.cn/gttbwnfvyv.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.havefunace.top/gtybtwwzwh.html

TS:   constructor(public name: string) {}
来源：http://hz.zhongyouzk.top/gtqrutdhxo.html

Java: User(String name) { this.name = name; }
来源：http://hz.c1oappe.top/gtdznbdgjt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.ydjk.org.cn/gtuiqdqnbq.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yonumen.top/gtcradcwrq.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yangfankeji.com/gtnggqxnqt.html

[G03] 实例属性
来源：http://hz.sweek.top/gtbokyimmy.html

Py:   self.name = "x"
来源：http://hz.zdqjudy.top/gtnzrkrhtc.html

PHP:  public string $name = "x";
来源：http://hz.iojbl.cn/gtrcmjtbda.html

JS:   this.name = "x";
来源：http://hz.daxiang520.top/gtbggnbkgz.html

TS:   name: string = "x";
来源：http://hz.cdnleiting.top/gtntvhmynp.html

Java: private String name;
来源：http://hz.zhaomingkeji.xyz/gtzxykttqt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.sysykeji.top/gtqubhmzvv.html

Ruby: @name = "x"
来源：http://hz.havefunace.top/gtfuiuhahu.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hysaishi.cn/gtghwegrul.html

[G04] 定义方法
来源：http://hz.hysaishi.cn/gtaksigdqy.html

Py:   def greet(self): return self.name
来源：http://hz.fengsongda.top/gtyibfoxie.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yvedp.cn/gtmmmechib.html

JS:   greet() { return this.name; }
来源：http://hz.yongpay.top/gtgytxltuy.html

TS:   greet(): string { return this.name; }
来源：http://hz.ppjwa.cn/gteaktkalb.html

Java: String greet() { return name; }
来源：http://hz.zhiwuduotai.top/gtswqjvpge.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yangfankeji.com/gtltvsfxdu.html

Ruby: def greet; @name; end
来源：http://hz.xingfuxueyuan.xyz/gtlzcktqrv.html

C#:   public string Greet() => Name;
来源：http://hz.yanxiufei.cn/gtftztyuxf.html

[G05] 继承
来源：http://hz.cdnleiting.top/gtvbrbjiku.html

Py:   class Admin(User): pass
来源：http://hz.nwbrower.top/gtemhqupoi.html

PHP:  class Admin extends User {}
来源：http://hz.vqdsnc.cn/gtoweuntyv.html

JS:   class Admin extends User {}
来源：http://hz.zdqjudy.top/gtsmihtaiq.html

TS:   class Admin extends User {}
来源：http://hz.iojbl.cn/gtdmcpjooi.html

Java: class Admin extends User {}
来源：http://hz.dianchejie.cn/gtmfuurxbi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.chenlongwang.top/gtdcrmryrv.html

Ruby: class Admin < User; end
来源：http://hz.cqqwz.cn/gthcwqfkhs.html

C#:   class Admin : User {}
来源：http://hz.jinqigfzy.top/gtzjvebmdy.html

[G06] 重写方法
来源：http://hz.shzxlz.cn/gtlmqdlwno.html

Py:   def greet(self): return "admin"
来源：http://hz.gogol.net.cn/gtijfnntjn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.quarkkingdee.top/gtxjsaexcq.html

JS:   greet() { return "admin"; }
来源：http://hz.yuxming.cn/gtvibmknqe.html

TS:   greet(): string { return "admin"; }
来源：http://hz.shangyingyoupin.top/gtdvgpqtun.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jqgfzy.top/gtgkmyljoe.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.ppjwa.cn/gtivsksalj.html

Ruby: def greet; "admin"; end
来源：http://hz.redwolf501.top/gtwvgofdlo.html

C#:   public override string Greet() => "admin";
来源：http://hz.ehwqpu.com/gtskzdnwhm.html

[G07] 调用父类方法
来源：http://hz.nwbrower.top/gtmlasebov.html

Py:   super().greet()
来源：http://hz.zhaomingkeji.xyz/gtnszknqza.html

PHP:  parent::greet();
来源：http://hz.andypj.xyz/gtjapyugcf.html

JS:   super.greet();
来源：http://hz.fzhhl.top/gtwwjhqfiv.html

TS:   super.greet();
来源：http://hz.shzxlz.cn/gtwzbanuor.html

Java: super.greet();
来源：http://hz.wangshuangyany.cn/gtvvgszcyr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.chenjidiqi.icu/gtkeyqoktb.html

Ruby: super
来源：http://hz.yuanzhike.top/gtjspibqtm.html

C#:   base.Greet();
来源：http://hz.jinyuanbaomall.cn/gtsymgtgcn.html

[G08] 静态方法与属性
来源：http://hz.zhoulong.xyz/gtwipsgbzy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.chenzaomai.com/gtuitwnjxc.html

PHP:  public static function f() {}
来源：http://hz.ydjk.org.cn/gtsjjbhxdf.html

JS:   static f() {}
来源：http://hz.birdmap.top/gtbsedmfus.html

TS:   static f(): void {}
来源：http://hz.wangdashe.top/gtxzphnwhj.html

Java: static void f() {}
来源：http://hz.wangdashe.top/gtqejawhmt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.xuetiantiany.cn/gtezgznvso.html

Ruby: def self.f; end
来源：http://hz.ehwqpu.com/gtlvhedwnf.html

C#:   public static void F() {}
来源：http://hz.zhaomingkeji.xyz/gtieujecyn.html

[G09] 接口 / 抽象类
来源：http://hz.aizwys.cn/gtjhmjnasd.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yonumen.top/gtqmfbfmtl.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yonumen.top/gtebgkksyg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yj20258.top/gtdirpifuy.html

TS:   interface Shape { area(): number; }
来源：http://hz.yueranfly.top/gtrlrbqchk.html

Java: interface Shape { double area(); }
来源：http://hz.meibo888.top/gtoiehxwen.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.andypj.xyz/gttzgknvsk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hywenlv.cn/gtywovxjye.html

C#:   interface IShape { double Area(); }
来源：http://hz.pycfn.com/gtlcbrfzti.html

[G10] 访问控制
来源：http://hz.gaohongyu789.top/gtkyjegzqo.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhongyouzk.top/gtnydjzgpf.html

PHP:  public / protected / private
来源：http://hz.cashguo.top/gtkizesbfx.html

JS:   #private 字段；其余公开
来源：http://hz.meibo888.top/gtemlnwowe.html

TS:   public / protected / private
来源：http://hz.sysykeji.top/gtqijdelut.html

Java: public / protected / private / 默认包级
来源：http://hz.gotoacloud.top/gtfeshebap.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.tanke756.top/gtaspfyagn.html

Ruby: public / protected / private
来源：http://hz.pengpengdd.cyou/gtqdtdhsxd.html

C#:   public / protected / private / internal
来源：http://hz.jinyuanbaomall.cn/gtlhjmznko.html

[G11] getter / setter
来源：http://hz.smart0.xyz/gtbbgbxtpz.html

Py:   @property 与 @x.setter
来源：http://hz.c1oappe.top/gtzpvnhqqe.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.chenjidiqi.icu/gtgsogtlbm.html

JS:   get name() { return this._name; }
来源：http://hz.dianchejie.cn/gttbapirur.html

TS:   get name(): string { return this._name; }
来源：http://hz.ydzc1.top/gteurotdzs.html

Java: public String getName() { return name; }
来源：http://hz.tianlin.xyz/gtsenfjkxi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.guannengcc.top/gtlcxdhpbt.html

Ruby: attr_accessor :name
来源：http://hz.xinyue.icu/gtiaqkppsf.html

C#:   public string Name { get; set; }
来源：http://hz.zhiwuduotai.top/gtmhhlyypd.html

[G12] 对象转字符串
来源：http://hz.dianchejie.cn/gtzmpawpqn.html

Py:   def __str__(self): return self.name
来源：http://hz.0kj1m.cn/gtkqgfcbeg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.andypj.xyz/gttgycibzj.html

JS:   toString() { return this.name; }
来源：http://hz.snrcjt.cn/gtawpkanpe.html

TS:   toString(): string { return this.name; }
来源：http://hz.nanxinkj.top/gtapbklllc.html

Java: @Override public String toString() { return name; }
来源：http://hz.xziqi.cn/gttofmaosp.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhijiandao.cn/gtrnprzvin.html

Ruby: def to_s; @name; end
来源：http://hz.xuanzx.com/gthgmjmahj.html

C#:   public override string ToString() => Name;
来源：http://hz.redwolf501.top/gthwnevipo.html

[G13] 判断对象类型
来源：http://hz.zhoulong.xyz/gtbsrjtydj.html

Py:   isinstance(u, User)
来源：http://hz.kuanghao11.cn/gtkeyttoyz.html

PHP:  $u instanceof User
来源：http://hz.chenlongwang.top/gthdgkrlqz.html

JS:   u instanceof User
来源：http://hz.hysaishi.cn/gtafyyryrt.html

TS:   u instanceof User
来源：http://hz.xuanzx.com/gtqarisxcw.html

Java: u instanceof User
来源：http://hz.tanke756.top/gtuuwxvjuf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ydzc1.top/gtefrluvmj.html

Ruby: u.is_a?(User)
来源：http://hz.nanxinkj.top/gtywzoalyc.html

C#:   u is User
来源：http://hz.gotoacloud.top/gtrtjyzbug.html

[G14] 数据类 / record
来源：http://hz.52xcode.cn/gtubodfhjd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jinghuilouyu.cn/gtoogsvilh.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.wangdashe.top/gtybssvbnc.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.shuidangran.top/gtiizddzrt.html

TS:   type User = { name: string; age: number };
来源：http://hz.daxiang520.top/gtkzjwfrpa.html

Java: record User(String name, int age) {}
来源：http://hz.wangshuangyany.cn/gtzkgbguky.html

Go:   type User struct { Name string; Age int }
来源：http://hz.c1oappe.top/gtutslynxa.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.sysykeji.top/gtwshrqynl.html

C#:   record User(string Name, int Age);
来源：http://hz.xziqi.cn/gtudkzryar.html

[G15] 枚举
来源：http://hz.yuanzhike.top/gthddqifvu.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.gaohongyu789.top/gtpdscvzck.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.gaohongyu789.top/gtrqfhtwkf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yanxiufei.cn/gtisugljni.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.redwolf501.top/gtfbvrzncy.html

Java: enum Color { RED, GREEN }
来源：http://hz.yvedp.cn/gtscenrdhy.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yj202588.top/gtbjqidpna.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yj20258888.top/gtxecplvwy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shzxlz.cn/gtrdjfwhxp.html

[G16] 对象转数组 / 字典
来源：http://hz.yj202588.top/gtpvfojtsz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.iojbl.cn/gtaojqdott.html

PHP:  get_object_vars($obj);
来源：http://hz.52xcode.cn/gtwrnatpfz.html

JS:   Object.entries(obj)
来源：http://hz.sxryk.cn/gtymcmytyf.html

TS:   Object.entries(obj)
来源：http://hz.vqdsnc.cn/gtjaclkweg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.52xcode.cn/gtlsirwpyg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.52xcode.cn/gtjcvfkkea.html

Ruby: obj.instance_variables
来源：http://hz.gzhubu.top/gtuuttqvmk.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yuanzhike.top/gtvgnddjgr.html

================================================================================
来源：http://hz.hammf.cn/gtzdqpfvtc.html

H. 异常与错误处理
来源：http://hz.yj202588.top/gtxnnrmump.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtjdufoqxv.html

[H01] try / catch 基础
来源：http://hz.daria6918.cn/gtzegdbxol.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yangfankeji.com/gtmhkdcbpj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.shanyushiyangtech.top/gtxkmkxstt.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jqgfzy.top/gthbfdtoxp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.nwbrower.top/gtmeelqwkk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.daxiang520.top/gtjdffanjg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.xingfuxueyuan.xyz/gtcresnxxv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.shanyushiyangtech.top/gtvtprdvby.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.wangdashe.top/gtkxbunpzd.html

[H02] finally / ensure 收尾
来源：http://hz.jinyuanbaomall.cn/gtozmkdsfw.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.ppjwa.cn/gtgggwlqzx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.nanxinkj.top/gtmrndjwao.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.vqdsnc.cn/gtvlbwqlka.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.tian-w.cn/gtlguoafgg.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhoulong.xyz/gtoysblkuf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.aizwys.cn/gtgedtpwfu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yj20258888.top/gthbqhzqke.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.guannengcc.top/gtnnjhwfnw.html

[H03] 主动抛出异常
来源：http://hz.yongpay.top/gtdhsfrptt.html

Py:   raise ValueError("错误信息")
来源：http://hz.zhengqikj.top/gtaqyehvvu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.sxryk.cn/gtdjtrlisw.html

JS:   throw new Error("错误信息");
来源：http://hz.snrcjt.cn/gtttpdwxzr.html

TS:   throw new Error("错误信息");
来源：http://hz.redwolf501.top/gtbsxxrqza.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jinghuilouyu.cn/gttaxprrdz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hammf.cn/gtonxiayqi.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.mhx1999.top/gtzqcmmabv.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.shangyingyoupin.top/gtcqdshkyq.html

[H04] 自定义异常类型
来源：http://hz.nanxinkj.top/gtuplemllu.html

Py:   class MyError(Exception): pass
来源：http://hz.52xcode.cn/gtxdiswouu.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.iojbl.cn/gtfvtvrusd.html

JS:   class MyError extends Error {}
来源：http://hz.jqgfzy.top/gtnddlyzkb.html

TS:   class MyError extends Error {}
来源：http://hz.ppjwa.cn/gtbulaxqmp.html

Java: class MyException extends RuntimeException {}
来源：http://hz.pycfn.com/gtxuzhjfvi.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.dianchejie.cn/gtunmfrupx.html

Ruby: class MyError < StandardError; end
来源：http://hz.yuanzhike.top/gttlsdxpnj.html

C#:   class MyException : Exception {}
来源：http://hz.aizwys.cn/gtszkpfoxt.html

[H05] 捕获特定类型
来源：http://hz.tanke756.top/gtvxkpmptt.html

Py:   except ValueError as e:
来源：http://hz.zhoulong.xyz/gtvdjleilp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.hammf.cn/gtlxgqmoch.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.bjfxy.top/gtshcetffy.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.smart0.xyz/gtlieqqpgj.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.shanyushiyangtech.top/gtpemccqlx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hywenlv.cn/gtvmndfwly.html

Ruby: rescue ArgumentError => e
来源：http://hz.gotoacloud.top/gtepejjvvu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yuanzhike.top/gtsnckqhbx.html

[H06] 可选值 / 空值安全访问
来源：http://hz.haohaochexian.top/gtcdxdzpji.html

Py:   value = d.get("k") or default
来源：http://hz.yanxiufei.cn/gtbymjzchi.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.c1oappe.top/gtnwdexbet.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.hammf.cn/gtdpvavmmo.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.aibaodan.cn/gtrkrnujlb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.hnxiangtu.top/gtcopxjoif.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.xuanzx.com/gtndvneakc.html

Ruby: d&.dig(:a, :b)
来源：http://hz.316326.xyz/gtajasiyne.html

C#:   obj?.A?.B ?? default
来源：http://hz.guowangkeji.top/gtkjbddiza.html

[H07] 断言
来源：http://hz.jiagoushi.top/gtsfjnjsmm.html

Py:   assert x > 0, "必须为正"
来源：http://hz.daxiang520.top/gtpihpytjf.html

PHP:  assert($x > 0);
来源：http://hz.xuanzx.com/gtvyxvgyrg.html

JS:   console.assert(x > 0);
来源：http://hz.ywan-chungtsiang.top/gtmsbcwvfr.html

TS:   console.assert(x > 0);
来源：http://hz.0kj1m.cn/gtstklfwmi.html

Java: assert x > 0 : "必须为正";
来源：http://hz.sufxvd.cn/gtixgbkjjb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.tanke756.top/gtgftnzipe.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.shuidangran.top/gtflidubnn.html

C#:   Debug.Assert(x > 0);
来源：http://hz.bjfxy.top/gtnjnlmnrc.html

[H08] 获取错误信息与堆栈
来源：http://hz.hywenlv.cn/gtputqveat.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.nanxinkj.top/gtghodqeou.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.52xcode.cn/gtxzyvwxex.html

JS:   e.message;  e.stack
来源：http://hz.vqdsnc.cn/gtnvgkgzeh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.ywan-chungtsiang.top/gtksxgtkmk.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hysaishi.cn/gtkertvkps.html

Go:   err.Error()
来源：http://hz.dashuyun.cn/gtinshfyyd.html

Ruby: e.message;  e.backtrace
来源：http://hz.chenzaomai.com/gtpkxcqnst.html

C#:   e.Message;  e.StackTrace
来源：http://hz.tanke756.top/gtomiqfurq.html

[H09] 带错误码的异常
来源：http://hz.mhx1999.top/gtsgoixbzw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.sufxvd.cn/gtknvpcink.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.316326.xyz/gtjcpbplaa.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.svipenyu.cn/gttvtzweuo.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.fzhhl.top/gtsfgycbtn.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.snrcjt.cn/gtqekeplcu.html


<!-- 参考信息 -->