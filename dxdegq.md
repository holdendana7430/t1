代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.meibo888.top/gtxuxsshtx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.cucudq.cn/gtkdhmjqty.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.316326.xyz/gtkfgxxjtt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhixingplan.top/gtiprlvngu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.fzhhl.top/gtxiinncof.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.snrcjt.cn/gtnffhkvfl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.jyoumei.cn/gtzxxqfets.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.hammf.cn/gtxewxzlxa.html

[F05] 判断文件或目录是否存在
来源：http://hz.birdmap.top/gtuokytmfc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yueranfly.top/gtfwbukhni.html

PHP:  file_exists("a.txt");
来源：http://hz.zhijiandao.cn/gtmwozmshy.html

JS:   fs.existsSync("a.txt")
来源：http://hz.dianchejie.cn/gtcyujuzen.html

TS:   fs.existsSync("a.txt")
来源：http://hz.ybcxt.top/gtxokbfmfl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.cdnleiting.top/gtduosfyeo.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jinqigufen.top/gtyereoofn.html

Ruby: File.exist?("a.txt")
来源：http://hz.jianghu66.top/gtcbbfavvp.html

C#:   File.Exists("a.txt")
来源：http://hz.jinghuilouyu.cn/gtrlekaufj.html

[F06] 删除文件
来源：http://hz.pycfn.com/gtvhudesbj.html

Py:   os.remove("a.txt")
来源：http://hz.ppjwa.cn/gtehxepavv.html

PHP:  unlink("a.txt");
来源：http://hz.ppjwa.cn/gtazqtzcld.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.sweek.top/gtdlihifwl.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jinqigfzy.top/gtafurktmj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yvedp.cn/gttzweobrr.html

Go:   os.Remove("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtxzfkxlat.html

Ruby: File.delete("a.txt")
来源：http://hz.jlsjyb.cn/gtmcpglaej.html

C#:   File.Delete("a.txt");
来源：http://hz.jinghuilouyu.cn/gtgyokeqih.html

[F07] 创建目录（含多级）
来源：http://hz.316326.xyz/gtdmaiefxj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jqgufenzy.top/gtszohfbhh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.xuanzx.com/gtrehccahz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yangfankeji.com/gtyhspoalt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hysaishi.cn/gtdjngkrzk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.smart0.xyz/gtqcmtwtyj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.tianlin.xyz/gtkppvsctr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jqgfzy.top/gtegmpcugr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.snrcjt.cn/gtkkwkkmzq.html

[F08] 遍历目录
来源：http://hz.iojbl.cn/gtvjhwqeav.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.guowangkeji.top/gtcmbosqic.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.0kj1m.cn/gtonlblawg.html

JS:   fs.readdirSync("dir")
来源：http://hz.zhijiandao.cn/gtzrvwjaeo.html

TS:   fs.readdirSync("dir")
来源：http://hz.ybcxt.top/gtqwycdmna.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.haohaochexian.top/gttuywpvmf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.meibo888.top/gtfysnnsts.html

Ruby: Dir.children("dir")
来源：http://hz.meibo888.top/gtqtljcqia.html

C#:   Directory.GetFiles("dir")
来源：http://hz.ydzc1.top/gtykikyqil.html

[F09] 获取文件大小
来源：http://hz.guowangkeji.top/gtwuvymdjs.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zhixingplan.top/gtrsmsdqrx.html

PHP:  filesize("a.txt");
来源：http://hz.redwolf501.top/gtmyctsvjo.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yvedp.cn/gtpvqpxkqn.html

TS:   fs.statSync("a.txt").size
来源：http://hz.smart0.xyz/gttkpptwqh.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yuxming.cn/gtffiiquep.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.redwolf501.top/gtruvejtre.html

Ruby: File.size("a.txt")
来源：http://hz.daria6918.cn/gtgboxwjvi.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yuanzhike.top/gtqryogpbu.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.316326.xyz/gteadccsih.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jinyuanbaomall.cn/gtistddnus.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.tianlin.xyz/gtertpwkbb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.gogol.net.cn/gthgboezcb.html

TS:   path.extname("a.txt")
来源：http://hz.aibaodan.cn/gttoihhwoq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.redwolf501.top/gtotxygqpj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.0kj1m.cn/gtucesernu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhijiandao.cn/gtrfsucwbi.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.cheryme.top/gtiniwwyik.html

[F11] 复制与移动文件
来源：http://hz.smart0.xyz/gtjugvpigr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.hywenlv.cn/gtgfkvlgil.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.hnxiangtu.top/gtgxphjagr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ivvv.top/gtkhluyfvh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.iojbl.cn/gtfcqrsolk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.hnxiangtu.top/gtlcossgsr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.nanxuanxn.top/gtdyzzcewn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.tianlin.xyz/gtwljqfudw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.sysykeji.top/gtlmdquqnp.html

[F12] CSV 读写
来源：http://hz.jianghu66.top/gtafirmzfj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.ivvv.top/gtkfrarjbz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hammf.cn/gtobwvfsch.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jqgfzy.top/gtonphbvcj.html

TS:   // 同上
来源：http://hz.quarkkingdee.top/gtlwhetort.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.xuanzx.com/gtjaxlelpi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zdqjudy.top/gtpsictlnf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.dashuyun.cn/gtqmzptlji.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jinyuanbaomall.cn/gtfidvvtpb.html

================================================================================
来源：http://hz.gotoacloud.top/gteagvdune.html

G. 面向对象
来源：http://hz.dashuyun.cn/gtxbhkomma.html

================================================================================
来源：http://hz.ybcxt.top/gtimwzmeki.html

[G01] 定义类
来源：http://hz.zhengqikj.top/gtocinqqbo.html

Py:   class User: pass
来源：http://hz.iojbl.cn/gtjlebtyxe.html

PHP:  class User {}
来源：http://hz.yvedp.cn/gtiotewdrf.html

JS:   class User {}
来源：http://hz.wangshuangyany.cn/gthtdzpguu.html

TS:   class User { name: string = ""; }
来源：http://hz.yuanzhike.top/gtvpblffjo.html

Java: class User {}
来源：http://hz.jianghu66.top/gtwppcsjmr.html

Go:   type User struct { Name string }
来源：http://hz.ywan-chungtsiang.top/gtcwpuuzsh.html

Ruby: class User; end
来源：http://hz.gogol.net.cn/gtnvtlwgcl.html

C#:   class User {}
来源：http://hz.gotoacloud.top/gtqtzogutj.html

[G02] 构造函数
来源：http://hz.daxiang520.top/gtotjiborr.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.52xcode.cn/gtpqlejqcu.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.xziqi.cn/gtbqexurru.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.gogol.net.cn/gtgriydjtl.html

TS:   constructor(public name: string) {}
来源：http://hz.yvedp.cn/gtcoygtinj.html

Java: User(String name) { this.name = name; }
来源：http://hz.yongpay.top/gtkrhrxujx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.iojbl.cn/gtsousfugj.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.dashuyun.cn/gtqdkxsmxx.html

C#:   public User(string name) { Name = name; }
来源：http://hz.nwbrower.top/gtgirgxrkg.html

[G03] 实例属性
来源：http://hz.shzxlz.cn/gtqtdassoa.html

Py:   self.name = "x"
来源：http://hz.ybcxt.top/gtngxssjap.html

PHP:  public string $name = "x";
来源：http://hz.ybcxt.top/gtdojixncb.html

JS:   this.name = "x";
来源：http://hz.fengsongda.top/gtednyabbf.html

TS:   name: string = "x";
来源：http://hz.yanxiufei.cn/gtgwvwzhlj.html

Java: private String name;
来源：http://hz.shangyingyoupin.top/gtxtzlngyr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.fzhhl.top/gtysqywrcr.html

Ruby: @name = "x"
来源：http://hz.cqqwz.cn/gtpfrslunr.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.pycfn.com/gtrmoczyyk.html

[G04] 定义方法
来源：http://hz.cucudq.cn/gtsrtyguxp.html

Py:   def greet(self): return self.name
来源：http://hz.chenlongwang.top/gtoqvybqqx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.wangshuangyany.cn/gtftitxgsk.html

JS:   greet() { return this.name; }
来源：http://hz.tanke756.top/gttlfynjxe.html

TS:   greet(): string { return this.name; }
来源：http://hz.gzhubu.top/gtjqvgrxpv.html

Java: String greet() { return name; }
来源：http://hz.sxryk.cn/gtskdmfodz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.316326.xyz/gtdhjunsqa.html

Ruby: def greet; @name; end
来源：http://hz.chenzaomai.com/gtkmcrpvvh.html

C#:   public string Greet() => Name;
来源：http://hz.zhoulong.xyz/gtewrudcvn.html

[G05] 继承
来源：http://hz.zhaomingkeji.xyz/gtvlvjxwmv.html

Py:   class Admin(User): pass
来源：http://hz.redwolf501.top/gtouulxzlp.html

PHP:  class Admin extends User {}
来源：http://hz.zdqjudy.top/gtarkshyqm.html

JS:   class Admin extends User {}
来源：http://hz.sysykeji.top/gtskikswhf.html

TS:   class Admin extends User {}
来源：http://hz.yanxiufei.cn/gtvqxhcykc.html

Java: class Admin extends User {}
来源：http://hz.jianghu66.top/gttxykipit.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.nanxinkj.top/gtdletsqxr.html

Ruby: class Admin < User; end
来源：http://hz.havefunace.top/gtadrxplmf.html

C#:   class Admin : User {}
来源：http://hz.daria6918.cn/gtszyfwpdo.html

[G06] 重写方法
来源：http://hz.daria6918.cn/gtgwmcjqcg.html

Py:   def greet(self): return "admin"
来源：http://hz.guowangkeji.top/gtlkuoizhk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jlsjyb.cn/gtbddalhkl.html

JS:   greet() { return "admin"; }
来源：http://hz.chenlongwang.top/gtxhibitwd.html

TS:   greet(): string { return "admin"; }
来源：http://hz.sufxvd.cn/gtvkpbvxod.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.shuidangran.top/gtegvprpgf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yj20258888.top/gtfjkkvxex.html

Ruby: def greet; "admin"; end
来源：http://hz.yangfankeji.com/gteecvsuoc.html

C#:   public override string Greet() => "admin";
来源：http://hz.yueranfly.top/gtqcwswdcu.html

[G07] 调用父类方法
来源：http://hz.jinghuilouyu.cn/gtdjdphwnq.html

Py:   super().greet()
来源：http://hz.kuanghao11.cn/gtnhvcvfkt.html

PHP:  parent::greet();
来源：http://hz.fengsongda.top/gtthrgcurp.html

JS:   super.greet();
来源：http://hz.jinqigfzy.top/gtzslrsova.html

TS:   super.greet();
来源：http://hz.zhijiandao.cn/gtxjcbxqey.html

Java: super.greet();
来源：http://hz.xylfe.cn/gtnbmirzmi.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yangfankeji.com/gtpvvbypxk.html

Ruby: super
来源：http://hz.jianghu66.top/gtlbhbfyca.html

C#:   base.Greet();
来源：http://hz.yj202588.top/gtevuljgzf.html

[G08] 静态方法与属性
来源：http://hz.shanyushiyangkeji.top/gtcmcxpynd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.tianlin.xyz/gtczxgejgf.html

PHP:  public static function f() {}
来源：http://hz.yuanzhike.top/gtaavsaqxt.html

JS:   static f() {}
来源：http://hz.zhiwuduotai.top/gtkioyxqav.html

TS:   static f(): void {}
来源：http://hz.yueranfly.top/gtxfmofkzr.html

Java: static void f() {}
来源：http://hz.zhengqikj.top/gtvpqgmskj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.iojbl.cn/gtdwgynluj.html

Ruby: def self.f; end
来源：http://hz.sxryk.cn/gtqtcszqiy.html

C#:   public static void F() {}
来源：http://hz.gogol.net.cn/gtygreakep.html

[G09] 接口 / 抽象类
来源：http://hz.pengpengdd.cyou/gtmhxbvdyj.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yonumen.top/gtoxqpyqmq.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.daria6918.cn/gtkpywtvej.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yj20258.top/gtczhmbyoq.html

TS:   interface Shape { area(): number; }
来源：http://hz.gotoacloud.top/gtkffeerlh.html

Java: interface Shape { double area(); }
来源：http://hz.52xcode.cn/gtjitbxpps.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zhiwuduotai.top/gtifgpcauh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hammf.cn/gtckqgagvj.html

C#:   interface IShape { double Area(); }
来源：http://hz.zhengqikj.top/gtvarvbupx.html

[G10] 访问控制
来源：http://hz.nanxinkj.top/gtwoaczoyw.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.iojbl.cn/gtqokpfqaa.html

PHP:  public / protected / private
来源：http://hz.sufxvd.cn/gtjegnaduk.html

JS:   #private 字段；其余公开
来源：http://hz.xinyue.icu/gtttothjpi.html

TS:   public / protected / private
来源：http://hz.zhengqikj.top/gtycfcctws.html

Java: public / protected / private / 默认包级
来源：http://hz.chenjidiqi.icu/gtuptplhvi.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.shzxlz.cn/gtgdqnifij.html

Ruby: public / protected / private
来源：http://hz.tianlin.xyz/gthgavorza.html

C#:   public / protected / private / internal
来源：http://hz.sysykeji.top/gtdfddzmne.html

[G11] getter / setter
来源：http://hz.zhiwuduotai.top/gtpvwwzfaq.html

Py:   @property 与 @x.setter
来源：http://hz.gogol.net.cn/gtiwtwdyhv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.nwbrower.top/gtghgfwrot.html

JS:   get name() { return this._name; }
来源：http://hz.gogol.net.cn/gtdiyosdjk.html

TS:   get name(): string { return this._name; }
来源：http://hz.zycfv.cn/gtqkzepieb.html

Java: public String getName() { return name; }
来源：http://hz.quarkkingdee.top/gtjugtlrcv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.hywenlv.cn/gtiqxgmsta.html

Ruby: attr_accessor :name
来源：http://hz.yonumen.top/gtdxatqwxk.html

C#:   public string Name { get; set; }
来源：http://hz.shzxlz.cn/gtpdxibczs.html

[G12] 对象转字符串
来源：http://hz.sxryk.cn/gtmdebbtcl.html

Py:   def __str__(self): return self.name
来源：http://hz.yj20258.top/gtindsjplj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jlsjyb.cn/gtucvwgbky.html

JS:   toString() { return this.name; }
来源：http://hz.chenzaomai.com/gtdmkstvsl.html

TS:   toString(): string { return this.name; }
来源：http://hz.mhx1999.top/gttftshmtu.html

Java: @Override public String toString() { return name; }
来源：http://hz.snrcjt.cn/gtwrgkzcky.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.shanyushiyangtech.top/gtypvjephq.html

Ruby: def to_s; @name; end
来源：http://hz.redwolf501.top/gtdaacjaiw.html

C#:   public override string ToString() => Name;
来源：http://hz.shangyingyoupin.top/gtjnffswir.html

[G13] 判断对象类型
来源：http://hz.ywan-chungtsiang.top/gtzwbwdagz.html

Py:   isinstance(u, User)
来源：http://hz.jqgfzy.top/gtsnwbmijq.html

PHP:  $u instanceof User
来源：http://hz.fengsongda.top/gtixpwpdog.html

JS:   u instanceof User
来源：http://hz.iojbl.cn/gtahayfodb.html

TS:   u instanceof User
来源：http://hz.yj20258888.top/gtwwaliqor.html

Java: u instanceof User
来源：http://hz.guowangkeji.top/gtgipbertq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.hysaishi.cn/gtrpnlaxmy.html

Ruby: u.is_a?(User)
来源：http://hz.chenlongwang.top/gtirecwlgr.html

C#:   u is User
来源：http://hz.hysaishi.cn/gtbtbpfvai.html

[G14] 数据类 / record
来源：http://hz.jqgfzy.top/gtmqahratc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.hnqzz.top/gtbyncnefy.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.chenzaomai.com/gtttwivgwy.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.xuanzx.com/gtcvmejpmm.html

TS:   type User = { name: string; age: number };
来源：http://hz.andypj.xyz/gtyvottupf.html

Java: record User(String name, int age) {}
来源：http://hz.kuanghao11.cn/gtysicswtw.html

Go:   type User struct { Name string; Age int }
来源：http://hz.quarkkingdee.top/gtjixulqko.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.daria6918.cn/gtddaqftbm.html

C#:   record User(string Name, int Age);
来源：http://hz.yonumen.top/gtfwjomjqw.html

[G15] 枚举
来源：http://hz.daxiang520.top/gtnzhjdbbx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.aizwys.cn/gtwbcpbggx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jinqigufen.top/gtamlcikiw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.c1oappe.top/gtcbycubgb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.wangdashe.top/gtasxcacod.html

Java: enum Color { RED, GREEN }
来源：http://hz.jianghu66.top/gtbkqhunfr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.pengpengdd.cyou/gtyqneunmg.html

Ruby: Color = %i[red green].freeze
来源：http://hz.wangshuangyany.cn/gtsdhhkmxl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yj202588.top/gtjcacqskj.html

[G16] 对象转数组 / 字典
来源：http://hz.yj20258.top/gtkdbmrsit.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.hfpthk.cn/gtqxncvygt.html

PHP:  get_object_vars($obj);
来源：http://hz.andypj.xyz/gtrzyhubai.html

JS:   Object.entries(obj)
来源：http://hz.cashguo.top/gtoqqnnecn.html

TS:   Object.entries(obj)
来源：http://hz.zhijiandao.cn/gtmiksqxry.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.aibaodan.cn/gtcnqfcohh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.tian-w.cn/gtyxszzezf.html

Ruby: obj.instance_variables
来源：http://hz.zhixingplan.top/gtlmiduyff.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jianghu66.top/gtvsotseex.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtsxmxpamv.html

H. 异常与错误处理
来源：http://hz.svipenyu.cn/gteuxwuxtw.html

================================================================================
来源：http://hz.xziqi.cn/gtjbkqepin.html

[H01] try / catch 基础
来源：http://hz.yj20258888.top/gtthbpeyve.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.ppjwa.cn/gtsmhzrwbw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yj20258.top/gtvqxedxpj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yanxiufei.cn/gtzdcggdmz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.c1oappe.top/gttatojzbg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.9152youxi.cn/gtwpuinpxm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.meibo888.top/gttqnmwehu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.havefunace.top/gtusevngdk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jlsjyb.cn/gtwhqzxfrj.html

[H02] finally / ensure 收尾
来源：http://hz.zhengqikj.top/gtwsgjzfkt.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jianghu66.top/gthluqtwhn.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.cheryme.top/gtxzhzwbfj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.birdmap.top/gtiqhmjeip.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.cucudq.cn/gtbnaloitl.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.gotoacloud.top/gtwiuaamyo.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hysaishi.cn/gtucgtzfaz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.cashguo.top/gteygonzjy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jinqigfzy.top/gtjkkcfxab.html

[H03] 主动抛出异常
来源：http://hz.shzxlz.cn/gtiriixavm.html

Py:   raise ValueError("错误信息")
来源：http://hz.xingfuxueyuan.xyz/gtvpsbmkam.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.feifeiyinyue.top/gtkjfdhybt.html

JS:   throw new Error("错误信息");
来源：http://hz.zdqjudy.top/gtffdueddj.html

TS:   throw new Error("错误信息");
来源：http://hz.quarkkingdee.top/gtphazbgwh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.daria6918.cn/gtkhwtuclr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.sxryk.cn/gtpftpzynj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.tian-w.cn/gtkhalgnbx.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.sxryk.cn/gtqptrbosd.html

[H04] 自定义异常类型
来源：http://hz.shanyushiyangtech.top/gtnxljqdzf.html

Py:   class MyError(Exception): pass
来源：http://hz.zhoulong.xyz/gtqqnvrilo.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.mhx1999.top/gtmbyfphta.html

JS:   class MyError extends Error {}
来源：http://hz.xuanzx.com/gtgplinmeb.html

TS:   class MyError extends Error {}
来源：http://hz.hywenlv.cn/gtzsfsxuoy.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zycfv.cn/gtushqpzyy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.aibaodan.cn/gthhkekigu.html

Ruby: class MyError < StandardError; end
来源：http://hz.ehwqpu.com/gtjctmnwsm.html

C#:   class MyException : Exception {}
来源：http://hz.shangyingyoupin.top/gthwkdgced.html

[H05] 捕获特定类型
来源：http://hz.pengpengdd.cyou/gtpjjrgqyx.html

Py:   except ValueError as e:
来源：http://hz.shuidangran.top/gtelsxvvnw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.hywenlv.cn/gtozoinxgv.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.xuanzx.com/gtbftqozqf.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.meibo888.top/gtttfarlta.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.nanxuanxn.top/gtrmrpiwem.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.tianlin.xyz/gtqzxxzkmm.html

Ruby: rescue ArgumentError => e
来源：http://hz.xylfe.cn/gtvtzglpie.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.nwbrower.top/gtjrhsanuo.html

[H06] 可选值 / 空值安全访问
来源：http://hz.wangdashe.top/gtebxqvbmg.html

Py:   value = d.get("k") or default
来源：http://hz.quarkkingdee.top/gtvxmeglwa.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.sysykeji.top/gtzcnhynyw.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ybcxt.top/gtjuvymgnp.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.shangyingyoupin.top/gtjarfhvpr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.gogol.net.cn/gtfyoafuat.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.fzhhl.top/gtqzcdtzna.html

Ruby: d&.dig(:a, :b)
来源：http://hz.gotoacloud.top/gtzpysjxmx.html

C#:   obj?.A?.B ?? default
来源：http://hz.nanxinkj.top/gtpdimbhqg.html

[H07] 断言
来源：http://hz.yonumen.top/gtanypnknq.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zhiwuduotai.top/gtzzbucafl.html

PHP:  assert($x > 0);
来源：http://hz.gaohongyu789.top/gthnhqjjam.html

JS:   console.assert(x > 0);
来源：http://hz.daria6918.cn/gtaoronnbs.html

TS:   console.assert(x > 0);
来源：http://hz.ehwqpu.com/gtjjoibeil.html

Java: assert x > 0 : "必须为正";
来源：http://hz.0kj1m.cn/gtktpheioc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ybcxt.top/gtyvbptokx.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.chenjidiqi.icu/gtafbqqahd.html

C#:   Debug.Assert(x > 0);
来源：http://hz.iojbl.cn/gtysoqcecg.html

[H08] 获取错误信息与堆栈
来源：http://hz.9152youxi.cn/gtuzyluyou.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.cucudq.cn/gtbdubkiha.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.xylfe.cn/gtvpijecta.html

JS:   e.message;  e.stack
来源：http://hz.yj20258888.top/gtzupobpzo.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jianghu66.top/gtcnhotoxz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.gogol.net.cn/gtghsmywyf.html

Go:   err.Error()
来源：http://hz.yueranfly.top/gtbnfyverd.html


<!-- 参考信息 -->