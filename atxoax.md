代发 wailian999

[F01] 读取整个文件
来源：http://hz.shzxlz.cn/gtfzvjjdhh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.52xcode.cn/gtncpsejta.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zycfv.cn/gtqjrgkcrj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.sweek.top/gtesmvbrxw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jianghu66.top/gtwnonslfu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.wangdashe.top/gtjrgcmrcs.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.shzxlz.cn/gtlpgdobsh.html

Ruby: File.read("a.txt")
来源：http://hz.zdqjudy.top/gttflsigik.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.xuanzx.com/gtumyeyjca.html

[F02] 逐行读取文件
来源：http://hz.sufxvd.cn/gtwvhylstx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.meibo888.top/gtljmxhvlz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.hysaishi.cn/gtqmjfcyld.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhaomingkeji.xyz/gtqtirzruv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shanyushiyangtech.top/gtookfkjuz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jinyuanbaomall.cn/gtyxmjaphd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.daxiang520.top/gttrcmyjsg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.iojbl.cn/gtqjyqzqdk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.xuetiantiany.cn/gtbcvplckj.html

[F03] 写入文件（覆盖）
来源：http://hz.shuidangran.top/gtbwzvweji.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.daria6918.cn/gtftgvrptz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.yuxming.cn/gtlxsabgyr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yj202588.top/gtaesddrae.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.nwbrower.top/gtnfnvwnbz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.sxryk.cn/gtvksddyeh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.vqdsnc.cn/gtnqgdwjcq.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yuanzhike.top/gtlzoupcrc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.zhiwuduotai.top/gtgmavoaxj.html

[F04] 追加写入文件
来源：http://hz.cashguo.top/gtnbkotduz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.gaohongyu789.top/gtqwasdoyv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.ydzc1.top/gtpvanznni.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhoulong.xyz/gtldvqywtm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.pengpengdd.cyou/gtqacpouwb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.hongshengwenyu.top/gtpivgxkso.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.chenjidiqi.icu/gtjzeyrrhw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.bjfxy.top/gtlmwrwbzq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.sufxvd.cn/gtsqzdmvuk.html

[F05] 判断文件或目录是否存在
来源：http://hz.kuanghao11.cn/gtiqrotzed.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zhiwuduotai.top/gtesoizvvm.html

PHP:  file_exists("a.txt");
来源：http://hz.iojbl.cn/gtywvpcemx.html

JS:   fs.existsSync("a.txt")
来源：http://hz.gzhubu.top/gtyeezlsdh.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yangfankeji.com/gtrkxqffkl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.fzhhl.top/gtwnimxbla.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.aibaodan.cn/gtptbbrhgs.html

Ruby: File.exist?("a.txt")
来源：http://hz.pycfn.com/gtuxubdpcc.html

C#:   File.Exists("a.txt")
来源：http://hz.pycfn.com/gtfzguqcsb.html

[F06] 删除文件
来源：http://hz.zdqjudy.top/gtvlfzxdkc.html

Py:   os.remove("a.txt")
来源：http://hz.zhoulong.xyz/gtxzysucmx.html

PHP:  unlink("a.txt");
来源：http://hz.guowangkeji.top/gtfyccpsfa.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.gaohongyu789.top/gtphyvegoi.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.xuanzx.com/gtsuqxucvj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.hysaishi.cn/gtyhubhzxp.html

Go:   os.Remove("a.txt")
来源：http://hz.xylfe.cn/gtjdpwqbeq.html

Ruby: File.delete("a.txt")
来源：http://hz.gotoacloud.top/gtlsvbjvud.html

C#:   File.Delete("a.txt");
来源：http://hz.cqqwz.cn/gteajpwqoa.html

[F07] 创建目录（含多级）
来源：http://hz.hfpthk.cn/gtikisspox.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.chenjidiqi.icu/gtwrdpzxjm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.snrcjt.cn/gtdlapoclk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.andypj.xyz/gtomfxiyts.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.quarkkingdee.top/gtltjbwhet.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.zhongyouzk.top/gtglyikysv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.birdmap.top/gtibhedane.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yvedp.cn/gtavxmucux.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.hysaishi.cn/gtkhdgptjo.html

[F08] 遍历目录
来源：http://hz.xingfuxueyuan.xyz/gtiuggqlqu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zhoulong.xyz/gtwntzrdek.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jinqigufen.top/gtlcgqzrik.html

JS:   fs.readdirSync("dir")
来源：http://hz.xylfe.cn/gtelfkphze.html

TS:   fs.readdirSync("dir")
来源：http://hz.52xcode.cn/gtrebnsjfm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yj20258888.top/gtiilrxzax.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.tanke756.top/gttwceqszg.html

Ruby: Dir.children("dir")
来源：http://hz.mhx1999.top/gtitnqfsim.html

C#:   Directory.GetFiles("dir")
来源：http://hz.ybcxt.top/gtxsjepljo.html

[F09] 获取文件大小
来源：http://hz.hywenlv.cn/gtewywvfnu.html

Py:   os.path.getsize("a.txt")
来源：http://hz.ydzc1.top/gtcfxeyhme.html

PHP:  filesize("a.txt");
来源：http://hz.chenlongwang.top/gtbrrlcbgk.html

JS:   fs.statSync("a.txt").size
来源：http://hz.xuanzx.com/gtywagvdmb.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zhiwuduotai.top/gtpikrolgg.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.aibaodan.cn/gtzwhxzpiw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yuanzhike.top/gtzgyffijx.html

Ruby: File.size("a.txt")
来源：http://hz.sufxvd.cn/gtjvkbrorg.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.cdnleiting.top/gtgoswujjj.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.pengpengdd.cyou/gtampwqfjx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zhoulong.xyz/gtdbylwjcq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.quarkkingdee.top/gtdxmotzrm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.xinyue.icu/gtherfqnqk.html

TS:   path.extname("a.txt")
来源：http://hz.hfpthk.cn/gtryyntome.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jinqigfzy.top/gtjzhqsweo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.ehwqpu.com/gtdfxgthow.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.daria6918.cn/gtmrbtbyyl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.chenjidiqi.icu/gtvvlergjx.html

[F11] 复制与移动文件
来源：http://hz.sxryk.cn/gtbgrgxbej.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.chenjidiqi.icu/gtdcdkjelk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.sweek.top/gtfeuouvci.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.wangdashe.top/gtwnaazbaw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jqgufenzy.top/gtsdvcxnkb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.nanxinkj.top/gtrxzvbvfd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.hnqzz.top/gtztybjpvc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.gotoacloud.top/gtxbuqgksw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.guannengcc.top/gtnenpwckw.html

[F12] CSV 读写
来源：http://hz.vqdsnc.cn/gtqhdnbfsz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yj202588.top/gtgbdmzhdc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hnqzz.top/gtypdrtouk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jinyuanbaomall.cn/gteufucwqb.html

TS:   // 同上
来源：http://hz.gogol.net.cn/gtjbdnpskf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.chenzaomai.com/gtxzbwziww.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yj20258.top/gtemlezszo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.shuidangran.top/gtvmrlzsqt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.shzxlz.cn/gtmhyjimzn.html

================================================================================
来源：http://hz.jinqigufen.top/gtpaomgcrz.html

G. 面向对象
来源：http://hz.nwbrower.top/gthzmqxork.html

================================================================================
来源：http://hz.0kj1m.cn/gtjpwazggh.html

[G01] 定义类
来源：http://hz.sxryk.cn/gtfktzfltp.html

Py:   class User: pass
来源：http://hz.ppjwa.cn/gtegabewcn.html

PHP:  class User {}
来源：http://hz.ydjk.org.cn/gtqnoklpxv.html

JS:   class User {}
来源：http://hz.nanxinkj.top/gtlkydqpcu.html

TS:   class User { name: string = ""; }
来源：http://hz.sxryk.cn/gtwewicztb.html

Java: class User {}
来源：http://hz.bjfxy.top/gtdljhbenn.html

Go:   type User struct { Name string }
来源：http://hz.yongpay.top/gtmnaqftem.html

Ruby: class User; end
来源：http://hz.bjfxy.top/gtsrwybckx.html

C#:   class User {}
来源：http://hz.hongshengwenyu.top/gthitexxlc.html

[G02] 构造函数
来源：http://hz.jyoumei.cn/gtengisbez.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yongpay.top/gtzsfqopzo.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.tanke756.top/gtecaqrcbs.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jinqigfzy.top/gtsdjoislx.html

TS:   constructor(public name: string) {}
来源：http://hz.hnqzz.top/gtugbfxwst.html

Java: User(String name) { this.name = name; }
来源：http://hz.zhixingplan.top/gtulmzuzgk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.wangshuangyany.cn/gtpgqxcpjd.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.cheryme.top/gtiuloyezj.html

C#:   public User(string name) { Name = name; }
来源：http://hz.shzxlz.cn/gtnhpjkctl.html

[G03] 实例属性
来源：http://hz.iojbl.cn/gtmbhvevpv.html

Py:   self.name = "x"
来源：http://hz.fengsongda.top/gtpmrqsjrr.html

PHP:  public string $name = "x";
来源：http://hz.jqgufenzy.top/gtfrvkmjwq.html

JS:   this.name = "x";
来源：http://hz.gaohongyu789.top/gtlyhkbihs.html

TS:   name: string = "x";
来源：http://hz.yangfankeji.com/gtyebcjidq.html

Java: private String name;
来源：http://hz.cucudq.cn/gtmvlmjakn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.shuidangran.top/gtcsztfell.html

Ruby: @name = "x"
来源：http://hz.ivvv.top/gtprvynfns.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.dianchejie.cn/gtnjbmjtkf.html

[G04] 定义方法
来源：http://hz.sufxvd.cn/gthlgrobmu.html

Py:   def greet(self): return self.name
来源：http://hz.dianchejie.cn/gtdycqwchg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.tian-w.cn/gttqdwfsxt.html

JS:   greet() { return this.name; }
来源：http://hz.xuetiantiany.cn/gtstxnsmry.html

TS:   greet(): string { return this.name; }
来源：http://hz.tian-w.cn/gtkmanfxrd.html

Java: String greet() { return name; }
来源：http://hz.vqdsnc.cn/gtscbloqjb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.xuetiantiany.cn/gtqbziyukd.html

Ruby: def greet; @name; end
来源：http://hz.meibo888.top/gtyiypxwwg.html

C#:   public string Greet() => Name;
来源：http://hz.andypj.xyz/gtmqxpaoyb.html

[G05] 继承
来源：http://hz.aizwys.cn/gtfmjgiwzo.html

Py:   class Admin(User): pass
来源：http://hz.yueranfly.top/gtoagwxqkr.html

PHP:  class Admin extends User {}
来源：http://hz.yueranfly.top/gtdlqiffsv.html

JS:   class Admin extends User {}
来源：http://hz.haohaochexian.top/gtfbtaabbf.html

TS:   class Admin extends User {}
来源：http://hz.hfpthk.cn/gtuwszvwdj.html

Java: class Admin extends User {}
来源：http://hz.xziqi.cn/gtdufeckgn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.fengsongda.top/gttsledkgm.html

Ruby: class Admin < User; end
来源：http://hz.shzxlz.cn/gtxivfhbvj.html

C#:   class Admin : User {}
来源：http://hz.zhijiandao.cn/gtamcvjzxa.html

[G06] 重写方法
来源：http://hz.hysaishi.cn/gtvhokrnga.html

Py:   def greet(self): return "admin"
来源：http://hz.daria6918.cn/gtndzrbcup.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.andypj.xyz/gtdepqbqvf.html

JS:   greet() { return "admin"; }
来源：http://hz.cdnleiting.top/gtwrfkuosi.html

TS:   greet(): string { return "admin"; }
来源：http://hz.cqqwz.cn/gtogaqkuqj.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.c1oappe.top/gtbnkegeyq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.wangdashe.top/gtmrpewpsq.html

Ruby: def greet; "admin"; end
来源：http://hz.wangdashe.top/gtpyralndi.html

C#:   public override string Greet() => "admin";
来源：http://hz.tian-w.cn/gtozhqlwde.html

[G07] 调用父类方法
来源：http://hz.yanxiufei.cn/gtcdnjwshd.html

Py:   super().greet()
来源：http://hz.zhoulong.xyz/gtqnirwjev.html

PHP:  parent::greet();
来源：http://hz.dashuyun.cn/gtpqqyuosf.html

JS:   super.greet();
来源：http://hz.wangshuangyany.cn/gtwcavbcbi.html

TS:   super.greet();
来源：http://hz.jlsjyb.cn/gtvhjfupgz.html

Java: super.greet();
来源：http://hz.chenjidiqi.icu/gtuxrasyos.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.gaohongyu789.top/gtgtgyopup.html

Ruby: super
来源：http://hz.shzxlz.cn/gtgrbqgvun.html

C#:   base.Greet();
来源：http://hz.zycfv.cn/gtzddseaqy.html

[G08] 静态方法与属性
来源：http://hz.meibo888.top/gtflslvptt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.daxiang520.top/gtdbcwsras.html

PHP:  public static function f() {}
来源：http://hz.yangfankeji.com/gtnflbwsyp.html

JS:   static f() {}
来源：http://hz.andypj.xyz/gtpodcgnef.html

TS:   static f(): void {}
来源：http://hz.pycfn.com/gtngekqrya.html

Java: static void f() {}
来源：http://hz.ivvv.top/gtxqapggaq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.cdnleiting.top/gtrpqzevpc.html

Ruby: def self.f; end
来源：http://hz.nwbrower.top/gtuvcaneeq.html

C#:   public static void F() {}
来源：http://hz.aibaodan.cn/gtaaxzjgiz.html

[G09] 接口 / 抽象类
来源：http://hz.zhaomingkeji.xyz/gthozzklwt.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.gotoacloud.top/gtqzvduylq.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.chenzaomai.com/gtpghezzkm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.nanxinkj.top/gtysppzyyi.html

TS:   interface Shape { area(): number; }
来源：http://hz.mhx1999.top/gtmfjyublk.html

Java: interface Shape { double area(); }
来源：http://hz.gotoacloud.top/gtdpiyvers.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.sysykeji.top/gttmqfulhk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhongyouzk.top/gttwnllodi.html

C#:   interface IShape { double Area(); }
来源：http://hz.316326.xyz/gtihgkqnvv.html

[G10] 访问控制
来源：http://hz.yuanzhike.top/gtbxicojii.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.sxryk.cn/gtsapiaskj.html

PHP:  public / protected / private
来源：http://hz.jinqigufen.top/gttbugwvaa.html

JS:   #private 字段；其余公开
来源：http://hz.cucudq.cn/gtaexeazvq.html

TS:   public / protected / private
来源：http://hz.zhengqikj.top/gtexrwctqz.html

Java: public / protected / private / 默认包级
来源：http://hz.jinyuanbaomall.cn/gtxpeqpqdc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ydzc1.top/gtbtedyvyh.html

Ruby: public / protected / private
来源：http://hz.gzhubu.top/gtqlerzfrk.html

C#:   public / protected / private / internal
来源：http://hz.yvedp.cn/gtqhfcsvko.html

[G11] getter / setter
来源：http://hz.tian-w.cn/gtlyhrshig.html

Py:   @property 与 @x.setter
来源：http://hz.nwbrower.top/gtvccqefco.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhoulong.xyz/gtnjihriwa.html

JS:   get name() { return this._name; }
来源：http://hz.jyoumei.cn/gtmfugkybz.html

TS:   get name(): string { return this._name; }
来源：http://hz.ywan-chungtsiang.top/gtcvquxpnv.html

Java: public String getName() { return name; }
来源：http://hz.hysaishi.cn/gtkzubqtts.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jinqigufen.top/gtdkwbebdu.html

Ruby: attr_accessor :name
来源：http://hz.zhixingplan.top/gtcoczhkfs.html

C#:   public string Name { get; set; }
来源：http://hz.52xcode.cn/gtnfzuxgri.html

[G12] 对象转字符串
来源：http://hz.zhengqikj.top/gtusvpfphz.html

Py:   def __str__(self): return self.name
来源：http://hz.guowangkeji.top/gtoyfhtinh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.cdnleiting.top/gtzafgtiun.html

JS:   toString() { return this.name; }
来源：http://hz.gotoacloud.top/gttfhcghoi.html

TS:   toString(): string { return this.name; }
来源：http://hz.tianlin.xyz/gtfcepfuwn.html

Java: @Override public String toString() { return name; }
来源：http://hz.cashguo.top/gtmsuddkhf.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhongyouzk.top/gtzvkzquqr.html

Ruby: def to_s; @name; end
来源：http://hz.xingfuxueyuan.xyz/gtijyrdhrh.html

C#:   public override string ToString() => Name;
来源：http://hz.dianchejie.cn/gtkbxulooz.html

[G13] 判断对象类型
来源：http://hz.zhijiandao.cn/gtigwjzhbg.html

Py:   isinstance(u, User)
来源：http://hz.meibo888.top/gtakkbbjvu.html

PHP:  $u instanceof User
来源：http://hz.zdqjudy.top/gtvjtlpiad.html

JS:   u instanceof User
来源：http://hz.xingfuxueyuan.xyz/gtzqepbuem.html

TS:   u instanceof User
来源：http://hz.c1oappe.top/gtaqfxshjo.html

Java: u instanceof User
来源：http://hz.hongshengwenyu.top/gtlncolkbg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.tianlin.xyz/gtuwytcvho.html

Ruby: u.is_a?(User)
来源：http://hz.ybcxt.top/gtrylqnsrm.html

C#:   u is User
来源：http://hz.yonumen.top/gtwyxnqzsy.html

[G14] 数据类 / record
来源：http://hz.jyoumei.cn/gtvmovpvfp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yangfankeji.com/gtzjmzwclw.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yuxming.cn/gtbonjtdgw.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.svipenyu.cn/gthnwltejt.html

TS:   type User = { name: string; age: number };
来源：http://hz.xylfe.cn/gtgaeumqrk.html

Java: record User(String name, int age) {}
来源：http://hz.guannengcc.top/gtqmyygcvk.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zhixingplan.top/gtdiikloos.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.cucudq.cn/gtqmpwcjva.html

C#:   record User(string Name, int Age);
来源：http://hz.snrcjt.cn/gtoaaeayai.html

[G15] 枚举
来源：http://hz.zhongyouzk.top/gtllskziyy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yonumen.top/gtxfvwjhjg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.cashguo.top/gtdqupvrtx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.wangdashe.top/gtyvonmmea.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.mhx1999.top/gtdvwlgibj.html

Java: enum Color { RED, GREEN }
来源：http://hz.zhoulong.xyz/gteowucwxm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jinyuanbaomall.cn/gtkkbhsvmm.html

Ruby: Color = %i[red green].freeze
来源：http://hz.chenlongwang.top/gtzddfedun.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.snrcjt.cn/gtughlhfxo.html

[G16] 对象转数组 / 字典
来源：http://hz.gogol.net.cn/gtquhupvrp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.ywan-chungtsiang.top/gtjmbdnuyx.html

PHP:  get_object_vars($obj);
来源：http://hz.xylfe.cn/gtrqhxjkgx.html

JS:   Object.entries(obj)
来源：http://hz.zhoulong.xyz/gtmdqrpxjr.html

TS:   Object.entries(obj)
来源：http://hz.jinyuanbaomall.cn/gtzizuirqa.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.shanyushiyangtech.top/gtmeywkbke.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.dashuyun.cn/gtzyedksoy.html

Ruby: obj.instance_variables
来源：http://hz.sufxvd.cn/gtthowpvwq.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.ydzc1.top/gtaywtnpmb.html

================================================================================
来源：http://hz.cheryme.top/gtmtrdqowk.html

H. 异常与错误处理
来源：http://hz.cheryme.top/gtlqpuugwo.html

================================================================================
来源：http://hz.sufxvd.cn/gtyivoffpj.html

[H01] try / catch 基础
来源：http://hz.shzxlz.cn/gtfcxgboot.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.dashuyun.cn/gtehqdpqxo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.gogol.net.cn/gtxvinrkdl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.ywan-chungtsiang.top/gtisoqtxpb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.dianchejie.cn/gtxjxmtxyt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zhiwuduotai.top/gtkpopuzui.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jinghuilouyu.cn/gtiftuvkob.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yj202588.top/gtlzvsdqez.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.chenzaomai.com/gtnkizdoeh.html

[H02] finally / ensure 收尾
来源：http://hz.iojbl.cn/gtzaatefjr.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zdqjudy.top/gtsswbizjw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xylfe.cn/gtecgddkst.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hongshengwenyu.top/gtdodrnsbe.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yvedp.cn/gtvjhntzpw.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zdqjudy.top/gtydijclea.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ppjwa.cn/gtntmedpka.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.zhengqikj.top/gtbgygeqsa.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.cheryme.top/gtdvrbdvwe.html

[H03] 主动抛出异常
来源：http://hz.wangshuangyany.cn/gtnirjzzea.html

Py:   raise ValueError("错误信息")
来源：http://hz.yuxming.cn/gtvbpdgxgz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.c1oappe.top/gtkfmgrjaj.html

JS:   throw new Error("错误信息");
来源：http://hz.jinyuanbaomall.cn/gtfkiwavoe.html

TS:   throw new Error("错误信息");
来源：http://hz.vqdsnc.cn/gtbxjmkakb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.gaohongyu789.top/gtlptinlcf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yangfankeji.com/gtxzgnuswx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.birdmap.top/gtpqjmupfr.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.cdnleiting.top/gtddhqlxxp.html

[H04] 自定义异常类型
来源：http://hz.52xcode.cn/gtjabaeilf.html

Py:   class MyError(Exception): pass
来源：http://hz.ywan-chungtsiang.top/gtaksiooak.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jyoumei.cn/gtcbroeqwk.html

JS:   class MyError extends Error {}
来源：http://hz.cucudq.cn/gtcjnygvlg.html

TS:   class MyError extends Error {}
来源：http://hz.yueranfly.top/gteharkdfd.html

Java: class MyException extends RuntimeException {}
来源：http://hz.shzxlz.cn/gtzgwivmrl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ybcxt.top/gtransinna.html

Ruby: class MyError < StandardError; end
来源：http://hz.shanyushiyangkeji.top/gtzwncxdor.html

C#:   class MyException : Exception {}
来源：http://hz.cdnleiting.top/gtukyocvqa.html

[H05] 捕获特定类型
来源：http://hz.zhixingplan.top/gtpkqggpoe.html

Py:   except ValueError as e:
来源：http://hz.xuanzx.com/gtwksxzyeq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yangfankeji.com/gtwmxooygp.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zhaomingkeji.xyz/gteqwjkbog.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhengqikj.top/gtdajfkudj.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.dashuyun.cn/gtxhgkxyqu.html


<!-- 参考信息 -->