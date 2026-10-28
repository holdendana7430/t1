代发 wailian999

C#:   File.Exists("a.txt")
来源：http://hz.aizwys.cn/gtueuneucp.html

[F06] 删除文件
来源：http://hz.iojbl.cn/gtafrafiym.html

Py:   os.remove("a.txt")
来源：http://hz.nanxuanxn.top/gtfqnnzohl.html

PHP:  unlink("a.txt");
来源：http://hz.shzxlz.cn/gtnceyvadr.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.svipenyu.cn/gtzrnosiix.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.svipenyu.cn/gtvvepoves.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.wangdashe.top/gtgnzrbfiv.html

Go:   os.Remove("a.txt")
来源：http://hz.ydzc1.top/gtxnsunats.html

Ruby: File.delete("a.txt")
来源：http://hz.hnqzz.top/gtcmcfxpaz.html

C#:   File.Delete("a.txt");
来源：http://hz.snrcjt.cn/gtgekstasw.html

[F07] 创建目录（含多级）
来源：http://hz.zdqjudy.top/gtauarosqv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.vqdsnc.cn/gtqytxvitu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.tianlin.xyz/gtiwayaiib.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cucudq.cn/gtepolofpy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xziqi.cn/gtczscohoz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.aibaodan.cn/gtvfeibxex.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hysaishi.cn/gtnvfiwaxh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.kuanghao11.cn/gtbeuxatze.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zhijiandao.cn/gtjzxnywuc.html

[F08] 遍历目录
来源：http://hz.shanyushiyangkeji.top/gtsfanqqwc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.cdnleiting.top/gtcrysqwih.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jinghuilouyu.cn/gtgunfnyow.html

JS:   fs.readdirSync("dir")
来源：http://hz.hammf.cn/gtsvyyikbk.html

TS:   fs.readdirSync("dir")
来源：http://hz.zhoulong.xyz/gtmndfleby.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.daxiang520.top/gtwcxcfesj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.daria6918.cn/gthcbshezw.html

Ruby: Dir.children("dir")
来源：http://hz.9152youxi.cn/gtuxjdillj.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yonumen.top/gtxnjxsvbs.html

[F09] 获取文件大小
来源：http://hz.tanke756.top/gtxzvmsrdl.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zhoulong.xyz/gtvbosjntq.html

PHP:  filesize("a.txt");
来源：http://hz.jinqigfzy.top/gthxrmlevo.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zhixingplan.top/gtmjyescen.html

TS:   fs.statSync("a.txt").size
来源：http://hz.cheryme.top/gtjtylwgmm.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.iojbl.cn/gtzamlpahg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yj20258888.top/gtdwyynupz.html

Ruby: File.size("a.txt")
来源：http://hz.jinqigufen.top/gtwszafbqc.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.aizwys.cn/gtirecxsxs.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.pengpengdd.cyou/gtbjkbwbsj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.xuetiantiany.cn/gtrovlplsx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.sweek.top/gtaqaziukf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.wangshuangyany.cn/gtvvghpagy.html

TS:   path.extname("a.txt")
来源：http://hz.jlsjyb.cn/gtuqbmbxts.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.ybcxt.top/gtjzqrztcq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jianghu66.top/gtmsvuwxwc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.guannengcc.top/gtlnhzsthb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yanxiufei.cn/gtpudwjlpc.html

[F11] 复制与移动文件
来源：http://hz.hywenlv.cn/gtjlahqjgc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.52xcode.cn/gtcbxthqmm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.smart0.xyz/gtkykhzgqu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ehwqpu.com/gtwfrztgrd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.kuanghao11.cn/gtpaznibrk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.vqdsnc.cn/gtehzlsqgi.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yj202588.top/gtqicqmsiz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.hywenlv.cn/gtzvtdlvny.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ppjwa.cn/gtmvdntgwv.html

[F12] CSV 读写
来源：http://hz.gotoacloud.top/gtuchmkdfr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.haohaochexian.top/gtqcosreuf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.gogol.net.cn/gtlysvhseb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.tanke756.top/gtvnxslvcf.html

TS:   // 同上
来源：http://hz.jianghu66.top/gtgwssuhoi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.c1oappe.top/gtdmjrjuyb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhaomingkeji.xyz/gtqmbcible.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.meibo888.top/gtoljbcmyw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.pycfn.com/gtghdhlzdo.html

================================================================================
来源：http://hz.sxryk.cn/gtvzmjficu.html

G. 面向对象
来源：http://hz.wangshuangyany.cn/gtanxywkvl.html

================================================================================
来源：http://hz.jqgfzy.top/gtahpbxgca.html

[G01] 定义类
来源：http://hz.yanxiufei.cn/gtsdkyqynf.html

Py:   class User: pass
来源：http://hz.hammf.cn/gtxoxytlmn.html

PHP:  class User {}
来源：http://hz.zycfv.cn/gtayawdxbi.html

JS:   class User {}
来源：http://hz.ehwqpu.com/gtseaazvii.html

TS:   class User { name: string = ""; }
来源：http://hz.vqdsnc.cn/gtblaotaps.html

Java: class User {}
来源：http://hz.chenzaomai.com/gtqwfkhtlp.html

Go:   type User struct { Name string }
来源：http://hz.xingfuxueyuan.xyz/gtndaqxyap.html

Ruby: class User; end
来源：http://hz.havefunace.top/gthpaktfws.html

C#:   class User {}
来源：http://hz.xuanzx.com/gtejooqjss.html

[G02] 构造函数
来源：http://hz.ybcxt.top/gtoezxcpbj.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.cqqwz.cn/gtfgdhrpvr.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.tianlin.xyz/gtakpkmjoc.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.feifeiyinyue.top/gtekcubafo.html

TS:   constructor(public name: string) {}
来源：http://hz.0kj1m.cn/gtbivvnhcr.html

Java: User(String name) { this.name = name; }
来源：http://hz.jinghuilouyu.cn/gtjdhuxyid.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hysaishi.cn/gtajiiggoe.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.pengpengdd.cyou/gtqqratchu.html

C#:   public User(string name) { Name = name; }
来源：http://hz.c1oappe.top/gtqqmamccw.html

[G03] 实例属性
来源：http://hz.hnqzz.top/gtectkufss.html

Py:   self.name = "x"
来源：http://hz.shangyingyoupin.top/gtwbdihcgr.html

PHP:  public string $name = "x";
来源：http://hz.sweek.top/gtzshrafpa.html

JS:   this.name = "x";
来源：http://hz.xziqi.cn/gttdhcethj.html

TS:   name: string = "x";
来源：http://hz.iojbl.cn/gturkelhfz.html

Java: private String name;
来源：http://hz.hfpthk.cn/gtfwlzhyin.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yangfankeji.com/gtracwyept.html

Ruby: @name = "x"
来源：http://hz.yanxiufei.cn/gtoixmrpzl.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hfpthk.cn/gtrsswknye.html

[G04] 定义方法
来源：http://hz.kuanghao11.cn/gtlyajvonk.html

Py:   def greet(self): return self.name
来源：http://hz.sufxvd.cn/gtpibyoend.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.cheryme.top/gtghrwatuo.html

JS:   greet() { return this.name; }
来源：http://hz.zhaomingkeji.xyz/gtepzfnwfq.html

TS:   greet(): string { return this.name; }
来源：http://hz.gzhubu.top/gtvumwbyiq.html

Java: String greet() { return name; }
来源：http://hz.pycfn.com/gtuevbmyja.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.gaohongyu789.top/gtsrthndnv.html

Ruby: def greet; @name; end
来源：http://hz.aibaodan.cn/gtfuuigatg.html

C#:   public string Greet() => Name;
来源：http://hz.shanyushiyangtech.top/gtnmwxpgds.html

[G05] 继承
来源：http://hz.jinqigufen.top/gtaefqbgvr.html

Py:   class Admin(User): pass
来源：http://hz.gaohongyu789.top/gtoeijpjoo.html

PHP:  class Admin extends User {}
来源：http://hz.aibaodan.cn/gtoadqfgwv.html

JS:   class Admin extends User {}
来源：http://hz.zhiwuduotai.top/gtnvexngzm.html

TS:   class Admin extends User {}
来源：http://hz.shzxlz.cn/gtbfeqbkxv.html

Java: class Admin extends User {}
来源：http://hz.vqdsnc.cn/gtnwbpdevc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.iojbl.cn/gtamdwrenu.html

Ruby: class Admin < User; end
来源：http://hz.vqdsnc.cn/gtukxvsfch.html

C#:   class Admin : User {}
来源：http://hz.gogol.net.cn/gtxkrlammh.html

[G06] 重写方法
来源：http://hz.havefunace.top/gtkrxonjtf.html

Py:   def greet(self): return "admin"
来源：http://hz.zhaomingkeji.xyz/gtbsnquhol.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.nwbrower.top/gtcobvclax.html

JS:   greet() { return "admin"; }
来源：http://hz.jqgfzy.top/gtlqjsnfpt.html

TS:   greet(): string { return "admin"; }
来源：http://hz.ywan-chungtsiang.top/gtknxopyuj.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.nwbrower.top/gtbecanuyk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.ehwqpu.com/gtacnsgzra.html

Ruby: def greet; "admin"; end
来源：http://hz.feifeiyinyue.top/gtbadyasdv.html

C#:   public override string Greet() => "admin";
来源：http://hz.sysykeji.top/gtoygfdzvc.html

[G07] 调用父类方法
来源：http://hz.guowangkeji.top/gtpyrdrozy.html

Py:   super().greet()
来源：http://hz.andypj.xyz/gtdkadhgxg.html

PHP:  parent::greet();
来源：http://hz.zycfv.cn/gtqwraieeh.html

JS:   super.greet();
来源：http://hz.cashguo.top/gtjdtinbwr.html

TS:   super.greet();
来源：http://hz.sweek.top/gtttoknwil.html

Java: super.greet();
来源：http://hz.wangshuangyany.cn/gtirhbaoyc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.bjfxy.top/gtqxqqkxse.html

Ruby: super
来源：http://hz.52xcode.cn/gtrabmjfiu.html

C#:   base.Greet();
来源：http://hz.jianghu66.top/gtsmdqhhwj.html

[G08] 静态方法与属性
来源：http://hz.hammf.cn/gttdtxadmd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.vqdsnc.cn/gtmqexxbeo.html

PHP:  public static function f() {}
来源：http://hz.xingfuxueyuan.xyz/gtivsmksxq.html

JS:   static f() {}
来源：http://hz.aizwys.cn/gtcfmtksmh.html

TS:   static f(): void {}
来源：http://hz.xuanzx.com/gtxszikhda.html

Java: static void f() {}
来源：http://hz.bjfxy.top/gtivyhfgoq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.ybcxt.top/gtbakzwmmj.html

Ruby: def self.f; end
来源：http://hz.shangyingyoupin.top/gtrwgsufpc.html

C#:   public static void F() {}
来源：http://hz.yj20258888.top/gtoeiyzufc.html

[G09] 接口 / 抽象类
来源：http://hz.zhijiandao.cn/gtxhzinyxo.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yangfankeji.com/gtrlufeysp.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.xziqi.cn/gtywaviawk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yj20258888.top/gtldeifxpb.html

TS:   interface Shape { area(): number; }
来源：http://hz.cqqwz.cn/gtwjqfxyam.html

Java: interface Shape { double area(); }
来源：http://hz.cheryme.top/gteehktrlw.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.cucudq.cn/gtcxorozca.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.nwbrower.top/gtqekuaodk.html

C#:   interface IShape { double Area(); }
来源：http://hz.guannengcc.top/gtujzvasqf.html

[G10] 访问控制
来源：http://hz.guowangkeji.top/gtcjzfnldk.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jqgfzy.top/gtrsmfzcdd.html

PHP:  public / protected / private
来源：http://hz.wangdashe.top/gtglxdqawp.html

JS:   #private 字段；其余公开
来源：http://hz.yongpay.top/gteeonugmv.html

TS:   public / protected / private
来源：http://hz.hnqzz.top/gtdcgwoxoo.html

Java: public / protected / private / 默认包级
来源：http://hz.smart0.xyz/gtucmhygik.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhaomingkeji.xyz/gtrvbwdnzp.html

Ruby: public / protected / private
来源：http://hz.kuanghao11.cn/gtgdydjuob.html

C#:   public / protected / private / internal
来源：http://hz.sufxvd.cn/gtiwufttme.html

[G11] getter / setter
来源：http://hz.kuanghao11.cn/gttlbwufcm.html

Py:   @property 与 @x.setter
来源：http://hz.shanyushiyangtech.top/gtvobfskzs.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.redwolf501.top/gtzgdppbef.html

JS:   get name() { return this._name; }
来源：http://hz.redwolf501.top/gtxiyqdhmc.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhoulong.xyz/gtiutuooun.html

Java: public String getName() { return name; }
来源：http://hz.vqdsnc.cn/gtiswwcyrk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zhijiandao.cn/gtbxwioxik.html

Ruby: attr_accessor :name
来源：http://hz.jinghuilouyu.cn/gtsnbnfyoo.html

C#:   public string Name { get; set; }
来源：http://hz.zhengqikj.top/gtfybxfnae.html

[G12] 对象转字符串
来源：http://hz.yvedp.cn/gtubweuvov.html

Py:   def __str__(self): return self.name
来源：http://hz.jqgfzy.top/gtjaxamufg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.hfpthk.cn/gtsqtpmlrs.html

JS:   toString() { return this.name; }
来源：http://hz.meibo888.top/gtmvzszjen.html

TS:   toString(): string { return this.name; }
来源：http://hz.quarkkingdee.top/gtfxcddexu.html

Java: @Override public String toString() { return name; }
来源：http://hz.hysaishi.cn/gtoinjatxx.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jiagoushi.top/gtwvyktwcn.html

Ruby: def to_s; @name; end
来源：http://hz.snrcjt.cn/gtlwjapbid.html

C#:   public override string ToString() => Name;
来源：http://hz.0kj1m.cn/gtvmneqxnr.html

[G13] 判断对象类型
来源：http://hz.ydzc1.top/gtrtfpznrb.html

Py:   isinstance(u, User)
来源：http://hz.zhengqikj.top/gthnmcgkcx.html

PHP:  $u instanceof User
来源：http://hz.jinghuilouyu.cn/gtuxozzqdl.html

JS:   u instanceof User
来源：http://hz.smart0.xyz/gtubvnuwmh.html

TS:   u instanceof User
来源：http://hz.wangdashe.top/gthbwumdkz.html

Java: u instanceof User
来源：http://hz.fengsongda.top/gtdqwobhlz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.c1oappe.top/gtkvdbvtrq.html

Ruby: u.is_a?(User)
来源：http://hz.xinyue.icu/gtrvsxkmrb.html

C#:   u is User
来源：http://hz.zhengqikj.top/gtchijhyqe.html

[G14] 数据类 / record
来源：http://hz.hnqzz.top/gtkhzxkwap.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.iojbl.cn/gtwajofyoo.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.chenzaomai.com/gtwdyjtsht.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.cqqwz.cn/gtcdbtpqlh.html

TS:   type User = { name: string; age: number };
来源：http://hz.gogol.net.cn/gthfnylnko.html

Java: record User(String name, int age) {}
来源：http://hz.hywenlv.cn/gtfjqddawt.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jinqigufen.top/gtufovqnsq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.tanke756.top/gtrnatwona.html

C#:   record User(string Name, int Age);
来源：http://hz.yueranfly.top/gtxoknsgrd.html

[G15] 枚举
来源：http://hz.dashuyun.cn/gtpmgbbfbz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yangfankeji.com/gtvjuewllk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.fzhhl.top/gtxsvztolq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.shzxlz.cn/gtfoervkjr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yueranfly.top/gtbgwtqjte.html

Java: enum Color { RED, GREEN }
来源：http://hz.yongpay.top/gtxksbiewi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.quarkkingdee.top/gtjjfqmwgl.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yongpay.top/gtltgpagaw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhiwuduotai.top/gtlhqwgyxk.html

[G16] 对象转数组 / 字典
来源：http://hz.cashguo.top/gtekghloju.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.nanxuanxn.top/gtcdzcfbag.html

PHP:  get_object_vars($obj);
来源：http://hz.yanxiufei.cn/gtqmlgxxgy.html

JS:   Object.entries(obj)
来源：http://hz.pycfn.com/gtckyyeaxv.html

TS:   Object.entries(obj)
来源：http://hz.ivvv.top/gtiludfotl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.chenlongwang.top/gtqmsqbeja.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.snrcjt.cn/gtnlccgwky.html

Ruby: obj.instance_variables
来源：http://hz.cheryme.top/gtzsrdrpli.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.gaohongyu789.top/gtvzbjlrwb.html

================================================================================
来源：http://hz.gogol.net.cn/gtxrzkfhnq.html

H. 异常与错误处理
来源：http://hz.wangshuangyany.cn/gtdbbwuvin.html

================================================================================
来源：http://hz.sysykeji.top/gtfzjiugpq.html

[H01] try / catch 基础
来源：http://hz.cdnleiting.top/gtxbrxwcue.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.cqqwz.cn/gtkryrvlif.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.cdnleiting.top/gtjcqhyrzl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yangfankeji.com/gtfsmyaaxy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.cucudq.cn/gtzkdxrgqy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.shangyingyoupin.top/gtanovfhiz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.cheryme.top/gtokxflmot.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ywan-chungtsiang.top/gtxdjfwvqh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhixingplan.top/gtahqlcymd.html

[H02] finally / ensure 收尾
来源：http://hz.shzxlz.cn/gtkstcxhgg.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.shanyushiyangkeji.top/gthwjwvgiw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yonumen.top/gtzbaxsmxr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.sysykeji.top/gtucrkfomq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.dianchejie.cn/gtmseeotjw.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yj20258888.top/gtvnwykdwx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.mhx1999.top/gteishpzkf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.wangdashe.top/gtoebdjens.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hywenlv.cn/gteksmvdnt.html

[H03] 主动抛出异常
来源：http://hz.yj20258888.top/gtfpjepaxc.html

Py:   raise ValueError("错误信息")
来源：http://hz.sufxvd.cn/gttlhuspdw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.snrcjt.cn/gttoixkteo.html

JS:   throw new Error("错误信息");
来源：http://hz.zhongyouzk.top/gtidxwayox.html

TS:   throw new Error("错误信息");
来源：http://hz.jyoumei.cn/gtubkasnre.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.nwbrower.top/gtylexpucm.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yj202588.top/gtitqurkgo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.feifeiyinyue.top/gteqdgctce.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.bjfxy.top/gtrijtdxpo.html

[H04] 自定义异常类型
来源：http://hz.jyoumei.cn/gtmpqiztbp.html

Py:   class MyError(Exception): pass
来源：http://hz.kuanghao11.cn/gtbmtkzrsn.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.tanke756.top/gtxajawngi.html

JS:   class MyError extends Error {}
来源：http://hz.haohaochexian.top/gtjlasoiux.html

TS:   class MyError extends Error {}
来源：http://hz.zdqjudy.top/gthxpiqxxq.html

Java: class MyException extends RuntimeException {}
来源：http://hz.havefunace.top/gtunjxnzta.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jlsjyb.cn/gtkzwxwzyp.html

Ruby: class MyError < StandardError; end
来源：http://hz.9152youxi.cn/gtzbmqfags.html

C#:   class MyException : Exception {}
来源：http://hz.ydzc1.top/gtfdcmqtbj.html

[H05] 捕获特定类型
来源：http://hz.cucudq.cn/gtelwublfk.html

Py:   except ValueError as e:
来源：http://hz.zhongyouzk.top/gtjjmeprvc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yongpay.top/gtnditsmvb.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.kuanghao11.cn/gtvwttuxsf.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yuanzhike.top/gtdossozfq.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zycfv.cn/gtsplkerlk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.shangyingyoupin.top/gtsgunhuwl.html

Ruby: rescue ArgumentError => e
来源：http://hz.hnxiangtu.top/gtjeeqrumi.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hongshengwenyu.top/gtxvjveydw.html

[H06] 可选值 / 空值安全访问
来源：http://hz.chenzaomai.com/gtaeyqzayt.html

Py:   value = d.get("k") or default
来源：http://hz.ybcxt.top/gtjgqzijsx.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.gzhubu.top/gtpwlicytc.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ydjk.org.cn/gtppwnzuik.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.kuanghao11.cn/gtxwjtmpzj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.0kj1m.cn/gtsrudjwpm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.aibaodan.cn/gtxaakzvjp.html

Ruby: d&.dig(:a, :b)
来源：http://hz.xuetiantiany.cn/gtslucbtfv.html

C#:   obj?.A?.B ?? default
来源：http://hz.ppjwa.cn/gttpjwnort.html

[H07] 断言
来源：http://hz.yongpay.top/gtpjzcerjb.html

Py:   assert x > 0, "必须为正"
来源：http://hz.sufxvd.cn/gtmzazeawb.html

PHP:  assert($x > 0);
来源：http://hz.jyoumei.cn/gtitokqwnx.html

JS:   console.assert(x > 0);
来源：http://hz.jqgfzy.top/gtipvdswtk.html

TS:   console.assert(x > 0);
来源：http://hz.hnxiangtu.top/gteqpjszoc.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zhaomingkeji.xyz/gtpdrzqqcm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.fengsongda.top/gtehhdsyhi.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yvedp.cn/gtkxtccbnp.html

C#:   Debug.Assert(x > 0);
来源：http://hz.sxryk.cn/gtlhzccqez.html

[H08] 获取错误信息与堆栈
来源：http://hz.zhoulong.xyz/gthfmpffqb.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ydzc1.top/gtukogdjbq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.chenzaomai.com/gtatufkyzh.html

JS:   e.message;  e.stack
来源：http://hz.9152youxi.cn/gtyjusdper.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zhongyouzk.top/gtnchucsxx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.nanxinkj.top/gtjnwqyumd.html

Go:   err.Error()
来源：http://hz.zycfv.cn/gtpkleetns.html

Ruby: e.message;  e.backtrace
来源：http://hz.yanxiufei.cn/gtkdchzjyl.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ehwqpu.com/gtyadoypbt.html

[H09] 带错误码的异常
来源：http://hz.xziqi.cn/gtpdlddahl.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.pengpengdd.cyou/gtgnpjahzk.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.hysaishi.cn/gtzvjipezf.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.sysykeji.top/gtsakbqygx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.svipenyu.cn/gtixambwki.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yj20258.top/gtoqiwlfmi.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.wangshuangyany.cn/gtilpfckfs.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.hysaishi.cn/gtwyvklisf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.hammf.cn/gtuytoubqg.html

[H10] 资源自动释放
来源：http://hz.ydjk.org.cn/gtfasnzuhp.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yuanzhike.top/gtnaarddsp.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.hammf.cn/gtcgjhtfbu.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.quarkkingdee.top/gtevmsfoic.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sufxvd.cn/gtiqmjscye.html


<!-- 参考信息 -->