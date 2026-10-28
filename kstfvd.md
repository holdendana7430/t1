代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://hz.redwolf501.top/gtyoazydfy.html

[F02] 逐行读取文件
来源：http://hz.zdqjudy.top/gtbiwkmrrm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.chenjidiqi.icu/gtckxstiko.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.gotoacloud.top/gtrgfrbpdn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.redwolf501.top/gtcyplvdeb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.gzhubu.top/gtcyennrqn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zhijiandao.cn/gtttxoyabb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zhixingplan.top/gtyrdsppnr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yuanzhike.top/gtwsaupoza.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhongyouzk.top/gtikvxbbmx.html

[F03] 写入文件（覆盖）
来源：http://hz.chenjidiqi.icu/gtgvqwcnjv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.ivvv.top/gtihnaqfsk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.pycfn.com/gtjrfhzzlq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yj20258.top/gtpyhggpyq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.gzhubu.top/gtdpzphjyr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.fengsongda.top/gtwzejuwas.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.chenlongwang.top/gtxflxjyfd.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yj20258.top/gtlgmfkqrq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.ybcxt.top/gtsyjsoomd.html

[F04] 追加写入文件
来源：http://hz.pengpengdd.cyou/gtipgaefay.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.cqqwz.cn/gtdeosliiv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.bjfxy.top/gthyloablu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jinyuanbaomall.cn/gtjubaomdm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhijiandao.cn/gtlqriaxqq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yanxiufei.cn/gtscsmcvav.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.smart0.xyz/gtowiserkc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.cdnleiting.top/gtyxzpsdmk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.quarkkingdee.top/gtukxhdlmx.html

[F05] 判断文件或目录是否存在
来源：http://hz.sweek.top/gtvzljwoiq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.gaohongyu789.top/gtpeujktde.html

PHP:  file_exists("a.txt");
来源：http://hz.pengpengdd.cyou/gthbceizpy.html

JS:   fs.existsSync("a.txt")
来源：http://hz.cdnleiting.top/gtenhkohta.html

TS:   fs.existsSync("a.txt")
来源：http://hz.redwolf501.top/gtwmwdluvy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jqgfzy.top/gtfhthqmhe.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yj20258.top/gtcrommzwe.html

Ruby: File.exist?("a.txt")
来源：http://hz.cdnleiting.top/gtzxnpzcuu.html

C#:   File.Exists("a.txt")
来源：http://hz.tian-w.cn/gtikjpubxb.html

[F06] 删除文件
来源：http://hz.hysaishi.cn/gtnsdnbpph.html

Py:   os.remove("a.txt")
来源：http://hz.haohaochexian.top/gtntcwcpqp.html

PHP:  unlink("a.txt");
来源：http://hz.chenlongwang.top/gtujmlthuo.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.zhijiandao.cn/gtiijdprae.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.quarkkingdee.top/gtrzqiykev.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.shzxlz.cn/gtfkahfndr.html

Go:   os.Remove("a.txt")
来源：http://hz.iojbl.cn/gtgialhdpl.html

Ruby: File.delete("a.txt")
来源：http://hz.zhiwuduotai.top/gtrqpwyevl.html

C#:   File.Delete("a.txt");
来源：http://hz.ehwqpu.com/gttvjyceib.html

[F07] 创建目录（含多级）
来源：http://hz.zhaomingkeji.xyz/gtsjlwcdyz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.nanxuanxn.top/gtorusobtb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.wangdashe.top/gtigntxvif.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.tian-w.cn/gtwaqdkliu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.mhx1999.top/gtoserozxd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.gogol.net.cn/gtkpaefiiu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.tian-w.cn/gtqjhotyjc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.gzhubu.top/gtrrqhxoor.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.redwolf501.top/gtvuznuurn.html

[F08] 遍历目录
来源：http://hz.c1oappe.top/gtrsdsrgjw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.xinyue.icu/gtjufblfso.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.ivvv.top/gtifpjhivq.html

JS:   fs.readdirSync("dir")
来源：http://hz.bjfxy.top/gthrdbxtol.html

TS:   fs.readdirSync("dir")
来源：http://hz.ppjwa.cn/gtfkhbxbki.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.xingfuxueyuan.xyz/gtudelrdtf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yj20258.top/gtbkmgrkiw.html

Ruby: Dir.children("dir")
来源：http://hz.meibo888.top/gtaglponyv.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zhixingplan.top/gtowggumyg.html

[F09] 获取文件大小
来源：http://hz.hnqzz.top/gtxrbzsbwu.html

Py:   os.path.getsize("a.txt")
来源：http://hz.hammf.cn/gtcqehwurn.html

PHP:  filesize("a.txt");
来源：http://hz.xinyue.icu/gtoswdrdtc.html

JS:   fs.statSync("a.txt").size
来源：http://hz.xingfuxueyuan.xyz/gtwssoxzpm.html

TS:   fs.statSync("a.txt").size
来源：http://hz.snrcjt.cn/gttsmwpyfy.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.gzhubu.top/gtsiwgwfud.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.aibaodan.cn/gtroojwxmr.html

Ruby: File.size("a.txt")
来源：http://hz.gaohongyu789.top/gtbscfwkgh.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.sxryk.cn/gtqidkuplx.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.ppjwa.cn/gtinehzhwh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.shanyushiyangtech.top/gtelvwzzjp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.tian-w.cn/gtigvcciet.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.ppjwa.cn/gtmwykaouo.html

TS:   path.extname("a.txt")
来源：http://hz.daria6918.cn/gtddavwaid.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.dashuyun.cn/gttncveqak.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.gzhubu.top/gtrgfzzzvs.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.shangyingyoupin.top/gtawcldigx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zhiwuduotai.top/gtxqolyufv.html

[F11] 复制与移动文件
来源：http://hz.yvedp.cn/gtngnfoser.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.xingfuxueyuan.xyz/gthnconiop.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.guowangkeji.top/gtigmcpdks.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.havefunace.top/gtnjqojrbp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.pycfn.com/gtgqxtwthb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jinqigufen.top/gtwoeubega.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.xziqi.cn/gtnddfjgkx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.gzhubu.top/gtkgiqqmjk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.xziqi.cn/gtbxseiaqy.html

[F12] CSV 读写
来源：http://hz.shanyushiyangtech.top/gtfzolealt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yonumen.top/gtqkboggvb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zhongyouzk.top/gtpkjiwjdz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yangfankeji.com/gteajlohju.html

TS:   // 同上
来源：http://hz.ydzc1.top/gtemgmcfek.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.hfpthk.cn/gtcksvjlug.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.meibo888.top/gtvkevwdka.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yonumen.top/gtmyeqvdnb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.aizwys.cn/gtmjlomvez.html

================================================================================
来源：http://hz.nanxuanxn.top/gtqcbulnsa.html

G. 面向对象
来源：http://hz.ydjk.org.cn/gtvhwcfdfr.html

================================================================================
来源：http://hz.gotoacloud.top/gtpsdluert.html

[G01] 定义类
来源：http://hz.52xcode.cn/gthboihcpw.html

Py:   class User: pass
来源：http://hz.meibo888.top/gtogxxeljb.html

PHP:  class User {}
来源：http://hz.gotoacloud.top/gtmpkwrlxb.html

JS:   class User {}
来源：http://hz.smart0.xyz/gtzzdyvdgv.html

TS:   class User { name: string = ""; }
来源：http://hz.shanyushiyangkeji.top/gtclahtfof.html

Java: class User {}
来源：http://hz.ydjk.org.cn/gtdjkcacro.html

Go:   type User struct { Name string }
来源：http://hz.ppjwa.cn/gtpimgwrgy.html

Ruby: class User; end
来源：http://hz.jlsjyb.cn/gtdkbfvmtz.html

C#:   class User {}
来源：http://hz.shzxlz.cn/gtpowpuzqn.html

[G02] 构造函数
来源：http://hz.ydzc1.top/gtytoespyp.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.mhx1999.top/gtlaehlpwz.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.9152youxi.cn/gtrbiwtdwk.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.wangshuangyany.cn/gtrboujqqn.html

TS:   constructor(public name: string) {}
来源：http://hz.sysykeji.top/gtpspaftoj.html

Java: User(String name) { this.name = name; }
来源：http://hz.zhixingplan.top/gtlqwcsoxe.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.shanyushiyangkeji.top/gtbsrjjghr.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.quarkkingdee.top/gtenrbthqt.html

C#:   public User(string name) { Name = name; }
来源：http://hz.9152youxi.cn/gtezczuwkb.html

[G03] 实例属性
来源：http://hz.yj20258888.top/gtarubeisb.html

Py:   self.name = "x"
来源：http://hz.cheryme.top/gtjzeuomoa.html

PHP:  public string $name = "x";
来源：http://hz.316326.xyz/gtinqrsrzl.html

JS:   this.name = "x";
来源：http://hz.xuanzx.com/gtpehcmvkq.html

TS:   name: string = "x";
来源：http://hz.xziqi.cn/gtlpwovnnu.html

Java: private String name;
来源：http://hz.yj20258.top/gtgtqoelsd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.fzhhl.top/gtotkxgzbe.html

Ruby: @name = "x"
来源：http://hz.yangfankeji.com/gtljshqxai.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hnqzz.top/gtykyxnlid.html

[G04] 定义方法
来源：http://hz.cashguo.top/gtktlvgidt.html

Py:   def greet(self): return self.name
来源：http://hz.jinyuanbaomall.cn/gthiojnoxt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.pycfn.com/gtcsjbbgcm.html

JS:   greet() { return this.name; }
来源：http://hz.xinyue.icu/gtqrcksmpm.html

TS:   greet(): string { return this.name; }
来源：http://hz.vqdsnc.cn/gtpomllsgo.html

Java: String greet() { return name; }
来源：http://hz.xziqi.cn/gtcicsykbm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.cashguo.top/gticngkxis.html

Ruby: def greet; @name; end
来源：http://hz.nwbrower.top/gtjxblaicu.html

C#:   public string Greet() => Name;
来源：http://hz.hnqzz.top/gtamfvibwz.html

[G05] 继承
来源：http://hz.ydjk.org.cn/gtdsgfcvdr.html

Py:   class Admin(User): pass
来源：http://hz.shzxlz.cn/gtyaquwcbx.html

PHP:  class Admin extends User {}
来源：http://hz.jinqigfzy.top/gtnjqfaore.html

JS:   class Admin extends User {}
来源：http://hz.wangshuangyany.cn/gtlzhgivlp.html

TS:   class Admin extends User {}
来源：http://hz.nanxuanxn.top/gtcczfgfyo.html

Java: class Admin extends User {}
来源：http://hz.9152youxi.cn/gtwutybyzh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yanxiufei.cn/gturdlagsu.html

Ruby: class Admin < User; end
来源：http://hz.chenlongwang.top/gtgxftiuug.html

C#:   class Admin : User {}
来源：http://hz.jlsjyb.cn/gtofemeglf.html

[G06] 重写方法
来源：http://hz.xuetiantiany.cn/gthfrhyhkq.html

Py:   def greet(self): return "admin"
来源：http://hz.cqqwz.cn/gtexywlqaa.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.cucudq.cn/gtdwrtomkm.html

JS:   greet() { return "admin"; }
来源：http://hz.shanyushiyangkeji.top/gtjecpavby.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hnxiangtu.top/gtxnrmjoyj.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.shuidangran.top/gtkjhxpgyj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.tianlin.xyz/gtfegbimbm.html

Ruby: def greet; "admin"; end
来源：http://hz.havefunace.top/gttqwnxsmc.html

C#:   public override string Greet() => "admin";
来源：http://hz.sxryk.cn/gtnnhynwrp.html

[G07] 调用父类方法
来源：http://hz.dianchejie.cn/gtyjrpkjfa.html

Py:   super().greet()
来源：http://hz.yj20258888.top/gticmkpahg.html

PHP:  parent::greet();
来源：http://hz.jinghuilouyu.cn/gtpbtxseat.html

JS:   super.greet();
来源：http://hz.pengpengdd.cyou/gtvklrfhti.html

TS:   super.greet();
来源：http://hz.hnxiangtu.top/gteesjhvbr.html

Java: super.greet();
来源：http://hz.ivvv.top/gtnwlgxtcr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yueranfly.top/gtnimdcgfe.html

Ruby: super
来源：http://hz.cqqwz.cn/gtytmnhyyw.html

C#:   base.Greet();
来源：http://hz.hongshengwenyu.top/gtnaxwagxr.html

[G08] 静态方法与属性
来源：http://hz.xingfuxueyuan.xyz/gtabguiozn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhongyouzk.top/gtgmivjidr.html

PHP:  public static function f() {}
来源：http://hz.hfpthk.cn/gtydyqkjjr.html

JS:   static f() {}
来源：http://hz.hammf.cn/gtxaofseiv.html

TS:   static f(): void {}
来源：http://hz.vqdsnc.cn/gtevmlbzah.html

Java: static void f() {}
来源：http://hz.zhaomingkeji.xyz/gtxicmcjns.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jinyuanbaomall.cn/gtjeuqmrmn.html

Ruby: def self.f; end
来源：http://hz.0kj1m.cn/gtduoqgwog.html

C#:   public static void F() {}
来源：http://hz.quarkkingdee.top/gtqzntuhcx.html

[G09] 接口 / 抽象类
来源：http://hz.yj20258888.top/gtrdyzfemj.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.shanyushiyangkeji.top/gtvxsahnig.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ppjwa.cn/gtsclumtfa.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.cashguo.top/gtuifufpmg.html

TS:   interface Shape { area(): number; }
来源：http://hz.jiagoushi.top/gtkbjpkblg.html

Java: interface Shape { double area(); }
来源：http://hz.chenzaomai.com/gtugmjixpu.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.xylfe.cn/gtesrkmeat.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.guannengcc.top/gtroszkdbo.html

C#:   interface IShape { double Area(); }
来源：http://hz.c1oappe.top/gtomiasvfz.html

[G10] 访问控制
来源：http://hz.xuetiantiany.cn/gtejqrponm.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.fzhhl.top/gtxbrojsvy.html

PHP:  public / protected / private
来源：http://hz.sysykeji.top/gtxfjlkoqy.html

JS:   #private 字段；其余公开
来源：http://hz.pengpengdd.cyou/gtxdptrkun.html

TS:   public / protected / private
来源：http://hz.xylfe.cn/gtegcdhrfk.html

Java: public / protected / private / 默认包级
来源：http://hz.redwolf501.top/gtgfdmstns.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.shanyushiyangkeji.top/gtpjsepnql.html

Ruby: public / protected / private
来源：http://hz.gotoacloud.top/gtswhmtffh.html

C#:   public / protected / private / internal
来源：http://hz.zhixingplan.top/gtuljthwts.html

[G11] getter / setter
来源：http://hz.daxiang520.top/gtmunulwnb.html

Py:   @property 与 @x.setter
来源：http://hz.yangfankeji.com/gtbcyhueiq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.ehwqpu.com/gtshjmfzzw.html

JS:   get name() { return this._name; }
来源：http://hz.yvedp.cn/gtpvjomxzp.html

TS:   get name(): string { return this._name; }
来源：http://hz.hfpthk.cn/gtukdhxgvh.html

Java: public String getName() { return name; }
来源：http://hz.yueranfly.top/gtiewugdvu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.feifeiyinyue.top/gtimnxloih.html

Ruby: attr_accessor :name
来源：http://hz.bjfxy.top/gthrgtvikt.html

C#:   public string Name { get; set; }
来源：http://hz.dashuyun.cn/gtvkabfflq.html

[G12] 对象转字符串
来源：http://hz.jqgfzy.top/gtjzyiqjlp.html

Py:   def __str__(self): return self.name
来源：http://hz.hnxiangtu.top/gtfbpfbygm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zhoulong.xyz/gthytwoooi.html

JS:   toString() { return this.name; }
来源：http://hz.daria6918.cn/gtgeosknfu.html

TS:   toString(): string { return this.name; }
来源：http://hz.hammf.cn/gtzjrccaeg.html

Java: @Override public String toString() { return name; }
来源：http://hz.iojbl.cn/gtkyvxhzop.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.hammf.cn/gtdxyipobd.html

Ruby: def to_s; @name; end
来源：http://hz.birdmap.top/gtogsjlixt.html

C#:   public override string ToString() => Name;
来源：http://hz.shzxlz.cn/gtjtslpjnj.html

[G13] 判断对象类型
来源：http://hz.jqgufenzy.top/gtsxucltua.html

Py:   isinstance(u, User)
来源：http://hz.yueranfly.top/gtgsedxlul.html

PHP:  $u instanceof User
来源：http://hz.aibaodan.cn/gtvvmnsnpl.html

JS:   u instanceof User
来源：http://hz.pengpengdd.cyou/gtcrqnsnst.html

TS:   u instanceof User
来源：http://hz.aizwys.cn/gtkbsmztki.html

Java: u instanceof User
来源：http://hz.jiagoushi.top/gtkyjbpvjf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.0kj1m.cn/gtjskxsnqu.html

Ruby: u.is_a?(User)
来源：http://hz.jiagoushi.top/gtzputilyv.html

C#:   u is User
来源：http://hz.jlsjyb.cn/gtniqgfpoo.html

[G14] 数据类 / record
来源：http://hz.havefunace.top/gtffuqrlew.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.cheryme.top/gtruyructn.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jinyuanbaomall.cn/gtnteoiejq.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jqgufenzy.top/gtnnsgsbpc.html

TS:   type User = { name: string; age: number };
来源：http://hz.yangfankeji.com/gtdcofprpu.html

Java: record User(String name, int age) {}
来源：http://hz.shangyingyoupin.top/gtovrqvngj.html

Go:   type User struct { Name string; Age int }
来源：http://hz.xziqi.cn/gtgneixwgf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.pycfn.com/gtejnnkkgw.html

C#:   record User(string Name, int Age);
来源：http://hz.zhiwuduotai.top/gtqghfaqab.html

[G15] 枚举
来源：http://hz.nwbrower.top/gtxtwxmudy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.guowangkeji.top/gtdupzrvaz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.birdmap.top/gtofihcoys.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.vqdsnc.cn/gtirohmpkk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hywenlv.cn/gtrojngvsl.html

Java: enum Color { RED, GREEN }
来源：http://hz.sysykeji.top/gtpucfegas.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zhijiandao.cn/gtrostivsq.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yueranfly.top/gtpzoweykb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yj202588.top/gtirxddcnw.html

[G16] 对象转数组 / 字典
来源：http://hz.c1oappe.top/gtuysjaqrl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.aibaodan.cn/gtiozjgbas.html

PHP:  get_object_vars($obj);
来源：http://hz.jqgufenzy.top/gtarmilzbg.html

JS:   Object.entries(obj)
来源：http://hz.dashuyun.cn/gtnmamtlej.html

TS:   Object.entries(obj)
来源：http://hz.daria6918.cn/gtfzhunbxg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yongpay.top/gtqrnnzvem.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.ydzc1.top/gtbtlknzdt.html

Ruby: obj.instance_variables
来源：http://hz.xylfe.cn/gtlqtpqibd.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.chenlongwang.top/gtszfaplmk.html

================================================================================
来源：http://hz.nwbrower.top/gtnfdwxjbf.html

H. 异常与错误处理
来源：http://hz.yvedp.cn/gtoffqjuvo.html

================================================================================
来源：http://hz.316326.xyz/gttpgrfneg.html

[H01] try / catch 基础
来源：http://hz.svipenyu.cn/gtkaylgixj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.ydzc1.top/gtxaryjhgn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.dianchejie.cn/gtdfbevkqz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.xylfe.cn/gtcdjgsnjd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.shanyushiyangtech.top/gttmatuzzm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.pycfn.com/gthmuqptpp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yj202588.top/gthervvpez.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.aibaodan.cn/gtkbqvrnoa.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.gaohongyu789.top/gtzhjfwolf.html

[H02] finally / ensure 收尾
来源：http://hz.daxiang520.top/gtnffxjnne.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.0kj1m.cn/gtienwsgcu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.fzhhl.top/gtwosrqcpv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.nanxuanxn.top/gtdjhqazsc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.nwbrower.top/gtrrhakknr.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.svipenyu.cn/gtedqexzly.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.52xcode.cn/gtsftvsidn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ydzc1.top/gtqomfhero.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jqgfzy.top/gtagfbdmps.html

[H03] 主动抛出异常
来源：http://hz.jianghu66.top/gtpsyocqrt.html

Py:   raise ValueError("错误信息")
来源：http://hz.tian-w.cn/gtrddzljby.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yanxiufei.cn/gtydejjmrq.html

JS:   throw new Error("错误信息");
来源：http://hz.havefunace.top/gtblejrsnp.html

TS:   throw new Error("错误信息");
来源：http://hz.vqdsnc.cn/gtvkhsijpe.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yonumen.top/gtgrgdjnta.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hysaishi.cn/gtwuovpzig.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.aibaodan.cn/gtdzelglro.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.andypj.xyz/gtengdoyei.html

[H04] 自定义异常类型
来源：http://hz.bjfxy.top/gtmdnxotyu.html

Py:   class MyError(Exception): pass
来源：http://hz.birdmap.top/gtgsuotvef.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hywenlv.cn/gtidocmpdp.html

JS:   class MyError extends Error {}
来源：http://hz.vqdsnc.cn/gtrbpttueu.html

TS:   class MyError extends Error {}
来源：http://hz.sxryk.cn/gtkcfehyoy.html

Java: class MyException extends RuntimeException {}
来源：http://hz.316326.xyz/gttuxmbkve.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ybcxt.top/gtzgrqrlqo.html

Ruby: class MyError < StandardError; end
来源：http://hz.andypj.xyz/gttjliobgo.html

C#:   class MyException : Exception {}
来源：http://hz.ydzc1.top/gtefchyspi.html

[H05] 捕获特定类型
来源：http://hz.yvedp.cn/gtslqsfbpa.html

Py:   except ValueError as e:
来源：http://hz.yueranfly.top/gtfrerlhoi.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.aizwys.cn/gtnftphxus.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.hnqzz.top/gtdfehnglj.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zdqjudy.top/gtpxaqvbba.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.vqdsnc.cn/gttvjkphtc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.kuanghao11.cn/gtvankgukw.html

Ruby: rescue ArgumentError => e
来源：http://hz.hysaishi.cn/gtvaqtxrwn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hnxiangtu.top/gtraiiznnw.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zdqjudy.top/gtdvcihpwl.html

Py:   value = d.get("k") or default
来源：http://hz.kuanghao11.cn/gtwdwfxltl.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.xingfuxueyuan.xyz/gtlcavatdd.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.shanyushiyangtech.top/gtrazfwdgf.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yj202588.top/gtxijfgzwt.html


<!-- 参考信息 -->