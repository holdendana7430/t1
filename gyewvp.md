代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jiagoushi.top/gtwoertkot.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.sxryk.cn/gtrjarlwhb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.svipenyu.cn/gtjmuoizxb.html

[F04] 追加写入文件
来源：http://hz.jinqigfzy.top/gtsgslhzto.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.birdmap.top/gttcrxworz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.ydzc1.top/gtwkcppwhy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.c1oappe.top/gthkwkbfrs.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jiagoushi.top/gtfjgmecrl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.wangshuangyany.cn/gtaxukfppq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.bjfxy.top/gtqulmhrvc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zhengqikj.top/gtzbgrogef.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.smart0.xyz/gtnqpwufze.html

[F05] 判断文件或目录是否存在
来源：http://hz.bjfxy.top/gtwpmbkbgf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.nwbrower.top/gtbcjlikky.html

PHP:  file_exists("a.txt");
来源：http://hz.chenjidiqi.icu/gtlxdskgld.html

JS:   fs.existsSync("a.txt")
来源：http://hz.snrcjt.cn/gtqfjoncww.html

TS:   fs.existsSync("a.txt")
来源：http://hz.shzxlz.cn/gtpwpfwjgj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.gzhubu.top/gtxqwoqtqz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jinqigufen.top/gtplcdpsza.html

Ruby: File.exist?("a.txt")
来源：http://hz.aibaodan.cn/gtqqprjpih.html

C#:   File.Exists("a.txt")
来源：http://hz.gogol.net.cn/gtrnptagdz.html

[F06] 删除文件
来源：http://hz.havefunace.top/gtgaksiqkl.html

Py:   os.remove("a.txt")
来源：http://hz.guowangkeji.top/gtfwajbrqn.html

PHP:  unlink("a.txt");
来源：http://hz.daria6918.cn/gtielzpmku.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.quarkkingdee.top/gtkuaszklw.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.dashuyun.cn/gtinwhtlwz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yj20258888.top/gtqxcqgkjd.html

Go:   os.Remove("a.txt")
来源：http://hz.hysaishi.cn/gtdumzdxfk.html

Ruby: File.delete("a.txt")
来源：http://hz.316326.xyz/gtieesuejm.html

C#:   File.Delete("a.txt");
来源：http://hz.nanxuanxn.top/gtnfyeqemo.html

[F07] 创建目录（含多级）
来源：http://hz.nanxuanxn.top/gtjpaemepj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jiagoushi.top/gtcyiiuxqw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.cashguo.top/gtbivmlvrl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shanyushiyangtech.top/gtgrvssnji.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.daria6918.cn/gttkjqfvrg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.bjfxy.top/gtuvxntvmq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.nanxinkj.top/gtvjircoxj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.andypj.xyz/gtozzmyoey.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yonumen.top/gtdzuwvlwx.html

[F08] 遍历目录
来源：http://hz.gaohongyu789.top/gtvppbujvz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.xuanzx.com/gttwziiibe.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.shangyingyoupin.top/gtobzrfyim.html

JS:   fs.readdirSync("dir")
来源：http://hz.shuidangran.top/gtmxcryhwf.html

TS:   fs.readdirSync("dir")
来源：http://hz.redwolf501.top/gtjxthaxcn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.gogol.net.cn/gtoxqrdrvz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yvedp.cn/gtfllrhiqu.html

Ruby: Dir.children("dir")
来源：http://hz.bjfxy.top/gtfktodhie.html

C#:   Directory.GetFiles("dir")
来源：http://hz.nwbrower.top/gtoiimbewp.html

[F09] 获取文件大小
来源：http://hz.hfpthk.cn/gtgkuibqla.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zdqjudy.top/gtmsdevijx.html

PHP:  filesize("a.txt");
来源：http://hz.xinyue.icu/gtzirmmxas.html

JS:   fs.statSync("a.txt").size
来源：http://hz.iojbl.cn/gtzqlgahyt.html

TS:   fs.statSync("a.txt").size
来源：http://hz.9152youxi.cn/gtxsjaavge.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jinqigfzy.top/gtkhnrucsw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.iojbl.cn/gtaidqerod.html

Ruby: File.size("a.txt")
来源：http://hz.yuxming.cn/gtrphuqtcl.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.xziqi.cn/gtnssbvpwc.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hfpthk.cn/gtrdmreupb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.svipenyu.cn/gtjvimjqvw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.hammf.cn/gteugdraou.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.meibo888.top/gtcaggueck.html

TS:   path.extname("a.txt")
来源：http://hz.yangfankeji.com/gtykysebob.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.bjfxy.top/gthtrqocee.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.svipenyu.cn/gteplptkpv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zycfv.cn/gtprppezgz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jiagoushi.top/gtklhmveux.html

[F11] 复制与移动文件
来源：http://hz.xuetiantiany.cn/gtsmgmvcjl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.aizwys.cn/gtjrkkffim.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.ehwqpu.com/gtbklgavqw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sxryk.cn/gtxzqlewhx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xuetiantiany.cn/gtlgbbttsd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.xziqi.cn/gtwnryfjym.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jyoumei.cn/gtycnjtoxi.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.pengpengdd.cyou/gtoznbkwgd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.fengsongda.top/gtbcvdgwcl.html

[F12] CSV 读写
来源：http://hz.gotoacloud.top/gtgfxdwzby.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.wangshuangyany.cn/gtxiahbfde.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.gotoacloud.top/gtnkvnhqze.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.cqqwz.cn/gtjymqrapg.html

TS:   // 同上
来源：http://hz.yj202588.top/gtzguxeueh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ywan-chungtsiang.top/gtqdmorsmj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.gzhubu.top/gtnlmwonao.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.cucudq.cn/gtzooebqvn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zhijiandao.cn/gttoldjcfd.html

================================================================================
来源：http://hz.hysaishi.cn/gtprgbrisf.html

G. 面向对象
来源：http://hz.ybcxt.top/gtpvwrtxxw.html

================================================================================
来源：http://hz.daxiang520.top/gtxpnkqnoz.html

[G01] 定义类
来源：http://hz.bjfxy.top/gttevwukjv.html

Py:   class User: pass
来源：http://hz.xuetiantiany.cn/gtnvzsewsz.html

PHP:  class User {}
来源：http://hz.gotoacloud.top/gtjistzkfe.html

JS:   class User {}
来源：http://hz.gaohongyu789.top/gtgmxbyeea.html

TS:   class User { name: string = ""; }
来源：http://hz.yuanzhike.top/gtvsvbsfcb.html

Java: class User {}
来源：http://hz.chenjidiqi.icu/gtpbkfrqxe.html

Go:   type User struct { Name string }
来源：http://hz.sxryk.cn/gtzffpwjlt.html

Ruby: class User; end
来源：http://hz.shzxlz.cn/gtzpppukuz.html

C#:   class User {}
来源：http://hz.vqdsnc.cn/gtvcoxysrr.html

[G02] 构造函数
来源：http://hz.quarkkingdee.top/gtkfjipscd.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.guowangkeji.top/gtkofiagrq.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.xziqi.cn/gtktnjkdqx.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.nwbrower.top/gtydrreftg.html

TS:   constructor(public name: string) {}
来源：http://hz.yvedp.cn/gthhfixcnk.html

Java: User(String name) { this.name = name; }
来源：http://hz.fzhhl.top/gteylbhrwg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.ppjwa.cn/gtyfzgpppf.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yonumen.top/gtvziqvmgs.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yanxiufei.cn/gtvpqhzxia.html

[G03] 实例属性
来源：http://hz.shzxlz.cn/gtgabtnbzg.html

Py:   self.name = "x"
来源：http://hz.shangyingyoupin.top/gttehmlzoz.html

PHP:  public string $name = "x";
来源：http://hz.jqgfzy.top/gtumdtepgf.html

JS:   this.name = "x";
来源：http://hz.hnxiangtu.top/gtibuovyfo.html

TS:   name: string = "x";
来源：http://hz.cashguo.top/gtogcmruio.html

Java: private String name;
来源：http://hz.jqgfzy.top/gtvrinaorh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hnqzz.top/gtlqhszuvw.html

Ruby: @name = "x"
来源：http://hz.havefunace.top/gtdxruyori.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.tianlin.xyz/gtcokpmgco.html

[G04] 定义方法
来源：http://hz.yangfankeji.com/gtvinpnuec.html

Py:   def greet(self): return self.name
来源：http://hz.yueranfly.top/gtfceapzjl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.daxiang520.top/gtlaspifzb.html

JS:   greet() { return this.name; }
来源：http://hz.daria6918.cn/gtyvfsjjgd.html

TS:   greet(): string { return this.name; }
来源：http://hz.yj20258.top/gtfbzibkhk.html

Java: String greet() { return name; }
来源：http://hz.shuidangran.top/gtmfkclmbk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.tanke756.top/gtbfmqqpfm.html

Ruby: def greet; @name; end
来源：http://hz.pengpengdd.cyou/gthvtlgkrx.html

C#:   public string Greet() => Name;
来源：http://hz.hnxiangtu.top/gtesfejwfv.html

[G05] 继承
来源：http://hz.redwolf501.top/gtrgpkwnmw.html

Py:   class Admin(User): pass
来源：http://hz.sweek.top/gtbltxwkjt.html

PHP:  class Admin extends User {}
来源：http://hz.hfpthk.cn/gtjvmkqwgj.html

JS:   class Admin extends User {}
来源：http://hz.meibo888.top/gtxqhnjowv.html

TS:   class Admin extends User {}
来源：http://hz.aizwys.cn/gtnplgueir.html

Java: class Admin extends User {}
来源：http://hz.zhengqikj.top/gtdhnleeeg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.tanke756.top/gtibnxcpte.html

Ruby: class Admin < User; end
来源：http://hz.chenlongwang.top/gtwysqoedx.html

C#:   class Admin : User {}
来源：http://hz.zycfv.cn/gtzfjmzkke.html

[G06] 重写方法
来源：http://hz.tianlin.xyz/gtjkqutpzn.html

Py:   def greet(self): return "admin"
来源：http://hz.sxryk.cn/gtqlbaqwtg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.hammf.cn/gtzfzlvaiv.html

JS:   greet() { return "admin"; }
来源：http://hz.shangyingyoupin.top/gttnjeneti.html

TS:   greet(): string { return "admin"; }
来源：http://hz.daria6918.cn/gtgkeqkqtz.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ydjk.org.cn/gtppwlxvgx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.ivvv.top/gtpjlztxdy.html

Ruby: def greet; "admin"; end
来源：http://hz.yangfankeji.com/gtugwlwmcx.html

C#:   public override string Greet() => "admin";
来源：http://hz.jyoumei.cn/gtivhvcztr.html

[G07] 调用父类方法
来源：http://hz.jiagoushi.top/gtwuhdylaa.html

Py:   super().greet()
来源：http://hz.shuidangran.top/gtzbvsdzpz.html

PHP:  parent::greet();
来源：http://hz.yangfankeji.com/gtqzyvcatq.html

JS:   super.greet();
来源：http://hz.52xcode.cn/gtmnkxihip.html

TS:   super.greet();
来源：http://hz.pycfn.com/gtferpkfks.html

Java: super.greet();
来源：http://hz.tian-w.cn/gttalazlkh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.hnxiangtu.top/gtlqnhzoag.html

Ruby: super
来源：http://hz.tianlin.xyz/gtjrdclwbl.html

C#:   base.Greet();
来源：http://hz.316326.xyz/gtergewpwb.html

[G08] 静态方法与属性
来源：http://hz.jqgufenzy.top/gttuvzcnyl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.daria6918.cn/gtrpnwzmqi.html

PHP:  public static function f() {}
来源：http://hz.kuanghao11.cn/gtsrzwvjtp.html

JS:   static f() {}
来源：http://hz.wangdashe.top/gtfokqirps.html

TS:   static f(): void {}
来源：http://hz.aibaodan.cn/gtqdjjpkfy.html

Java: static void f() {}
来源：http://hz.yongpay.top/gtrbkpshza.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhongyouzk.top/gtoyubpbgj.html

Ruby: def self.f; end
来源：http://hz.pycfn.com/gtooayfcjg.html

C#:   public static void F() {}
来源：http://hz.hfpthk.cn/gttjupauzg.html

[G09] 接口 / 抽象类
来源：http://hz.zdqjudy.top/gtyxmjdego.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zycfv.cn/gtduifpvrh.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jiagoushi.top/gtklspnwcl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zhiwuduotai.top/gtiyfjomsb.html

TS:   interface Shape { area(): number; }
来源：http://hz.ppjwa.cn/gtkefyketw.html

Java: interface Shape { double area(); }
来源：http://hz.zhiwuduotai.top/gthqieslbc.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.cucudq.cn/gtieprpdzz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.shzxlz.cn/gtziwghrwq.html

C#:   interface IShape { double Area(); }
来源：http://hz.xuanzx.com/gteghkbxds.html

[G10] 访问控制
来源：http://hz.zhoulong.xyz/gtcutxuvqe.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.chenlongwang.top/gtrrydspvk.html

PHP:  public / protected / private
来源：http://hz.c1oappe.top/gtniikdesd.html

JS:   #private 字段；其余公开
来源：http://hz.xziqi.cn/gtowlomjit.html

TS:   public / protected / private
来源：http://hz.kuanghao11.cn/gttfkgvikg.html

Java: public / protected / private / 默认包级
来源：http://hz.wangshuangyany.cn/gtwtavpgms.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.cucudq.cn/gtdlfnlpad.html

Ruby: public / protected / private
来源：http://hz.cdnleiting.top/gtzspwllsu.html

C#:   public / protected / private / internal
来源：http://hz.hnxiangtu.top/gtmzqfexdj.html

[G11] getter / setter
来源：http://hz.xuanzx.com/gtlrxvqvig.html

Py:   @property 与 @x.setter
来源：http://hz.sweek.top/gtpzyhncbs.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhengqikj.top/gthuujyygo.html

JS:   get name() { return this._name; }
来源：http://hz.meibo888.top/gtlmwjzfii.html

TS:   get name(): string { return this._name; }
来源：http://hz.xylfe.cn/gtrqujezmw.html

Java: public String getName() { return name; }
来源：http://hz.ehwqpu.com/gtkslfgrwa.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.xuetiantiany.cn/gtyfyimxhu.html

Ruby: attr_accessor :name
来源：http://hz.shzxlz.cn/gtfisuytmw.html

C#:   public string Name { get; set; }
来源：http://hz.aizwys.cn/gtrulrmbsz.html

[G12] 对象转字符串
来源：http://hz.jianghu66.top/gtrxeplqxs.html

Py:   def __str__(self): return self.name
来源：http://hz.tianlin.xyz/gtszxawdvv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.wangdashe.top/gtdtdbnlmn.html

JS:   toString() { return this.name; }
来源：http://hz.chenjidiqi.icu/gtxyrxeaiy.html

TS:   toString(): string { return this.name; }
来源：http://hz.pengpengdd.cyou/gthxehfpxz.html

Java: @Override public String toString() { return name; }
来源：http://hz.tianlin.xyz/gtvlqknngw.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.andypj.xyz/gtxqerzewd.html

Ruby: def to_s; @name; end
来源：http://hz.havefunace.top/gtcuhlcqrk.html

C#:   public override string ToString() => Name;
来源：http://hz.tianlin.xyz/gtadxzcdlh.html

[G13] 判断对象类型
来源：http://hz.birdmap.top/gtkakdpecx.html

Py:   isinstance(u, User)
来源：http://hz.zhaomingkeji.xyz/gtvoyxaflw.html

PHP:  $u instanceof User
来源：http://hz.ivvv.top/gtoojfqxyg.html

JS:   u instanceof User
来源：http://hz.dashuyun.cn/gtxntmkxsm.html

TS:   u instanceof User
来源：http://hz.zdqjudy.top/gtbdbyqagg.html

Java: u instanceof User
来源：http://hz.hnqzz.top/gtfxpbocor.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yuxming.cn/gtdfzllvvf.html

Ruby: u.is_a?(User)
来源：http://hz.nwbrower.top/gtoprvxyho.html

C#:   u is User
来源：http://hz.yanxiufei.cn/gtuaclfoal.html

[G14] 数据类 / record
来源：http://hz.jiagoushi.top/gtztvrdakv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.tanke756.top/gtjutjldqk.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.nanxuanxn.top/gtldubqcai.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.aizwys.cn/gtonsawlzf.html

TS:   type User = { name: string; age: number };
来源：http://hz.jyoumei.cn/gtpjbjwqvj.html

Java: record User(String name, int age) {}
来源：http://hz.aizwys.cn/gtwtuuabdm.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zhoulong.xyz/gtvtanumnv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.316326.xyz/gtwyorcgex.html

C#:   record User(string Name, int Age);
来源：http://hz.sysykeji.top/gtyodvtsyz.html

[G15] 枚举
来源：http://hz.zycfv.cn/gtpwvzgdvr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.xuetiantiany.cn/gtqvomwpgz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.sweek.top/gtinxobplq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.xuetiantiany.cn/gtthmgxeyv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jinghuilouyu.cn/gtygtkyctk.html

Java: enum Color { RED, GREEN }
来源：http://hz.yuxming.cn/gtvoroylye.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yongpay.top/gtwbflirla.html

Ruby: Color = %i[red green].freeze
来源：http://hz.smart0.xyz/gttwapmlft.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yj20258.top/gtoocrjodf.html

[G16] 对象转数组 / 字典
来源：http://hz.yangfankeji.com/gtpwoqwteo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhongyouzk.top/gtukurxkzo.html

PHP:  get_object_vars($obj);
来源：http://hz.ybcxt.top/gtoxkohygx.html

JS:   Object.entries(obj)
来源：http://hz.sysykeji.top/gtopfgyxyi.html

TS:   Object.entries(obj)
来源：http://hz.yj202588.top/gtbxfzkzzd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.svipenyu.cn/gtuottuwif.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.zhiwuduotai.top/gticscolsu.html

Ruby: obj.instance_variables
来源：http://hz.birdmap.top/gtsmtfctpu.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.cdnleiting.top/gtzeyzkpbs.html

================================================================================
来源：http://hz.feifeiyinyue.top/gthtbtvfjo.html

H. 异常与错误处理
来源：http://hz.jinqigfzy.top/gtnmacygkf.html

================================================================================
来源：http://hz.fzhhl.top/gtpphpymdv.html

[H01] try / catch 基础
来源：http://hz.ywan-chungtsiang.top/gtuaadqkgp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jianghu66.top/gtkamgtzpu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.havefunace.top/gtvydcynpz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.haohaochexian.top/gtouaiijpc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yuanzhike.top/gtwasykwan.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zhiwuduotai.top/gtubvfexzi.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zhiwuduotai.top/gtonlwvkou.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yongpay.top/gtfywnbokr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zdqjudy.top/gtythtappb.html

[H02] finally / ensure 收尾
来源：http://hz.tianlin.xyz/gteavhjtwe.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yj20258.top/gtrxnjiwdh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.bjfxy.top/gtquwzteet.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.aizwys.cn/gtadtkvdyd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.0kj1m.cn/gtezauphtx.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yvedp.cn/gtoryoloky.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jinghuilouyu.cn/gtxsbwagsh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jlsjyb.cn/gttjugkdds.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zhengqikj.top/gtiqnyjbko.html

[H03] 主动抛出异常
来源：http://hz.zhixingplan.top/gttypazkpd.html

Py:   raise ValueError("错误信息")
来源：http://hz.9152youxi.cn/gtznjcbtwt.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.andypj.xyz/gtdxexzpcl.html

JS:   throw new Error("错误信息");
来源：http://hz.shanyushiyangtech.top/gtmccrijau.html

TS:   throw new Error("错误信息");
来源：http://hz.iojbl.cn/gtpaspjxgl.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.tanke756.top/gtliklryar.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.wangdashe.top/gtqsjfzksx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.aibaodan.cn/gthxksdiyq.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.hnqzz.top/gtpihhldxd.html

[H04] 自定义异常类型
来源：http://hz.cheryme.top/gtwuujgrhj.html

Py:   class MyError(Exception): pass
来源：http://hz.pycfn.com/gtsymcwnao.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.xylfe.cn/gtembjnhms.html

JS:   class MyError extends Error {}
来源：http://hz.yuanzhike.top/gtmzdstzri.html

TS:   class MyError extends Error {}
来源：http://hz.cucudq.cn/gtijerzavr.html

Java: class MyException extends RuntimeException {}
来源：http://hz.gzhubu.top/gtzmxogwlg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.hysaishi.cn/gtyszmxfyd.html

Ruby: class MyError < StandardError; end
来源：http://hz.cdnleiting.top/gtafxjtgoz.html

C#:   class MyException : Exception {}
来源：http://hz.316326.xyz/gtagdkgkjl.html

[H05] 捕获特定类型
来源：http://hz.pycfn.com/gtdtqxrfrh.html

Py:   except ValueError as e:
来源：http://hz.gogol.net.cn/gtkrqnseqq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.9152youxi.cn/gthfmszvwx.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.havefunace.top/gtdjhjedln.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.haohaochexian.top/gtghnjfkse.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jyoumei.cn/gtskgjnmxl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jinqigufen.top/gtqponhhdi.html

Ruby: rescue ArgumentError => e
来源：http://hz.hnqzz.top/gtzjzdzlla.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.guannengcc.top/gtcjvzkick.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yongpay.top/gtgawaikui.html

Py:   value = d.get("k") or default
来源：http://hz.xinyue.icu/gtzlpseiok.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.birdmap.top/gtwbpmxxwf.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zhijiandao.cn/gtctjzpqcl.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.andypj.xyz/gtpogmtywv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ybcxt.top/gtbuhcoprf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jinqigfzy.top/gtmbiogrrt.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jqgufenzy.top/gtkwkpsdde.html

C#:   obj?.A?.B ?? default
来源：http://hz.0kj1m.cn/gtfnjojmdp.html

[H07] 断言
来源：http://hz.cqqwz.cn/gtrbabifrn.html

Py:   assert x > 0, "必须为正"
来源：http://hz.dashuyun.cn/gtinofanny.html

PHP:  assert($x > 0);
来源：http://hz.zdqjudy.top/gtrssmtgxq.html

JS:   console.assert(x > 0);
来源：http://hz.fzhhl.top/gtrplxxjad.html

TS:   console.assert(x > 0);
来源：http://hz.cashguo.top/gtchrzjjwg.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ybcxt.top/gtjabkyvnv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.gaohongyu789.top/gttsqxemjl.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.52xcode.cn/gtbvxykpoc.html

C#:   Debug.Assert(x > 0);
来源：http://hz.cheryme.top/gtbpuaecle.html

[H08] 获取错误信息与堆栈
来源：http://hz.cashguo.top/gtuumoadro.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jianghu66.top/gtxnbrtjbb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.hfpthk.cn/gtqowszeww.html


<!-- 参考信息 -->