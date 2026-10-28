代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://hz.hfpthk.cn/gteyypigxk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.gaohongyu789.top/gtyhmnurlg.html

PHP:  file_exists("a.txt");
来源：http://hz.haohaochexian.top/gtfftegbsk.html

JS:   fs.existsSync("a.txt")
来源：http://hz.52xcode.cn/gttabspexi.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhijiandao.cn/gtommlxtfi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.shanyushiyangkeji.top/gtncscemhn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ehwqpu.com/gtcyulkeab.html

Ruby: File.exist?("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtepgqpasb.html

C#:   File.Exists("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtkycgzkvg.html

[F06] 删除文件
来源：http://hz.chenjidiqi.icu/gtenrnfekj.html

Py:   os.remove("a.txt")
来源：http://hz.0kj1m.cn/gtdgujbguy.html

PHP:  unlink("a.txt");
来源：http://hz.xinyue.icu/gtvuinuqmd.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.jyoumei.cn/gtwtiukdyj.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.ehwqpu.com/gtecnksmgd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.pycfn.com/gtctkblvdm.html

Go:   os.Remove("a.txt")
来源：http://hz.hfpthk.cn/gtyvqemlhx.html

Ruby: File.delete("a.txt")
来源：http://hz.hfpthk.cn/gtqqfexfdk.html

C#:   File.Delete("a.txt");
来源：http://hz.jiagoushi.top/gtalddvuin.html

[F07] 创建目录（含多级）
来源：http://hz.zhengqikj.top/gtvfcvpxpn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zhijiandao.cn/gtxyxfcmtw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.hnxiangtu.top/gtbyemsxhj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xziqi.cn/gtbqiygvni.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.quarkkingdee.top/gtswacogum.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.kuanghao11.cn/gtbrjqacfp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yuxming.cn/gtauzylinh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.quarkkingdee.top/gtokjuplvg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.svipenyu.cn/gtehcnsfma.html

[F08] 遍历目录
来源：http://hz.jianghu66.top/gtutmtemdt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.jinqigfzy.top/gtqquvwnvq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.xuanzx.com/gtljtltqpx.html

JS:   fs.readdirSync("dir")
来源：http://hz.tianlin.xyz/gteidvqrtr.html

TS:   fs.readdirSync("dir")
来源：http://hz.guowangkeji.top/gtzsoevpvo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.ehwqpu.com/gtjwpxzcbk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jinqigfzy.top/gtraixeigg.html

Ruby: Dir.children("dir")
来源：http://hz.yueranfly.top/gttlnuzpsb.html

C#:   Directory.GetFiles("dir")
来源：http://hz.daxiang520.top/gtkznsrxyz.html

[F09] 获取文件大小
来源：http://hz.wangshuangyany.cn/gtdbhbdvnz.html

Py:   os.path.getsize("a.txt")
来源：http://hz.ehwqpu.com/gtqxoghtjg.html

PHP:  filesize("a.txt");
来源：http://hz.yj202588.top/gtabqonqoa.html

JS:   fs.statSync("a.txt").size
来源：http://hz.dianchejie.cn/gtwymqsfyq.html

TS:   fs.statSync("a.txt").size
来源：http://hz.mhx1999.top/gtlqsgasne.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zycfv.cn/gtoczxcodr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.sufxvd.cn/gtqlaxhtia.html

Ruby: File.size("a.txt")
来源：http://hz.redwolf501.top/gtrhznfooo.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.daxiang520.top/gthhsnyveq.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.c1oappe.top/gtkmxpmihf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.hfpthk.cn/gtzrvdarls.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yuanzhike.top/gtwhvuyxvv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yanxiufei.cn/gtdcswpvpq.html

TS:   path.extname("a.txt")
来源：http://hz.zhengqikj.top/gthlsayqco.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.xylfe.cn/gtdqcfsjja.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.kuanghao11.cn/gttkorqaka.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.wangshuangyany.cn/gtyfincfdb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yongpay.top/gtnzpyfuyt.html

[F11] 复制与移动文件
来源：http://hz.jinyuanbaomall.cn/gttcayezzc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.gaohongyu789.top/gtfmjgedtg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.chenlongwang.top/gtkapofjih.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shuidangran.top/gtrsjsseiq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.nanxinkj.top/gtbwxfiooj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.shuidangran.top/gtbhistfzi.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jianghu66.top/gtvjjgfxit.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.guannengcc.top/gtueolubid.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.smart0.xyz/gthezoctfc.html

[F12] CSV 读写
来源：http://hz.aizwys.cn/gteyltgzbn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.ydzc1.top/gtzgolnmlf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.ivvv.top/gtltfcratf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.nwbrower.top/gtwrcuugkr.html

TS:   // 同上
来源：http://hz.chenjidiqi.icu/gtetszlcjk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.feifeiyinyue.top/gtixibzhwa.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.hongshengwenyu.top/gtpsrltdtu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.pycfn.com/gtmiepjqso.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.xinyue.icu/gtzjehlgxz.html

================================================================================
来源：http://hz.ppjwa.cn/gtenliqhkp.html

G. 面向对象
来源：http://hz.yanxiufei.cn/gtqhujzlyh.html

================================================================================
来源：http://hz.sufxvd.cn/gtweyovlgu.html

[G01] 定义类
来源：http://hz.bjfxy.top/gtzcivumic.html

Py:   class User: pass
来源：http://hz.pengpengdd.cyou/gtsbiuxukm.html

PHP:  class User {}
来源：http://hz.jqgfzy.top/gtprroggtn.html

JS:   class User {}
来源：http://hz.redwolf501.top/gtqszpyrrr.html

TS:   class User { name: string = ""; }
来源：http://hz.bjfxy.top/gtkybuxpbs.html

Java: class User {}
来源：http://hz.hammf.cn/gtmzjtskyp.html

Go:   type User struct { Name string }
来源：http://hz.yj202588.top/gtbxfevjot.html

Ruby: class User; end
来源：http://hz.0kj1m.cn/gtdutscxhz.html

C#:   class User {}
来源：http://hz.hywenlv.cn/gtfabjzbwt.html

[G02] 构造函数
来源：http://hz.pengpengdd.cyou/gtgjvbmvvj.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yj202588.top/gtwcmzhpaw.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jinqigufen.top/gtdxlxedhf.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhengqikj.top/gtfoeufpie.html

TS:   constructor(public name: string) {}
来源：http://hz.tanke756.top/gthyeyozgg.html

Java: User(String name) { this.name = name; }
来源：http://hz.ivvv.top/gtxhakeaey.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.xylfe.cn/gtvafabmra.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yangfankeji.com/gtvluicspj.html

C#:   public User(string name) { Name = name; }
来源：http://hz.shanyushiyangkeji.top/gtzshhcnkv.html

[G03] 实例属性
来源：http://hz.zdqjudy.top/gtybfxqqnd.html

Py:   self.name = "x"
来源：http://hz.shangyingyoupin.top/gtumtujosi.html

PHP:  public string $name = "x";
来源：http://hz.andypj.xyz/gtffjhfart.html

JS:   this.name = "x";
来源：http://hz.hysaishi.cn/gtkoqkempi.html

TS:   name: string = "x";
来源：http://hz.tian-w.cn/gtdeescivy.html

Java: private String name;
来源：http://hz.pycfn.com/gtyzndjeqk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.cashguo.top/gtyfwmbtfl.html

Ruby: @name = "x"
来源：http://hz.xuanzx.com/gtnvszcbry.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.cucudq.cn/gtboigbkre.html

[G04] 定义方法
来源：http://hz.feifeiyinyue.top/gtcsphfpvo.html

Py:   def greet(self): return self.name
来源：http://hz.birdmap.top/gthagrntgl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hywenlv.cn/gtxikdynci.html

JS:   greet() { return this.name; }
来源：http://hz.guannengcc.top/gtcmkuoula.html

TS:   greet(): string { return this.name; }
来源：http://hz.zhongyouzk.top/gtwwjosang.html

Java: String greet() { return name; }
来源：http://hz.guannengcc.top/gtnfodxbjo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.snrcjt.cn/gtreooydjn.html

Ruby: def greet; @name; end
来源：http://hz.ivvv.top/gtuhqmtonh.html

C#:   public string Greet() => Name;
来源：http://hz.wangdashe.top/gtpgwpfheu.html

[G05] 继承
来源：http://hz.fzhhl.top/gtgfiyxieh.html

Py:   class Admin(User): pass
来源：http://hz.zhijiandao.cn/gtrzavnpkx.html

PHP:  class Admin extends User {}
来源：http://hz.shanyushiyangkeji.top/gtnpztdlud.html

JS:   class Admin extends User {}
来源：http://hz.aibaodan.cn/gtpfiuswwp.html

TS:   class Admin extends User {}
来源：http://hz.guowangkeji.top/gtxdecfmnh.html

Java: class Admin extends User {}
来源：http://hz.aibaodan.cn/gtozgkeewk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.gaohongyu789.top/gtgqgzzgin.html

Ruby: class Admin < User; end
来源：http://hz.birdmap.top/gtsixovora.html

C#:   class Admin : User {}
来源：http://hz.shzxlz.cn/gtryxvgksn.html

[G06] 重写方法
来源：http://hz.xinyue.icu/gtrrfkmivi.html

Py:   def greet(self): return "admin"
来源：http://hz.jiagoushi.top/gtheidhtth.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.hysaishi.cn/gtnmmofwkw.html

JS:   greet() { return "admin"; }
来源：http://hz.cucudq.cn/gtoopwmxto.html

TS:   greet(): string { return "admin"; }
来源：http://hz.daxiang520.top/gtngrfrlbc.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jiagoushi.top/gtvkxvzuwi.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.ywan-chungtsiang.top/gtaedylsjt.html

Ruby: def greet; "admin"; end
来源：http://hz.yj20258.top/gtqndlqlhd.html

C#:   public override string Greet() => "admin";
来源：http://hz.cheryme.top/gtqlsxxbbq.html

[G07] 调用父类方法
来源：http://hz.gzhubu.top/gtmnbdnzho.html

Py:   super().greet()
来源：http://hz.zhongyouzk.top/gtrkhdpcnn.html

PHP:  parent::greet();
来源：http://hz.gzhubu.top/gtwhuyqlwu.html

JS:   super.greet();
来源：http://hz.zhiwuduotai.top/gtyzwhcmgq.html

TS:   super.greet();
来源：http://hz.hammf.cn/gtzphcctka.html

Java: super.greet();
来源：http://hz.andypj.xyz/gtrsobyisz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zhijiandao.cn/gtntjiunrj.html

Ruby: super
来源：http://hz.meibo888.top/gtogckzbdo.html

C#:   base.Greet();
来源：http://hz.zhaomingkeji.xyz/gttyebxact.html

[G08] 静态方法与属性
来源：http://hz.birdmap.top/gtuxghbgzy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.chenjidiqi.icu/gttbehsama.html

PHP:  public static function f() {}
来源：http://hz.ydjk.org.cn/gtuotjvycg.html

JS:   static f() {}
来源：http://hz.shanyushiyangtech.top/gtsrraowav.html

TS:   static f(): void {}
来源：http://hz.iojbl.cn/gtdfgehrzu.html

Java: static void f() {}
来源：http://hz.birdmap.top/gtusbnoszt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.ybcxt.top/gtagxdtvfq.html

Ruby: def self.f; end
来源：http://hz.daria6918.cn/gtmqmzfloi.html

C#:   public static void F() {}
来源：http://hz.haohaochexian.top/gtveingwqm.html

[G09] 接口 / 抽象类
来源：http://hz.zhongyouzk.top/gtjgjcuhio.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.xylfe.cn/gtjdolxvwf.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.hnxiangtu.top/gtuxeozhzh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.gotoacloud.top/gtsceqbevb.html

TS:   interface Shape { area(): number; }
来源：http://hz.hywenlv.cn/gtsmtknwwj.html

Java: interface Shape { double area(); }
来源：http://hz.shangyingyoupin.top/gtsfopepod.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yueranfly.top/gtavrfwqwt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.haohaochexian.top/gtawkqxzgu.html

C#:   interface IShape { double Area(); }
来源：http://hz.yuanzhike.top/gtzlovyzjx.html

[G10] 访问控制
来源：http://hz.ydzc1.top/gtfuokcyxs.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.gotoacloud.top/gtofroovew.html

PHP:  public / protected / private
来源：http://hz.zhixingplan.top/gtutxcizss.html

JS:   #private 字段；其余公开
来源：http://hz.bjfxy.top/gtytxzyvgq.html

TS:   public / protected / private
来源：http://hz.chenjidiqi.icu/gtoekgcxag.html

Java: public / protected / private / 默认包级
来源：http://hz.andypj.xyz/gtchwmjcrp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yj20258.top/gtgffyjifr.html

Ruby: public / protected / private
来源：http://hz.kuanghao11.cn/gtukvkecrl.html

C#:   public / protected / private / internal
来源：http://hz.pengpengdd.cyou/gtpldqcskj.html

[G11] getter / setter
来源：http://hz.gogol.net.cn/gtuiszxebk.html

Py:   @property 与 @x.setter
来源：http://hz.cdnleiting.top/gttjilqjar.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.daria6918.cn/gtdhurwqht.html

JS:   get name() { return this._name; }
来源：http://hz.smart0.xyz/gtoeuucvux.html

TS:   get name(): string { return this._name; }
来源：http://hz.meibo888.top/gtxwdibjok.html

Java: public String getName() { return name; }
来源：http://hz.tian-w.cn/gtuoslmlyr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yj20258888.top/gthdennuqa.html

Ruby: attr_accessor :name
来源：http://hz.fengsongda.top/gtutvndmle.html

C#:   public string Name { get; set; }
来源：http://hz.xziqi.cn/gtcalfksiu.html

[G12] 对象转字符串
来源：http://hz.jlsjyb.cn/gtuirwwpfj.html

Py:   def __str__(self): return self.name
来源：http://hz.xingfuxueyuan.xyz/gtxatwhujt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.dashuyun.cn/gtabahhruu.html

JS:   toString() { return this.name; }
来源：http://hz.gaohongyu789.top/gtjtesaphx.html

TS:   toString(): string { return this.name; }
来源：http://hz.chenjidiqi.icu/gtpvakofzz.html

Java: @Override public String toString() { return name; }
来源：http://hz.xziqi.cn/gtgxnclcoe.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhoulong.xyz/gtriieuesh.html

Ruby: def to_s; @name; end
来源：http://hz.ywan-chungtsiang.top/gtovytojrk.html

C#:   public override string ToString() => Name;
来源：http://hz.jianghu66.top/gtcsywopnr.html

[G13] 判断对象类型
来源：http://hz.guowangkeji.top/gtarfgimbt.html

Py:   isinstance(u, User)
来源：http://hz.yonumen.top/gthcpeabjx.html

PHP:  $u instanceof User
来源：http://hz.316326.xyz/gtxbcnaexj.html

JS:   u instanceof User
来源：http://hz.tian-w.cn/gtjdpocxkn.html

TS:   u instanceof User
来源：http://hz.316326.xyz/gtltsgkbai.html

Java: u instanceof User
来源：http://hz.zhongyouzk.top/gtzezuojxe.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.xuanzx.com/gtxdeizuti.html

Ruby: u.is_a?(User)
来源：http://hz.daria6918.cn/gtcbxjtvoi.html

C#:   u is User
来源：http://hz.feifeiyinyue.top/gtgvakfyje.html

[G14] 数据类 / record
来源：http://hz.shuidangran.top/gttehsasir.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zhengqikj.top/gttcnxpmcg.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.fengsongda.top/gtxafikgny.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.gotoacloud.top/gtmqicqlzx.html

TS:   type User = { name: string; age: number };
来源：http://hz.guannengcc.top/gtwihndsnm.html

Java: record User(String name, int age) {}
来源：http://hz.fengsongda.top/gtjqqwgzcn.html

Go:   type User struct { Name string; Age int }
来源：http://hz.cucudq.cn/gtpbpktldo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.dashuyun.cn/gtecdlkouu.html

C#:   record User(string Name, int Age);
来源：http://hz.yuanzhike.top/gtcwwjbahm.html

[G15] 枚举
来源：http://hz.xuetiantiany.cn/gturintiqy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jqgufenzy.top/gtnajyryik.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.cheryme.top/gtqxicyhtg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jianghu66.top/gtszewcbsz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shangyingyoupin.top/gtviergvtl.html

Java: enum Color { RED, GREEN }
来源：http://hz.sxryk.cn/gtyvklvzjf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.hammf.cn/gttpflhslp.html

Ruby: Color = %i[red green].freeze
来源：http://hz.xingfuxueyuan.xyz/gtnibdxhrx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.pengpengdd.cyou/gtdhtupdtn.html

[G16] 对象转数组 / 字典
来源：http://hz.ivvv.top/gtcfudnynn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jianghu66.top/gtworjdsry.html

PHP:  get_object_vars($obj);
来源：http://hz.chenlongwang.top/gtlgawbbbv.html

JS:   Object.entries(obj)
来源：http://hz.jlsjyb.cn/gtytztqpjp.html

TS:   Object.entries(obj)
来源：http://hz.jinqigfzy.top/gtiipbqjki.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ivvv.top/gtqxngkrcu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.xylfe.cn/gtkedgqdpo.html

Ruby: obj.instance_variables
来源：http://hz.aibaodan.cn/gtmtoaiorx.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.vqdsnc.cn/gtjeombmne.html

================================================================================
来源：http://hz.gotoacloud.top/gtpyvjahat.html

H. 异常与错误处理
来源：http://hz.0kj1m.cn/gthinbshbc.html

================================================================================
来源：http://hz.jianghu66.top/gtilewsjfu.html

[H01] try / catch 基础
来源：http://hz.hnqzz.top/gtghaysjst.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.0kj1m.cn/gtuvwiqcmq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.bjfxy.top/gtjxqerjah.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.cqqwz.cn/gtvynjncng.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yvedp.cn/gtqnjxmdrf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.nanxinkj.top/gtxiuydkdo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yj20258888.top/gtugfnvbvo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.kuanghao11.cn/gtotxckjiy.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.daria6918.cn/gtnkogvbsg.html

[H02] finally / ensure 收尾
来源：http://hz.redwolf501.top/gtekgltyss.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zhijiandao.cn/gtzuyccjwj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.tian-w.cn/gththismzo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.ydjk.org.cn/gtfqompjlq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yuanzhike.top/gtxxpcildm.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jianghu66.top/gtjhrftwls.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.sxryk.cn/gthiiiuhyi.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.xuanzx.com/gtzjfssusj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.ehwqpu.com/gtilhthspg.html

[H03] 主动抛出异常
来源：http://hz.ivvv.top/gtlfmiwdew.html

Py:   raise ValueError("错误信息")
来源：http://hz.ywan-chungtsiang.top/gttbkytqjh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.tanke756.top/gtqckbwahg.html

JS:   throw new Error("错误信息");
来源：http://hz.jinqigufen.top/gtrriklfio.html

TS:   throw new Error("错误信息");
来源：http://hz.svipenyu.cn/gtugqyecdd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.kuanghao11.cn/gtreogbrqq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.gotoacloud.top/gtuwkfidnw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.sxryk.cn/gtfbvrkzqm.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zycfv.cn/gtkpgwzudd.html

[H04] 自定义异常类型
来源：http://hz.ybcxt.top/gtsqqgxwfq.html

Py:   class MyError(Exception): pass
来源：http://hz.jinghuilouyu.cn/gtlauohwae.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zdqjudy.top/gtdayshiry.html

JS:   class MyError extends Error {}
来源：http://hz.aizwys.cn/gtcpgpexii.html

TS:   class MyError extends Error {}
来源：http://hz.cdnleiting.top/gtvpkrvquz.html

Java: class MyException extends RuntimeException {}
来源：http://hz.hfpthk.cn/gtbdsnvuzq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ehwqpu.com/gtkvzjcsxn.html

Ruby: class MyError < StandardError; end
来源：http://hz.yuanzhike.top/gtptxdkctr.html

C#:   class MyException : Exception {}
来源：http://hz.gotoacloud.top/gtgkuuvoxx.html

[H05] 捕获特定类型
来源：http://hz.tian-w.cn/gtnvvtinxc.html

Py:   except ValueError as e:
来源：http://hz.tian-w.cn/gtsihhffas.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhoulong.xyz/gtryqkdbkx.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.chenzaomai.com/gtyccjzepl.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.vqdsnc.cn/gtstscnwbt.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jianghu66.top/gtbydblyje.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.xinyue.icu/gtikcmyhac.html

Ruby: rescue ArgumentError => e
来源：http://hz.zdqjudy.top/gtxhgcqddo.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jianghu66.top/gttugtzblf.html

[H06] 可选值 / 空值安全访问
来源：http://hz.kuanghao11.cn/gtdcyvhxvc.html

Py:   value = d.get("k") or default
来源：http://hz.shuidangran.top/gtbgcnlont.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.gotoacloud.top/gtudtjnvhb.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.chenlongwang.top/gtktwizndf.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.ywan-chungtsiang.top/gtvrsuxhgb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.gzhubu.top/gtsvbnvxun.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.sysykeji.top/gtbbjnutlm.html

Ruby: d&.dig(:a, :b)
来源：http://hz.daria6918.cn/gtfkzopyaq.html

C#:   obj?.A?.B ?? default
来源：http://hz.zhijiandao.cn/gtxeuufbrh.html

[H07] 断言
来源：http://hz.iojbl.cn/gtyuaaawyf.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yj202588.top/gtfdlnmegr.html

PHP:  assert($x > 0);
来源：http://hz.zhengqikj.top/gtssawqmmb.html

JS:   console.assert(x > 0);
来源：http://hz.hongshengwenyu.top/gtfhpcwqbi.html

TS:   console.assert(x > 0);
来源：http://hz.xziqi.cn/gtvnqdhdec.html

Java: assert x > 0 : "必须为正";
来源：http://hz.guannengcc.top/gtuquilhyy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.sufxvd.cn/gtocehxkza.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhijiandao.cn/gtyjkarttl.html

C#:   Debug.Assert(x > 0);
来源：http://hz.sxryk.cn/gtlgglpbmm.html

[H08] 获取错误信息与堆栈
来源：http://hz.aizwys.cn/gtbbrytlya.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yongpay.top/gtreusgfnl.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jianghu66.top/gtgnkczyod.html

JS:   e.message;  e.stack
来源：http://hz.jiagoushi.top/gtdurrtxmm.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.fzhhl.top/gtdsmfhazi.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.cucudq.cn/gtbdtrfjol.html

Go:   err.Error()
来源：http://hz.nanxinkj.top/gtzhvelbhd.html

Ruby: e.message;  e.backtrace
来源：http://hz.gzhubu.top/gtckffvfvp.html

C#:   e.Message;  e.StackTrace
来源：http://hz.meibo888.top/gtisnzcevx.html

[H09] 带错误码的异常
来源：http://hz.xinyue.icu/gtbwxoicwe.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.cdnleiting.top/gtaghkjwme.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.sysykeji.top/gtzfhezpzx.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.fzhhl.top/gtnrlfousm.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.ivvv.top/gtlhdngter.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.52xcode.cn/gtdtujxckc.html


<!-- 参考信息 -->