代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.nwbrower.top/gtduazogfd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yj20258.top/gtaqixphty.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yangfankeji.com/gtbaqpcwps.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zhijiandao.cn/gtokqxwift.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.haohaochexian.top/gtnvzhfgqh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.pengpengdd.cyou/gtzvivebfs.html

[F03] 写入文件（覆盖）
来源：http://hz.jlsjyb.cn/gttexihzyq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hnxiangtu.top/gtpjewiksw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.meibo888.top/gtteeasdyc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.guowangkeji.top/gtzkorhfid.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yangfankeji.com/gtbgbsdrkq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.hongshengwenyu.top/gtprrcxrcq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.svipenyu.cn/gtxhebaeii.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.xingfuxueyuan.xyz/gtqfchwrkw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yongpay.top/gtokdvxovw.html

[F04] 追加写入文件
来源：http://hz.zycfv.cn/gtvfmvtkfo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.xylfe.cn/gtayqvwzxg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.snrcjt.cn/gtjjvtdnbt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xinyue.icu/gtwqudtufw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhixingplan.top/gtocqzuvgv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.52xcode.cn/gtdfcdzeqy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.ehwqpu.com/gtvkppskdl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.dashuyun.cn/gtisetxmfs.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yangfankeji.com/gtmjzfckdm.html

[F05] 判断文件或目录是否存在
来源：http://hz.nwbrower.top/gtsluzeedc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.svipenyu.cn/gtneqrzsom.html

PHP:  file_exists("a.txt");
来源：http://hz.hysaishi.cn/gtpohvxetw.html

JS:   fs.existsSync("a.txt")
来源：http://hz.c1oappe.top/gtxtezhqdv.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yangfankeji.com/gtuxqjsvhq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.chenjidiqi.icu/gttuisqgxg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yj202588.top/gthfecgkwp.html

Ruby: File.exist?("a.txt")
来源：http://hz.nanxinkj.top/gtofwvdkhw.html

C#:   File.Exists("a.txt")
来源：http://hz.jinqigufen.top/gtgmltxnid.html

[F06] 删除文件
来源：http://hz.ywan-chungtsiang.top/gtrwldeggy.html

Py:   os.remove("a.txt")
来源：http://hz.cheryme.top/gtydlpvpkn.html

PHP:  unlink("a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtkloncpls.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.haohaochexian.top/gtclvltdgu.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jinqigfzy.top/gtnkblxkgj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.nwbrower.top/gtqssdqbiq.html

Go:   os.Remove("a.txt")
来源：http://hz.zhengqikj.top/gtcmppnmnw.html

Ruby: File.delete("a.txt")
来源：http://hz.cashguo.top/gtashecxro.html

C#:   File.Delete("a.txt");
来源：http://hz.yj202588.top/gtqvzwacus.html

[F07] 创建目录（含多级）
来源：http://hz.haohaochexian.top/gtzziroura.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.xuetiantiany.cn/gtvgtzwymn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.ydzc1.top/gtfekdfbiu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ivvv.top/gtaxnwpuzv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xinyue.icu/gtglfcclha.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.guowangkeji.top/gtbcttamul.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yonumen.top/gtnxsjcmbk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.dashuyun.cn/gttbqhvdas.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.dianchejie.cn/gtbcpxbzjd.html

[F08] 遍历目录
来源：http://hz.9152youxi.cn/gtftkqbltg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.birdmap.top/gtdgcokvcq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.mhx1999.top/gtefiwlzqa.html

JS:   fs.readdirSync("dir")
来源：http://hz.fengsongda.top/gtfpfkquon.html

TS:   fs.readdirSync("dir")
来源：http://hz.cheryme.top/gtafflgjeo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.chenjidiqi.icu/gtanbpqdho.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.pycfn.com/gtiimpsogg.html

Ruby: Dir.children("dir")
来源：http://hz.jinghuilouyu.cn/gtjpeutyuy.html

C#:   Directory.GetFiles("dir")
来源：http://hz.svipenyu.cn/gtnvahotev.html

[F09] 获取文件大小
来源：http://hz.yangfankeji.com/gtpxshmsix.html

Py:   os.path.getsize("a.txt")
来源：http://hz.gogol.net.cn/gtodytloiz.html

PHP:  filesize("a.txt");
来源：http://hz.cqqwz.cn/gtsewjcuza.html

JS:   fs.statSync("a.txt").size
来源：http://hz.gzhubu.top/gttuuoktwb.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zdqjudy.top/gtjevibwfm.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yj20258.top/gttmyjtmve.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yj20258888.top/gtujxqxdbb.html

Ruby: File.size("a.txt")
来源：http://hz.guowangkeji.top/gtgjufaymj.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.gzhubu.top/gtlhfaixzw.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.shanyushiyangkeji.top/gtbdcehivc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jlsjyb.cn/gtmfzlxkmr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.daria6918.cn/gthlgurrsv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yj20258.top/gtvsqpfwwz.html

TS:   path.extname("a.txt")
来源：http://hz.haohaochexian.top/gtuqmhzkxg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yangfankeji.com/gtfuiclyay.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zhixingplan.top/gthnmipspm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhixingplan.top/gteqbvfzsr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yongpay.top/gtqazicaym.html

[F11] 复制与移动文件
来源：http://hz.redwolf501.top/gtevvhxjby.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.dianchejie.cn/gtzmhvgqzl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.dashuyun.cn/gtwcxcfhwb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.0kj1m.cn/gtzxssyypo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yongpay.top/gtzuvnujbl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jinyuanbaomall.cn/gtiuwnhsqo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jinghuilouyu.cn/gtlujmspuq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jinghuilouyu.cn/gtwhcyspqs.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.smart0.xyz/gtrticfnjp.html

[F12] CSV 读写
来源：http://hz.gotoacloud.top/gtqsctcvmv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.bjfxy.top/gtyecjqlxi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.xingfuxueyuan.xyz/gtphcikzqf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.gzhubu.top/gthpdghemj.html

TS:   // 同上
来源：http://hz.chenzaomai.com/gtwblrtqnr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.tanke756.top/gtuiapliye.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.chenlongwang.top/gtzymkzhxt.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.mhx1999.top/gtsgwawbrt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.shanyushiyangtech.top/gtqqtghfnj.html

================================================================================
来源：http://hz.aibaodan.cn/gtevxrcino.html

G. 面向对象
来源：http://hz.snrcjt.cn/gtiiifxwyc.html

================================================================================
来源：http://hz.cheryme.top/gtobpbogqd.html

[G01] 定义类
来源：http://hz.jqgfzy.top/gtqcwgkzzn.html

Py:   class User: pass
来源：http://hz.zhaomingkeji.xyz/gtuevycgjk.html

PHP:  class User {}
来源：http://hz.jianghu66.top/gtodpfiryv.html

JS:   class User {}
来源：http://hz.shanyushiyangtech.top/gtpzuftvnd.html

TS:   class User { name: string = ""; }
来源：http://hz.wangshuangyany.cn/gthmqrskwp.html

Java: class User {}
来源：http://hz.gogol.net.cn/gtshyznlmx.html

Go:   type User struct { Name string }
来源：http://hz.guowangkeji.top/gtzykkuhvq.html

Ruby: class User; end
来源：http://hz.quarkkingdee.top/gtjonyeegx.html

C#:   class User {}
来源：http://hz.zhaomingkeji.xyz/gtwkixpsbh.html

[G02] 构造函数
来源：http://hz.ydjk.org.cn/gtlphomofb.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.gogol.net.cn/gtcygpxbly.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zhijiandao.cn/gtxcvsroel.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.cucudq.cn/gtqfkuernx.html

TS:   constructor(public name: string) {}
来源：http://hz.yuanzhike.top/gthinvswjy.html

Java: User(String name) { this.name = name; }
来源：http://hz.hysaishi.cn/gtzegaolwa.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jlsjyb.cn/gtxsysjypf.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.daria6918.cn/gtkijcmyqb.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yonumen.top/gtjqtrqyjy.html

[G03] 实例属性
来源：http://hz.wangdashe.top/gttmeydnzb.html

Py:   self.name = "x"
来源：http://hz.ydjk.org.cn/gthicvalqd.html

PHP:  public string $name = "x";
来源：http://hz.shangyingyoupin.top/gtscycdizv.html

JS:   this.name = "x";
来源：http://hz.redwolf501.top/gttbqussjz.html

TS:   name: string = "x";
来源：http://hz.tianlin.xyz/gtlnflzvkt.html

Java: private String name;
来源：http://hz.aibaodan.cn/gtfqyigrgx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.meibo888.top/gtkguxisso.html

Ruby: @name = "x"
来源：http://hz.yonumen.top/gtvsxvnqsv.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zhixingplan.top/gtgwhdvuhd.html

[G04] 定义方法
来源：http://hz.daria6918.cn/gtxxpqscdw.html

Py:   def greet(self): return self.name
来源：http://hz.smart0.xyz/gtznyxundw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.smart0.xyz/gtwcxzvase.html

JS:   greet() { return this.name; }
来源：http://hz.yj20258888.top/gtjpkkmqch.html

TS:   greet(): string { return this.name; }
来源：http://hz.andypj.xyz/gtmegnimab.html

Java: String greet() { return name; }
来源：http://hz.jlsjyb.cn/gtstlhivef.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jinqigufen.top/gtctsctffz.html

Ruby: def greet; @name; end
来源：http://hz.yuanzhike.top/gthvhdmhrb.html

C#:   public string Greet() => Name;
来源：http://hz.zhixingplan.top/gtqmnczvuk.html

[G05] 继承
来源：http://hz.aibaodan.cn/gtaswkgbci.html

Py:   class Admin(User): pass
来源：http://hz.zhijiandao.cn/gtddidxhmp.html

PHP:  class Admin extends User {}
来源：http://hz.tian-w.cn/gtryuhgnet.html

JS:   class Admin extends User {}
来源：http://hz.wangshuangyany.cn/gtssoyxciz.html

TS:   class Admin extends User {}
来源：http://hz.cheryme.top/gteorfrjxi.html

Java: class Admin extends User {}
来源：http://hz.aibaodan.cn/gtqfxemzci.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.kuanghao11.cn/gtbxfgnvmc.html

Ruby: class Admin < User; end
来源：http://hz.cheryme.top/gtukdoiiwm.html

C#:   class Admin : User {}
来源：http://hz.chenjidiqi.icu/gtdvwrvhhr.html

[G06] 重写方法
来源：http://hz.fzhhl.top/gtowalicoz.html

Py:   def greet(self): return "admin"
来源：http://hz.snrcjt.cn/gtjyfkauqe.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.hammf.cn/gtsbebzduh.html

JS:   greet() { return "admin"; }
来源：http://hz.shuidangran.top/gtimuqonqj.html

TS:   greet(): string { return "admin"; }
来源：http://hz.aibaodan.cn/gtghrhvdql.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.shanyushiyangtech.top/gtlhpkkgah.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.316326.xyz/gtrnlaeaxq.html

Ruby: def greet; "admin"; end
来源：http://hz.zhoulong.xyz/gtyzovffnd.html

C#:   public override string Greet() => "admin";
来源：http://hz.0kj1m.cn/gtodidsogk.html

[G07] 调用父类方法
来源：http://hz.yvedp.cn/gtsphkjupk.html

Py:   super().greet()
来源：http://hz.fengsongda.top/gtzqyjsxnv.html

PHP:  parent::greet();
来源：http://hz.daria6918.cn/gtmvhxbbap.html

JS:   super.greet();
来源：http://hz.ivvv.top/gtxeytptxm.html

TS:   super.greet();
来源：http://hz.52xcode.cn/gtqvaoijix.html

Java: super.greet();
来源：http://hz.zhoulong.xyz/gtkmaljvba.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.hywenlv.cn/gtjijgrsib.html

Ruby: super
来源：http://hz.shanyushiyangtech.top/gtzlrwicah.html

C#:   base.Greet();
来源：http://hz.wangdashe.top/gtjlergjpd.html

[G08] 静态方法与属性
来源：http://hz.guowangkeji.top/gtyftkuewg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.haohaochexian.top/gtxmpaebpe.html

PHP:  public static function f() {}
来源：http://hz.nwbrower.top/gtisltccpk.html

JS:   static f() {}
来源：http://hz.ppjwa.cn/gtwbzibbmz.html

TS:   static f(): void {}
来源：http://hz.ivvv.top/gtnldvyext.html

Java: static void f() {}
来源：http://hz.jqgfzy.top/gtgkugrhrk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.0kj1m.cn/gtlpntxsnu.html

Ruby: def self.f; end
来源：http://hz.jiagoushi.top/gtpllxamlc.html

C#:   public static void F() {}
来源：http://hz.xuanzx.com/gtbozqevwy.html

[G09] 接口 / 抽象类
来源：http://hz.yongpay.top/gthnxvhtne.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.shzxlz.cn/gtodcxnhbi.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.xuanzx.com/gtpiosqiio.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yuanzhike.top/gthkinfgfv.html

TS:   interface Shape { area(): number; }
来源：http://hz.wangdashe.top/gtkrkbjiwz.html

Java: interface Shape { double area(); }
来源：http://hz.cucudq.cn/gtlgauwome.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.52xcode.cn/gtmagerdfk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.kuanghao11.cn/gtqovbrwtr.html

C#:   interface IShape { double Area(); }
来源：http://hz.yueranfly.top/gthzgkbxlk.html

[G10] 访问控制
来源：http://hz.kuanghao11.cn/gtsphhbsvz.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.xingfuxueyuan.xyz/gtnifcmpvs.html

PHP:  public / protected / private
来源：http://hz.jlsjyb.cn/gtjereqhft.html

JS:   #private 字段；其余公开
来源：http://hz.xinyue.icu/gtdgvxpukb.html

TS:   public / protected / private
来源：http://hz.dianchejie.cn/gtdknktifs.html

Java: public / protected / private / 默认包级
来源：http://hz.xingfuxueyuan.xyz/gtpkycnrlp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.cheryme.top/gttdqooqol.html

Ruby: public / protected / private
来源：http://hz.redwolf501.top/gtlncropbo.html

C#:   public / protected / private / internal
来源：http://hz.hnxiangtu.top/gtshyhvlfb.html

[G11] getter / setter
来源：http://hz.ehwqpu.com/gtvhhmglmu.html

Py:   @property 与 @x.setter
来源：http://hz.yangfankeji.com/gttqrfltfn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.shuidangran.top/gtkufdjmjn.html

JS:   get name() { return this._name; }
来源：http://hz.cdnleiting.top/gtotdxppig.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhiwuduotai.top/gtkojtsgqw.html

Java: public String getName() { return name; }
来源：http://hz.hywenlv.cn/gtokzguzfd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.ppjwa.cn/gtivtfnwkc.html

Ruby: attr_accessor :name
来源：http://hz.sysykeji.top/gtydvgxkeu.html

C#:   public string Name { get; set; }
来源：http://hz.zhaomingkeji.xyz/gtmkikydnu.html

[G12] 对象转字符串
来源：http://hz.yueranfly.top/gtmzyfnibe.html

Py:   def __str__(self): return self.name
来源：http://hz.hnqzz.top/gtoarpgnnc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.nanxuanxn.top/gtwfmqdhzp.html

JS:   toString() { return this.name; }
来源：http://hz.cheryme.top/gtpurnmaji.html

TS:   toString(): string { return this.name; }
来源：http://hz.9152youxi.cn/gtjrojnqps.html

Java: @Override public String toString() { return name; }
来源：http://hz.yuanzhike.top/gtitrcjkur.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.daxiang520.top/gthqkdklet.html

Ruby: def to_s; @name; end
来源：http://hz.yongpay.top/gtdopyiiml.html

C#:   public override string ToString() => Name;
来源：http://hz.gzhubu.top/gtvbwfyyah.html

[G13] 判断对象类型
来源：http://hz.zhoulong.xyz/gthqycgzzo.html

Py:   isinstance(u, User)
来源：http://hz.aizwys.cn/gthcabsmoz.html

PHP:  $u instanceof User
来源：http://hz.sufxvd.cn/gttfeuvolq.html

JS:   u instanceof User
来源：http://hz.shanyushiyangkeji.top/gtfgumitwo.html

TS:   u instanceof User
来源：http://hz.xuanzx.com/gtbgvndxtb.html

Java: u instanceof User
来源：http://hz.52xcode.cn/gtsbkzlvxl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jyoumei.cn/gtqxejqwis.html

Ruby: u.is_a?(User)
来源：http://hz.zhixingplan.top/gtkaqgafmz.html

C#:   u is User
来源：http://hz.nanxuanxn.top/gtowdgepfp.html

[G14] 数据类 / record
来源：http://hz.ywan-chungtsiang.top/gtvhndskqf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.shuidangran.top/gtuajjiccm.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jyoumei.cn/gtwohwmieb.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.guowangkeji.top/gtzotqwjdl.html

TS:   type User = { name: string; age: number };
来源：http://hz.gotoacloud.top/gtreupzzkl.html

Java: record User(String name, int age) {}
来源：http://hz.yvedp.cn/gtqvttbsge.html

Go:   type User struct { Name string; Age int }
来源：http://hz.ppjwa.cn/gtsefxcsrf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jinyuanbaomall.cn/gtdqavoazj.html

C#:   record User(string Name, int Age);
来源：http://hz.smart0.xyz/gtvrtfcpfu.html

[G15] 枚举
来源：http://hz.xylfe.cn/gtrexuaxww.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yj20258.top/gtluncxqzo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.xingfuxueyuan.xyz/gtrlkwznxs.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.mhx1999.top/gtvdwvbyiw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zdqjudy.top/gtddmlstmy.html

Java: enum Color { RED, GREEN }
来源：http://hz.xziqi.cn/gtnnszqzbe.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.xuetiantiany.cn/gthpuykypt.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ywan-chungtsiang.top/gtftvuszly.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhoulong.xyz/gtfbqumotm.html

[G16] 对象转数组 / 字典
来源：http://hz.jianghu66.top/gtdagjdvds.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.xingfuxueyuan.xyz/gtiggnqbkr.html

PHP:  get_object_vars($obj);
来源：http://hz.quarkkingdee.top/gtrhzfzuzz.html

JS:   Object.entries(obj)
来源：http://hz.zhaomingkeji.xyz/gteprdsneb.html

TS:   Object.entries(obj)
来源：http://hz.sxryk.cn/gtdwkuxhyt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.smart0.xyz/gtnpjhgjwo.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.feifeiyinyue.top/gthfouwzml.html

Ruby: obj.instance_variables
来源：http://hz.c1oappe.top/gtskilbjil.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.cqqwz.cn/gtxjxtxzkf.html

================================================================================
来源：http://hz.jqgufenzy.top/gtbrkejxol.html

H. 异常与错误处理
来源：http://hz.zhijiandao.cn/gtkxhrpdmm.html

================================================================================
来源：http://hz.mhx1999.top/gtxkxzzjqt.html

[H01] try / catch 基础
来源：http://hz.ehwqpu.com/gtzqmqartu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.pycfn.com/gtmgdydrtr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ivvv.top/gtkfwfxbdm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.vqdsnc.cn/gtkajzkexf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.cdnleiting.top/gtgryycskn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ywan-chungtsiang.top/gtoamelwof.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yongpay.top/gtbwtszuny.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.gaohongyu789.top/gtjhdwghon.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zycfv.cn/gtlyberjie.html

[H02] finally / ensure 收尾
来源：http://hz.quarkkingdee.top/gtswvvzvup.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.dashuyun.cn/gtepsqdfrv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.vqdsnc.cn/gtypqyydsm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.pengpengdd.cyou/gtfyhslibn.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zdqjudy.top/gtjyacjqga.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hywenlv.cn/gtufiirnyj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.guowangkeji.top/gtgqwhmxzw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.vqdsnc.cn/gtaqvomvtb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jlsjyb.cn/gtqjylbymt.html

[H03] 主动抛出异常
来源：http://hz.shzxlz.cn/gtdldicesg.html

Py:   raise ValueError("错误信息")
来源：http://hz.aizwys.cn/gtzmkietzl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.chenlongwang.top/gtczenzaqv.html

JS:   throw new Error("错误信息");
来源：http://hz.gzhubu.top/gtdfhgjypo.html

TS:   throw new Error("错误信息");
来源：http://hz.nwbrower.top/gtzcpmgjrg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.cqqwz.cn/gtblpadbki.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.haohaochexian.top/gtdqlwhyex.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.gotoacloud.top/gthtlckjjk.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.shanyushiyangtech.top/gtedlmizpe.html

[H04] 自定义异常类型
来源：http://hz.xziqi.cn/gtbpomwvip.html

Py:   class MyError(Exception): pass
来源：http://hz.shanyushiyangkeji.top/gtwycfxtfr.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hysaishi.cn/gtebexfxpy.html

JS:   class MyError extends Error {}
来源：http://hz.redwolf501.top/gtxfxxyngl.html

TS:   class MyError extends Error {}
来源：http://hz.aibaodan.cn/gtthbbmjnm.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jianghu66.top/gttfanyjhc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.shangyingyoupin.top/gtwsneobdg.html

Ruby: class MyError < StandardError; end
来源：http://hz.ybcxt.top/gtqcwjculd.html

C#:   class MyException : Exception {}
来源：http://hz.xinyue.icu/gtlzhhvnxp.html

[H05] 捕获特定类型
来源：http://hz.ehwqpu.com/gtagxrukfu.html

Py:   except ValueError as e:
来源：http://hz.zhijiandao.cn/gtypphcmuf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.hywenlv.cn/gtidumyrjr.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.hammf.cn/gtwtjzordw.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.ydjk.org.cn/gtptnymqgy.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yj20258.top/gtijfyxtms.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.bjfxy.top/gtykfbplnk.html

Ruby: rescue ArgumentError => e
来源：http://hz.xylfe.cn/gtrwhgqbsf.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhaomingkeji.xyz/gtddqnhrzz.html

[H06] 可选值 / 空值安全访问
来源：http://hz.dashuyun.cn/gtetwldzwu.html

Py:   value = d.get("k") or default
来源：http://hz.fzhhl.top/gtwyzrpzvi.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.chenlongwang.top/gtkzhsdmio.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yvedp.cn/gtafzjrzoq.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jianghu66.top/gtgielubuo.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.snrcjt.cn/gtayxkfyiq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yanxiufei.cn/gtcakymxkq.html

Ruby: d&.dig(:a, :b)
来源：http://hz.havefunace.top/gtxjzmgkmp.html

C#:   obj?.A?.B ?? default
来源：http://hz.sufxvd.cn/gtkvygfpvl.html


<!-- 参考信息 -->