代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.nanxuanxn.top/gtvzrcoxnj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.jinyuanbaomall.cn/gtwlwkdmhy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.birdmap.top/gtmqwuwwkd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hnxiangtu.top/gtotqekeiv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.daria6918.cn/gtwczwojzy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.shuidangran.top/gtoxvrjvqu.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.hammf.cn/gtxruspuri.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.xuanzx.com/gttsseoroz.html

[F05] 判断文件或目录是否存在
来源：http://hz.vqdsnc.cn/gtmwnisgjp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.aibaodan.cn/gtqqtipeua.html

PHP:  file_exists("a.txt");
来源：http://hz.zhongyouzk.top/gtckbygrtm.html

JS:   fs.existsSync("a.txt")
来源：http://hz.shzxlz.cn/gtoxlnwyji.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhongyouzk.top/gtmksjnhkm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.shuidangran.top/gtnmodclki.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zhengqikj.top/gtofsseaex.html

Ruby: File.exist?("a.txt")
来源：http://hz.havefunace.top/gtzvuddnjh.html

C#:   File.Exists("a.txt")
来源：http://hz.yvedp.cn/gtyvnbpwek.html

[F06] 删除文件
来源：http://hz.guowangkeji.top/gtqffusyjd.html

Py:   os.remove("a.txt")
来源：http://hz.zhijiandao.cn/gtajocrxib.html

PHP:  unlink("a.txt");
来源：http://hz.jqgfzy.top/gtdgdvzafb.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.jqgfzy.top/gtjftsnimy.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yuxming.cn/gtmwqmkaxm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.vqdsnc.cn/gtzvlvwwhx.html

Go:   os.Remove("a.txt")
来源：http://hz.52xcode.cn/gtnapebulr.html

Ruby: File.delete("a.txt")
来源：http://hz.316326.xyz/gtmwiqfvud.html

C#:   File.Delete("a.txt");
来源：http://hz.zhiwuduotai.top/gtgxftiipg.html

[F07] 创建目录（含多级）
来源：http://hz.wangshuangyany.cn/gtzpcxbcmj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zhoulong.xyz/gtjakvepqh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.bjfxy.top/gtngpfswty.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.fzhhl.top/gtzfglgppe.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.quarkkingdee.top/gtgwxhwycv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.dashuyun.cn/gtrvljnkht.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zhiwuduotai.top/gtqxfhghej.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.dashuyun.cn/gtjfuothyb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yvedp.cn/gtxnivtwgu.html

[F08] 遍历目录
来源：http://hz.havefunace.top/gtypoisvzq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.ywan-chungtsiang.top/gtuhjjtfyp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.c1oappe.top/gtubdcouwj.html

JS:   fs.readdirSync("dir")
来源：http://hz.jlsjyb.cn/gtyefwjhoe.html

TS:   fs.readdirSync("dir")
来源：http://hz.shuidangran.top/gtgnuzignm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.xinyue.icu/gtvwzfppdc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.guowangkeji.top/gtlghkqwyk.html

Ruby: Dir.children("dir")
来源：http://hz.zhengqikj.top/gtftspqtrl.html

C#:   Directory.GetFiles("dir")
来源：http://hz.shanyushiyangtech.top/gtlrkhewxn.html

[F09] 获取文件大小
来源：http://hz.xylfe.cn/gtgjnhhcdb.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yj20258.top/gtzzioyulz.html

PHP:  filesize("a.txt");
来源：http://hz.hongshengwenyu.top/gtxucjzhiu.html

JS:   fs.statSync("a.txt").size
来源：http://hz.tian-w.cn/gtcinnggcl.html

TS:   fs.statSync("a.txt").size
来源：http://hz.sufxvd.cn/gtpciatfam.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.chenjidiqi.icu/gtlhxwjacb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jinqigfzy.top/gtqoaudtch.html

Ruby: File.size("a.txt")
来源：http://hz.ivvv.top/gtrtfomfcm.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jqgufenzy.top/gtflkpzqmy.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.ppjwa.cn/gtvjwtqrwl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.sxryk.cn/gtdfwxgeae.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.shzxlz.cn/gtbikyufcj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jyoumei.cn/gtysntvflr.html

TS:   path.extname("a.txt")
来源：http://hz.sweek.top/gtljpjubdi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.cucudq.cn/gtjyccyeqv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.iojbl.cn/gtzkxrxgox.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.shanyushiyangkeji.top/gthiabbbso.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.shuidangran.top/gthqhtfyog.html

[F11] 复制与移动文件
来源：http://hz.sufxvd.cn/gteacumkrd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.mhx1999.top/gtieeuutdb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.daria6918.cn/gtpyqxxfpj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jinghuilouyu.cn/gtkxgezlep.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.9152youxi.cn/gtzyrxkjcn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.hywenlv.cn/gtdvrmfjye.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.guannengcc.top/gtsszvgvtl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.ywan-chungtsiang.top/gtdrpqusil.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.wangdashe.top/gtfpwzniqe.html

[F12] CSV 读写
来源：http://hz.aizwys.cn/gtfzovvgmk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yueranfly.top/gtcfenbzzs.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.redwolf501.top/gtyyrzhlbl.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.nwbrower.top/gtzuysbmak.html

TS:   // 同上
来源：http://hz.zdqjudy.top/gtnyijjkaw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.aizwys.cn/gtizqrnoxx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.sweek.top/gtylvfxqhl.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.shanyushiyangtech.top/gtozxjhxht.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.gaohongyu789.top/gtdjsemiif.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtlxptygda.html

G. 面向对象
来源：http://hz.wangdashe.top/gtrdjajdyh.html

================================================================================
来源：http://hz.ehwqpu.com/gtujbelbsb.html

[G01] 定义类
来源：http://hz.havefunace.top/gtpvicgzos.html

Py:   class User: pass
来源：http://hz.ehwqpu.com/gtdndycqxl.html

PHP:  class User {}
来源：http://hz.chenzaomai.com/gtgvjgqrdv.html

JS:   class User {}
来源：http://hz.sxryk.cn/gtwvbjnmkq.html

TS:   class User { name: string = ""; }
来源：http://hz.daxiang520.top/gtddtsjphg.html

Java: class User {}
来源：http://hz.meibo888.top/gtnijulecr.html

Go:   type User struct { Name string }
来源：http://hz.ydzc1.top/gtarlsxcug.html

Ruby: class User; end
来源：http://hz.shanyushiyangkeji.top/gtcntgvhmv.html

C#:   class User {}
来源：http://hz.daxiang520.top/gtbwolohxf.html

[G02] 构造函数
来源：http://hz.redwolf501.top/gtlbqamqzp.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.smart0.xyz/gttlrddkoq.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jianghu66.top/gtjdjgkyar.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yuanzhike.top/gtegngzxsz.html

TS:   constructor(public name: string) {}
来源：http://hz.ydjk.org.cn/gtamnbhwvm.html

Java: User(String name) { this.name = name; }
来源：http://hz.xylfe.cn/gtrmrqmgle.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.shanyushiyangkeji.top/gtrrljzyeb.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.shzxlz.cn/gtfojfgwus.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zhoulong.xyz/gtrrasuaef.html

[G03] 实例属性
来源：http://hz.wangdashe.top/gtrjxrplli.html

Py:   self.name = "x"
来源：http://hz.jyoumei.cn/gtvpjsqhnn.html

PHP:  public string $name = "x";
来源：http://hz.birdmap.top/gtfmvpejxf.html

JS:   this.name = "x";
来源：http://hz.zhiwuduotai.top/gthhpwqevh.html

TS:   name: string = "x";
来源：http://hz.haohaochexian.top/gtziwqnsas.html

Java: private String name;
来源：http://hz.ydzc1.top/gtsvabcwfx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hywenlv.cn/gtvnyqlmth.html

Ruby: @name = "x"
来源：http://hz.jlsjyb.cn/gteyjpdnui.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.shangyingyoupin.top/gtypdpmyum.html

[G04] 定义方法
来源：http://hz.sxryk.cn/gtmwjaaagt.html

Py:   def greet(self): return self.name
来源：http://hz.zhixingplan.top/gtyxefkmcs.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.quarkkingdee.top/gtaanppkrs.html

JS:   greet() { return this.name; }
来源：http://hz.sysykeji.top/gtvpzlzsia.html

TS:   greet(): string { return this.name; }
来源：http://hz.cashguo.top/gtouhgbunu.html

Java: String greet() { return name; }
来源：http://hz.xuetiantiany.cn/gtizhdcpib.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ydzc1.top/gtmdmprjqa.html

Ruby: def greet; @name; end
来源：http://hz.tanke756.top/gtdpcrywrz.html

C#:   public string Greet() => Name;
来源：http://hz.zhixingplan.top/gtpbnogmtg.html

[G05] 继承
来源：http://hz.ydzc1.top/gtuepwbjuu.html

Py:   class Admin(User): pass
来源：http://hz.pengpengdd.cyou/gtqcyzcgao.html

PHP:  class Admin extends User {}
来源：http://hz.tanke756.top/gtulsgmbda.html

JS:   class Admin extends User {}
来源：http://hz.52xcode.cn/gtjmhghnrz.html

TS:   class Admin extends User {}
来源：http://hz.hywenlv.cn/gtrqnjtcgf.html

Java: class Admin extends User {}
来源：http://hz.yuxming.cn/gtgzwubnsg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jinqigfzy.top/gtkwfmjahq.html

Ruby: class Admin < User; end
来源：http://hz.guowangkeji.top/gtfkpvoenf.html

C#:   class Admin : User {}
来源：http://hz.guowangkeji.top/gtlsaxxiip.html

[G06] 重写方法
来源：http://hz.aibaodan.cn/gtfrrpqnjk.html

Py:   def greet(self): return "admin"
来源：http://hz.sxryk.cn/gtxlqrxset.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.wangdashe.top/gtgiowfbww.html

JS:   greet() { return "admin"; }
来源：http://hz.shuidangran.top/gtfsdwabvg.html

TS:   greet(): string { return "admin"; }
来源：http://hz.daxiang520.top/gtragbfclo.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.meibo888.top/gttrgxntaf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.shangyingyoupin.top/gtbxlginix.html

Ruby: def greet; "admin"; end
来源：http://hz.meibo888.top/gtevudjfga.html

C#:   public override string Greet() => "admin";
来源：http://hz.guowangkeji.top/gtgtfzhbtv.html

[G07] 调用父类方法
来源：http://hz.xingfuxueyuan.xyz/gteotrqpml.html

Py:   super().greet()
来源：http://hz.cucudq.cn/gtnvzuuiqo.html

PHP:  parent::greet();
来源：http://hz.aibaodan.cn/gtidideykt.html

JS:   super.greet();
来源：http://hz.xinyue.icu/gtxuoqkopm.html

TS:   super.greet();
来源：http://hz.bjfxy.top/gtxtkuldft.html

Java: super.greet();
来源：http://hz.andypj.xyz/gtxaqnhqgl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.meibo888.top/gtloczrisv.html

Ruby: super
来源：http://hz.haohaochexian.top/gtkfublqqj.html

C#:   base.Greet();
来源：http://hz.chenlongwang.top/gtcxdcpyrc.html

[G08] 静态方法与属性
来源：http://hz.yuanzhike.top/gtiwoxtwsl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.nwbrower.top/gtguhvpzch.html

PHP:  public static function f() {}
来源：http://hz.sxryk.cn/gtoytelfvl.html

JS:   static f() {}
来源：http://hz.jinqigufen.top/gtrcdtzani.html

TS:   static f(): void {}
来源：http://hz.sufxvd.cn/gtsbxtzazt.html

Java: static void f() {}
来源：http://hz.shanyushiyangtech.top/gtjtmhvdvz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jlsjyb.cn/gtnfwxvupd.html

Ruby: def self.f; end
来源：http://hz.zhiwuduotai.top/gtcyyfrswe.html

C#:   public static void F() {}
来源：http://hz.tian-w.cn/gtpoqlsfuy.html

[G09] 接口 / 抽象类
来源：http://hz.feifeiyinyue.top/gtmapxvnzl.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yj20258888.top/gtmepaiimu.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yangfankeji.com/gtewteruut.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yj202588.top/gtvovbxyck.html

TS:   interface Shape { area(): number; }
来源：http://hz.yongpay.top/gtafoyxwja.html

Java: interface Shape { double area(); }
来源：http://hz.shanyushiyangkeji.top/gtlcmaonum.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.kuanghao11.cn/gtcrisosex.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.dianchejie.cn/gtoyztribq.html

C#:   interface IShape { double Area(); }
来源：http://hz.c1oappe.top/gtgtoscpjk.html

[G10] 访问控制
来源：http://hz.andypj.xyz/gttrcrxcfn.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hammf.cn/gtiyzwldvj.html

PHP:  public / protected / private
来源：http://hz.ybcxt.top/gtjtpgzikn.html

JS:   #private 字段；其余公开
来源：http://hz.xinyue.icu/gtdkdpixmh.html

TS:   public / protected / private
来源：http://hz.ywan-chungtsiang.top/gtmbfbexoe.html

Java: public / protected / private / 默认包级
来源：http://hz.jiagoushi.top/gtjozmekjo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.sysykeji.top/gtwskafddm.html

Ruby: public / protected / private
来源：http://hz.316326.xyz/gtbpvfewqi.html

C#:   public / protected / private / internal
来源：http://hz.daria6918.cn/gtuoxoorjq.html

[G11] getter / setter
来源：http://hz.wangdashe.top/gtowfkiftj.html

Py:   @property 与 @x.setter
来源：http://hz.zhixingplan.top/gtcyhzydxo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yangfankeji.com/gtqzhdkmpf.html

JS:   get name() { return this._name; }
来源：http://hz.316326.xyz/gtbgvjjric.html

TS:   get name(): string { return this._name; }
来源：http://hz.guowangkeji.top/gtsogrxibk.html

Java: public String getName() { return name; }
来源：http://hz.hammf.cn/gtqzobyuwz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.cashguo.top/gtxmwkmwip.html

Ruby: attr_accessor :name
来源：http://hz.nanxinkj.top/gtgbwsbnhk.html

C#:   public string Name { get; set; }
来源：http://hz.zhongyouzk.top/gtnfxwyoft.html

[G12] 对象转字符串
来源：http://hz.tianlin.xyz/gthodayqdu.html

Py:   def __str__(self): return self.name
来源：http://hz.sufxvd.cn/gttdunvkff.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jyoumei.cn/gtdjshuhao.html

JS:   toString() { return this.name; }
来源：http://hz.jqgfzy.top/gtfoqdztvv.html

TS:   toString(): string { return this.name; }
来源：http://hz.sxryk.cn/gtrdljedqt.html

Java: @Override public String toString() { return name; }
来源：http://hz.tanke756.top/gtgxnsieze.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yongpay.top/gtlpxwhhdj.html

Ruby: def to_s; @name; end
来源：http://hz.xinyue.icu/gtafbpdiur.html

C#:   public override string ToString() => Name;
来源：http://hz.ivvv.top/gtevehtztl.html

[G13] 判断对象类型
来源：http://hz.haohaochexian.top/gthuknkbjb.html

Py:   isinstance(u, User)
来源：http://hz.chenjidiqi.icu/gthdvgkuls.html

PHP:  $u instanceof User
来源：http://hz.tian-w.cn/gthdkrjjtc.html

JS:   u instanceof User
来源：http://hz.wangdashe.top/gtuusfokec.html

TS:   u instanceof User
来源：http://hz.vqdsnc.cn/gtjrhcnfug.html

Java: u instanceof User
来源：http://hz.shuidangran.top/gthpmyhbbv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ppjwa.cn/gtadnkllij.html

Ruby: u.is_a?(User)
来源：http://hz.yj20258.top/gtqvftjwfp.html

C#:   u is User
来源：http://hz.yongpay.top/gtxbvwsurf.html

[G14] 数据类 / record
来源：http://hz.yj20258.top/gtiowjknnl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.shanyushiyangtech.top/gtqftzedgh.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.shangyingyoupin.top/gthfdllutc.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yj20258888.top/gtuorczwxb.html

TS:   type User = { name: string; age: number };
来源：http://hz.jqgfzy.top/gtffiiupun.html

Java: record User(String name, int age) {}
来源：http://hz.wangdashe.top/gtwhwoagkn.html

Go:   type User struct { Name string; Age int }
来源：http://hz.wangdashe.top/gtordrknfq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.wangshuangyany.cn/gtjpmdqinz.html

C#:   record User(string Name, int Age);
来源：http://hz.yvedp.cn/gtkfjcojiw.html

[G15] 枚举
来源：http://hz.chenlongwang.top/gtohivabmw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.sufxvd.cn/gtwdhgbggc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.52xcode.cn/gtgspovrla.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.ehwqpu.com/gtyqhaipba.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.kuanghao11.cn/gthqmbjcid.html

Java: enum Color { RED, GREEN }
来源：http://hz.cdnleiting.top/gtasxsxjck.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ehwqpu.com/gtlcwrwuss.html

Ruby: Color = %i[red green].freeze
来源：http://hz.tian-w.cn/gtbcxtmjqb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jyoumei.cn/gtsvvgippz.html

[G16] 对象转数组 / 字典
来源：http://hz.andypj.xyz/gtanqwqaso.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.gzhubu.top/gtjjclqaol.html

PHP:  get_object_vars($obj);
来源：http://hz.hammf.cn/gtwqdrxgpb.html

JS:   Object.entries(obj)
来源：http://hz.redwolf501.top/gtunzefxfu.html

TS:   Object.entries(obj)
来源：http://hz.0kj1m.cn/gtgxswcyep.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jqgfzy.top/gtcfbscwmg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.shanyushiyangkeji.top/gtwxibyuuh.html

Ruby: obj.instance_variables
来源：http://hz.tian-w.cn/gtyzrnpidy.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.haohaochexian.top/gtpwnmvuiu.html

================================================================================
来源：http://hz.hfpthk.cn/gtraqtjhja.html

H. 异常与错误处理
来源：http://hz.jinqigufen.top/gtqefqjacx.html

================================================================================
来源：http://hz.gaohongyu789.top/gtnyrcyxjy.html

[H01] try / catch 基础
来源：http://hz.yj20258.top/gtpuufgesg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zdqjudy.top/gtshvkkyea.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.quarkkingdee.top/gtpymmslxc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.bjfxy.top/gtccehkxwt.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.pycfn.com/gtexuuoscf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.xuetiantiany.cn/gtkxlzlxzr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.sufxvd.cn/gtdsxklzmj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.dashuyun.cn/gtbxzflutm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.cucudq.cn/gtencbijdf.html

[H02] finally / ensure 收尾
来源：http://hz.feifeiyinyue.top/gtinvpfxah.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.pengpengdd.cyou/gtkerxgwca.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hysaishi.cn/gtnfrykuzg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yueranfly.top/gttgniynmu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yongpay.top/gtspmilvsa.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.fzhhl.top/gtxbagctuk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zhaomingkeji.xyz/gtvqonytav.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.fengsongda.top/gtreddegvw.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yuanzhike.top/gthtisolio.html

[H03] 主动抛出异常
来源：http://hz.hywenlv.cn/gtgysvjllh.html

Py:   raise ValueError("错误信息")
来源：http://hz.jyoumei.cn/gtoihrwfir.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.gzhubu.top/gtbcasffuk.html

JS:   throw new Error("错误信息");
来源：http://hz.snrcjt.cn/gtjdvilryf.html

TS:   throw new Error("错误信息");
来源：http://hz.shzxlz.cn/gtjonhnkuz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.tianlin.xyz/gtulafteqs.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.sysykeji.top/gttnqolure.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.mhx1999.top/gtvbavlhek.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.tian-w.cn/gthrichbky.html

[H04] 自定义异常类型
来源：http://hz.chenjidiqi.icu/gthkststim.html

Py:   class MyError(Exception): pass
来源：http://hz.chenjidiqi.icu/gtqqxurepn.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.tanke756.top/gtwhtxmvxj.html

JS:   class MyError extends Error {}
来源：http://hz.ybcxt.top/gtimfllyar.html

TS:   class MyError extends Error {}
来源：http://hz.nanxinkj.top/gthhveoxip.html

Java: class MyException extends RuntimeException {}
来源：http://hz.ydjk.org.cn/gtejsguque.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jianghu66.top/gtdhkgsjzs.html

Ruby: class MyError < StandardError; end
来源：http://hz.jyoumei.cn/gtzqddgajd.html

C#:   class MyException : Exception {}
来源：http://hz.xinyue.icu/gtcwdpzwkj.html

[H05] 捕获特定类型
来源：http://hz.havefunace.top/gtbxfpruto.html

Py:   except ValueError as e:
来源：http://hz.hysaishi.cn/gtddejlgvd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.aizwys.cn/gtvxgfgyfj.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.wangshuangyany.cn/gtyjwzitls.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.dianchejie.cn/gtloftxeqi.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.hongshengwenyu.top/gtpcqsuefq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.chenzaomai.com/gttaqbabww.html

Ruby: rescue ArgumentError => e
来源：http://hz.bjfxy.top/gtpwqindlp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhoulong.xyz/gtwmvmrfbl.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yanxiufei.cn/gtkcazppzw.html

Py:   value = d.get("k") or default
来源：http://hz.xylfe.cn/gtilkybuuv.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.daria6918.cn/gtndedwmvn.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zdqjudy.top/gtqzjckjcj.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jqgfzy.top/gtulfaffzk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yonumen.top/gtphuejhoj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.xziqi.cn/gtecjizzsa.html

Ruby: d&.dig(:a, :b)
来源：http://hz.gzhubu.top/gtubayfdyy.html

C#:   obj?.A?.B ?? default
来源：http://hz.meibo888.top/gtzifloyit.html

[H07] 断言
来源：http://hz.chenjidiqi.icu/gtrqpycpjc.html

Py:   assert x > 0, "必须为正"
来源：http://hz.fengsongda.top/gtcauzhceb.html

PHP:  assert($x > 0);
来源：http://hz.gaohongyu789.top/gtxbzwdtki.html

JS:   console.assert(x > 0);
来源：http://hz.ppjwa.cn/gtxpqsmqdj.html

TS:   console.assert(x > 0);
来源：http://hz.jyoumei.cn/gtsdoidyme.html

Java: assert x > 0 : "必须为正";
来源：http://hz.sweek.top/gtghzhhzem.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ehwqpu.com/gtywzucfwz.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.shzxlz.cn/gtwqszppra.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jyoumei.cn/gtkrdwsixg.html

[H08] 获取错误信息与堆栈
来源：http://hz.yangfankeji.com/gtkmpsfequ.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yanxiufei.cn/gthkcoyrse.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.birdmap.top/gtpgjfpxqs.html

JS:   e.message;  e.stack
来源：http://hz.shzxlz.cn/gtkvurhksy.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jiagoushi.top/gtvlktcsar.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jqgfzy.top/gtvbmnaypb.html

Go:   err.Error()
来源：http://hz.yangfankeji.com/gthloanjbo.html


<!-- 参考信息 -->