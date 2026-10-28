代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://hz.havefunace.top/gtbyisnvny.html

[F02] 逐行读取文件
来源：http://hz.chenjidiqi.icu/gtdnboppyo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jinqigufen.top/gthympmbfe.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yonumen.top/gtlismtgjx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hnxiangtu.top/gtrwnalqfz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.9152youxi.cn/gtflpqahyu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.chenlongwang.top/gtlhcgqvul.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.cheryme.top/gtqhjmcdsv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yanxiufei.cn/gtrpjavsmq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.tian-w.cn/gtrnopoubi.html

[F03] 写入文件（覆盖）
来源：http://hz.daria6918.cn/gtywtchqiu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.nanxinkj.top/gthkzpmgdk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.c1oappe.top/gtgwsjaneg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhongyouzk.top/gtvonlbhpy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jinqigfzy.top/gtbzwvhoyv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.aizwys.cn/gtmwsycweq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.hnqzz.top/gtexjgrewk.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jqgufenzy.top/gtyyzfjlei.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.meibo888.top/gtzenyhvxe.html

[F04] 追加写入文件
来源：http://hz.yj202588.top/gtbvdyckbh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.sweek.top/gtdyopendg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.gotoacloud.top/gtttfajkwh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.guannengcc.top/gtaphzdbbq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hongshengwenyu.top/gtzehuyyvv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.sysykeji.top/gtktuyrkjq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.c1oappe.top/gtqvpkzvvc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zycfv.cn/gtjyrwrrzh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.ydjk.org.cn/gtbhnakozi.html

[F05] 判断文件或目录是否存在
来源：http://hz.haohaochexian.top/gtmptvsbby.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yj20258888.top/gtjofxzkaj.html

PHP:  file_exists("a.txt");
来源：http://hz.zhaomingkeji.xyz/gtvtvptjnv.html

JS:   fs.existsSync("a.txt")
来源：http://hz.pengpengdd.cyou/gtetvvgoaj.html

TS:   fs.existsSync("a.txt")
来源：http://hz.daria6918.cn/gtdrelqlpc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yongpay.top/gtxzglnnrv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.hywenlv.cn/gtpinphuik.html

Ruby: File.exist?("a.txt")
来源：http://hz.ehwqpu.com/gtlyggbghb.html

C#:   File.Exists("a.txt")
来源：http://hz.havefunace.top/gtvzrdndgx.html

[F06] 删除文件
来源：http://hz.gogol.net.cn/gtoeftqsmu.html

Py:   os.remove("a.txt")
来源：http://hz.dianchejie.cn/gtegsyvmrm.html

PHP:  unlink("a.txt");
来源：http://hz.shuidangran.top/gtxeszhzds.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.gzhubu.top/gtqbmbsvqd.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hammf.cn/gticxjohey.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.sxryk.cn/gtacagjdtt.html

Go:   os.Remove("a.txt")
来源：http://hz.tianlin.xyz/gtayrbwyst.html

Ruby: File.delete("a.txt")
来源：http://hz.hywenlv.cn/gtplugshut.html

C#:   File.Delete("a.txt");
来源：http://hz.shuidangran.top/gttezizbcx.html

[F07] 创建目录（含多级）
来源：http://hz.jinyuanbaomall.cn/gtysoztcwq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jinyuanbaomall.cn/gtgkbdvcbz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.shangyingyoupin.top/gtvaqvazxf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhijiandao.cn/gtxvkhkvfr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.tianlin.xyz/gtxfnxijcc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.chenlongwang.top/gtgzctugql.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.xylfe.cn/gtwsgkiknl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.chenjidiqi.icu/gtfsrkkzef.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yongpay.top/gtuyjucdjb.html

[F08] 遍历目录
来源：http://hz.birdmap.top/gtgyhtnmny.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.cheryme.top/gtcdozbwoo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.nwbrower.top/gtkhnipbai.html

JS:   fs.readdirSync("dir")
来源：http://hz.bjfxy.top/gtnujkahvw.html

TS:   fs.readdirSync("dir")
来源：http://hz.zhengqikj.top/gttpeftmze.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.wangshuangyany.cn/gtixomoqzi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.redwolf501.top/gtodgcclku.html

Ruby: Dir.children("dir")
来源：http://hz.52xcode.cn/gtikwnpzza.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zhoulong.xyz/gtdcntcctz.html

[F09] 获取文件大小
来源：http://hz.andypj.xyz/gtgcdsarsf.html

Py:   os.path.getsize("a.txt")
来源：http://hz.xylfe.cn/gtfbnbhqna.html

PHP:  filesize("a.txt");
来源：http://hz.shanyushiyangtech.top/gtadhwysfw.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jinyuanbaomall.cn/gttwfheskh.html

TS:   fs.statSync("a.txt").size
来源：http://hz.cdnleiting.top/gtxhentyxw.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yangfankeji.com/gtxldbcvsr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hnxiangtu.top/gtsfjosbnc.html

Ruby: File.size("a.txt")
来源：http://hz.kuanghao11.cn/gtnzclmxat.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yj202588.top/gtjoxvzlgd.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.shzxlz.cn/gtkiezoxko.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.nanxuanxn.top/gtnbfyfdgi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yuanzhike.top/gtmhfelsgd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.ydjk.org.cn/gtxuyjpwme.html

TS:   path.extname("a.txt")
来源：http://hz.nanxuanxn.top/gtmrtojcjw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.ywan-chungtsiang.top/gtohzrexxk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yj20258888.top/gtnarlvfio.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.hfpthk.cn/gtbazfnozp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yj202588.top/gtzuoahngb.html

[F11] 复制与移动文件
来源：http://hz.cashguo.top/gtgljbpqov.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yvedp.cn/gtwaggmbfe.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yongpay.top/gtbniweprd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jlsjyb.cn/gtysnesckv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.fzhhl.top/gtncqpbspv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yonumen.top/gtpcuwwbaq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.gogol.net.cn/gtifxmjiho.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.bjfxy.top/gtuklfuept.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jinqigufen.top/gttyvzkqdn.html

[F12] CSV 读写
来源：http://hz.tianlin.xyz/gtzusdnkbx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.nanxinkj.top/gtjjaiuzrt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.daria6918.cn/gtpbmsbbsq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.chenlongwang.top/gtsbxgguds.html

TS:   // 同上
来源：http://hz.xuanzx.com/gthsvwisja.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.mhx1999.top/gtuwqefwil.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.nanxinkj.top/gtpwebfukm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yuanzhike.top/gtslgxdmiy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zhiwuduotai.top/gtwaoutfcn.html

================================================================================
来源：http://hz.gzhubu.top/gtklbkszof.html

G. 面向对象
来源：http://hz.52xcode.cn/gtdfpuidrl.html

================================================================================
来源：http://hz.nanxinkj.top/gtzemqdajy.html

[G01] 定义类
来源：http://hz.vqdsnc.cn/gtajuioard.html

Py:   class User: pass
来源：http://hz.yueranfly.top/gtnlbkgsyl.html

PHP:  class User {}
来源：http://hz.meibo888.top/gtoiwnlpay.html

JS:   class User {}
来源：http://hz.zhoulong.xyz/gtyjsnicce.html

TS:   class User { name: string = ""; }
来源：http://hz.gaohongyu789.top/gttfyotgid.html

Java: class User {}
来源：http://hz.shanyushiyangkeji.top/gtftfzunrr.html

Go:   type User struct { Name string }
来源：http://hz.zhoulong.xyz/gtpwkxivxa.html

Ruby: class User; end
来源：http://hz.sufxvd.cn/gtdljmetae.html

C#:   class User {}
来源：http://hz.yj202588.top/gtjzglwfpj.html

[G02] 构造函数
来源：http://hz.ehwqpu.com/gttkuuyrme.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.xziqi.cn/gtxjltoulo.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.chenzaomai.com/gtagwnqiyg.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.snrcjt.cn/gtkxfjxdfe.html

TS:   constructor(public name: string) {}
来源：http://hz.sufxvd.cn/gtbkrvyapj.html

Java: User(String name) { this.name = name; }
来源：http://hz.hnxiangtu.top/gtzgpqwwue.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.316326.xyz/gtxrkqadno.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.kuanghao11.cn/gtyokuvgix.html

C#:   public User(string name) { Name = name; }
来源：http://hz.gzhubu.top/gtaouvrekf.html

[G03] 实例属性
来源：http://hz.hnqzz.top/gtqhidyhvo.html

Py:   self.name = "x"
来源：http://hz.zhijiandao.cn/gtqxmczpni.html

PHP:  public string $name = "x";
来源：http://hz.zhaomingkeji.xyz/gtdoqoiuna.html

JS:   this.name = "x";
来源：http://hz.316326.xyz/gtytvwafia.html

TS:   name: string = "x";
来源：http://hz.xinyue.icu/gtfzsnylxf.html

Java: private String name;
来源：http://hz.mhx1999.top/gtjqnphgxq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.tanke756.top/gtopiyyycg.html

Ruby: @name = "x"
来源：http://hz.xylfe.cn/gttlfdiskw.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.xuanzx.com/gtiqygvdtp.html

[G04] 定义方法
来源：http://hz.nanxuanxn.top/gtzzmflztj.html

Py:   def greet(self): return self.name
来源：http://hz.yvedp.cn/gthzsrqefk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.shzxlz.cn/gtypjjeisa.html

JS:   greet() { return this.name; }
来源：http://hz.zhixingplan.top/gtqpwbndpd.html

TS:   greet(): string { return this.name; }
来源：http://hz.c1oappe.top/gttawgfvvc.html

Java: String greet() { return name; }
来源：http://hz.zhaomingkeji.xyz/gtthvcmfpb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jyoumei.cn/gtqsdodjtz.html

Ruby: def greet; @name; end
来源：http://hz.ivvv.top/gtdexyeatx.html

C#:   public string Greet() => Name;
来源：http://hz.cucudq.cn/gtbzuabcak.html

[G05] 继承
来源：http://hz.jinqigfzy.top/gtktvnnfdl.html

Py:   class Admin(User): pass
来源：http://hz.xingfuxueyuan.xyz/gtgrbvgvnx.html

PHP:  class Admin extends User {}
来源：http://hz.ppjwa.cn/gtkbejyyoa.html

JS:   class Admin extends User {}
来源：http://hz.hammf.cn/gtsgfgeapk.html

TS:   class Admin extends User {}
来源：http://hz.zhixingplan.top/gtilcqnana.html

Java: class Admin extends User {}
来源：http://hz.52xcode.cn/gtraikppcm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.shanyushiyangtech.top/gtgtyfefhw.html

Ruby: class Admin < User; end
来源：http://hz.yueranfly.top/gtaeazcdbi.html

C#:   class Admin : User {}
来源：http://hz.fzhhl.top/gtrlanchti.html

[G06] 重写方法
来源：http://hz.xziqi.cn/gtwvtbrenw.html

Py:   def greet(self): return "admin"
来源：http://hz.yuxming.cn/gtvudqlbkw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.redwolf501.top/gtysaumpwu.html

JS:   greet() { return "admin"; }
来源：http://hz.mhx1999.top/gteprkclgn.html

TS:   greet(): string { return "admin"; }
来源：http://hz.ybcxt.top/gtbablpqnf.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jqgfzy.top/gtrjexcsdf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jianghu66.top/gtknzxlmya.html

Ruby: def greet; "admin"; end
来源：http://hz.ydjk.org.cn/gtonvyrknb.html

C#:   public override string Greet() => "admin";
来源：http://hz.jqgfzy.top/gtutpmiigz.html

[G07] 调用父类方法
来源：http://hz.pengpengdd.cyou/gtevsuojfw.html

Py:   super().greet()
来源：http://hz.xuanzx.com/gtxbivwxdw.html

PHP:  parent::greet();
来源：http://hz.iojbl.cn/gtshnvjbff.html

JS:   super.greet();
来源：http://hz.ydjk.org.cn/gttoqtcvax.html

TS:   super.greet();
来源：http://hz.zhengqikj.top/gtdepvvsfz.html

Java: super.greet();
来源：http://hz.yuanzhike.top/gtbpuhstjn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.wangdashe.top/gtjvdkilgv.html

Ruby: super
来源：http://hz.sysykeji.top/gtfzgzsjiz.html

C#:   base.Greet();
来源：http://hz.smart0.xyz/gtlzaoewvt.html

[G08] 静态方法与属性
来源：http://hz.cheryme.top/gtaxrugtud.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.guowangkeji.top/gtxwqropvn.html

PHP:  public static function f() {}
来源：http://hz.zhoulong.xyz/gtizjcwuvx.html

JS:   static f() {}
来源：http://hz.aibaodan.cn/gtvmjbltaf.html

TS:   static f(): void {}
来源：http://hz.shzxlz.cn/gthwxbtufu.html

Java: static void f() {}
来源：http://hz.xingfuxueyuan.xyz/gttiusgpmq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.hnqzz.top/gtjkgkrruj.html

Ruby: def self.f; end
来源：http://hz.52xcode.cn/gtkiaeupcy.html

C#:   public static void F() {}
来源：http://hz.shuidangran.top/gtdvukvzih.html

[G09] 接口 / 抽象类
来源：http://hz.yj20258888.top/gtlccubdwi.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.wangdashe.top/gtsjvglurq.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.hywenlv.cn/gtprjdtvyq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.xuetiantiany.cn/gtundgdodg.html

TS:   interface Shape { area(): number; }
来源：http://hz.hysaishi.cn/gtaqbulfeb.html

Java: interface Shape { double area(); }
来源：http://hz.sufxvd.cn/gtndperzdb.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.birdmap.top/gthxbmpcgr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yj20258888.top/gtmjutfadf.html

C#:   interface IShape { double Area(); }
来源：http://hz.c1oappe.top/gtxsijgnbi.html

[G10] 访问控制
来源：http://hz.snrcjt.cn/gtxsoxblre.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jiagoushi.top/gtkeldteyr.html

PHP:  public / protected / private
来源：http://hz.cucudq.cn/gtgfoklesw.html

JS:   #private 字段；其余公开
来源：http://hz.guannengcc.top/gtzzavahkt.html

TS:   public / protected / private
来源：http://hz.daria6918.cn/gtzzydgems.html

Java: public / protected / private / 默认包级
来源：http://hz.dianchejie.cn/gtvbsegdhx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jyoumei.cn/gtphwnlspr.html

Ruby: public / protected / private
来源：http://hz.fzhhl.top/gtexcmjlcs.html

C#:   public / protected / private / internal
来源：http://hz.nwbrower.top/gtoclmqwjh.html

[G11] getter / setter
来源：http://hz.jinyuanbaomall.cn/gtdggfgfhk.html

Py:   @property 与 @x.setter
来源：http://hz.svipenyu.cn/gtmdalrijn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yangfankeji.com/gtetrriosu.html

JS:   get name() { return this._name; }
来源：http://hz.yuxming.cn/gtnseqtprm.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhongyouzk.top/gttaqvmnqf.html

Java: public String getName() { return name; }
来源：http://hz.hongshengwenyu.top/gtljxdhgsp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jlsjyb.cn/gtnyiymkbn.html

Ruby: attr_accessor :name
来源：http://hz.zhongyouzk.top/gtcamrwvaj.html

C#:   public string Name { get; set; }
来源：http://hz.zhixingplan.top/gtbovbpvdw.html

[G12] 对象转字符串
来源：http://hz.tian-w.cn/gtlppjkxyi.html

Py:   def __str__(self): return self.name
来源：http://hz.sweek.top/gtdbaiqfsd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.pycfn.com/gtbvoynazs.html

JS:   toString() { return this.name; }
来源：http://hz.shuidangran.top/gtsqsnpnwk.html

TS:   toString(): string { return this.name; }
来源：http://hz.fzhhl.top/gtxamsfgay.html

Java: @Override public String toString() { return name; }
来源：http://hz.quarkkingdee.top/gtaefvhjml.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.feifeiyinyue.top/gtyippzpqd.html

Ruby: def to_s; @name; end
来源：http://hz.yj20258.top/gttotznhsi.html

C#:   public override string ToString() => Name;
来源：http://hz.zhengqikj.top/gtbmyegkpk.html

[G13] 判断对象类型
来源：http://hz.dianchejie.cn/gtadeqgsyk.html

Py:   isinstance(u, User)
来源：http://hz.tanke756.top/gtcpxcjwjk.html

PHP:  $u instanceof User
来源：http://hz.52xcode.cn/gtmvhamfhi.html

JS:   u instanceof User
来源：http://hz.gogol.net.cn/gtopjtvoqo.html

TS:   u instanceof User
来源：http://hz.xziqi.cn/gtasnqwdfb.html

Java: u instanceof User
来源：http://hz.zhijiandao.cn/gtjphgmdsu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ydjk.org.cn/gtjsgowkal.html

Ruby: u.is_a?(User)
来源：http://hz.jinghuilouyu.cn/gtcdaiwyzu.html

C#:   u is User
来源：http://hz.dashuyun.cn/gthxkphhmm.html

[G14] 数据类 / record
来源：http://hz.gzhubu.top/gtrdvcokvd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.ybcxt.top/gtlipjmsxf.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.gzhubu.top/gthmiwfsey.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.xuetiantiany.cn/gtaivzpwid.html

TS:   type User = { name: string; age: number };
来源：http://hz.jianghu66.top/gtgyrbmxwz.html

Java: record User(String name, int age) {}
来源：http://hz.sweek.top/gtmiswrugy.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zhaomingkeji.xyz/gthxcielwi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.fzhhl.top/gtfwrkhztp.html

C#:   record User(string Name, int Age);
来源：http://hz.zhoulong.xyz/gtnfyxhaco.html

[G15] 枚举
来源：http://hz.c1oappe.top/gtpostston.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.meibo888.top/gtvllcuihp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zycfv.cn/gtartqrqaa.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.guowangkeji.top/gtryevsvob.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hysaishi.cn/gtbqyvjbqb.html

Java: enum Color { RED, GREEN }
来源：http://hz.yuxming.cn/gtyljlfbeu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.xingfuxueyuan.xyz/gtsmevoqka.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zhoulong.xyz/gtisxmamck.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sufxvd.cn/gtribcsxko.html

[G16] 对象转数组 / 字典
来源：http://hz.yuxming.cn/gtgqzqtfop.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.sysykeji.top/gtdwkkujsq.html

PHP:  get_object_vars($obj);
来源：http://hz.aibaodan.cn/gtwxxedhzp.html

JS:   Object.entries(obj)
来源：http://hz.xingfuxueyuan.xyz/gtljyssnua.html

TS:   Object.entries(obj)
来源：http://hz.cqqwz.cn/gtmxvbvfvm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jqgufenzy.top/gtiupuplmm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.c1oappe.top/gtkdhqynuw.html

Ruby: obj.instance_variables
来源：http://hz.ehwqpu.com/gtautgpbki.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.aizwys.cn/gtlgvqorpp.html

================================================================================
来源：http://hz.hfpthk.cn/gtpoyqjjmn.html

H. 异常与错误处理
来源：http://hz.cashguo.top/gtwgtoprpm.html

================================================================================
来源：http://hz.xylfe.cn/gtwpxtcjuy.html

[H01] try / catch 基础
来源：http://hz.jqgufenzy.top/gtklkzhkbg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.shanyushiyangkeji.top/gtpmvesifo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.daxiang520.top/gtaptfbrra.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.ydjk.org.cn/gtsybkmrtt.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.meibo888.top/gtqfwpfosw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.wangdashe.top/gtfepyxvhe.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.cucudq.cn/gtgeptbwnr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.vqdsnc.cn/gttuizknbo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.dianchejie.cn/gtcfuikbbq.html

[H02] finally / ensure 收尾
来源：http://hz.iojbl.cn/gtpjjsfwqr.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.316326.xyz/gtaykrvdtc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.nanxuanxn.top/gtaxblojcr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.cheryme.top/gtkkpzleli.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zdqjudy.top/gtyxakpxij.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jinghuilouyu.cn/gtlpzwqryt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.fzhhl.top/gtfucmuged.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.wangdashe.top/gtynmsvqnk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jlsjyb.cn/gtjpblmzql.html

[H03] 主动抛出异常
来源：http://hz.9152youxi.cn/gtktkqasgy.html

Py:   raise ValueError("错误信息")
来源：http://hz.meibo888.top/gtcjxyzsxo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.0kj1m.cn/gtijjwreod.html

JS:   throw new Error("错误信息");
来源：http://hz.jianghu66.top/gtlrhuwdor.html

TS:   throw new Error("错误信息");
来源：http://hz.pycfn.com/gtedwuamdk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jianghu66.top/gtxlthrfcu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.cheryme.top/gtepvbgiwq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.daxiang520.top/gtngumorop.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.fengsongda.top/gtxofpowwk.html

[H04] 自定义异常类型
来源：http://hz.pycfn.com/gtxxhyzshy.html

Py:   class MyError(Exception): pass
来源：http://hz.smart0.xyz/gtduboyqvm.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jyoumei.cn/gtkipcmtgh.html

JS:   class MyError extends Error {}
来源：http://hz.sysykeji.top/gtuzouhajx.html

TS:   class MyError extends Error {}
来源：http://hz.chenzaomai.com/gtssgowrxu.html

Java: class MyException extends RuntimeException {}
来源：http://hz.fengsongda.top/gtyzkahzmd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.iojbl.cn/gtvhalsrtz.html

Ruby: class MyError < StandardError; end
来源：http://hz.pycfn.com/gtfozutzza.html

C#:   class MyException : Exception {}
来源：http://hz.ybcxt.top/gtproswtkn.html

[H05] 捕获特定类型
来源：http://hz.guannengcc.top/gtwglfuqph.html

Py:   except ValueError as e:
来源：http://hz.shangyingyoupin.top/gtuuwiobfv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.pengpengdd.cyou/gtnveizzwn.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.chenlongwang.top/gtwvyrhosx.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.gzhubu.top/gtebvagbgk.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.svipenyu.cn/gtfdtljanf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.ivvv.top/gtmwvlpwhk.html

Ruby: rescue ArgumentError => e
来源：http://hz.hongshengwenyu.top/gtpcqoksrx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.cashguo.top/gtdblrzwbv.html

[H06] 可选值 / 空值安全访问
来源：http://hz.cucudq.cn/gtzfwfqknm.html

Py:   value = d.get("k") or default
来源：http://hz.ydjk.org.cn/gtswawvhtt.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.nanxuanxn.top/gtdzexyjcx.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.cashguo.top/gtaregxtcr.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.quarkkingdee.top/gtzbnekeht.html


<!-- 参考信息 -->