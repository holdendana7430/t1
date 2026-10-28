代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.quarkkingdee.top/gtedkkqdex.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.shanyushiyangtech.top/gtzawuksxg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yuxming.cn/gtnczzggdt.html

Ruby: s.bytesize;  s.length
来源：http://hz.zhaomingkeji.xyz/gtyfpnupgr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.aibaodan.cn/gtfuiucwlg.html

================================================================================
来源：http://hz.ppjwa.cn/gtcxxoyiwk.html

F. 文件与目录
来源：http://hz.zhijiandao.cn/gthqkpilxt.html

================================================================================
来源：http://hz.svipenyu.cn/gtntiyvfkx.html

[F01] 读取整个文件
来源：http://hz.jinyuanbaomall.cn/gtfsihfypx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.nwbrower.top/gttmrnsfbd.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yueranfly.top/gtnzkpenki.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.pengpengdd.cyou/gtftzcwhrj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.cqqwz.cn/gtcqazmnql.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.wangdashe.top/gtjjwrnsfc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhijiandao.cn/gtunewitcg.html

Ruby: File.read("a.txt")
来源：http://hz.dashuyun.cn/gtauqaudan.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.tianlin.xyz/gtnojamhrz.html

[F02] 逐行读取文件
来源：http://hz.feifeiyinyue.top/gttcfmqoet.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.cashguo.top/gtqrlekemc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.guowangkeji.top/gtixuqyurq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hammf.cn/gtzngeigjc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.meibo888.top/gtudwvocbi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jinqigufen.top/gtzwaeolne.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zhengqikj.top/gtuzipiomx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.tianlin.xyz/gtygazhufz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhaomingkeji.xyz/gtpqvvcruh.html

[F03] 写入文件（覆盖）
来源：http://hz.zycfv.cn/gtmgocghnr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.daxiang520.top/gtzkbusdfy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.shanyushiyangkeji.top/gtexkveses.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.wangdashe.top/gtivkktblj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.fengsongda.top/gtdrashlyf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.shanyushiyangkeji.top/gtkeqwdngu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.ydjk.org.cn/gtitwchgzf.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.vqdsnc.cn/gtokopdumd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.shanyushiyangkeji.top/gtgrgecidl.html

[F04] 追加写入文件
来源：http://hz.52xcode.cn/gtbjzfncix.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.pycfn.com/gtawbxfils.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yanxiufei.cn/gtlhigpfkb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.pengpengdd.cyou/gtkvhrenun.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xziqi.cn/gtcfypscwq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.shangyingyoupin.top/gtdhtjcnqv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.nwbrower.top/gtqvnjuojt.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.tian-w.cn/gtccktqlho.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.vqdsnc.cn/gtoqewmsdy.html

[F05] 判断文件或目录是否存在
来源：http://hz.ehwqpu.com/gtobhyjags.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.dianchejie.cn/gttficajkx.html

PHP:  file_exists("a.txt");
来源：http://hz.yvedp.cn/gtcawuvnnh.html

JS:   fs.existsSync("a.txt")
来源：http://hz.ehwqpu.com/gtkdafsvoe.html

TS:   fs.existsSync("a.txt")
来源：http://hz.gaohongyu789.top/gtjlkklmfs.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hongshengwenyu.top/gtfnqgqpwx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.fengsongda.top/gthaerlivu.html

Ruby: File.exist?("a.txt")
来源：http://hz.zhoulong.xyz/gtibzkkgin.html

C#:   File.Exists("a.txt")
来源：http://hz.guowangkeji.top/gtxpopgskj.html

[F06] 删除文件
来源：http://hz.quarkkingdee.top/gtqnlnihal.html

Py:   os.remove("a.txt")
来源：http://hz.ppjwa.cn/gtcjddxejx.html

PHP:  unlink("a.txt");
来源：http://hz.wangdashe.top/gtdojsyidl.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.jqgufenzy.top/gtptprjpmx.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.meibo888.top/gtrgdttgkj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.birdmap.top/gtgdplqrqj.html

Go:   os.Remove("a.txt")
来源：http://hz.yuxming.cn/gtxopzeyak.html

Ruby: File.delete("a.txt")
来源：http://hz.birdmap.top/gtobpwlbrb.html

C#:   File.Delete("a.txt");
来源：http://hz.iojbl.cn/gtmyhpnzrq.html

[F07] 创建目录（含多级）
来源：http://hz.smart0.xyz/gtcgzamnur.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.fzhhl.top/gtcmrwgzru.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.gaohongyu789.top/gtrshczdoh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.daxiang520.top/gthysbqttz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cashguo.top/gtptzizjuh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.tanke756.top/gtrcfbtvji.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.cucudq.cn/gtcwfjdifl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.tianlin.xyz/gtqwypifwr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.ydzc1.top/gttgniqnzy.html

[F08] 遍历目录
来源：http://hz.tianlin.xyz/gtqzixzjzh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.quarkkingdee.top/gtepeekvwc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.ydjk.org.cn/gtcqdnygvh.html

JS:   fs.readdirSync("dir")
来源：http://hz.feifeiyinyue.top/gtsifbdxsc.html

TS:   fs.readdirSync("dir")
来源：http://hz.jiagoushi.top/gtodzwzqnv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.cucudq.cn/gtdjuacboe.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.c1oappe.top/gtietqifug.html

Ruby: Dir.children("dir")
来源：http://hz.shzxlz.cn/gtlxcwuehs.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zhengqikj.top/gtshhhqzeu.html

[F09] 获取文件大小
来源：http://hz.yanxiufei.cn/gtyvmhdgma.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yj202588.top/gtkofkmqvg.html

PHP:  filesize("a.txt");
来源：http://hz.feifeiyinyue.top/gtrmwxaftb.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jinyuanbaomall.cn/gtqmutgkwg.html

TS:   fs.statSync("a.txt").size
来源：http://hz.ehwqpu.com/gtixxymsvs.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.redwolf501.top/gtpqmgcltz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yueranfly.top/gtuwpfeqzp.html

Ruby: File.size("a.txt")
来源：http://hz.sufxvd.cn/gtplvzkrrt.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.sysykeji.top/gtvfugqmmv.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.haohaochexian.top/gtioybkgcu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zhixingplan.top/gtklaggaeb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.meibo888.top/gtudcnglho.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.aibaodan.cn/gtbqaoxazp.html

TS:   path.extname("a.txt")
来源：http://hz.quarkkingdee.top/gtgnuybmsz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.chenjidiqi.icu/gtievjkoev.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.316326.xyz/gtmjuiiull.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yvedp.cn/gtynohhlxr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jinyuanbaomall.cn/gtdodecpng.html

[F11] 复制与移动文件
来源：http://hz.meibo888.top/gtnmkxbjnc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.hongshengwenyu.top/gtyocvaqwx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.fengsongda.top/gtwheoqswc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cqqwz.cn/gtirprizqz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhiwuduotai.top/gtzraesbsm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.shanyushiyangtech.top/gtscvpxuyj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.pengpengdd.cyou/gtiwgksbnk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.pycfn.com/gtfrtomium.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.hammf.cn/gtmyusbohs.html

[F12] CSV 读写
来源：http://hz.gaohongyu789.top/gtrjwgetvp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yvedp.cn/gtxljdnyop.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yj202588.top/gtcslowjgy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.aibaodan.cn/gtuhgsjnps.html

TS:   // 同上
来源：http://hz.hnqzz.top/gtdaxzvmea.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.birdmap.top/gtvemxfwqd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.sweek.top/gtnvkrvqws.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.xingfuxueyuan.xyz/gteklptwtp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jianghu66.top/gtmtvrmdqg.html

================================================================================
来源：http://hz.yanxiufei.cn/gtuoyxrhht.html

G. 面向对象
来源：http://hz.zhaomingkeji.xyz/gtawkgazmn.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtnwvngakz.html

[G01] 定义类
来源：http://hz.yuxming.cn/gtendxccys.html

Py:   class User: pass
来源：http://hz.zhiwuduotai.top/gtmsqrgkvu.html

PHP:  class User {}
来源：http://hz.yvedp.cn/gtbhoklduy.html

JS:   class User {}
来源：http://hz.jinqigufen.top/gtffqmrnij.html

TS:   class User { name: string = ""; }
来源：http://hz.smart0.xyz/gthsnwthxj.html

Java: class User {}
来源：http://hz.yangfankeji.com/gtmoesrvdn.html

Go:   type User struct { Name string }
来源：http://hz.sysykeji.top/gtqxmzmcsy.html

Ruby: class User; end
来源：http://hz.snrcjt.cn/gthgdmtpqs.html

C#:   class User {}
来源：http://hz.jlsjyb.cn/gtaofkjavt.html

[G02] 构造函数
来源：http://hz.jinghuilouyu.cn/gtvvpytoab.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.vqdsnc.cn/gtfiiqkkiw.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.cheryme.top/gtnatjcehp.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jinqigfzy.top/gtlibtfbou.html

TS:   constructor(public name: string) {}
来源：http://hz.zhengqikj.top/gtyulkgyrw.html

Java: User(String name) { this.name = name; }
来源：http://hz.jinqigufen.top/gtxlkyccrg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.fzhhl.top/gtofrlodfb.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.iojbl.cn/gtlqrzbvec.html

C#:   public User(string name) { Name = name; }
来源：http://hz.svipenyu.cn/gtyeapuvql.html

[G03] 实例属性
来源：http://hz.smart0.xyz/gtryflwovk.html

Py:   self.name = "x"
来源：http://hz.shuidangran.top/gtfcfqvufp.html

PHP:  public string $name = "x";
来源：http://hz.shanyushiyangkeji.top/gtknqoeico.html

JS:   this.name = "x";
来源：http://hz.cashguo.top/gtfcrercxq.html

TS:   name: string = "x";
来源：http://hz.tanke756.top/gtmfousous.html

Java: private String name;
来源：http://hz.hywenlv.cn/gtjyyktlay.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hysaishi.cn/gtpanzhklf.html

Ruby: @name = "x"
来源：http://hz.sxryk.cn/gtlejoojat.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jqgfzy.top/gtdovurxwp.html

[G04] 定义方法
来源：http://hz.ydjk.org.cn/gtrgactamu.html

Py:   def greet(self): return self.name
来源：http://hz.9152youxi.cn/gtyphxmvui.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.wangdashe.top/gtrxkuoxys.html

JS:   greet() { return this.name; }
来源：http://hz.ppjwa.cn/gtlphtvsjl.html

TS:   greet(): string { return this.name; }
来源：http://hz.shanyushiyangkeji.top/gtacbiskyf.html

Java: String greet() { return name; }
来源：http://hz.yongpay.top/gtxovysfry.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.52xcode.cn/gtufdsipbc.html

Ruby: def greet; @name; end
来源：http://hz.9152youxi.cn/gtaqdhqhif.html

C#:   public string Greet() => Name;
来源：http://hz.tianlin.xyz/gtdkvjvmmi.html

[G05] 继承
来源：http://hz.yanxiufei.cn/gtopgrslog.html

Py:   class Admin(User): pass
来源：http://hz.yj20258888.top/gtnkuqslbz.html

PHP:  class Admin extends User {}
来源：http://hz.jinqigfzy.top/gtyejmpxpd.html

JS:   class Admin extends User {}
来源：http://hz.chenzaomai.com/gtpweyksdp.html

TS:   class Admin extends User {}
来源：http://hz.xylfe.cn/gtlcghobqk.html

Java: class Admin extends User {}
来源：http://hz.cdnleiting.top/gtzozjnbfr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.cheryme.top/gtgetkjjgy.html

Ruby: class Admin < User; end
来源：http://hz.gogol.net.cn/gtnngnrgnd.html

C#:   class Admin : User {}
来源：http://hz.kuanghao11.cn/gtrftvuqsa.html

[G06] 重写方法
来源：http://hz.ybcxt.top/gtmdwcpsew.html

Py:   def greet(self): return "admin"
来源：http://hz.fengsongda.top/gtokbwdrxa.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.sysykeji.top/gtboyckzts.html

JS:   greet() { return "admin"; }
来源：http://hz.wangdashe.top/gtnxfqsaig.html

TS:   greet(): string { return "admin"; }
来源：http://hz.nwbrower.top/gtepeenwtj.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.aibaodan.cn/gtpmaniewd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.cqqwz.cn/gttdtxfccr.html

Ruby: def greet; "admin"; end
来源：http://hz.wangdashe.top/gtwixyzebl.html

C#:   public override string Greet() => "admin";
来源：http://hz.yuanzhike.top/gtgmgqrisv.html

[G07] 调用父类方法
来源：http://hz.jqgufenzy.top/gtyzssoetq.html

Py:   super().greet()
来源：http://hz.fzhhl.top/gtgkqxktvx.html

PHP:  parent::greet();
来源：http://hz.hywenlv.cn/gtqdruvrxc.html

JS:   super.greet();
来源：http://hz.jyoumei.cn/gttuaslnrr.html

TS:   super.greet();
来源：http://hz.yvedp.cn/gtzvgfouzr.html

Java: super.greet();
来源：http://hz.pycfn.com/gtvtyydfdn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jqgufenzy.top/gtgoyoulxs.html

Ruby: super
来源：http://hz.9152youxi.cn/gtgzhykemx.html

C#:   base.Greet();
来源：http://hz.quarkkingdee.top/gtcqxtfbpq.html

[G08] 静态方法与属性
来源：http://hz.ywan-chungtsiang.top/gtffucxsbz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.sweek.top/gtbojwibve.html

PHP:  public static function f() {}
来源：http://hz.sysykeji.top/gtnvulogxj.html

JS:   static f() {}
来源：http://hz.tianlin.xyz/gtysuklvan.html

TS:   static f(): void {}
来源：http://hz.havefunace.top/gtthwmsyph.html

Java: static void f() {}
来源：http://hz.yuxming.cn/gtovvvphwj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.xuetiantiany.cn/gtpajtodjb.html

Ruby: def self.f; end
来源：http://hz.jinyuanbaomall.cn/gtwxsczsmz.html

C#:   public static void F() {}
来源：http://hz.haohaochexian.top/gtgdgrjeir.html

[G09] 接口 / 抽象类
来源：http://hz.chenjidiqi.icu/gtislferhh.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.chenlongwang.top/gtudjiepxb.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jinyuanbaomall.cn/gthsyccooj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.nanxuanxn.top/gtkjqvjjqa.html

TS:   interface Shape { area(): number; }
来源：http://hz.yvedp.cn/gtkkooslcu.html

Java: interface Shape { double area(); }
来源：http://hz.redwolf501.top/gtciobzzwb.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.daria6918.cn/gtmpckofcp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jlsjyb.cn/gtkoimesap.html

C#:   interface IShape { double Area(); }
来源：http://hz.hysaishi.cn/gtqjwfdkeb.html

[G10] 访问控制
来源：http://hz.meibo888.top/gtsllujyps.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.xuetiantiany.cn/gtyqhdzzow.html

PHP:  public / protected / private
来源：http://hz.52xcode.cn/gtgdwkesmw.html

JS:   #private 字段；其余公开
来源：http://hz.jinyuanbaomall.cn/gtkxucuchr.html

TS:   public / protected / private
来源：http://hz.nanxinkj.top/gtarvyuvli.html

Java: public / protected / private / 默认包级
来源：http://hz.zhixingplan.top/gtajlqzzog.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.hfpthk.cn/gtxwwjnqny.html

Ruby: public / protected / private
来源：http://hz.mhx1999.top/gtlnwbjyai.html

C#:   public / protected / private / internal
来源：http://hz.meibo888.top/gtzgzduyrx.html

[G11] getter / setter
来源：http://hz.jqgufenzy.top/gtpdiqvvai.html

Py:   @property 与 @x.setter
来源：http://hz.jlsjyb.cn/gtqbacjqdh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhixingplan.top/gtptbzjyxw.html

JS:   get name() { return this._name; }
来源：http://hz.jinghuilouyu.cn/gtytmttngp.html

TS:   get name(): string { return this._name; }
来源：http://hz.jianghu66.top/gteukuamfc.html

Java: public String getName() { return name; }
来源：http://hz.guannengcc.top/gtguxcydez.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.sysykeji.top/gtqwtqszvc.html

Ruby: attr_accessor :name
来源：http://hz.guannengcc.top/gtrkkprvzn.html

C#:   public string Name { get; set; }
来源：http://hz.yangfankeji.com/gtsdssoazv.html

[G12] 对象转字符串
来源：http://hz.yanxiufei.cn/gtqjipfxmu.html

Py:   def __str__(self): return self.name
来源：http://hz.nanxuanxn.top/gttzckfmrx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.xingfuxueyuan.xyz/gtfpjucqhf.html

JS:   toString() { return this.name; }
来源：http://hz.jinyuanbaomall.cn/gtwxgnyqpe.html

TS:   toString(): string { return this.name; }
来源：http://hz.nanxuanxn.top/gtorfxkswk.html

Java: @Override public String toString() { return name; }
来源：http://hz.ehwqpu.com/gtltyffcrb.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.dianchejie.cn/gtwqgmlhud.html

Ruby: def to_s; @name; end
来源：http://hz.sxryk.cn/gtkzcardfe.html

C#:   public override string ToString() => Name;
来源：http://hz.xuanzx.com/gtmjpzwuet.html

[G13] 判断对象类型
来源：http://hz.fzhhl.top/gtitjbnttb.html

Py:   isinstance(u, User)
来源：http://hz.feifeiyinyue.top/gtfhwhpohm.html

PHP:  $u instanceof User
来源：http://hz.zycfv.cn/gtrajfsuwg.html

JS:   u instanceof User
来源：http://hz.haohaochexian.top/gtsbvwzofi.html

TS:   u instanceof User
来源：http://hz.vqdsnc.cn/gtvbtivxfl.html

Java: u instanceof User
来源：http://hz.ybcxt.top/gtwbxmgsql.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.cdnleiting.top/gthqgxrkbl.html

Ruby: u.is_a?(User)
来源：http://hz.guowangkeji.top/gtdluibagh.html

C#:   u is User
来源：http://hz.shzxlz.cn/gtbvlmvcno.html

[G14] 数据类 / record
来源：http://hz.yj20258.top/gtnbwqjmon.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yj20258.top/gtgsaossgg.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.cdnleiting.top/gtrlrxomkj.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.wangdashe.top/gtzbbtwkdf.html

TS:   type User = { name: string; age: number };
来源：http://hz.cdnleiting.top/gttkybbvlz.html

Java: record User(String name, int age) {}
来源：http://hz.yj202588.top/gtmyhdzgkq.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jqgufenzy.top/gtocxhyakm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.9152youxi.cn/gtdyboxgwc.html

C#:   record User(string Name, int Age);
来源：http://hz.gotoacloud.top/gtvruczffv.html

[G15] 枚举
来源：http://hz.jinqigufen.top/gtuuxewlwu.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.shanyushiyangkeji.top/gthwnloolj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.pengpengdd.cyou/gthnzspahv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.sweek.top/gtdfnvondf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.wangshuangyany.cn/gtgjwcicjq.html

Java: enum Color { RED, GREEN }
来源：http://hz.shanyushiyangtech.top/gtpwbglbyp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ywan-chungtsiang.top/gtfucahbwg.html

Ruby: Color = %i[red green].freeze
来源：http://hz.sufxvd.cn/gtxslgxiur.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhijiandao.cn/gtfwfesbif.html

[G16] 对象转数组 / 字典
来源：http://hz.redwolf501.top/gtytcdsdza.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.gzhubu.top/gtqeawsmib.html

PHP:  get_object_vars($obj);
来源：http://hz.hfpthk.cn/gttcjbultp.html

JS:   Object.entries(obj)
来源：http://hz.xinyue.icu/gttynytipz.html

TS:   Object.entries(obj)
来源：http://hz.ydzc1.top/gtrrexnacw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ybcxt.top/gtllivnydx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.chenzaomai.com/gtiaffhlto.html

Ruby: obj.instance_variables
来源：http://hz.guowangkeji.top/gtmoamewqf.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.daxiang520.top/gtgptdlkrn.html

================================================================================
来源：http://hz.aizwys.cn/gtsbhzlnnl.html

H. 异常与错误处理
来源：http://hz.sweek.top/gtrtqpdzhg.html

================================================================================
来源：http://hz.jinqigufen.top/gtzhiqtmdy.html

[H01] try / catch 基础
来源：http://hz.gaohongyu789.top/gtovupadar.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.sufxvd.cn/gtasslktyp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.bjfxy.top/gtuwgyxzle.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.xziqi.cn/gtdajvohmx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yuanzhike.top/gtbdhtfrsm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jinqigfzy.top/gtqqgftunu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zycfv.cn/gtbcgvjivu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yj202588.top/gtoqjwugyp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.hammf.cn/gtuzufaiic.html

[H02] finally / ensure 收尾
来源：http://hz.nanxinkj.top/gtwsjhflqb.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jiagoushi.top/gtfbfwqejr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.gotoacloud.top/gtjfrvlpdo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.shuidangran.top/gtpekwcils.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.svipenyu.cn/gtecjbpjys.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.iojbl.cn/gtwrffnitq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ehwqpu.com/gttschpepj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.hywenlv.cn/gtomfzgruy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.ydjk.org.cn/gtlxeipdku.html

[H03] 主动抛出异常
来源：http://hz.jianghu66.top/gtusdkgbfl.html

Py:   raise ValueError("错误信息")
来源：http://hz.ehwqpu.com/gtsfsdwuhu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.gotoacloud.top/gtrviiznxq.html

JS:   throw new Error("错误信息");
来源：http://hz.havefunace.top/gtewvejkua.html

TS:   throw new Error("错误信息");
来源：http://hz.tanke756.top/gtlfkhaxaz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.wangdashe.top/gtafrptmgh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.cqqwz.cn/gtslismvhn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.xinyue.icu/gtknotyvxu.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.xylfe.cn/gtdffjeeew.html

[H04] 自定义异常类型
来源：http://hz.jqgufenzy.top/gtwleuvlrl.html

Py:   class MyError(Exception): pass
来源：http://hz.zycfv.cn/gtnzzbngvz.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.shuidangran.top/gtbuwdvdzf.html

JS:   class MyError extends Error {}
来源：http://hz.9152youxi.cn/gtzjybcakg.html

TS:   class MyError extends Error {}
来源：http://hz.wangdashe.top/gttwrivpuv.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zycfv.cn/gtezaeukdw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.aibaodan.cn/gtndujgyhs.html


<!-- 参考信息 -->