代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.kuanghao11.cn/gtincryseg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.svipenyu.cn/gtkdxwilnz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jqgfzy.top/gtxcejjtqn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.nanxinkj.top/gttpxyexyz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.dianchejie.cn/gtevgojtqh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zhaomingkeji.xyz/gtfpctwcpc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.hysaishi.cn/gthbxkumsn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.smart0.xyz/gtfbxigkqf.html

[F05] 判断文件或目录是否存在
来源：http://hz.chenlongwang.top/gthpwcdsbh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.hysaishi.cn/gtmhgawasn.html

PHP:  file_exists("a.txt");
来源：http://hz.yonumen.top/gtcxgnrnat.html

JS:   fs.existsSync("a.txt")
来源：http://hz.shzxlz.cn/gttygrhpbw.html

TS:   fs.existsSync("a.txt")
来源：http://hz.ivvv.top/gtswpxwypb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.ppjwa.cn/gtsvlvjdkh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ppjwa.cn/gtsyqlmfzh.html

Ruby: File.exist?("a.txt")
来源：http://hz.haohaochexian.top/gthlkyeqqg.html

C#:   File.Exists("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtokxueocd.html

[F06] 删除文件
来源：http://hz.zhengqikj.top/gtlngotlqn.html

Py:   os.remove("a.txt")
来源：http://hz.bjfxy.top/gtwuwscczh.html

PHP:  unlink("a.txt");
来源：http://hz.jqgfzy.top/gtpqljskbt.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hnqzz.top/gtpxybbhcv.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.cqqwz.cn/gtahfbijne.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.smart0.xyz/gtqderaqmu.html

Go:   os.Remove("a.txt")
来源：http://hz.meibo888.top/gtrbbvzppc.html

Ruby: File.delete("a.txt")
来源：http://hz.jinqigufen.top/gtfnqmljgr.html

C#:   File.Delete("a.txt");
来源：http://hz.yongpay.top/gtehemdvju.html

[F07] 创建目录（含多级）
来源：http://hz.xuetiantiany.cn/gtmqbsjcer.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.cheryme.top/gtczwbnhra.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.kuanghao11.cn/gtcbivypsl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.chenjidiqi.icu/gtouwzjbpx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zycfv.cn/gtypjiktwq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.shuidangran.top/gtwdkqtuog.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.fzhhl.top/gtqxltdihz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.sweek.top/gtrdtxtmed.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.tianlin.xyz/gtlyrxetfz.html

[F08] 遍历目录
来源：http://hz.kuanghao11.cn/gtawnwnabi.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zhixingplan.top/gtxnomrhio.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jinqigfzy.top/gtegkpxiwa.html

JS:   fs.readdirSync("dir")
来源：http://hz.zhengqikj.top/gtnmcprtod.html

TS:   fs.readdirSync("dir")
来源：http://hz.jianghu66.top/gtbgclytdg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zhaomingkeji.xyz/gthjcnprps.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zhijiandao.cn/gtevihqsiq.html

Ruby: Dir.children("dir")
来源：http://hz.shzxlz.cn/gtuptqgnvd.html

C#:   Directory.GetFiles("dir")
来源：http://hz.52xcode.cn/gtpzvtequo.html

[F09] 获取文件大小
来源：http://hz.snrcjt.cn/gtmafgenor.html

Py:   os.path.getsize("a.txt")
来源：http://hz.hnxiangtu.top/gtoabwcvsw.html

PHP:  filesize("a.txt");
来源：http://hz.pycfn.com/gtskqtypug.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zdqjudy.top/gthmlyxxhh.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yj20258.top/gtmprjuwpa.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.hfpthk.cn/gtcenxmsmj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.daxiang520.top/gtuxawupov.html

Ruby: File.size("a.txt")
来源：http://hz.zhiwuduotai.top/gtgpgdgwgu.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.cheryme.top/gtfkelsijc.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.wangshuangyany.cn/gtmqevwexe.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jqgufenzy.top/gtikrafkgh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.gzhubu.top/gtvpxdjimx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.gzhubu.top/gtgcecricq.html

TS:   path.extname("a.txt")
来源：http://hz.gaohongyu789.top/gttqdedseg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.shanyushiyangkeji.top/gtmgtswzaj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jianghu66.top/gtfdskecvz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhiwuduotai.top/gtpczyteul.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yj20258.top/gttokbazaa.html

[F11] 复制与移动文件
来源：http://hz.snrcjt.cn/gtpglffeuq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.ppjwa.cn/gtyrrmhlvd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zhoulong.xyz/gtnpjjbjvg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.kuanghao11.cn/gthcpakjni.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.mhx1999.top/gtgcbrmuyn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.smart0.xyz/gtzcspjind.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.zhengqikj.top/gtmwewmbpn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.xinyue.icu/gtvcpvcbpa.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yuanzhike.top/gtchuhorzh.html

[F12] CSV 读写
来源：http://hz.yangfankeji.com/gtbxkcuqcb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xuetiantiany.cn/gtygwkzcpx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.gotoacloud.top/gtvisnznpe.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.shangyingyoupin.top/gtpfiwtatc.html

TS:   // 同上
来源：http://hz.andypj.xyz/gtklmrucew.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ydzc1.top/gtmsavzrie.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.hnqzz.top/gtxituyyzt.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ivvv.top/gtnrsuyudi.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.ppjwa.cn/gtmurmqveb.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gticqhmflw.html

G. 面向对象
来源：http://hz.daria6918.cn/gtrravcriu.html

================================================================================
来源：http://hz.smart0.xyz/gtzfhsdbhh.html

[G01] 定义类
来源：http://hz.316326.xyz/gtxxdugkrx.html

Py:   class User: pass
来源：http://hz.nanxuanxn.top/gteiwkjazm.html

PHP:  class User {}
来源：http://hz.feifeiyinyue.top/gtovwxatfj.html

JS:   class User {}
来源：http://hz.andypj.xyz/gtyjaoezth.html

TS:   class User { name: string = ""; }
来源：http://hz.tianlin.xyz/gtonzjjacb.html

Java: class User {}
来源：http://hz.ppjwa.cn/gtcliulqdl.html

Go:   type User struct { Name string }
来源：http://hz.kuanghao11.cn/gtdaddnnzr.html

Ruby: class User; end
来源：http://hz.yueranfly.top/gtbnasplbf.html

C#:   class User {}
来源：http://hz.ehwqpu.com/gturmazjqx.html

[G02] 构造函数
来源：http://hz.xuetiantiany.cn/gtawnhqglb.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jinghuilouyu.cn/gtzjllslbx.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hywenlv.cn/gtsmtnlcnm.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.wangshuangyany.cn/gtszjbqnve.html

TS:   constructor(public name: string) {}
来源：http://hz.ydjk.org.cn/gtwbuoqujr.html

Java: User(String name) { this.name = name; }
来源：http://hz.zhoulong.xyz/gtoumqkkzj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.bjfxy.top/gtktfpolyl.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.shzxlz.cn/gtdugbnrjo.html

C#:   public User(string name) { Name = name; }
来源：http://hz.shanyushiyangtech.top/gtupmiyvar.html

[G03] 实例属性
来源：http://hz.shangyingyoupin.top/gtnvmzrfsp.html

Py:   self.name = "x"
来源：http://hz.iojbl.cn/gtsnaqlcqc.html

PHP:  public string $name = "x";
来源：http://hz.aizwys.cn/gtqwzgzexa.html

JS:   this.name = "x";
来源：http://hz.guannengcc.top/gtpshtgrfi.html

TS:   name: string = "x";
来源：http://hz.feifeiyinyue.top/gtknpqojvj.html

Java: private String name;
来源：http://hz.ywan-chungtsiang.top/gtiotqaqnb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.smart0.xyz/gtqorxozts.html

Ruby: @name = "x"
来源：http://hz.chenlongwang.top/gtytfcszum.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.birdmap.top/gtqwexkebl.html

[G04] 定义方法
来源：http://hz.daxiang520.top/gtiluqycyf.html

Py:   def greet(self): return self.name
来源：http://hz.yj202588.top/gtocfrbdad.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.gaohongyu789.top/gtookkuvyj.html

JS:   greet() { return this.name; }
来源：http://hz.sxryk.cn/gtxwmvffaq.html

TS:   greet(): string { return this.name; }
来源：http://hz.vqdsnc.cn/gtyyxhkcea.html

Java: String greet() { return name; }
来源：http://hz.cucudq.cn/gtcbgcasxb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zhixingplan.top/gtgmcxgdyq.html

Ruby: def greet; @name; end
来源：http://hz.zhengqikj.top/gtkqkswqrn.html

C#:   public string Greet() => Name;
来源：http://hz.yvedp.cn/gtqakytmty.html

[G05] 继承
来源：http://hz.wangshuangyany.cn/gtihyyvcjn.html

Py:   class Admin(User): pass
来源：http://hz.yangfankeji.com/gtxiiqejbk.html

PHP:  class Admin extends User {}
来源：http://hz.havefunace.top/gtemyhpawc.html

JS:   class Admin extends User {}
来源：http://hz.kuanghao11.cn/gtdgioieuh.html

TS:   class Admin extends User {}
来源：http://hz.sufxvd.cn/gtnaxyohyx.html

Java: class Admin extends User {}
来源：http://hz.yonumen.top/gtyczmukwy.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zhongyouzk.top/gtnpbnyhfq.html

Ruby: class Admin < User; end
来源：http://hz.ydjk.org.cn/gtfjishpgv.html

C#:   class Admin : User {}
来源：http://hz.jinghuilouyu.cn/gtxehapawk.html

[G06] 重写方法
来源：http://hz.sweek.top/gtzpbilggc.html

Py:   def greet(self): return "admin"
来源：http://hz.sxryk.cn/gtjekvelio.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.quarkkingdee.top/gtmuqospva.html

JS:   greet() { return "admin"; }
来源：http://hz.yongpay.top/gtujqjmmte.html

TS:   greet(): string { return "admin"; }
来源：http://hz.dianchejie.cn/gtqigwongg.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jianghu66.top/gtgqsdandy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.iojbl.cn/gtgsqjzqwb.html

Ruby: def greet; "admin"; end
来源：http://hz.daxiang520.top/gtzikranzs.html

C#:   public override string Greet() => "admin";
来源：http://hz.tian-w.cn/gtxwttogfu.html

[G07] 调用父类方法
来源：http://hz.yvedp.cn/gtxzvzymgv.html

Py:   super().greet()
来源：http://hz.iojbl.cn/gtafrwvpko.html

PHP:  parent::greet();
来源：http://hz.aizwys.cn/gtfecuvaqg.html

JS:   super.greet();
来源：http://hz.shanyushiyangkeji.top/gtvvrrepql.html

TS:   super.greet();
来源：http://hz.iojbl.cn/gtrcyzgwgt.html

Java: super.greet();
来源：http://hz.fzhhl.top/gtqybhgoru.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.daxiang520.top/gtydnxzzth.html

Ruby: super
来源：http://hz.yvedp.cn/gtszdilbzn.html

C#:   base.Greet();
来源：http://hz.wangshuangyany.cn/gthvlevnqu.html

[G08] 静态方法与属性
来源：http://hz.mhx1999.top/gtklbjddcl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.xinyue.icu/gtjutykvge.html

PHP:  public static function f() {}
来源：http://hz.ehwqpu.com/gtbxtjsnxn.html

JS:   static f() {}
来源：http://hz.yongpay.top/gtsacpezub.html

TS:   static f(): void {}
来源：http://hz.vqdsnc.cn/gtoucqgqci.html

Java: static void f() {}
来源：http://hz.9152youxi.cn/gtbncqzwom.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.52xcode.cn/gtjkwbdvrh.html

Ruby: def self.f; end
来源：http://hz.zhaomingkeji.xyz/gtykodjewb.html

C#:   public static void F() {}
来源：http://hz.jinqigfzy.top/gtccqvcnyh.html

[G09] 接口 / 抽象类
来源：http://hz.iojbl.cn/gtgpdssvof.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.shzxlz.cn/gtuaqvffzw.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ybcxt.top/gtidvllzkl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.tanke756.top/gtdrofyzig.html

TS:   interface Shape { area(): number; }
来源：http://hz.hammf.cn/gtxmhdpmkw.html

Java: interface Shape { double area(); }
来源：http://hz.zhongyouzk.top/gtrdgftwck.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yuxming.cn/gtbolnfhqu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.xingfuxueyuan.xyz/gtywfostvy.html

C#:   interface IShape { double Area(); }
来源：http://hz.ydjk.org.cn/gtkltiixoq.html

[G10] 访问控制
来源：http://hz.c1oappe.top/gtmdzrhtnf.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.ydjk.org.cn/gtlesqqdkw.html

PHP:  public / protected / private
来源：http://hz.c1oappe.top/gtuslxtrmu.html

JS:   #private 字段；其余公开
来源：http://hz.aibaodan.cn/gtnzvctzme.html

TS:   public / protected / private
来源：http://hz.0kj1m.cn/gtdbgecyux.html

Java: public / protected / private / 默认包级
来源：http://hz.wangshuangyany.cn/gteteketzg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.gzhubu.top/gtlicsmsme.html

Ruby: public / protected / private
来源：http://hz.hfpthk.cn/gtxjygewnt.html

C#:   public / protected / private / internal
来源：http://hz.haohaochexian.top/gtoajqsuox.html

[G11] getter / setter
来源：http://hz.c1oappe.top/gtrxtlbqsl.html

Py:   @property 与 @x.setter
来源：http://hz.hfpthk.cn/gtfwssbgaq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.snrcjt.cn/gtyunbzsoo.html

JS:   get name() { return this._name; }
来源：http://hz.gzhubu.top/gtvbeohydr.html

TS:   get name(): string { return this._name; }
来源：http://hz.daria6918.cn/gtcreelcgr.html

Java: public String getName() { return name; }
来源：http://hz.tian-w.cn/gtzvzfhoon.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.cucudq.cn/gtamaqlnll.html

Ruby: attr_accessor :name
来源：http://hz.ydzc1.top/gtcqtbapea.html

C#:   public string Name { get; set; }
来源：http://hz.shzxlz.cn/gtqwfrsgfo.html

[G12] 对象转字符串
来源：http://hz.yuxming.cn/gttfswqisc.html

Py:   def __str__(self): return self.name
来源：http://hz.havefunace.top/gtvaebquad.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.xylfe.cn/gtvbtlcnuz.html

JS:   toString() { return this.name; }
来源：http://hz.hnxiangtu.top/gtfbrhebvp.html

TS:   toString(): string { return this.name; }
来源：http://hz.jinyuanbaomall.cn/gtgyxuwxrw.html

Java: @Override public String toString() { return name; }
来源：http://hz.zhaomingkeji.xyz/gtedlubfxs.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.chenjidiqi.icu/gtutjpyxhl.html

Ruby: def to_s; @name; end
来源：http://hz.gogol.net.cn/gtwqwoiash.html

C#:   public override string ToString() => Name;
来源：http://hz.hammf.cn/gtdeuzmaue.html

[G13] 判断对象类型
来源：http://hz.gotoacloud.top/gtkgogtobf.html

Py:   isinstance(u, User)
来源：http://hz.vqdsnc.cn/gtcbkntqts.html

PHP:  $u instanceof User
来源：http://hz.havefunace.top/gtrlengupy.html

JS:   u instanceof User
来源：http://hz.jqgufenzy.top/gtcqdjzpbl.html

TS:   u instanceof User
来源：http://hz.9152youxi.cn/gttnruscvl.html

Java: u instanceof User
来源：http://hz.wangshuangyany.cn/gtcjaifirc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.wangshuangyany.cn/gtgxrkeyvw.html

Ruby: u.is_a?(User)
来源：http://hz.guannengcc.top/gtyaoqidfv.html

C#:   u is User
来源：http://hz.jlsjyb.cn/gthfthhufs.html

[G14] 数据类 / record
来源：http://hz.zhixingplan.top/gtxtkyinpm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.ydjk.org.cn/gtrmxsfise.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yuxming.cn/gteyhaviae.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.nanxuanxn.top/gtnscsbjzf.html

TS:   type User = { name: string; age: number };
来源：http://hz.zhengqikj.top/gtzgxwyzeo.html

Java: record User(String name, int age) {}
来源：http://hz.jinqigfzy.top/gtcpafqnfs.html

Go:   type User struct { Name string; Age int }
来源：http://hz.xziqi.cn/gthparhfju.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.kuanghao11.cn/gthosttuye.html

C#:   record User(string Name, int Age);
来源：http://hz.jinqigfzy.top/gtiisiwjbk.html

[G15] 枚举
来源：http://hz.52xcode.cn/gtmbtwwnnz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.ybcxt.top/gtgvglzmfx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.shanyushiyangkeji.top/gtvygbeuws.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yuanzhike.top/gthzorcsvy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.dashuyun.cn/gtoanaddsp.html

Java: enum Color { RED, GREEN }
来源：http://hz.jinqigufen.top/gtzzlyjfsq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.gotoacloud.top/gtonguauus.html

Ruby: Color = %i[red green].freeze
来源：http://hz.pengpengdd.cyou/gttcekkaqx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yuanzhike.top/gtozrefiso.html

[G16] 对象转数组 / 字典
来源：http://hz.nanxinkj.top/gtprtylura.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.nwbrower.top/gtivhawkvl.html

PHP:  get_object_vars($obj);
来源：http://hz.dianchejie.cn/gtxtiwdkdu.html

JS:   Object.entries(obj)
来源：http://hz.hfpthk.cn/gtayactail.html

TS:   Object.entries(obj)
来源：http://hz.aibaodan.cn/gtgzazdroo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zycfv.cn/gtooybclsr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.tian-w.cn/gttwoyyjgr.html

Ruby: obj.instance_variables
来源：http://hz.vqdsnc.cn/gtlqeqvltv.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.hysaishi.cn/gthcbuhmtb.html

================================================================================
来源：http://hz.52xcode.cn/gtukaegsne.html

H. 异常与错误处理
来源：http://hz.9152youxi.cn/gtqqqjhzml.html

================================================================================
来源：http://hz.c1oappe.top/gtiaobrhyz.html

[H01] try / catch 基础
来源：http://hz.xingfuxueyuan.xyz/gtyucuqzjg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yueranfly.top/gtsnehklxp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.gaohongyu789.top/gtweevzmvu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.xingfuxueyuan.xyz/gtjerbpnad.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.aibaodan.cn/gtrtzixkjr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.wangdashe.top/gtylorxmek.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jiagoushi.top/gtfwiafjjn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.vqdsnc.cn/gthitkzaox.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhongyouzk.top/gtaolfwltn.html

[H02] finally / ensure 收尾
来源：http://hz.sweek.top/gtsefezylp.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.sweek.top/gtucwywlup.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.ydzc1.top/gtaxvwwyrc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhiwuduotai.top/gtpacqnpcx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.cucudq.cn/gtnlbcwcii.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.gaohongyu789.top/gtkuknratj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jinghuilouyu.cn/gtwadxwoye.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ppjwa.cn/gthohygljl.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.dashuyun.cn/gttgulnyui.html

[H03] 主动抛出异常
来源：http://hz.guannengcc.top/gtmzsechtp.html

Py:   raise ValueError("错误信息")
来源：http://hz.shuidangran.top/gtiupgxgvl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.gotoacloud.top/gtqgcayvwl.html

JS:   throw new Error("错误信息");
来源：http://hz.ybcxt.top/gtyrsiuhpa.html

TS:   throw new Error("错误信息");
来源：http://hz.birdmap.top/gtjjpzgndj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.cucudq.cn/gtdbqhkmny.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.xylfe.cn/gtpjfzuikm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.sysykeji.top/gtirbypfso.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jinyuanbaomall.cn/gtcilxywtl.html

[H04] 自定义异常类型
来源：http://hz.jiagoushi.top/gtlokyqzzm.html

Py:   class MyError(Exception): pass
来源：http://hz.dashuyun.cn/gtwveyyfpu.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.vqdsnc.cn/gtdkssaswe.html

JS:   class MyError extends Error {}
来源：http://hz.wangshuangyany.cn/gtglzlzhng.html

TS:   class MyError extends Error {}
来源：http://hz.shanyushiyangtech.top/gtyujqbejt.html

Java: class MyException extends RuntimeException {}
来源：http://hz.ivvv.top/gtizvzfjid.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.dianchejie.cn/gtlaxvbprj.html

Ruby: class MyError < StandardError; end
来源：http://hz.ydjk.org.cn/gtpagaoweh.html

C#:   class MyException : Exception {}
来源：http://hz.shanyushiyangkeji.top/gtyqxiezzh.html

[H05] 捕获特定类型
来源：http://hz.c1oappe.top/gtibvjronh.html

Py:   except ValueError as e:
来源：http://hz.0kj1m.cn/gtmklwzuul.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.xuanzx.com/gtcsjsgnce.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.smart0.xyz/gtjjnztkmc.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.chenzaomai.com/gtzhgmdrpf.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.vqdsnc.cn/gtiftgyjkx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.birdmap.top/gtdbofqwjo.html

Ruby: rescue ArgumentError => e
来源：http://hz.tian-w.cn/gtobzzicly.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.pengpengdd.cyou/gtwutglbbo.html

[H06] 可选值 / 空值安全访问
来源：http://hz.gaohongyu789.top/gtkininxqd.html

Py:   value = d.get("k") or default
来源：http://hz.sxryk.cn/gtifkupjzr.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.xinyue.icu/gtcpzrdcwd.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yj20258.top/gtrbmfxpxe.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zhiwuduotai.top/gthkpldxbe.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.aibaodan.cn/gtnkbovmxj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yvedp.cn/gtvucxgzqz.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhijiandao.cn/gtvswaswod.html

C#:   obj?.A?.B ?? default
来源：http://hz.svipenyu.cn/gtrmvumqtq.html

[H07] 断言
来源：http://hz.shzxlz.cn/gtuazubcoq.html

Py:   assert x > 0, "必须为正"
来源：http://hz.xingfuxueyuan.xyz/gtpgzdhjfs.html

PHP:  assert($x > 0);
来源：http://hz.shanyushiyangtech.top/gtxyjzxghd.html

JS:   console.assert(x > 0);
来源：http://hz.cheryme.top/gtnnpujgig.html

TS:   console.assert(x > 0);
来源：http://hz.hywenlv.cn/gtscciedav.html

Java: assert x > 0 : "必须为正";
来源：http://hz.vqdsnc.cn/gtkozghege.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.haohaochexian.top/gtwyoyhsbm.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.chenjidiqi.icu/gtoxeidefr.html

C#:   Debug.Assert(x > 0);
来源：http://hz.dianchejie.cn/gtupxlyiiq.html

[H08] 获取错误信息与堆栈
来源：http://hz.shzxlz.cn/gtxryocjez.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.316326.xyz/gtqweyzxqt.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.smart0.xyz/gtpplqdjuh.html

JS:   e.message;  e.stack
来源：http://hz.sufxvd.cn/gtcugfoprg.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yueranfly.top/gtfojvrfwr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.gaohongyu789.top/gtrckbmsth.html

Go:   err.Error()
来源：http://hz.jyoumei.cn/gtgtickkvg.html


<!-- 参考信息 -->