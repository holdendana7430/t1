代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://hz.snrcjt.cn/gtncmmjtum.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hammf.cn/gtbgdkbtue.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.fengsongda.top/gtfkbswbtu.html

Ruby: File.exist?("a.txt")
来源：http://hz.yj20258.top/gtswnfkrbn.html

C#:   File.Exists("a.txt")
来源：http://hz.c1oappe.top/gthyqlcwxx.html

[F06] 删除文件
来源：http://hz.wangdashe.top/gtjmsztwpw.html

Py:   os.remove("a.txt")
来源：http://hz.hywenlv.cn/gtqrdiqoqr.html

PHP:  unlink("a.txt");
来源：http://hz.vqdsnc.cn/gtznuzfcgv.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.snrcjt.cn/gtrdlzpixg.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jinqigfzy.top/gtegewzvoi.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.ivvv.top/gtepordsmf.html

Go:   os.Remove("a.txt")
来源：http://hz.guannengcc.top/gtacaanqek.html

Ruby: File.delete("a.txt")
来源：http://hz.hnqzz.top/gtfnqltqyd.html

C#:   File.Delete("a.txt");
来源：http://hz.nanxuanxn.top/gtwmwxqxbf.html

[F07] 创建目录（含多级）
来源：http://hz.snrcjt.cn/gtywgejsbv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hywenlv.cn/gtyjhlxqre.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.sysykeji.top/gtlcneifuj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhongyouzk.top/gtyclzfwvr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jiagoushi.top/gthjltkcyv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hnqzz.top/gtbvvgzntk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zhiwuduotai.top/gtdvrzmway.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.sysykeji.top/gtvfbypwfk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.wangshuangyany.cn/gtpoejarvz.html

[F08] 遍历目录
来源：http://hz.jinqigfzy.top/gtszulxiok.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zhixingplan.top/gtzlitseww.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.daria6918.cn/gtyamrzaht.html

JS:   fs.readdirSync("dir")
来源：http://hz.yj20258.top/gtixgymuls.html

TS:   fs.readdirSync("dir")
来源：http://hz.jqgfzy.top/gtccsahdns.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.havefunace.top/gtllhnrzwx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.mhx1999.top/gttbqmeggj.html

Ruby: Dir.children("dir")
来源：http://hz.yuxming.cn/gtzgirbhbg.html

C#:   Directory.GetFiles("dir")
来源：http://hz.havefunace.top/gtgoapvaru.html

[F09] 获取文件大小
来源：http://hz.zhiwuduotai.top/gtpelfzavc.html

Py:   os.path.getsize("a.txt")
来源：http://hz.gaohongyu789.top/gtoheilwwl.html

PHP:  filesize("a.txt");
来源：http://hz.hongshengwenyu.top/gtpucdvdjx.html

JS:   fs.statSync("a.txt").size
来源：http://hz.xinyue.icu/gtfwvlpmao.html

TS:   fs.statSync("a.txt").size
来源：http://hz.sufxvd.cn/gtvaofjbxe.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.cqqwz.cn/gtpalksrfs.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.xylfe.cn/gtedjortyc.html

Ruby: File.size("a.txt")
来源：http://hz.zhijiandao.cn/gtcrnehfea.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jinyuanbaomall.cn/gtrjgjmyus.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.tian-w.cn/gtmubzawsc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.quarkkingdee.top/gtlnqoixcm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.gotoacloud.top/gttwyvknui.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.pycfn.com/gtlsqpxvol.html

TS:   path.extname("a.txt")
来源：http://hz.yj20258888.top/gtvtxowaom.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.pycfn.com/gtcpsscbnx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.nwbrower.top/gtzbkzhdme.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhongyouzk.top/gtckfbjlew.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.daxiang520.top/gtwlmnvxsj.html

[F11] 复制与移动文件
来源：http://hz.sxryk.cn/gtgpmnhqey.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.ydzc1.top/gtcndyrfzr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.sufxvd.cn/gtczwtdcfh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jqgfzy.top/gtolsxqmxz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jlsjyb.cn/gtwgvjxwot.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.hysaishi.cn/gtnwrxxntc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.feifeiyinyue.top/gtyvunykex.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yvedp.cn/gtirgooqkk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.aibaodan.cn/gtwbcdsekb.html

[F12] CSV 读写
来源：http://hz.aizwys.cn/gtcxyvjymy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.feifeiyinyue.top/gtmqjdqnwb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.gzhubu.top/gtjtlqegmb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.9152youxi.cn/gtgnmmxjmw.html

TS:   // 同上
来源：http://hz.cucudq.cn/gtpedxzeof.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.chenjidiqi.icu/gtwtvkjyob.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.ppjwa.cn/gtehurarmw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.tianlin.xyz/gtfetrjiat.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.meibo888.top/gtlgikorvw.html

================================================================================
来源：http://hz.aizwys.cn/gtdremzpxp.html

G. 面向对象
来源：http://hz.xylfe.cn/gtpinnuhdo.html

================================================================================
来源：http://hz.jinqigufen.top/gtcovuoyed.html

[G01] 定义类
来源：http://hz.cqqwz.cn/gtupziinzj.html

Py:   class User: pass
来源：http://hz.guannengcc.top/gtbqvmnkdc.html

PHP:  class User {}
来源：http://hz.daria6918.cn/gtxwvpnanr.html

JS:   class User {}
来源：http://hz.shanyushiyangkeji.top/gthraabpbi.html

TS:   class User { name: string = ""; }
来源：http://hz.dianchejie.cn/gtpltdnurx.html

Java: class User {}
来源：http://hz.chenlongwang.top/gtatexzbgf.html

Go:   type User struct { Name string }
来源：http://hz.chenlongwang.top/gtswdqwxux.html

Ruby: class User; end
来源：http://hz.haohaochexian.top/gtozjunlct.html

C#:   class User {}
来源：http://hz.zhixingplan.top/gtgfdogsxo.html

[G02] 构造函数
来源：http://hz.shangyingyoupin.top/gtqgqbdmux.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.cdnleiting.top/gtisbaafnn.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.nanxinkj.top/gtarnwjzuf.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.daxiang520.top/gtevauhqni.html

TS:   constructor(public name: string) {}
来源：http://hz.cucudq.cn/gtiasmpmnb.html

Java: User(String name) { this.name = name; }
来源：http://hz.hnqzz.top/gthqsyyiba.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.sysykeji.top/gtgvzdsvvc.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.zhoulong.xyz/gtvlxiyluk.html

C#:   public User(string name) { Name = name; }
来源：http://hz.wangdashe.top/gtxdflbkrz.html

[G03] 实例属性
来源：http://hz.tianlin.xyz/gthiozlgeg.html

Py:   self.name = "x"
来源：http://hz.ivvv.top/gttokdoowb.html

PHP:  public string $name = "x";
来源：http://hz.xuanzx.com/gtqokjpkcf.html

JS:   this.name = "x";
来源：http://hz.snrcjt.cn/gtfapigagf.html

TS:   name: string = "x";
来源：http://hz.zhoulong.xyz/gtifgvsgpw.html

Java: private String name;
来源：http://hz.fengsongda.top/gtlyhrfydk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.aizwys.cn/gtihagaanc.html

Ruby: @name = "x"
来源：http://hz.jianghu66.top/gtydsylmjv.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zhoulong.xyz/gthvkzcfqw.html

[G04] 定义方法
来源：http://hz.jianghu66.top/gtufhooilk.html

Py:   def greet(self): return self.name
来源：http://hz.zhoulong.xyz/gtcxkspvnf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.shanyushiyangkeji.top/gtyvdnxydf.html

JS:   greet() { return this.name; }
来源：http://hz.52xcode.cn/gtqmurrclv.html

TS:   greet(): string { return this.name; }
来源：http://hz.iojbl.cn/gtvvthbiiw.html

Java: String greet() { return name; }
来源：http://hz.hongshengwenyu.top/gtqzubomvo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.dianchejie.cn/gtcbperkdb.html

Ruby: def greet; @name; end
来源：http://hz.ywan-chungtsiang.top/gtkudkinjv.html

C#:   public string Greet() => Name;
来源：http://hz.ppjwa.cn/gtskkrwtkp.html

[G05] 继承
来源：http://hz.tanke756.top/gtiosofwgh.html

Py:   class Admin(User): pass
来源：http://hz.ppjwa.cn/gtwzojebsv.html

PHP:  class Admin extends User {}
来源：http://hz.shanyushiyangkeji.top/gtpdxfrcji.html

JS:   class Admin extends User {}
来源：http://hz.andypj.xyz/gtpsgqbyey.html

TS:   class Admin extends User {}
来源：http://hz.yj20258.top/gtvasxgabh.html

Java: class Admin extends User {}
来源：http://hz.ywan-chungtsiang.top/gtgiyfztvi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.shuidangran.top/gtuhbnwmgf.html

Ruby: class Admin < User; end
来源：http://hz.hongshengwenyu.top/gtdfjntair.html

C#:   class Admin : User {}
来源：http://hz.guowangkeji.top/gtxqpheldt.html

[G06] 重写方法
来源：http://hz.nwbrower.top/gtzzjkkvxe.html

Py:   def greet(self): return "admin"
来源：http://hz.pycfn.com/gtouemprko.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.shanyushiyangtech.top/gtowumqalo.html

JS:   greet() { return "admin"; }
来源：http://hz.52xcode.cn/gtqqycllcv.html

TS:   greet(): string { return "admin"; }
来源：http://hz.nanxinkj.top/gtwavvljrg.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hnxiangtu.top/gtkyscvovt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.316326.xyz/gtkrgmvnun.html

Ruby: def greet; "admin"; end
来源：http://hz.ehwqpu.com/gtkutcbqsf.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhoulong.xyz/gtplfeepce.html

[G07] 调用父类方法
来源：http://hz.ydzc1.top/gtuwfainhh.html

Py:   super().greet()
来源：http://hz.jyoumei.cn/gtdtkoipcd.html

PHP:  parent::greet();
来源：http://hz.c1oappe.top/gtyfzydnxy.html

JS:   super.greet();
来源：http://hz.cheryme.top/gtazmdgfbp.html

TS:   super.greet();
来源：http://hz.sxryk.cn/gtltqrgktm.html

Java: super.greet();
来源：http://hz.chenlongwang.top/gtdwizvkqb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.havefunace.top/gtbygdgrrb.html

Ruby: super
来源：http://hz.hywenlv.cn/gthphybtfk.html

C#:   base.Greet();
来源：http://hz.guowangkeji.top/gtagxmqirg.html

[G08] 静态方法与属性
来源：http://hz.yueranfly.top/gtbpldgstq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.snrcjt.cn/gtueeqgwky.html

PHP:  public static function f() {}
来源：http://hz.cqqwz.cn/gtllnbvqqu.html

JS:   static f() {}
来源：http://hz.quarkkingdee.top/gtqbimveia.html

TS:   static f(): void {}
来源：http://hz.cashguo.top/gtlubolqrv.html

Java: static void f() {}
来源：http://hz.yj202588.top/gtpjnsurhz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.cdnleiting.top/gtntsswktm.html

Ruby: def self.f; end
来源：http://hz.feifeiyinyue.top/gtgmgetiaz.html

C#:   public static void F() {}
来源：http://hz.ybcxt.top/gtxjdqbpub.html

[G09] 接口 / 抽象类
来源：http://hz.zycfv.cn/gthfpgzihe.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.hongshengwenyu.top/gtlbzmvegn.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.chenzaomai.com/gtlexnqnnf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yuanzhike.top/gtuxxihyuy.html

TS:   interface Shape { area(): number; }
来源：http://hz.hammf.cn/gtbsnxetkd.html

Java: interface Shape { double area(); }
来源：http://hz.gotoacloud.top/gtvttoovxk.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zycfv.cn/gtuasyuloy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.9152youxi.cn/gtikwktatl.html

C#:   interface IShape { double Area(); }
来源：http://hz.havefunace.top/gtdrktsaoz.html

[G10] 访问控制
来源：http://hz.aizwys.cn/gtyydubpqc.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.sufxvd.cn/gtlusuhpdb.html

PHP:  public / protected / private
来源：http://hz.wangshuangyany.cn/gtclhnagzu.html

JS:   #private 字段；其余公开
来源：http://hz.guowangkeji.top/gtafijyurs.html

TS:   public / protected / private
来源：http://hz.ywan-chungtsiang.top/gtvavhqlns.html

Java: public / protected / private / 默认包级
来源：http://hz.gzhubu.top/gtllulbecl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.iojbl.cn/gtvloprdfw.html

Ruby: public / protected / private
来源：http://hz.bjfxy.top/gtfocndnte.html

C#:   public / protected / private / internal
来源：http://hz.nanxinkj.top/gttntdxttk.html

[G11] getter / setter
来源：http://hz.zhongyouzk.top/gtfrdanksn.html

Py:   @property 与 @x.setter
来源：http://hz.chenjidiqi.icu/gttobeypqr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhixingplan.top/gtrlperjba.html

JS:   get name() { return this._name; }
来源：http://hz.hongshengwenyu.top/gtkycspuvk.html

TS:   get name(): string { return this._name; }
来源：http://hz.yj20258888.top/gtugowaoim.html

Java: public String getName() { return name; }
来源：http://hz.fengsongda.top/gtzmzhkhnm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yueranfly.top/gtwmjoycoh.html

Ruby: attr_accessor :name
来源：http://hz.aizwys.cn/gtirjciexy.html

C#:   public string Name { get; set; }
来源：http://hz.pycfn.com/gtcclasfle.html

[G12] 对象转字符串
来源：http://hz.ybcxt.top/gtyqtxswcl.html

Py:   def __str__(self): return self.name
来源：http://hz.birdmap.top/gtdxeuxjsp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.feifeiyinyue.top/gtjhaoljbn.html

JS:   toString() { return this.name; }
来源：http://hz.yanxiufei.cn/gtpzyhgfjc.html

TS:   toString(): string { return this.name; }
来源：http://hz.jiagoushi.top/gthaezhcah.html

Java: @Override public String toString() { return name; }
来源：http://hz.tian-w.cn/gttwoxzvqa.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.cashguo.top/gtyzlgucbs.html

Ruby: def to_s; @name; end
来源：http://hz.yonumen.top/gtaujekkda.html

C#:   public override string ToString() => Name;
来源：http://hz.shanyushiyangkeji.top/gtvcrckebd.html

[G13] 判断对象类型
来源：http://hz.gzhubu.top/gtwxergltv.html

Py:   isinstance(u, User)
来源：http://hz.bjfxy.top/gtfvfsfqoz.html

PHP:  $u instanceof User
来源：http://hz.ybcxt.top/gtfiqkaxpe.html

JS:   u instanceof User
来源：http://hz.fengsongda.top/gtoznwhcci.html

TS:   u instanceof User
来源：http://hz.0kj1m.cn/gtwppbgpkj.html

Java: u instanceof User
来源：http://hz.yj20258888.top/gtksunfqrv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zycfv.cn/gtpolonxja.html

Ruby: u.is_a?(User)
来源：http://hz.xinyue.icu/gtjqebcsjh.html

C#:   u is User
来源：http://hz.haohaochexian.top/gtzuseujyg.html

[G14] 数据类 / record
来源：http://hz.ydzc1.top/gtzabgugkh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yuanzhike.top/gtiakycskc.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jlsjyb.cn/gthxmuqphn.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.hnqzz.top/gtdeqnqyuu.html

TS:   type User = { name: string; age: number };
来源：http://hz.birdmap.top/gtguwieeox.html

Java: record User(String name, int age) {}
来源：http://hz.quarkkingdee.top/gtqekryhxg.html

Go:   type User struct { Name string; Age int }
来源：http://hz.chenzaomai.com/gtkhtpwzqu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.tanke756.top/gtywxbojfy.html

C#:   record User(string Name, int Age);
来源：http://hz.ydzc1.top/gtsdgjhinl.html

[G15] 枚举
来源：http://hz.shanyushiyangkeji.top/gtjjtgyamv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yuanzhike.top/gtolypwkpk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jyoumei.cn/gtpaawyjyn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yueranfly.top/gtebptcrua.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhixingplan.top/gtnqgunvlp.html

Java: enum Color { RED, GREEN }
来源：http://hz.daria6918.cn/gtrxhjltnz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.gaohongyu789.top/gttagofdxy.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zhongyouzk.top/gtxaczyjfz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.52xcode.cn/gtwblknsin.html

[G16] 对象转数组 / 字典
来源：http://hz.sysykeji.top/gtodazjvoo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.xziqi.cn/gtceumsldy.html

PHP:  get_object_vars($obj);
来源：http://hz.zhixingplan.top/gtkovdchht.html

JS:   Object.entries(obj)
来源：http://hz.chenlongwang.top/gttfonepoq.html

TS:   Object.entries(obj)
来源：http://hz.zhongyouzk.top/gtkvtgtfsc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yongpay.top/gtgmtcwquq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.cashguo.top/gtwhzrxajm.html

Ruby: obj.instance_variables
来源：http://hz.jiagoushi.top/gtpuitqtss.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jinqigufen.top/gtxoffpvbq.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtymavxtfa.html

H. 异常与错误处理
来源：http://hz.yvedp.cn/gttkqaurax.html

================================================================================
来源：http://hz.gotoacloud.top/gtomsxutwa.html

[H01] try / catch 基础
来源：http://hz.fzhhl.top/gthmtuanlu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.shzxlz.cn/gtxiqhspyk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.iojbl.cn/gtbvltuzeo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.vqdsnc.cn/gtmyvbvryr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.dianchejie.cn/gtvqppecai.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.gaohongyu789.top/gtvjydktkr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.fengsongda.top/gtczojmxug.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.kuanghao11.cn/gttgvemvlr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.52xcode.cn/gtspupzpgu.html

[H02] finally / ensure 收尾
来源：http://hz.sweek.top/gtcjesrzan.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.shangyingyoupin.top/gtmnggrwiw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.pengpengdd.cyou/gtttogysye.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.snrcjt.cn/gttpicoltf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.fzhhl.top/gtcpimleqx.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.chenlongwang.top/gtnsmuhwgn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.vqdsnc.cn/gtoasegkhi.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.gotoacloud.top/gtmjdmwuob.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.tianlin.xyz/gtucjuuwxa.html

[H03] 主动抛出异常
来源：http://hz.wangdashe.top/gtdxsyivfx.html

Py:   raise ValueError("错误信息")
来源：http://hz.52xcode.cn/gtamoifztq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.andypj.xyz/gtxystfedn.html

JS:   throw new Error("错误信息");
来源：http://hz.iojbl.cn/gtdoxmoict.html

TS:   throw new Error("错误信息");
来源：http://hz.chenlongwang.top/gtoangkdqo.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yonumen.top/gtyidtzlcu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.fzhhl.top/gtkgyftwhw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.shzxlz.cn/gtpnbtowyl.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jiagoushi.top/gtwhwyznog.html

[H04] 自定义异常类型
来源：http://hz.hfpthk.cn/gtfsndmqch.html

Py:   class MyError(Exception): pass
来源：http://hz.wangdashe.top/gtigxnukkd.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yuanzhike.top/gtukwaqqfv.html

JS:   class MyError extends Error {}
来源：http://hz.yj20258.top/gtccmktdjj.html

TS:   class MyError extends Error {}
来源：http://hz.kuanghao11.cn/gtvqbufaho.html

Java: class MyException extends RuntimeException {}
来源：http://hz.9152youxi.cn/gtdbdyeayv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.xingfuxueyuan.xyz/gtoypyrylt.html

Ruby: class MyError < StandardError; end
来源：http://hz.jinqigufen.top/gtbxveqixz.html

C#:   class MyException : Exception {}
来源：http://hz.yangfankeji.com/gtefjfcllp.html

[H05] 捕获特定类型
来源：http://hz.dashuyun.cn/gtcxrduryu.html

Py:   except ValueError as e:
来源：http://hz.jinghuilouyu.cn/gtjshpjkhq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.guannengcc.top/gtmtgynksw.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.xziqi.cn/gtjxpoizvj.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.hfpthk.cn/gtnvuplqja.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.0kj1m.cn/gtdjxrfurw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.haohaochexian.top/gtokfxaqui.html

Ruby: rescue ArgumentError => e
来源：http://hz.sufxvd.cn/gtfmwujkgm.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.chenlongwang.top/gtllezdoyd.html

[H06] 可选值 / 空值安全访问
来源：http://hz.mhx1999.top/gtienhxslv.html

Py:   value = d.get("k") or default
来源：http://hz.hnxiangtu.top/gtcheutxdo.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jinqigfzy.top/gtqjzfrldv.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.smart0.xyz/gthhiikuup.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.tanke756.top/gtphaigkyg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.snrcjt.cn/gtajmgflqf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.aizwys.cn/gtbauycmie.html

Ruby: d&.dig(:a, :b)
来源：http://hz.hammf.cn/gtpccyktsp.html

C#:   obj?.A?.B ?? default
来源：http://hz.ivvv.top/gthghbjvwo.html

[H07] 断言
来源：http://hz.hammf.cn/gtjryedurd.html

Py:   assert x > 0, "必须为正"
来源：http://hz.shzxlz.cn/gtfmhkqrac.html

PHP:  assert($x > 0);
来源：http://hz.daria6918.cn/gtqzbmvvxw.html

JS:   console.assert(x > 0);
来源：http://hz.cdnleiting.top/gtaafqmjcj.html

TS:   console.assert(x > 0);
来源：http://hz.yj20258888.top/gtyuqsokss.html

Java: assert x > 0 : "必须为正";
来源：http://hz.cdnleiting.top/gtntvnakdh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.wangshuangyany.cn/gtolwctwwc.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhijiandao.cn/gtbpozpppm.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jiagoushi.top/gtoyzpybul.html

[H08] 获取错误信息与堆栈
来源：http://hz.tian-w.cn/gtbyclmnvs.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yongpay.top/gtzanbokbo.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.fengsongda.top/gtqrrveklb.html

JS:   e.message;  e.stack
来源：http://hz.nanxinkj.top/gtblooibti.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.aibaodan.cn/gtxjtzsspj.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.nanxinkj.top/gtcydpkhun.html

Go:   err.Error()
来源：http://hz.shanyushiyangtech.top/gtscctzgng.html

Ruby: e.message;  e.backtrace
来源：http://hz.zhongyouzk.top/gtbapuvecn.html

C#:   e.Message;  e.StackTrace
来源：http://hz.hammf.cn/gtbvldmbpq.html

[H09] 带错误码的异常
来源：http://hz.zhijiandao.cn/gtfvmxazjc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zhijiandao.cn/gtrqjctjlt.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.shzxlz.cn/gtkelsssgg.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.sxryk.cn/gtunfjmuvn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.sufxvd.cn/gtqmrzkmfl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.aibaodan.cn/gtinevkteo.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.gzhubu.top/gtrzfqtagj.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yvedp.cn/gticqqnnfy.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jlsjyb.cn/gtnuaagzze.html

[H10] 资源自动释放
来源：http://hz.chenjidiqi.icu/gtolhqdbrb.html


<!-- 参考信息 -->