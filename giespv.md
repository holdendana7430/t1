代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.kuanghao11.cn/gtibemszmw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.smart0.xyz/gtuznnwtyj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.nanxinkj.top/gtimsfezlz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.c1oappe.top/gtlpdxzsry.html

[F05] 判断文件或目录是否存在
来源：http://hz.hongshengwenyu.top/gtvpvmyptd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zdqjudy.top/gtdlbkyfzx.html

PHP:  file_exists("a.txt");
来源：http://hz.dashuyun.cn/gtluhdpntp.html

JS:   fs.existsSync("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtdmcfwcaj.html

TS:   fs.existsSync("a.txt")
来源：http://hz.c1oappe.top/gtniqzrkbq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jinyuanbaomall.cn/gtetpbfqjg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.gotoacloud.top/gtqgpxocpp.html

Ruby: File.exist?("a.txt")
来源：http://hz.xziqi.cn/gtdcrhaneu.html

C#:   File.Exists("a.txt")
来源：http://hz.guannengcc.top/gterurtzzp.html

[F06] 删除文件
来源：http://hz.redwolf501.top/gttlujbzxt.html

Py:   os.remove("a.txt")
来源：http://hz.iojbl.cn/gtjbdapfix.html

PHP:  unlink("a.txt");
来源：http://hz.kuanghao11.cn/gtqmpgzhjb.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.c1oappe.top/gtengsxdiu.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.xuetiantiany.cn/gtftgbwqed.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.aibaodan.cn/gttwqpxvxc.html

Go:   os.Remove("a.txt")
来源：http://hz.jinqigfzy.top/gtbnhiouxj.html

Ruby: File.delete("a.txt")
来源：http://hz.tanke756.top/gtobwflpve.html

C#:   File.Delete("a.txt");
来源：http://hz.shuidangran.top/gtkohkpxcx.html

[F07] 创建目录（含多级）
来源：http://hz.andypj.xyz/gtoalsyavx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.snrcjt.cn/gtyvvmpesx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.ydjk.org.cn/gthqdtfopb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.gogol.net.cn/gtbqthpksi.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yuanzhike.top/gtkmjetwxx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.sufxvd.cn/gtjomdpgeo.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hysaishi.cn/gtunrqaiai.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jianghu66.top/gtcyxghqdy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jiagoushi.top/gtnhtzwhan.html

[F08] 遍历目录
来源：http://hz.zhiwuduotai.top/gtojsmtqzt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.sysykeji.top/gtkejqswbl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.zhiwuduotai.top/gtrccmwmat.html

JS:   fs.readdirSync("dir")
来源：http://hz.dashuyun.cn/gtxpouptft.html

TS:   fs.readdirSync("dir")
来源：http://hz.52xcode.cn/gtywmdmqwc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jqgufenzy.top/gtlsrhfwma.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zhiwuduotai.top/gtaesewrkn.html

Ruby: Dir.children("dir")
来源：http://hz.vqdsnc.cn/gtaopxmmuh.html

C#:   Directory.GetFiles("dir")
来源：http://hz.tian-w.cn/gtxzdpskhv.html

[F09] 获取文件大小
来源：http://hz.xuanzx.com/gtevlcliyy.html

Py:   os.path.getsize("a.txt")
来源：http://hz.chenjidiqi.icu/gtntzqvpyg.html

PHP:  filesize("a.txt");
来源：http://hz.yj20258888.top/gtjqnoyxhd.html

JS:   fs.statSync("a.txt").size
来源：http://hz.nanxinkj.top/gtgnsvlcqd.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yj20258.top/gtdphlwfed.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.xuetiantiany.cn/gtgngdipik.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yueranfly.top/gtfufgtnfy.html

Ruby: File.size("a.txt")
来源：http://hz.birdmap.top/gtynwlouvy.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yuxming.cn/gteuztsgeh.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yongpay.top/gtwfdlmxcz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.daria6918.cn/gtogtwymxh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.aizwys.cn/gtxrqqcwjg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.dianchejie.cn/gtrtmeqhce.html

TS:   path.extname("a.txt")
来源：http://hz.hammf.cn/gtfgaplnzp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.hnqzz.top/gtcpibgcyj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.cheryme.top/gtqsgzabzh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.cheryme.top/gtaklcwzsn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.svipenyu.cn/gtbnycpxcj.html

[F11] 复制与移动文件
来源：http://hz.ydjk.org.cn/gtskxpepiv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jlsjyb.cn/gtxjnktlxw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yangfankeji.com/gtyzqkwydl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hfpthk.cn/gtbccwrimg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.guannengcc.top/gtcohvstgi.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.fengsongda.top/gthchwmncu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jiagoushi.top/gtkprfxhgg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.iojbl.cn/gtjkefheot.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.cashguo.top/gtxsuenkcd.html

[F12] CSV 读写
来源：http://hz.feifeiyinyue.top/gttdxbkyti.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xinyue.icu/gtsgsjdxie.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.xinyue.icu/gtxfohedqe.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zhaomingkeji.xyz/gtiowdetum.html

TS:   // 同上
来源：http://hz.zhixingplan.top/gtgktxlhwe.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yj20258.top/gtonvilgoz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.chenlongwang.top/gtkkqwaikl.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.hysaishi.cn/gtkpmpbpog.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yuanzhike.top/gtqavdccsy.html

================================================================================
来源：http://hz.jinqigfzy.top/gthadsjmqi.html

G. 面向对象
来源：http://hz.chenzaomai.com/gtokvcmkcn.html

================================================================================
来源：http://hz.aizwys.cn/gtuokfrxjx.html

[G01] 定义类
来源：http://hz.birdmap.top/gtscjxefoa.html

Py:   class User: pass
来源：http://hz.redwolf501.top/gtrjkfxicw.html

PHP:  class User {}
来源：http://hz.ehwqpu.com/gtlhcndush.html

JS:   class User {}
来源：http://hz.quarkkingdee.top/gtujjmfyqp.html

TS:   class User { name: string = ""; }
来源：http://hz.chenjidiqi.icu/gtuvqscowz.html

Java: class User {}
来源：http://hz.zdqjudy.top/gtvvkeidac.html

Go:   type User struct { Name string }
来源：http://hz.shuidangran.top/gtdcrgrywv.html

Ruby: class User; end
来源：http://hz.nanxinkj.top/gtosmutkzv.html

C#:   class User {}
来源：http://hz.quarkkingdee.top/gtwpjgsqit.html

[G02] 构造函数
来源：http://hz.gotoacloud.top/gtomgcjeox.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.snrcjt.cn/gteyltnlbq.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.chenzaomai.com/gtosgyeisf.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.pengpengdd.cyou/gtkwwvtatk.html

TS:   constructor(public name: string) {}
来源：http://hz.sufxvd.cn/gtwexwkptk.html

Java: User(String name) { this.name = name; }
来源：http://hz.jianghu66.top/gtesmegbld.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zhixingplan.top/gtcpsdkkpt.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.shanyushiyangtech.top/gtnbgazffg.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jinyuanbaomall.cn/gtzhqdclin.html

[G03] 实例属性
来源：http://hz.hammf.cn/gtzerpfynk.html

Py:   self.name = "x"
来源：http://hz.shanyushiyangkeji.top/gtfyvqhevj.html

PHP:  public string $name = "x";
来源：http://hz.jqgfzy.top/gtoncnbmha.html

JS:   this.name = "x";
来源：http://hz.zycfv.cn/gtnojheljq.html

TS:   name: string = "x";
来源：http://hz.cashguo.top/gtcktitsix.html

Java: private String name;
来源：http://hz.iojbl.cn/gtbbeebyyu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hywenlv.cn/gtfyksfgug.html

Ruby: @name = "x"
来源：http://hz.smart0.xyz/gtiorsizmc.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.snrcjt.cn/gtszqoidrm.html

[G04] 定义方法
来源：http://hz.nanxinkj.top/gtorzbylgx.html

Py:   def greet(self): return self.name
来源：http://hz.pycfn.com/gtpnkvabji.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yueranfly.top/gtgxrpxdwv.html

JS:   greet() { return this.name; }
来源：http://hz.yj202588.top/gttznxmuyx.html

TS:   greet(): string { return this.name; }
来源：http://hz.xylfe.cn/gtrrsnxaaf.html

Java: String greet() { return name; }
来源：http://hz.chenzaomai.com/gtibfdoeec.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zhoulong.xyz/gtrygpbaya.html

Ruby: def greet; @name; end
来源：http://hz.chenjidiqi.icu/gtdaiqfaty.html

C#:   public string Greet() => Name;
来源：http://hz.shanyushiyangtech.top/gtsicdjfgb.html

[G05] 继承
来源：http://hz.jianghu66.top/gtsgeqgduv.html

Py:   class Admin(User): pass
来源：http://hz.gotoacloud.top/gtlwemllqr.html

PHP:  class Admin extends User {}
来源：http://hz.yuanzhike.top/gtkdrphgzt.html

JS:   class Admin extends User {}
来源：http://hz.wangshuangyany.cn/gtiwwpoyfe.html

TS:   class Admin extends User {}
来源：http://hz.xziqi.cn/gtrncikpmb.html

Java: class Admin extends User {}
来源：http://hz.yj20258888.top/gtwxkgfwyd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jyoumei.cn/gtujhqkojy.html

Ruby: class Admin < User; end
来源：http://hz.hongshengwenyu.top/gtutlrxyko.html

C#:   class Admin : User {}
来源：http://hz.yueranfly.top/gtzpdftmdr.html

[G06] 重写方法
来源：http://hz.guowangkeji.top/gthruswkvc.html

Py:   def greet(self): return "admin"
来源：http://hz.hongshengwenyu.top/gtaakselsc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.cdnleiting.top/gtavknbpmm.html

JS:   greet() { return "admin"; }
来源：http://hz.xziqi.cn/gthkmtysvi.html

TS:   greet(): string { return "admin"; }
来源：http://hz.sysykeji.top/gtehcpepsh.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jinqigufen.top/gtbzpmqrdb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.shzxlz.cn/gtlgiaikjo.html

Ruby: def greet; "admin"; end
来源：http://hz.gzhubu.top/gtfkbxoolj.html

C#:   public override string Greet() => "admin";
来源：http://hz.ivvv.top/gtiqrqwdnn.html

[G07] 调用父类方法
来源：http://hz.zhongyouzk.top/gtidwwzrnh.html

Py:   super().greet()
来源：http://hz.xuetiantiany.cn/gtczdqgyns.html

PHP:  parent::greet();
来源：http://hz.vqdsnc.cn/gtqskyqhwk.html

JS:   super.greet();
来源：http://hz.bjfxy.top/gtoriyxbga.html

TS:   super.greet();
来源：http://hz.ywan-chungtsiang.top/gtlktysxzs.html

Java: super.greet();
来源：http://hz.xuanzx.com/gtwfhhzjwo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.fzhhl.top/gtllsrkfgb.html

Ruby: super
来源：http://hz.ppjwa.cn/gtcscjsomy.html

C#:   base.Greet();
来源：http://hz.jlsjyb.cn/gtywqtmtdc.html

[G08] 静态方法与属性
来源：http://hz.gogol.net.cn/gtjyihyfjp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.iojbl.cn/gtlplkepss.html

PHP:  public static function f() {}
来源：http://hz.pycfn.com/gthceyzcyh.html

JS:   static f() {}
来源：http://hz.yj20258.top/gtlwweiidz.html

TS:   static f(): void {}
来源：http://hz.yueranfly.top/gtsjhkeiaq.html

Java: static void f() {}
来源：http://hz.jinghuilouyu.cn/gtqrujtfti.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yanxiufei.cn/gthtlmscdr.html

Ruby: def self.f; end
来源：http://hz.shzxlz.cn/gtveqlakzk.html

C#:   public static void F() {}
来源：http://hz.52xcode.cn/gtfhaptolb.html

[G09] 接口 / 抽象类
来源：http://hz.chenlongwang.top/gtmjgsalyr.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yongpay.top/gtpjhgddet.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.guannengcc.top/gtlblvsgbr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yj20258.top/gtdkzmtjnq.html

TS:   interface Shape { area(): number; }
来源：http://hz.jinghuilouyu.cn/gtqgruprpp.html

Java: interface Shape { double area(); }
来源：http://hz.zycfv.cn/gthhyhwior.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jinqigfzy.top/gtgobprngi.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hammf.cn/gtwnngxwoc.html

C#:   interface IShape { double Area(); }
来源：http://hz.jqgufenzy.top/gtuzxrnrpq.html

[G10] 访问控制
来源：http://hz.sxryk.cn/gtnogzoznl.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.shanyushiyangkeji.top/gtcnzqucli.html

PHP:  public / protected / private
来源：http://hz.jyoumei.cn/gtvgbbnatx.html

JS:   #private 字段；其余公开
来源：http://hz.hywenlv.cn/gtizegslhn.html

TS:   public / protected / private
来源：http://hz.hfpthk.cn/gtykkegzdr.html

Java: public / protected / private / 默认包级
来源：http://hz.sufxvd.cn/gtfrxljwig.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.guowangkeji.top/gtmigpwkos.html

Ruby: public / protected / private
来源：http://hz.kuanghao11.cn/gtclhdcehv.html

C#:   public / protected / private / internal
来源：http://hz.smart0.xyz/gtrobdcjwp.html

[G11] getter / setter
来源：http://hz.yuanzhike.top/gtwolziwqt.html

Py:   @property 与 @x.setter
来源：http://hz.jqgufenzy.top/gtnahrjwer.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.andypj.xyz/gtyqomisew.html

JS:   get name() { return this._name; }
来源：http://hz.tanke756.top/gtgpaogsox.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhaomingkeji.xyz/gtzaryppiw.html

Java: public String getName() { return name; }
来源：http://hz.yongpay.top/gtfojxmrsn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.aizwys.cn/gtxykuqnnc.html

Ruby: attr_accessor :name
来源：http://hz.hammf.cn/gtjoioquic.html

C#:   public string Name { get; set; }
来源：http://hz.guowangkeji.top/gtwuvurquc.html

[G12] 对象转字符串
来源：http://hz.gotoacloud.top/gtuscbvboj.html

Py:   def __str__(self): return self.name
来源：http://hz.feifeiyinyue.top/gtbhqfokoz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yueranfly.top/gtysptseov.html

JS:   toString() { return this.name; }
来源：http://hz.nanxinkj.top/gthorvllvm.html

TS:   toString(): string { return this.name; }
来源：http://hz.birdmap.top/gtylptkarw.html

Java: @Override public String toString() { return name; }
来源：http://hz.kuanghao11.cn/gtnlncabxl.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jiagoushi.top/gtwqiiccqw.html

Ruby: def to_s; @name; end
来源：http://hz.jinghuilouyu.cn/gtzsvuuccm.html

C#:   public override string ToString() => Name;
来源：http://hz.0kj1m.cn/gtjlvufyrq.html

[G13] 判断对象类型
来源：http://hz.jiagoushi.top/gtvgbzslib.html

Py:   isinstance(u, User)
来源：http://hz.yueranfly.top/gtbzddnhre.html

PHP:  $u instanceof User
来源：http://hz.yongpay.top/gtwakaxole.html

JS:   u instanceof User
来源：http://hz.shanyushiyangtech.top/gthxferozm.html

TS:   u instanceof User
来源：http://hz.xuanzx.com/gttnzaemvq.html

Java: u instanceof User
来源：http://hz.fengsongda.top/gtyzzpzvyn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.hfpthk.cn/gtykcmpren.html

Ruby: u.is_a?(User)
来源：http://hz.shzxlz.cn/gtfhfygwgb.html

C#:   u is User
来源：http://hz.xuetiantiany.cn/gtrvrndbqx.html

[G14] 数据类 / record
来源：http://hz.gogol.net.cn/gtuessjyic.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jianghu66.top/gtzfppgroj.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.fengsongda.top/gtiolxdlkn.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhixingplan.top/gtyfpzvazu.html

TS:   type User = { name: string; age: number };
来源：http://hz.316326.xyz/gtrlmtkvso.html

Java: record User(String name, int age) {}
来源：http://hz.shuidangran.top/gtacacmeru.html

Go:   type User struct { Name string; Age int }
来源：http://hz.birdmap.top/gtlyydcpzq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.smart0.xyz/gtfmobtxff.html

C#:   record User(string Name, int Age);
来源：http://hz.gotoacloud.top/gtupvvvius.html

[G15] 枚举
来源：http://hz.birdmap.top/gtdvxlqimk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.shangyingyoupin.top/gtkarcvxls.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jinghuilouyu.cn/gtzacchffu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.sxryk.cn/gtlksvdvmz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yanxiufei.cn/gtvuwjerrl.html

Java: enum Color { RED, GREEN }
来源：http://hz.cheryme.top/gtqpauqxdo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.nanxinkj.top/gticmcnasa.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ydjk.org.cn/gtzuoyztqx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhijiandao.cn/gtnjsgmpjf.html

[G16] 对象转数组 / 字典
来源：http://hz.shanyushiyangtech.top/gtyltfjkcx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.redwolf501.top/gtgttsidhd.html

PHP:  get_object_vars($obj);
来源：http://hz.daxiang520.top/gtjlwbpkbj.html

JS:   Object.entries(obj)
来源：http://hz.yj20258.top/gtuzixsaim.html

TS:   Object.entries(obj)
来源：http://hz.yongpay.top/gtemwtgmrv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhixingplan.top/gtbghmfxor.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.snrcjt.cn/gtggnitxck.html

Ruby: obj.instance_variables
来源：http://hz.hnxiangtu.top/gtxlfgdfft.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.sufxvd.cn/gtrztyjnhs.html

================================================================================
来源：http://hz.0kj1m.cn/gthauzadvb.html

H. 异常与错误处理
来源：http://hz.9152youxi.cn/gtpapydrmg.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtmhhcoosa.html

[H01] try / catch 基础
来源：http://hz.jinqigfzy.top/gtwpqlreep.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.fengsongda.top/gtfwhawvcx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.shangyingyoupin.top/gtkkkuyvdu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.aizwys.cn/gtmjuzjpbc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.chenzaomai.com/gtrsatpyql.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.shangyingyoupin.top/gtcxulgfkn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.hysaishi.cn/gtlnadmmha.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.xingfuxueyuan.xyz/gtcuaozvru.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jianghu66.top/gtfkhxdtfm.html

[H02] finally / ensure 收尾
来源：http://hz.hnxiangtu.top/gtkrdlbanc.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jianghu66.top/gtxcjgunjj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhiwuduotai.top/gtqjhdiaim.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.kuanghao11.cn/gtkysagyao.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ywan-chungtsiang.top/gtmgmecvly.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.feifeiyinyue.top/gtjkjbrbfu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.shuidangran.top/gtefxzifxc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.chenlongwang.top/gtsatagczc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jinyuanbaomall.cn/gtnimkdarc.html

[H03] 主动抛出异常
来源：http://hz.xziqi.cn/gtmtfxjdtq.html

Py:   raise ValueError("错误信息")
来源：http://hz.meibo888.top/gtycqzvemt.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.dashuyun.cn/gtbwphsfvk.html

JS:   throw new Error("错误信息");
来源：http://hz.nwbrower.top/gtqdbgfpya.html

TS:   throw new Error("错误信息");
来源：http://hz.9152youxi.cn/gtmcrbzcbz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.pengpengdd.cyou/gtfdwxqdsa.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.gzhubu.top/gtnwvdmaeg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jlsjyb.cn/gthissgloy.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.chenlongwang.top/gtleauubtd.html

[H04] 自定义异常类型
来源：http://hz.chenzaomai.com/gtiouaedmo.html

Py:   class MyError(Exception): pass
来源：http://hz.wangdashe.top/gtmhcawenu.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.tianlin.xyz/gtwhnpdffa.html

JS:   class MyError extends Error {}
来源：http://hz.nanxuanxn.top/gtrdyrktiq.html

TS:   class MyError extends Error {}
来源：http://hz.hnxiangtu.top/gtgjogzijj.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yj202588.top/gtsnjhwxca.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.tianlin.xyz/gtsttmdlcs.html

Ruby: class MyError < StandardError; end
来源：http://hz.birdmap.top/gtcbahhnse.html

C#:   class MyException : Exception {}
来源：http://hz.hnxiangtu.top/gtdwwpwkjw.html

[H05] 捕获特定类型
来源：http://hz.0kj1m.cn/gtqppaieys.html

Py:   except ValueError as e:
来源：http://hz.yj20258888.top/gtbbogsynt.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.shanyushiyangkeji.top/gtlkkicvdo.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.dianchejie.cn/gtdphekxsl.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.gaohongyu789.top/gtyqruwykd.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.sxryk.cn/gtsdmednbf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.sweek.top/gtvuwtiyhu.html

Ruby: rescue ArgumentError => e
来源：http://hz.chenzaomai.com/gtxfujgjce.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.meibo888.top/gteqzrstbf.html

[H06] 可选值 / 空值安全访问
来源：http://hz.316326.xyz/gttbsjxnrv.html

Py:   value = d.get("k") or default
来源：http://hz.nanxuanxn.top/gtasgrbvtc.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yuxming.cn/gtrkayykiy.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zhoulong.xyz/gtpyytrbnb.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.fzhhl.top/gtgrvhbxif.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.gzhubu.top/gtqlglrczl.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.sxryk.cn/gtwryxlpja.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jinyuanbaomall.cn/gtprupncxh.html

C#:   obj?.A?.B ?? default
来源：http://hz.xingfuxueyuan.xyz/gtywveyngu.html

[H07] 断言
来源：http://hz.yj202588.top/gtcdgwtyku.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yuanzhike.top/gtghbvkhcf.html

PHP:  assert($x > 0);
来源：http://hz.zhiwuduotai.top/gtypgfetig.html

JS:   console.assert(x > 0);
来源：http://hz.xuanzx.com/gtkoxieesx.html

TS:   console.assert(x > 0);
来源：http://hz.meibo888.top/gtvqwlzcnb.html

Java: assert x > 0 : "必须为正";
来源：http://hz.smart0.xyz/gtwqwzqhux.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.wangdashe.top/gtisjnsdvs.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.316326.xyz/gtjdszenaz.html

C#:   Debug.Assert(x > 0);
来源：http://hz.pengpengdd.cyou/gtcaiipkol.html

[H08] 获取错误信息与堆栈
来源：http://hz.andypj.xyz/gtkpvryyyl.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ydjk.org.cn/gtdiochevb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.smart0.xyz/gtudfmiiyq.html

JS:   e.message;  e.stack
来源：http://hz.shangyingyoupin.top/gtgrqcwrpe.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.xziqi.cn/gtnewrkapc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.vqdsnc.cn/gtfdsgbewd.html

Go:   err.Error()
来源：http://hz.xziqi.cn/gtjprnswbq.html

Ruby: e.message;  e.backtrace
来源：http://hz.ivvv.top/gtmmksddim.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhongyouzk.top/gtfgbavsfi.html

[H09] 带错误码的异常
来源：http://hz.316326.xyz/gtpgintemj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.sufxvd.cn/gtysiiwltb.html


<!-- 参考信息 -->