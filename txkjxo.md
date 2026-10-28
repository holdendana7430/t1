代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.chenzaomai.com/gtzagbynyt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jianghu66.top/gttmtgubba.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.nanxuanxn.top/gtjpkqajgu.html

Ruby: File.read("a.txt")
来源：http://hz.xuanzx.com/gtwlamgznq.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.gogol.net.cn/gtemrbomll.html

[F02] 逐行读取文件
来源：http://hz.bjfxy.top/gtqnzghrvh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.dianchejie.cn/gtptceuoau.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.guowangkeji.top/gtptvxlqxw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.sxryk.cn/gtlryvpdwl.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.chenlongwang.top/gtfrqoppgg.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.andypj.xyz/gtaargvchb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.shanyushiyangkeji.top/gtzojvefir.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yueranfly.top/gteftpxgdp.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.nanxuanxn.top/gtzzihmvln.html

[F03] 写入文件（覆盖）
来源：http://hz.dashuyun.cn/gtucuhjysx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hammf.cn/gtzucabvgk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.yj202588.top/gthzsnqhlg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.meibo888.top/gtuwnisnmr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ydjk.org.cn/gtsexbhfoj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.tanke756.top/gttnjgnaim.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yangfankeji.com/gtnhpztzkc.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.hywenlv.cn/gtyoyxwbvu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.9152youxi.cn/gtljaccurv.html

[F04] 追加写入文件
来源：http://hz.cashguo.top/gtdelnasbs.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.9152youxi.cn/gtovhfxzie.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.nanxinkj.top/gtbrjfzoye.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jqgfzy.top/gtuddgpkcs.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jqgfzy.top/gtdlkxdaaz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.cashguo.top/gtqdnqvarx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.cashguo.top/gtwtvttzul.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.xingfuxueyuan.xyz/gtyxhmyyaf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.fengsongda.top/gtemwejwrj.html

[F05] 判断文件或目录是否存在
来源：http://hz.yj20258.top/gttghceqed.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.shzxlz.cn/gttvuledwy.html

PHP:  file_exists("a.txt");
来源：http://hz.ppjwa.cn/gthieskxqt.html

JS:   fs.existsSync("a.txt")
来源：http://hz.cucudq.cn/gtfpgtxfaq.html

TS:   fs.existsSync("a.txt")
来源：http://hz.kuanghao11.cn/gtoeinrkwm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.chenlongwang.top/gtrrfxmsjz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.hysaishi.cn/gtwidlftwq.html

Ruby: File.exist?("a.txt")
来源：http://hz.kuanghao11.cn/gtxtvykyjk.html

C#:   File.Exists("a.txt")
来源：http://hz.havefunace.top/gtggcddqrg.html

[F06] 删除文件
来源：http://hz.smart0.xyz/gtjnhyarws.html

Py:   os.remove("a.txt")
来源：http://hz.yanxiufei.cn/gtrrtrxpto.html

PHP:  unlink("a.txt");
来源：http://hz.bjfxy.top/gtyeyijphg.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.nanxinkj.top/gtqzbralqb.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.ehwqpu.com/gtsjrqqgws.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.ivvv.top/gttcfsvjfi.html

Go:   os.Remove("a.txt")
来源：http://hz.guannengcc.top/gtgpvcbsho.html

Ruby: File.delete("a.txt")
来源：http://hz.aizwys.cn/gtgmviwmwn.html

C#:   File.Delete("a.txt");
来源：http://hz.yj20258888.top/gtjplohfcs.html

[F07] 创建目录（含多级）
来源：http://hz.shanyushiyangkeji.top/gtkurfbfow.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.ivvv.top/gtswuynnom.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.snrcjt.cn/gtopzxivut.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.sysykeji.top/gtsoudpcxl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jyoumei.cn/gtitwrccud.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hnxiangtu.top/gtudfooubi.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zhoulong.xyz/gtsnkjuxdv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.smart0.xyz/gtefhaulgy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jiagoushi.top/gtppjsqosb.html

[F08] 遍历目录
来源：http://hz.haohaochexian.top/gticewvlvl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.chenjidiqi.icu/gtvmmwufbm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.tanke756.top/gtiqrrslok.html

JS:   fs.readdirSync("dir")
来源：http://hz.chenlongwang.top/gtbuuqauvh.html

TS:   fs.readdirSync("dir")
来源：http://hz.kuanghao11.cn/gtnusmqmth.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yj20258888.top/gtkbqgvywl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.shanyushiyangkeji.top/gtlsqmewkt.html

Ruby: Dir.children("dir")
来源：http://hz.gogol.net.cn/gtnxgjohbt.html

C#:   Directory.GetFiles("dir")
来源：http://hz.c1oappe.top/gtnddiccmq.html

[F09] 获取文件大小
来源：http://hz.zhongyouzk.top/gtdyyqduxt.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jlsjyb.cn/gtpvglivsp.html

PHP:  filesize("a.txt");
来源：http://hz.cqqwz.cn/gtutxprmlc.html

JS:   fs.statSync("a.txt").size
来源：http://hz.hnxiangtu.top/gtackxcapr.html

TS:   fs.statSync("a.txt").size
来源：http://hz.haohaochexian.top/gtpkzjsjfs.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.vqdsnc.cn/gtgertwylv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zdqjudy.top/gtbpawpbri.html

Ruby: File.size("a.txt")
来源：http://hz.smart0.xyz/gtgkhtrqii.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.zhixingplan.top/gtcabhkjra.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.aizwys.cn/gtlhxxbemo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.ivvv.top/gtvjuwdcje.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.316326.xyz/gtcjzojkwq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.hywenlv.cn/gtisdbiakk.html

TS:   path.extname("a.txt")
来源：http://hz.dashuyun.cn/gtwknjitgj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.nanxuanxn.top/gthcwguojs.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.hnxiangtu.top/gtnudskzoy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.hysaishi.cn/gtcqcpgedc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.chenzaomai.com/gtdqinqica.html

[F11] 复制与移动文件
来源：http://hz.dianchejie.cn/gtynsjxbkn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yueranfly.top/gtsgjpxjmb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yj20258.top/gtevznchsx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.redwolf501.top/gtohmmpiaf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ppjwa.cn/gtvlrocpzi.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.shanyushiyangtech.top/gtpmyiyktx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.andypj.xyz/gtkkysuwis.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.aizwys.cn/gtezxgskjs.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.kuanghao11.cn/gtjwzvkmiu.html

[F12] CSV 读写
来源：http://hz.jianghu66.top/gtwjbtezbz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.nwbrower.top/gtdamdsgzv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.pengpengdd.cyou/gtqsqglnnv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.aizwys.cn/gtyqumnyiu.html

TS:   // 同上
来源：http://hz.wangshuangyany.cn/gtybcwnwlb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.havefunace.top/gthbngjiny.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.c1oappe.top/gtlhjrwdtm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ydjk.org.cn/gtchfmwqmz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.gaohongyu789.top/gtiyzcivqw.html

================================================================================
来源：http://hz.yangfankeji.com/gtasdjfrul.html

G. 面向对象
来源：http://hz.yueranfly.top/gtgxumvcen.html

================================================================================
来源：http://hz.zhixingplan.top/gtbkfmylmj.html

[G01] 定义类
来源：http://hz.yanxiufei.cn/gtedewjyxr.html

Py:   class User: pass
来源：http://hz.guannengcc.top/gtaocbozia.html

PHP:  class User {}
来源：http://hz.jyoumei.cn/gtaymuxqmx.html

JS:   class User {}
来源：http://hz.jinghuilouyu.cn/gtlfmzqrbp.html

TS:   class User { name: string = ""; }
来源：http://hz.yj20258.top/gtbjpvchfv.html

Java: class User {}
来源：http://hz.fengsongda.top/gtdsrarjrx.html

Go:   type User struct { Name string }
来源：http://hz.nwbrower.top/gtbsemvqwf.html

Ruby: class User; end
来源：http://hz.chenzaomai.com/gtmhrlpcgw.html

C#:   class User {}
来源：http://hz.svipenyu.cn/gtxqtswfkx.html

[G02] 构造函数
来源：http://hz.zhengqikj.top/gtzldcfqzk.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.sxryk.cn/gtrmfxzign.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.snrcjt.cn/gtyjnbadkt.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.hammf.cn/gtnmesfuvh.html

TS:   constructor(public name: string) {}
来源：http://hz.zhongyouzk.top/gttkyijogs.html

Java: User(String name) { this.name = name; }
来源：http://hz.shanyushiyangtech.top/gtbnhzlamn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yvedp.cn/gtjhbifwyf.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.daxiang520.top/gtyotzhspz.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zhoulong.xyz/gtldsclulf.html

[G03] 实例属性
来源：http://hz.ywan-chungtsiang.top/gtsyrfjhxv.html

Py:   self.name = "x"
来源：http://hz.yongpay.top/gtxpugsvfv.html

PHP:  public string $name = "x";
来源：http://hz.iojbl.cn/gtdqixyaqa.html

JS:   this.name = "x";
来源：http://hz.zdqjudy.top/gtpzsbpagq.html

TS:   name: string = "x";
来源：http://hz.jiagoushi.top/gtkhrmoitx.html

Java: private String name;
来源：http://hz.jlsjyb.cn/gtnybnbzks.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.aibaodan.cn/gtpzoceala.html

Ruby: @name = "x"
来源：http://hz.yj20258888.top/gttddamsob.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.xingfuxueyuan.xyz/gtgieaxevj.html

[G04] 定义方法
来源：http://hz.havefunace.top/gtbxvvnntk.html

Py:   def greet(self): return self.name
来源：http://hz.svipenyu.cn/gtxrjrucpk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.redwolf501.top/gtkfjiaxdo.html

JS:   greet() { return this.name; }
来源：http://hz.pengpengdd.cyou/gtlpqmywal.html

TS:   greet(): string { return this.name; }
来源：http://hz.cashguo.top/gtskpmwqoi.html

Java: String greet() { return name; }
来源：http://hz.gzhubu.top/gtloujzvmm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.mhx1999.top/gtkkmxbvsk.html

Ruby: def greet; @name; end
来源：http://hz.hongshengwenyu.top/gtidtkwqlr.html

C#:   public string Greet() => Name;
来源：http://hz.cqqwz.cn/gtqwpblbjy.html

[G05] 继承
来源：http://hz.ywan-chungtsiang.top/gtdckudohs.html

Py:   class Admin(User): pass
来源：http://hz.xziqi.cn/gtmkvpuhbt.html

PHP:  class Admin extends User {}
来源：http://hz.hongshengwenyu.top/gttbuwrknq.html

JS:   class Admin extends User {}
来源：http://hz.sweek.top/gttbkwwsyz.html

TS:   class Admin extends User {}
来源：http://hz.hnxiangtu.top/gttvjbqqgs.html

Java: class Admin extends User {}
来源：http://hz.redwolf501.top/gtkfbzunxv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ywan-chungtsiang.top/gtuxfiyvsd.html

Ruby: class Admin < User; end
来源：http://hz.shuidangran.top/gtjiawtjbf.html

C#:   class Admin : User {}
来源：http://hz.yueranfly.top/gtnxfzxwje.html

[G06] 重写方法
来源：http://hz.yueranfly.top/gtfjkmvpap.html

Py:   def greet(self): return "admin"
来源：http://hz.sufxvd.cn/gteghioesl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.wangdashe.top/gtugzizcxg.html

JS:   greet() { return "admin"; }
来源：http://hz.ydjk.org.cn/gtlygyvlwk.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yongpay.top/gtvcfmdpxx.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.andypj.xyz/gtflhmcmhx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhaomingkeji.xyz/gtomasgwht.html

Ruby: def greet; "admin"; end
来源：http://hz.jiagoushi.top/gthixwerkl.html

C#:   public override string Greet() => "admin";
来源：http://hz.shuidangran.top/gtejmncrmg.html

[G07] 调用父类方法
来源：http://hz.hysaishi.cn/gttpjmlsli.html

Py:   super().greet()
来源：http://hz.jinqigufen.top/gtedsiysvs.html

PHP:  parent::greet();
来源：http://hz.dianchejie.cn/gtqboqrszm.html

JS:   super.greet();
来源：http://hz.0kj1m.cn/gtfvoqprcw.html

TS:   super.greet();
来源：http://hz.ybcxt.top/gtfcgnegsz.html

Java: super.greet();
来源：http://hz.sxryk.cn/gtfesynvvj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yj20258888.top/gtblvqhelx.html

Ruby: super
来源：http://hz.sxryk.cn/gtcuosdibl.html

C#:   base.Greet();
来源：http://hz.xuetiantiany.cn/gtmnokkdxn.html

[G08] 静态方法与属性
来源：http://hz.zhongyouzk.top/gtapzlhgwv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhoulong.xyz/gtexmetage.html

PHP:  public static function f() {}
来源：http://hz.zhengqikj.top/gtfqpbporl.html

JS:   static f() {}
来源：http://hz.xuetiantiany.cn/gtqqjfaboa.html

TS:   static f(): void {}
来源：http://hz.cdnleiting.top/gtywrtngnf.html

Java: static void f() {}
来源：http://hz.zhongyouzk.top/gtycaygccr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yj202588.top/gtgzaifwag.html

Ruby: def self.f; end
来源：http://hz.ydjk.org.cn/gtqegvdmws.html

C#:   public static void F() {}
来源：http://hz.zhijiandao.cn/gttmdsqmrf.html

[G09] 接口 / 抽象类
来源：http://hz.hysaishi.cn/gthgssrghc.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.wangdashe.top/gtsrwwaawh.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zhixingplan.top/gtvtqfbzet.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ivvv.top/gtwmuawfwn.html

TS:   interface Shape { area(): number; }
来源：http://hz.xinyue.icu/gtdoccgrid.html

Java: interface Shape { double area(); }
来源：http://hz.yanxiufei.cn/gttoqwyijq.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.daxiang520.top/gtlhnkywig.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.xylfe.cn/gtnyosajpu.html

C#:   interface IShape { double Area(); }
来源：http://hz.meibo888.top/gtnzypghzt.html

[G10] 访问控制
来源：http://hz.c1oappe.top/gtombdoika.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jiagoushi.top/gtkbpbuxlu.html

PHP:  public / protected / private
来源：http://hz.shanyushiyangkeji.top/gtkxgyidpu.html

JS:   #private 字段；其余公开
来源：http://hz.jianghu66.top/gtwqksfvyh.html

TS:   public / protected / private
来源：http://hz.hnqzz.top/gtcfozfccn.html

Java: public / protected / private / 默认包级
来源：http://hz.hfpthk.cn/gtarlpfddd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.0kj1m.cn/gtvrrcdndl.html

Ruby: public / protected / private
来源：http://hz.hywenlv.cn/gtydgwhuie.html

C#:   public / protected / private / internal
来源：http://hz.kuanghao11.cn/gtzgjxgrey.html

[G11] getter / setter
来源：http://hz.gogol.net.cn/gtsntfmtrb.html

Py:   @property 与 @x.setter
来源：http://hz.cheryme.top/gtkmgnyavf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.shanyushiyangkeji.top/gtbhrwudpt.html

JS:   get name() { return this._name; }
来源：http://hz.zhixingplan.top/gtdacdagrm.html

TS:   get name(): string { return this._name; }
来源：http://hz.ehwqpu.com/gtqbywrlqz.html

Java: public String getName() { return name; }
来源：http://hz.xingfuxueyuan.xyz/gtgsxwanah.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.xylfe.cn/gtukmaadau.html

Ruby: attr_accessor :name
来源：http://hz.yuxming.cn/gtfcrdqrzf.html

C#:   public string Name { get; set; }
来源：http://hz.9152youxi.cn/gttcikipbh.html

[G12] 对象转字符串
来源：http://hz.bjfxy.top/gtkjlxmqyq.html

Py:   def __str__(self): return self.name
来源：http://hz.guowangkeji.top/gtmwzdofql.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.nanxinkj.top/gtudzzatwj.html

JS:   toString() { return this.name; }
来源：http://hz.jianghu66.top/gtwgetqvux.html

TS:   toString(): string { return this.name; }
来源：http://hz.xinyue.icu/gtyhlqldwc.html

Java: @Override public String toString() { return name; }
来源：http://hz.sweek.top/gtrvyjthvu.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.tian-w.cn/gthplbrqkl.html

Ruby: def to_s; @name; end
来源：http://hz.yj202588.top/gtqmdvfmrk.html

C#:   public override string ToString() => Name;
来源：http://hz.jyoumei.cn/gtnmnjxtmb.html

[G13] 判断对象类型
来源：http://hz.zhengqikj.top/gtazqipbqa.html

Py:   isinstance(u, User)
来源：http://hz.jinqigufen.top/gtaptyzlha.html

PHP:  $u instanceof User
来源：http://hz.ehwqpu.com/gtvdfvujyi.html

JS:   u instanceof User
来源：http://hz.ppjwa.cn/gttjjwmlmo.html

TS:   u instanceof User
来源：http://hz.wangdashe.top/gtfhrftjlg.html

Java: u instanceof User
来源：http://hz.guowangkeji.top/gtrgywkvan.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jlsjyb.cn/gtgteyipdp.html

Ruby: u.is_a?(User)
来源：http://hz.zhixingplan.top/gtunknsnmb.html

C#:   u is User
来源：http://hz.xingfuxueyuan.xyz/gtkqyyjgtd.html

[G14] 数据类 / record
来源：http://hz.andypj.xyz/gtbicopmot.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yangfankeji.com/gtflumydgw.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.shanyushiyangkeji.top/gtfgykoqgy.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.cqqwz.cn/gtrlzgzpmq.html

TS:   type User = { name: string; age: number };
来源：http://hz.zdqjudy.top/gttcvghhyp.html

Java: record User(String name, int age) {}
来源：http://hz.xingfuxueyuan.xyz/gtezgvhmpg.html

Go:   type User struct { Name string; Age int }
来源：http://hz.sxryk.cn/gtpiplcztq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.daxiang520.top/gtjykujwsf.html

C#:   record User(string Name, int Age);
来源：http://hz.gogol.net.cn/gtnpozqjim.html

[G15] 枚举
来源：http://hz.snrcjt.cn/gtcrqintqk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.hnqzz.top/gtbkmiifua.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jlsjyb.cn/gtgonscela.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.nanxinkj.top/gtdoirjuvn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sysykeji.top/gtliwvwpri.html

Java: enum Color { RED, GREEN }
来源：http://hz.snrcjt.cn/gtrgnstpcp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.cqqwz.cn/gtcugqgpkb.html

Ruby: Color = %i[red green].freeze
来源：http://hz.pycfn.com/gtorvkytcy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.kuanghao11.cn/gtitradyzw.html

[G16] 对象转数组 / 字典
来源：http://hz.gotoacloud.top/gtvhyvlcve.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.hammf.cn/gtkolyamnw.html

PHP:  get_object_vars($obj);
来源：http://hz.xylfe.cn/gtutshqxob.html

JS:   Object.entries(obj)
来源：http://hz.jinqigfzy.top/gthuvocgdb.html

TS:   Object.entries(obj)
来源：http://hz.hywenlv.cn/gtkcnnvuso.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.cdnleiting.top/gtnbyytmif.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.cheryme.top/gtbldjshhz.html

Ruby: obj.instance_variables
来源：http://hz.haohaochexian.top/gtqyvywjwt.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.iojbl.cn/gtpswqpasr.html

================================================================================
来源：http://hz.zhengqikj.top/gteonapkyk.html

H. 异常与错误处理
来源：http://hz.pycfn.com/gtfokvctga.html

================================================================================
来源：http://hz.chenjidiqi.icu/gteenzwbtl.html

[H01] try / catch 基础
来源：http://hz.tian-w.cn/gtqybmpmgh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.cqqwz.cn/gtnqyeylvd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.iojbl.cn/gtnxvxyaql.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.ywan-chungtsiang.top/gtlwkiojrn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.andypj.xyz/gtofjsjqro.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zhijiandao.cn/gtepsjtcwv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.snrcjt.cn/gthcflnies.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.aizwys.cn/gtrbwxdfgz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.hongshengwenyu.top/gtjfnkfhtq.html

[H02] finally / ensure 收尾
来源：http://hz.aibaodan.cn/gtywpgqjbt.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.wangdashe.top/gtczpfdjxa.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.snrcjt.cn/gtznjeewbi.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.mhx1999.top/gtllojxzwz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.fengsongda.top/gtljknteji.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yj20258888.top/gtptwobusj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.birdmap.top/gtucfyvoys.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.cashguo.top/gtwdyxnllj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.aizwys.cn/gtbjyosvpj.html

[H03] 主动抛出异常
来源：http://hz.316326.xyz/gttutfsiml.html

Py:   raise ValueError("错误信息")
来源：http://hz.hfpthk.cn/gtkiukliqq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.gogol.net.cn/gtwzvxluzt.html

JS:   throw new Error("错误信息");
来源：http://hz.xuetiantiany.cn/gtmavskocr.html

TS:   throw new Error("错误信息");
来源：http://hz.fengsongda.top/gtxogfbuqb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.c1oappe.top/gtwdppgxfg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.cqqwz.cn/gtjofmsaav.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.havefunace.top/gtopxfjcru.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.hywenlv.cn/gteftvueig.html

[H04] 自定义异常类型
来源：http://hz.fzhhl.top/gtwhgxfect.html

Py:   class MyError(Exception): pass
来源：http://hz.hnxiangtu.top/gtykelnfie.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.sxryk.cn/gttinreyaf.html

JS:   class MyError extends Error {}
来源：http://hz.cdnleiting.top/gtfganqjtu.html

TS:   class MyError extends Error {}
来源：http://hz.zhiwuduotai.top/gtkprlqwjf.html

Java: class MyException extends RuntimeException {}
来源：http://hz.gotoacloud.top/gttyldeehb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.svipenyu.cn/gtsnuydrde.html

Ruby: class MyError < StandardError; end
来源：http://hz.havefunace.top/gtlbczqsdr.html

C#:   class MyException : Exception {}
来源：http://hz.ydjk.org.cn/gtoymhzxcd.html

[H05] 捕获特定类型
来源：http://hz.guannengcc.top/gtmjsiaibs.html

Py:   except ValueError as e:
来源：http://hz.aizwys.cn/gtqarnxqhm.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.gotoacloud.top/gtllxpkriz.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.fzhhl.top/gtoxsguizw.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jqgfzy.top/gtkcwzmsip.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.c1oappe.top/gtlubpwlkh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hnqzz.top/gtmoisjqqu.html

Ruby: rescue ArgumentError => e
来源：http://hz.meibo888.top/gtnkiwmikm.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.fzhhl.top/gtzbvrlvwz.html

[H06] 可选值 / 空值安全访问
来源：http://hz.hysaishi.cn/gtnpuydxiy.html


<!-- 参考信息 -->