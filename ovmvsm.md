代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://hz.hysaishi.cn/gtmbmpawfs.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.snrcjt.cn/gtvnpzytgq.html

PHP:  file_exists("a.txt");
来源：http://hz.tianlin.xyz/gtmtblgbbq.html

JS:   fs.existsSync("a.txt")
来源：http://hz.mhx1999.top/gtvjeyjrya.html

TS:   fs.existsSync("a.txt")
来源：http://hz.jqgufenzy.top/gtvwcqujjm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.zhongyouzk.top/gtgcinusgt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zhongyouzk.top/gteajatbqk.html

Ruby: File.exist?("a.txt")
来源：http://hz.meibo888.top/gttvfppled.html

C#:   File.Exists("a.txt")
来源：http://hz.yongpay.top/gthfrcngda.html

[F06] 删除文件
来源：http://hz.ivvv.top/gtjfpotfuh.html

Py:   os.remove("a.txt")
来源：http://hz.yongpay.top/gtmpsuihwp.html

PHP:  unlink("a.txt");
来源：http://hz.dianchejie.cn/gtthoiukrz.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.iojbl.cn/gtazzivjzd.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hywenlv.cn/gtolniextz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.shanyushiyangkeji.top/gtrwhwuoke.html

Go:   os.Remove("a.txt")
来源：http://hz.cdnleiting.top/gtlwubjuok.html

Ruby: File.delete("a.txt")
来源：http://hz.yonumen.top/gtwrsyhaam.html

C#:   File.Delete("a.txt");
来源：http://hz.daria6918.cn/gtxwjvysea.html

[F07] 创建目录（含多级）
来源：http://hz.chenlongwang.top/gtfhnbwoxd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.cashguo.top/gtyuxezbld.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.bjfxy.top/gtjibhxyiw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ehwqpu.com/gtloguaijc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yj20258888.top/gtkhzfopbm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yongpay.top/gtquohpceq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.daxiang520.top/gtztpqeeii.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.aibaodan.cn/gtfrbgngnf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.feifeiyinyue.top/gtqinfndlb.html

[F08] 遍历目录
来源：http://hz.0kj1m.cn/gttnwsqjsr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.aizwys.cn/gtxnpaxldd.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.ehwqpu.com/gtxylvapxo.html

JS:   fs.readdirSync("dir")
来源：http://hz.gotoacloud.top/gtpxpcbzuw.html

TS:   fs.readdirSync("dir")
来源：http://hz.svipenyu.cn/gtagcafzej.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yj20258.top/gtveclpvqi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.dashuyun.cn/gtsclghlqj.html

Ruby: Dir.children("dir")
来源：http://hz.gaohongyu789.top/gtcvpsxpdl.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zdqjudy.top/gtzsjeyson.html

[F09] 获取文件大小
来源：http://hz.guannengcc.top/gtkcyaszie.html

Py:   os.path.getsize("a.txt")
来源：http://hz.shanyushiyangtech.top/gtjvrlnblu.html

PHP:  filesize("a.txt");
来源：http://hz.ywan-chungtsiang.top/gtlpkydagh.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yongpay.top/gtgepmzkwo.html

TS:   fs.statSync("a.txt").size
来源：http://hz.shangyingyoupin.top/gtwuvpogsz.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.shanyushiyangtech.top/gtgoavylxe.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.ywan-chungtsiang.top/gtgzmnqreb.html

Ruby: File.size("a.txt")
来源：http://hz.hnxiangtu.top/gtkctmrkzt.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jyoumei.cn/gtnlngjtfu.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.ybcxt.top/gtwvffowru.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.redwolf501.top/gtjfoxtdwr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.svipenyu.cn/gtrhzillxv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.kuanghao11.cn/gtsssgbqwt.html

TS:   path.extname("a.txt")
来源：http://hz.fzhhl.top/gtsjhicmtp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.ppjwa.cn/gtuecwsdjb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.mhx1999.top/gtlgnbwtgz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhiwuduotai.top/gthylznpeh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yueranfly.top/gtonmpipux.html

[F11] 复制与移动文件
来源：http://hz.hnxiangtu.top/gtzlnftama.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.sxryk.cn/gtxdhzqsqq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.haohaochexian.top/gtnxoyssnu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.guannengcc.top/gtnndbzbvq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.gotoacloud.top/gtddcnwwyw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.snrcjt.cn/gtljjekhkb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.nanxinkj.top/gtxskazfkl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.tanke756.top/gtkrrkocty.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.0kj1m.cn/gtwlifogyh.html

[F12] CSV 读写
来源：http://hz.jinqigfzy.top/gtgphjpren.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xuanzx.com/gtamtsmrxz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zhongyouzk.top/gtonaiafiy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yanxiufei.cn/gtuvxwcdwr.html

TS:   // 同上
来源：http://hz.yuanzhike.top/gtzuczcusp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jinghuilouyu.cn/gtzzfudkbw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.redwolf501.top/gtvtvdrcic.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ehwqpu.com/gtnxhdihoj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.xinyue.icu/gtrakhgebw.html

================================================================================
来源：http://hz.jiagoushi.top/gtinbrvnlb.html

G. 面向对象
来源：http://hz.haohaochexian.top/gthshhpvrs.html

================================================================================
来源：http://hz.xuetiantiany.cn/gteowvxwux.html

[G01] 定义类
来源：http://hz.cdnleiting.top/gtowxwnvxe.html

Py:   class User: pass
来源：http://hz.jqgfzy.top/gtqujqjoym.html

PHP:  class User {}
来源：http://hz.pengpengdd.cyou/gtvfhmczaf.html

JS:   class User {}
来源：http://hz.jinghuilouyu.cn/gtqhubwaea.html

TS:   class User { name: string = ""; }
来源：http://hz.zdqjudy.top/gtpynzlzcy.html

Java: class User {}
来源：http://hz.dashuyun.cn/gtmtdpgcrz.html

Go:   type User struct { Name string }
来源：http://hz.jyoumei.cn/gttgecujko.html

Ruby: class User; end
来源：http://hz.yvedp.cn/gtvqvfwekz.html

C#:   class User {}
来源：http://hz.316326.xyz/gtmxskluxq.html

[G02] 构造函数
来源：http://hz.shanyushiyangtech.top/gtuzubbobj.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhaomingkeji.xyz/gtfogvypvm.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hfpthk.cn/gtyakcmfhj.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.haohaochexian.top/gtflznwxhp.html

TS:   constructor(public name: string) {}
来源：http://hz.tian-w.cn/gtgxkwbazb.html

Java: User(String name) { this.name = name; }
来源：http://hz.yonumen.top/gtajnwrprj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yj20258.top/gthfsbpgic.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.iojbl.cn/gtgefnzsjc.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jqgfzy.top/gtqztsjubb.html

[G03] 实例属性
来源：http://hz.sxryk.cn/gttbfcppdp.html

Py:   self.name = "x"
来源：http://hz.feifeiyinyue.top/gtwxavexod.html

PHP:  public string $name = "x";
来源：http://hz.wangdashe.top/gtziyafrkk.html

JS:   this.name = "x";
来源：http://hz.nwbrower.top/gttnvhdrgq.html

TS:   name: string = "x";
来源：http://hz.xziqi.cn/gtchkecynb.html

Java: private String name;
来源：http://hz.bjfxy.top/gtacjfttwv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yuxming.cn/gtevijktrz.html

Ruby: @name = "x"
来源：http://hz.quarkkingdee.top/gtsrtcawoc.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.birdmap.top/gtighulrgb.html

[G04] 定义方法
来源：http://hz.zdqjudy.top/gttrtqwjtw.html

Py:   def greet(self): return self.name
来源：http://hz.hfpthk.cn/gtpyszmltc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.cdnleiting.top/gtrawgrznl.html

JS:   greet() { return this.name; }
来源：http://hz.jqgufenzy.top/gtgpbhocco.html

TS:   greet(): string { return this.name; }
来源：http://hz.jinghuilouyu.cn/gtwewpohbo.html

Java: String greet() { return name; }
来源：http://hz.chenjidiqi.icu/gtfojrazyn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yanxiufei.cn/gtrmwcnpdh.html

Ruby: def greet; @name; end
来源：http://hz.vqdsnc.cn/gtztzqpbau.html

C#:   public string Greet() => Name;
来源：http://hz.feifeiyinyue.top/gtkkaeupvm.html

[G05] 继承
来源：http://hz.zycfv.cn/gtshohzrmp.html

Py:   class Admin(User): pass
来源：http://hz.quarkkingdee.top/gtbivjigfh.html

PHP:  class Admin extends User {}
来源：http://hz.gaohongyu789.top/gtilqjoeyk.html

JS:   class Admin extends User {}
来源：http://hz.shuidangran.top/gtkkjvtxft.html

TS:   class Admin extends User {}
来源：http://hz.tian-w.cn/gtxusveypt.html

Java: class Admin extends User {}
来源：http://hz.yonumen.top/gtxchdzrvo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.gogol.net.cn/gtjjinkiqj.html

Ruby: class Admin < User; end
来源：http://hz.nwbrower.top/gtysbrqhvp.html

C#:   class Admin : User {}
来源：http://hz.zhaomingkeji.xyz/gtfgesnieb.html

[G06] 重写方法
来源：http://hz.jianghu66.top/gtzmhytzds.html

Py:   def greet(self): return "admin"
来源：http://hz.zdqjudy.top/gtxqxaozmt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.dashuyun.cn/gtuidxlauj.html

JS:   greet() { return "admin"; }
来源：http://hz.feifeiyinyue.top/gtsjyjbfbe.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jinqigufen.top/gtfuarhszn.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.shzxlz.cn/gthkruiicz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.ehwqpu.com/gtjxetrrbe.html

Ruby: def greet; "admin"; end
来源：http://hz.jinyuanbaomall.cn/gtbyxplvim.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhoulong.xyz/gtlsaoksoq.html

[G07] 调用父类方法
来源：http://hz.shanyushiyangtech.top/gtcugsfiip.html

Py:   super().greet()
来源：http://hz.cashguo.top/gtxuvqvnmg.html

PHP:  parent::greet();
来源：http://hz.svipenyu.cn/gtkpjafoxm.html

JS:   super.greet();
来源：http://hz.feifeiyinyue.top/gtmccvpqmr.html

TS:   super.greet();
来源：http://hz.xuanzx.com/gtnmzlekii.html

Java: super.greet();
来源：http://hz.bjfxy.top/gtmgxfkmqs.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jyoumei.cn/gtqicmatqq.html

Ruby: super
来源：http://hz.ivvv.top/gtlakhkxyc.html

C#:   base.Greet();
来源：http://hz.yj202588.top/gtkxkwfgtr.html

[G08] 静态方法与属性
来源：http://hz.ehwqpu.com/gtprmjjckm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.ywan-chungtsiang.top/gtpnzrjbba.html

PHP:  public static function f() {}
来源：http://hz.xingfuxueyuan.xyz/gtfnitnsig.html

JS:   static f() {}
来源：http://hz.birdmap.top/gtkzwvstof.html

TS:   static f(): void {}
来源：http://hz.havefunace.top/gttkwguesx.html

Java: static void f() {}
来源：http://hz.smart0.xyz/gtkaciiwut.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.xingfuxueyuan.xyz/gtgbyeqnmu.html

Ruby: def self.f; end
来源：http://hz.zhixingplan.top/gtzbidosgh.html

C#:   public static void F() {}
来源：http://hz.52xcode.cn/gtpalmeerk.html

[G09] 接口 / 抽象类
来源：http://hz.fzhhl.top/gtvcircgsb.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yuanzhike.top/gtxttgptpy.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.wangshuangyany.cn/gtnlmxwhiq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ybcxt.top/gtaeavizri.html

TS:   interface Shape { area(): number; }
来源：http://hz.zhoulong.xyz/gtecnkmvhx.html

Java: interface Shape { double area(); }
来源：http://hz.chenlongwang.top/gtsuehogod.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yanxiufei.cn/gtkbzcvppy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jiagoushi.top/gthvoktwmh.html

C#:   interface IShape { double Area(); }
来源：http://hz.zycfv.cn/gtsvzyfpxz.html

[G10] 访问控制
来源：http://hz.vqdsnc.cn/gtcqvchuff.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.xuetiantiany.cn/gtjojggrwd.html

PHP:  public / protected / private
来源：http://hz.yuanzhike.top/gtrezsilct.html

JS:   #private 字段；其余公开
来源：http://hz.snrcjt.cn/gthvwvnimi.html

TS:   public / protected / private
来源：http://hz.xuanzx.com/gtftftmfwu.html

Java: public / protected / private / 默认包级
来源：http://hz.andypj.xyz/gtzzifpnyi.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.redwolf501.top/gtkkoeuwwo.html

Ruby: public / protected / private
来源：http://hz.bjfxy.top/gtvpervqvl.html

C#:   public / protected / private / internal
来源：http://hz.daria6918.cn/gtaffrkrif.html

[G11] getter / setter
来源：http://hz.xylfe.cn/gtptxolicq.html

Py:   @property 与 @x.setter
来源：http://hz.jyoumei.cn/gtxbvrhwpv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jinghuilouyu.cn/gttdumpvwg.html

JS:   get name() { return this._name; }
来源：http://hz.bjfxy.top/gtsniphykw.html

TS:   get name(): string { return this._name; }
来源：http://hz.shzxlz.cn/gtwqjvvpwg.html

Java: public String getName() { return name; }
来源：http://hz.jinghuilouyu.cn/gtekwgskag.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.feifeiyinyue.top/gtpurqsfrh.html

Ruby: attr_accessor :name
来源：http://hz.hnqzz.top/gtbtacpfyw.html

C#:   public string Name { get; set; }
来源：http://hz.yonumen.top/gttnwikusq.html

[G12] 对象转字符串
来源：http://hz.tanke756.top/gtluvntybz.html

Py:   def __str__(self): return self.name
来源：http://hz.zhoulong.xyz/gtwzpcrngi.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jqgfzy.top/gtzuotvgjy.html

JS:   toString() { return this.name; }
来源：http://hz.ydjk.org.cn/gtdfhxnrpn.html

TS:   toString(): string { return this.name; }
来源：http://hz.shanyushiyangtech.top/gtgfyxungt.html

Java: @Override public String toString() { return name; }
来源：http://hz.guannengcc.top/gtamgfmwxg.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zdqjudy.top/gtesrrxgue.html

Ruby: def to_s; @name; end
来源：http://hz.yj202588.top/gtcddmidjs.html

C#:   public override string ToString() => Name;
来源：http://hz.xziqi.cn/gtlsngsxwv.html

[G13] 判断对象类型
来源：http://hz.tanke756.top/gtqgeiyyvt.html

Py:   isinstance(u, User)
来源：http://hz.shangyingyoupin.top/gtzwyyweaa.html

PHP:  $u instanceof User
来源：http://hz.c1oappe.top/gtihwgykio.html

JS:   u instanceof User
来源：http://hz.tian-w.cn/gtghpcmrhk.html

TS:   u instanceof User
来源：http://hz.daria6918.cn/gttvctkshf.html

Java: u instanceof User
来源：http://hz.yueranfly.top/gtmmubqskw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.cucudq.cn/gtlwgwwrry.html

Ruby: u.is_a?(User)
来源：http://hz.cashguo.top/gtuhyygllp.html

C#:   u is User
来源：http://hz.wangshuangyany.cn/gtilkqgcsu.html

[G14] 数据类 / record
来源：http://hz.yuanzhike.top/gthjrvbhfm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.fengsongda.top/gtsstjemow.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jqgfzy.top/gtjxcrlcqr.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.quarkkingdee.top/gtxicnrkaq.html

TS:   type User = { name: string; age: number };
来源：http://hz.hnqzz.top/gthabvfbcc.html

Java: record User(String name, int age) {}
来源：http://hz.nanxinkj.top/gtcydlbccr.html

Go:   type User struct { Name string; Age int }
来源：http://hz.hnqzz.top/gtcqnweocg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.pengpengdd.cyou/gtfoyzevsw.html

C#:   record User(string Name, int Age);
来源：http://hz.yj20258.top/gtutgawqsm.html

[G15] 枚举
来源：http://hz.hnxiangtu.top/gtgrvmmyhk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.fzhhl.top/gtvflyxyhn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yj20258888.top/gtosrcsnyu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.tian-w.cn/gtvjbhwpmm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.0kj1m.cn/gtvdjlsvsg.html

Java: enum Color { RED, GREEN }
来源：http://hz.nwbrower.top/gtbhvllgyt.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yj20258.top/gtajlyprjp.html

Ruby: Color = %i[red green].freeze
来源：http://hz.dashuyun.cn/gtsiayeeou.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ehwqpu.com/gteyxxkvey.html

[G16] 对象转数组 / 字典
来源：http://hz.zhengqikj.top/gthbbmmxmc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yongpay.top/gtjtvvilug.html

PHP:  get_object_vars($obj);
来源：http://hz.daria6918.cn/gtlkkyerpo.html

JS:   Object.entries(obj)
来源：http://hz.hnxiangtu.top/gteztngzun.html

TS:   Object.entries(obj)
来源：http://hz.snrcjt.cn/gtdwnrxtpn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.xingfuxueyuan.xyz/gttzslwhiw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hammf.cn/gtzeoiumjk.html

Ruby: obj.instance_variables
来源：http://hz.ywan-chungtsiang.top/gtmkakkkpt.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.bjfxy.top/gtlokaqzok.html

================================================================================
来源：http://hz.jyoumei.cn/gtihbzvzup.html

H. 异常与错误处理
来源：http://hz.cucudq.cn/gtemvwyjwt.html

================================================================================
来源：http://hz.havefunace.top/gtgsytvgxn.html

[H01] try / catch 基础
来源：http://hz.yongpay.top/gtfpzpbqfd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.vqdsnc.cn/gtordodkgm.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.daxiang520.top/gtobcayrmo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yj20258.top/gtdtknthcl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.dashuyun.cn/gtisdidrra.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.hongshengwenyu.top/gtudpbptbd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.hysaishi.cn/gtfvnucisi.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.shuidangran.top/gtwqfotbef.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yongpay.top/gttsmvxoyb.html

[H02] finally / ensure 收尾
来源：http://hz.zhoulong.xyz/gtffzapcqo.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yj20258.top/gttmciivqa.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.shangyingyoupin.top/gtnlpiorbz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.dianchejie.cn/gtuvtwqcbw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yj202588.top/gtbvwfvdyi.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.birdmap.top/gtqxbmnyah.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hnqzz.top/gtpinpfwbh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.hfpthk.cn/gtmsbrgctn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zycfv.cn/gtofjcehni.html

[H03] 主动抛出异常
来源：http://hz.zhaomingkeji.xyz/gtkbwxlbsx.html

Py:   raise ValueError("错误信息")
来源：http://hz.fengsongda.top/gtpvqevnmx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jqgfzy.top/gtpeutkevy.html

JS:   throw new Error("错误信息");
来源：http://hz.gogol.net.cn/gtsbmwwrwg.html

TS:   throw new Error("错误信息");
来源：http://hz.nwbrower.top/gtqflmrnsv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.fzhhl.top/gtpgqdrnmh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hywenlv.cn/gtaonpjnqf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.0kj1m.cn/gtghbzptkv.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.hywenlv.cn/gtxecztzpe.html

[H04] 自定义异常类型
来源：http://hz.cdnleiting.top/gtxfyhzeii.html

Py:   class MyError(Exception): pass
来源：http://hz.guannengcc.top/gtacyokzzh.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.ehwqpu.com/gtdneqsneb.html

JS:   class MyError extends Error {}
来源：http://hz.yj20258.top/gtgyhzrhwm.html

TS:   class MyError extends Error {}
来源：http://hz.andypj.xyz/gtqruxgbvp.html

Java: class MyException extends RuntimeException {}
来源：http://hz.9152youxi.cn/gtqezhiedv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zhongyouzk.top/gtowdygrqu.html

Ruby: class MyError < StandardError; end
来源：http://hz.jinqigufen.top/gtmuvmvoiu.html

C#:   class MyException : Exception {}
来源：http://hz.zhongyouzk.top/gtomckfugp.html

[H05] 捕获特定类型
来源：http://hz.ydjk.org.cn/gtguxcivdw.html

Py:   except ValueError as e:
来源：http://hz.zdqjudy.top/gtdmivkbxt.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.gzhubu.top/gtrrvpmtyf.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.quarkkingdee.top/gtonqidphz.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.ivvv.top/gtsokkukjf.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jiagoushi.top/gtpomsrawi.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hfpthk.cn/gtubtlvdji.html

Ruby: rescue ArgumentError => e
来源：http://hz.zhiwuduotai.top/gtdcinuwpj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhongyouzk.top/gtealknzuy.html

[H06] 可选值 / 空值安全访问
来源：http://hz.kuanghao11.cn/gtgxiochdd.html

Py:   value = d.get("k") or default
来源：http://hz.wangdashe.top/gtgmyulitd.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yuanzhike.top/gtriruomvc.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.gotoacloud.top/gtsvkkotaa.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.ywan-chungtsiang.top/gtxehcyrkz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.hongshengwenyu.top/gtsuwustan.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.xuanzx.com/gtesjypjqr.html

Ruby: d&.dig(:a, :b)
来源：http://hz.guannengcc.top/gtrfpfxwau.html

C#:   obj?.A?.B ?? default
来源：http://hz.yj20258888.top/gtnsppmxvh.html

[H07] 断言
来源：http://hz.xuanzx.com/gtlvlprqgz.html

Py:   assert x > 0, "必须为正"
来源：http://hz.ehwqpu.com/gtldaxrpgm.html

PHP:  assert($x > 0);
来源：http://hz.meibo888.top/gthdrhoief.html

JS:   console.assert(x > 0);
来源：http://hz.yuanzhike.top/gtfeupjapi.html

TS:   console.assert(x > 0);
来源：http://hz.52xcode.cn/gtmsifhaiv.html

Java: assert x > 0 : "必须为正";
来源：http://hz.cqqwz.cn/gttkxlfuzw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ybcxt.top/gthuctzsin.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhongyouzk.top/gthxldqffv.html

C#:   Debug.Assert(x > 0);
来源：http://hz.gzhubu.top/gtjlqtcgoe.html

[H08] 获取错误信息与堆栈
来源：http://hz.chenjidiqi.icu/gtttxvnlnc.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yangfankeji.com/gtbjkqynue.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.shanyushiyangkeji.top/gthpffhkco.html

JS:   e.message;  e.stack
来源：http://hz.shanyushiyangkeji.top/gtrzpncjcs.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.haohaochexian.top/gtexkpoiji.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jinqigfzy.top/gtqnkojtnk.html

Go:   err.Error()
来源：http://hz.haohaochexian.top/gtdrxkgdvd.html

Ruby: e.message;  e.backtrace
来源：http://hz.quarkkingdee.top/gtjodswxag.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhengqikj.top/gtsuwtxdhd.html

[H09] 带错误码的异常
来源：http://hz.chenzaomai.com/gtnuypazek.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.xylfe.cn/gtdtnhrfdo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jinghuilouyu.cn/gtnhnajxry.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.ivvv.top/gthkgjcofd.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.hnxiangtu.top/gtbenxdfak.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.gaohongyu789.top/gtsiylglpn.html


<!-- 参考信息 -->