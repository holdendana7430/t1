代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.xziqi.cn/gtnsprzmap.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.chenjidiqi.icu/gtlljgqqgv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.shuidangran.top/gtudezzcgc.html

Ruby: File.read("a.txt")
来源：http://hz.cqqwz.cn/gtfqzsukak.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.gogol.net.cn/gtnvozxbon.html

[F02] 逐行读取文件
来源：http://hz.pengpengdd.cyou/gtvrnnwnnp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jinqigufen.top/gtayoxzsjf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.ivvv.top/gtvprxpalp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yj202588.top/gttvebqwst.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.iojbl.cn/gtwnszmkag.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.aizwys.cn/gtfhacuqtv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zhiwuduotai.top/gthcokavyj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.0kj1m.cn/gtzqxwxyki.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.guannengcc.top/gtjoxgvnnn.html

[F03] 写入文件（覆盖）
来源：http://hz.316326.xyz/gtczczlzyo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zhijiandao.cn/gthmafzcfm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.cdnleiting.top/gtlcnqweaz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.meibo888.top/gtarvffqga.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.tian-w.cn/gtpzpohhlz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.andypj.xyz/gtcmrthhou.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.ybcxt.top/gtxonizdfz.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.svipenyu.cn/gtalxlkodi.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.316326.xyz/gtobxwjyzn.html

[F04] 追加写入文件
来源：http://hz.sxryk.cn/gtjgevfeim.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.haohaochexian.top/gtepjtokyb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.aibaodan.cn/gtfvakzrsy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yvedp.cn/gtnfmxgego.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ydjk.org.cn/gtbqatjtdg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.shuidangran.top/gtcukflctj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jyoumei.cn/gthtlvsfds.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.hywenlv.cn/gtzwcwfdqw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yonumen.top/gtsuzntveo.html

[F05] 判断文件或目录是否存在
来源：http://hz.xziqi.cn/gtzwrernde.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.ydzc1.top/gtcrwnibib.html

PHP:  file_exists("a.txt");
来源：http://hz.chenzaomai.com/gtmknioetc.html

JS:   fs.existsSync("a.txt")
来源：http://hz.redwolf501.top/gtlfacaaqx.html

TS:   fs.existsSync("a.txt")
来源：http://hz.daxiang520.top/gtsltmhkvl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.svipenyu.cn/gtcfdttuaz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.aizwys.cn/gtyxeoguzu.html

Ruby: File.exist?("a.txt")
来源：http://hz.tianlin.xyz/gtnicmmmne.html

C#:   File.Exists("a.txt")
来源：http://hz.hammf.cn/gtvrsacrwr.html

[F06] 删除文件
来源：http://hz.ydzc1.top/gtwhyhmyeh.html

Py:   os.remove("a.txt")
来源：http://hz.kuanghao11.cn/gtrujbhcxp.html

PHP:  unlink("a.txt");
来源：http://hz.mhx1999.top/gtdyaxzvpt.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.ydzc1.top/gtdveeidlv.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.dianchejie.cn/gtaqchqigh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.cheryme.top/gtjsehjkqo.html

Go:   os.Remove("a.txt")
来源：http://hz.snrcjt.cn/gtuseabiyl.html

Ruby: File.delete("a.txt")
来源：http://hz.sweek.top/gtvqcrgzhb.html

C#:   File.Delete("a.txt");
来源：http://hz.jyoumei.cn/gtforlmube.html

[F07] 创建目录（含多级）
来源：http://hz.snrcjt.cn/gtmmlhumqi.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hongshengwenyu.top/gtffhesnqg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.nanxinkj.top/gtksxmxtdk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhijiandao.cn/gtmvgordcq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jyoumei.cn/gtiibzvtmj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.xuanzx.com/gtbksynkyz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.shzxlz.cn/gtgruzcdly.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zhongyouzk.top/gtdmrchhec.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jiagoushi.top/gtkvtnazgy.html

[F08] 遍历目录
来源：http://hz.smart0.xyz/gtkzcsrmbx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.tanke756.top/gtzfmlzjvk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.daxiang520.top/gthxghbejx.html

JS:   fs.readdirSync("dir")
来源：http://hz.hysaishi.cn/gtyzxjfwtf.html

TS:   fs.readdirSync("dir")
来源：http://hz.chenlongwang.top/gtncqhaggk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.xuanzx.com/gtgblkfxfb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jinghuilouyu.cn/gtdbqqfhst.html

Ruby: Dir.children("dir")
来源：http://hz.yuxming.cn/gtyhkpaqia.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zhengqikj.top/gtizsmscrc.html

[F09] 获取文件大小
来源：http://hz.jiagoushi.top/gtxtcphtao.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zycfv.cn/gteytvfioz.html

PHP:  filesize("a.txt");
来源：http://hz.gaohongyu789.top/gtlflztedp.html

JS:   fs.statSync("a.txt").size
来源：http://hz.ehwqpu.com/gtfnrzvaye.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jianghu66.top/gtrowwrrnh.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jqgfzy.top/gtmztckhwh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.dianchejie.cn/gtcgwtbogs.html

Ruby: File.size("a.txt")
来源：http://hz.shanyushiyangtech.top/gtvqsztidv.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jqgufenzy.top/gtfdoejvnj.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zhijiandao.cn/gtpmcwarqd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yj20258888.top/gtfnkhfoqj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtxxhjbgxw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.cheryme.top/gtxklehcsp.html

TS:   path.extname("a.txt")
来源：http://hz.xziqi.cn/gtbdxtsrzg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yongpay.top/gtiojilrpu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.ydzc1.top/gttfhqllfm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.hongshengwenyu.top/gtzocclnhr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yangfankeji.com/gtvmmdpoxe.html

[F11] 复制与移动文件
来源：http://hz.jinqigfzy.top/gtzokkstfc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jinqigufen.top/gtvefhueiz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.ppjwa.cn/gtiaaafrjw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ivvv.top/gtstixvopx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.smart0.xyz/gtmjzamcza.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jinghuilouyu.cn/gtwkosiohf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.chenlongwang.top/gtagjnqmnh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.hammf.cn/gtkfhslguf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zdqjudy.top/gtkesszkva.html

[F12] CSV 读写
来源：http://hz.jianghu66.top/gtapzgpumw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yueranfly.top/gtnttuwvkw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yonumen.top/gtmnoieoml.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.cashguo.top/gtlamhzdeb.html

TS:   // 同上
来源：http://hz.jinqigufen.top/gtwlciuinh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.dashuyun.cn/gtpgjlchih.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.ydzc1.top/gttqqiyzpb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yj20258888.top/gtgvavmcwv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.shangyingyoupin.top/gtdtpyrxzu.html

================================================================================
来源：http://hz.cashguo.top/gtmtilbnld.html

G. 面向对象
来源：http://hz.redwolf501.top/gtyfzuyuyw.html

================================================================================
来源：http://hz.yuanzhike.top/gtlcavlukg.html

[G01] 定义类
来源：http://hz.ybcxt.top/gtnyqalhhy.html

Py:   class User: pass
来源：http://hz.xingfuxueyuan.xyz/gtgbenzlwd.html

PHP:  class User {}
来源：http://hz.jianghu66.top/gtfbdfjqbc.html

JS:   class User {}
来源：http://hz.yueranfly.top/gtqdsxmvxs.html

TS:   class User { name: string = ""; }
来源：http://hz.snrcjt.cn/gtbgxaiytf.html

Java: class User {}
来源：http://hz.yonumen.top/gtaehtpwkp.html

Go:   type User struct { Name string }
来源：http://hz.guannengcc.top/gtpeuotpma.html

Ruby: class User; end
来源：http://hz.yanxiufei.cn/gtwvwuhiau.html

C#:   class User {}
来源：http://hz.snrcjt.cn/gtxhdabgqs.html

[G02] 构造函数
来源：http://hz.jinqigufen.top/gtlvbtyzqx.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.daria6918.cn/gtwhaecrsn.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.shuidangran.top/gtcnagwmiw.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yonumen.top/gtveitltvs.html

TS:   constructor(public name: string) {}
来源：http://hz.ydjk.org.cn/gtlsnttugd.html

Java: User(String name) { this.name = name; }
来源：http://hz.sysykeji.top/gtsbnasgpa.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zycfv.cn/gtepnztadi.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.wangdashe.top/gtgxvhleaj.html

C#:   public User(string name) { Name = name; }
来源：http://hz.nanxuanxn.top/gtdqohujqk.html

[G03] 实例属性
来源：http://hz.wangdashe.top/gtyjcaqkry.html

Py:   self.name = "x"
来源：http://hz.sysykeji.top/gtcbrenitd.html

PHP:  public string $name = "x";
来源：http://hz.dashuyun.cn/gtxsgnenxs.html

JS:   this.name = "x";
来源：http://hz.yongpay.top/gtyzbcfdle.html

TS:   name: string = "x";
来源：http://hz.gzhubu.top/gtsgwzesjz.html

Java: private String name;
来源：http://hz.feifeiyinyue.top/gtjcgorsac.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.feifeiyinyue.top/gtdecbjwwf.html

Ruby: @name = "x"
来源：http://hz.aizwys.cn/gtrpuikbvs.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zhoulong.xyz/gtyfdjnnzi.html

[G04] 定义方法
来源：http://hz.yanxiufei.cn/gtdgjyqggj.html

Py:   def greet(self): return self.name
来源：http://hz.c1oappe.top/gtljjvmvvv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.xziqi.cn/gtcyjzhnnv.html

JS:   greet() { return this.name; }
来源：http://hz.bjfxy.top/gtjwatqefp.html

TS:   greet(): string { return this.name; }
来源：http://hz.gotoacloud.top/gtgfwxlcvf.html

Java: String greet() { return name; }
来源：http://hz.cucudq.cn/gtwmczwswg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.sweek.top/gtimmopzxj.html

Ruby: def greet; @name; end
来源：http://hz.andypj.xyz/gtnrpnvqih.html

C#:   public string Greet() => Name;
来源：http://hz.cqqwz.cn/gtwsuoapre.html

[G05] 继承
来源：http://hz.chenzaomai.com/gtexarokhu.html

Py:   class Admin(User): pass
来源：http://hz.0kj1m.cn/gtimgsokax.html

PHP:  class Admin extends User {}
来源：http://hz.yj20258888.top/gthyrvevuv.html

JS:   class Admin extends User {}
来源：http://hz.52xcode.cn/gtkinnskhq.html

TS:   class Admin extends User {}
来源：http://hz.hnxiangtu.top/gtxcwwaodr.html

Java: class Admin extends User {}
来源：http://hz.nwbrower.top/gtpnvriedi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.tian-w.cn/gttienoyyf.html

Ruby: class Admin < User; end
来源：http://hz.jinqigufen.top/gtodhgwrbc.html

C#:   class Admin : User {}
来源：http://hz.feifeiyinyue.top/gtcsneodis.html

[G06] 重写方法
来源：http://hz.wangshuangyany.cn/gtxoetytkn.html

Py:   def greet(self): return "admin"
来源：http://hz.fzhhl.top/gtvgdsypac.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.hysaishi.cn/gtlrqpknql.html

JS:   greet() { return "admin"; }
来源：http://hz.nanxuanxn.top/gtphatgimy.html

TS:   greet(): string { return "admin"; }
来源：http://hz.haohaochexian.top/gtxytyluus.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.bjfxy.top/gttfjlmbpf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jinghuilouyu.cn/gtieurfzrv.html

Ruby: def greet; "admin"; end
来源：http://hz.chenzaomai.com/gtucublkud.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhaomingkeji.xyz/gtknyjnaqm.html

[G07] 调用父类方法
来源：http://hz.meibo888.top/gtvhbgqitu.html

Py:   super().greet()
来源：http://hz.sufxvd.cn/gtuhqidfvs.html

PHP:  parent::greet();
来源：http://hz.yuxming.cn/gtcaqutrol.html

JS:   super.greet();
来源：http://hz.cucudq.cn/gtcsgxxhda.html

TS:   super.greet();
来源：http://hz.pycfn.com/gtwojubejg.html

Java: super.greet();
来源：http://hz.yuanzhike.top/gtzgqhakgh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.nanxinkj.top/gtycuqzkzb.html

Ruby: super
来源：http://hz.hywenlv.cn/gtimrjlcuk.html

C#:   base.Greet();
来源：http://hz.hammf.cn/gtagjrikdq.html

[G08] 静态方法与属性
来源：http://hz.0kj1m.cn/gtmcuhabxo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yangfankeji.com/gtdaxydsit.html

PHP:  public static function f() {}
来源：http://hz.xziqi.cn/gtrktrqpeh.html

JS:   static f() {}
来源：http://hz.ydzc1.top/gtxnvokrzi.html

TS:   static f(): void {}
来源：http://hz.ybcxt.top/gtkloemsbj.html

Java: static void f() {}
来源：http://hz.redwolf501.top/gtvuvmvybz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.fengsongda.top/gtfgbntmep.html

Ruby: def self.f; end
来源：http://hz.shangyingyoupin.top/gtzadmqejm.html

C#:   public static void F() {}
来源：http://hz.52xcode.cn/gtaxacqxod.html

[G09] 接口 / 抽象类
来源：http://hz.redwolf501.top/gtgtohgntc.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zycfv.cn/gtodxnhile.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.aibaodan.cn/gtmcvnniyf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.wangdashe.top/gtzjfdtvax.html

TS:   interface Shape { area(): number; }
来源：http://hz.sysykeji.top/gtkslortma.html

Java: interface Shape { double area(); }
来源：http://hz.yanxiufei.cn/gtslvpbjyr.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.gogol.net.cn/gtctxstiwc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.fengsongda.top/gtmuiabegl.html

C#:   interface IShape { double Area(); }
来源：http://hz.smart0.xyz/gtssbvzfda.html

[G10] 访问控制
来源：http://hz.cashguo.top/gtnbxrhsft.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhoulong.xyz/gtzvwffizr.html

PHP:  public / protected / private
来源：http://hz.birdmap.top/gtwetsyylf.html

JS:   #private 字段；其余公开
来源：http://hz.yuxming.cn/gtoqqxemor.html

TS:   public / protected / private
来源：http://hz.zhoulong.xyz/gttxwkwfna.html

Java: public / protected / private / 默认包级
来源：http://hz.jyoumei.cn/gtwbjlkfjs.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.xuanzx.com/gtustiyywe.html

Ruby: public / protected / private
来源：http://hz.pengpengdd.cyou/gtjhicmmtx.html

C#:   public / protected / private / internal
来源：http://hz.svipenyu.cn/gtbbgetqtu.html

[G11] getter / setter
来源：http://hz.jinyuanbaomall.cn/gtehssuafz.html

Py:   @property 与 @x.setter
来源：http://hz.shanyushiyangkeji.top/gtcpuxrykf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yangfankeji.com/gtqrnagudm.html

JS:   get name() { return this._name; }
来源：http://hz.zhixingplan.top/gtsybdsavo.html

TS:   get name(): string { return this._name; }
来源：http://hz.pycfn.com/gturzdedup.html

Java: public String getName() { return name; }
来源：http://hz.cheryme.top/gtosvltykv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.fzhhl.top/gtqkingtka.html

Ruby: attr_accessor :name
来源：http://hz.redwolf501.top/gtoabilnqf.html

C#:   public string Name { get; set; }
来源：http://hz.aibaodan.cn/gtykvwzdkw.html

[G12] 对象转字符串
来源：http://hz.jiagoushi.top/gttbxschgr.html

Py:   def __str__(self): return self.name
来源：http://hz.xuanzx.com/gtghbptkog.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.gotoacloud.top/gtdoiyipsf.html

JS:   toString() { return this.name; }
来源：http://hz.shzxlz.cn/gtsvfhclfb.html

TS:   toString(): string { return this.name; }
来源：http://hz.ehwqpu.com/gtyreoacgk.html

Java: @Override public String toString() { return name; }
来源：http://hz.yangfankeji.com/gtemppfgvg.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yueranfly.top/gtyjtqljeb.html

Ruby: def to_s; @name; end
来源：http://hz.yonumen.top/gtgftqnnrq.html

C#:   public override string ToString() => Name;
来源：http://hz.shanyushiyangtech.top/gtsvmfekrg.html

[G13] 判断对象类型
来源：http://hz.shuidangran.top/gtgqzliicy.html

Py:   isinstance(u, User)
来源：http://hz.jyoumei.cn/gtgioutmlv.html

PHP:  $u instanceof User
来源：http://hz.guannengcc.top/gtubswbfod.html

JS:   u instanceof User
来源：http://hz.aibaodan.cn/gtutaernmj.html

TS:   u instanceof User
来源：http://hz.meibo888.top/gthfiozeyj.html

Java: u instanceof User
来源：http://hz.guowangkeji.top/gtgsttrlxl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.svipenyu.cn/gtbrbpzxok.html

Ruby: u.is_a?(User)
来源：http://hz.shuidangran.top/gtcaptmsrp.html

C#:   u is User
来源：http://hz.yuanzhike.top/gtoozkyers.html

[G14] 数据类 / record
来源：http://hz.jianghu66.top/gtwhekattg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.kuanghao11.cn/gtzenmwdek.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.wangdashe.top/gtighrljzm.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zycfv.cn/gtxjjxuszg.html

TS:   type User = { name: string; age: number };
来源：http://hz.vqdsnc.cn/gtaclwrksk.html

Java: record User(String name, int age) {}
来源：http://hz.smart0.xyz/gtrfooculz.html

Go:   type User struct { Name string; Age int }
来源：http://hz.ybcxt.top/gtggcbxumz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.guannengcc.top/gtgcipnamv.html

C#:   record User(string Name, int Age);
来源：http://hz.ydzc1.top/gtsmnsrlwf.html

[G15] 枚举
来源：http://hz.nanxinkj.top/gtfrqaeqwl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yj202588.top/gthbwtkvsi.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ybcxt.top/gtfxbsaoul.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hnqzz.top/gtucxktagp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yj202588.top/gttzwcjglr.html

Java: enum Color { RED, GREEN }
来源：http://hz.sweek.top/gtyuyfzdjt.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jyoumei.cn/gtjlbafpzb.html

Ruby: Color = %i[red green].freeze
来源：http://hz.shuidangran.top/gtiyvotwqe.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.nwbrower.top/gtnpytoiwi.html

[G16] 对象转数组 / 字典
来源：http://hz.sysykeji.top/gtuwhrpmvk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.guowangkeji.top/gthoffbnnp.html

PHP:  get_object_vars($obj);
来源：http://hz.xuetiantiany.cn/gtfgokybwq.html

JS:   Object.entries(obj)
来源：http://hz.shangyingyoupin.top/gtmnddfatb.html

TS:   Object.entries(obj)
来源：http://hz.xuanzx.com/gtmfdpzhqr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.redwolf501.top/gtriozksfq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jqgufenzy.top/gtswgnryyn.html

Ruby: obj.instance_variables
来源：http://hz.smart0.xyz/gtwtdkmjfe.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.chenlongwang.top/gtwenlengi.html

================================================================================
来源：http://hz.ehwqpu.com/gtcejgbgbi.html

H. 异常与错误处理
来源：http://hz.9152youxi.cn/gthyzsbnfg.html

================================================================================
来源：http://hz.hnxiangtu.top/gtlqxxoizw.html

[H01] try / catch 基础
来源：http://hz.jqgfzy.top/gtplxygtvr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.hammf.cn/gtqpnynuar.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.gotoacloud.top/gtyzztctjw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.9152youxi.cn/gtxzlgazzg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.shanyushiyangkeji.top/gtkcqdecxi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.shangyingyoupin.top/gtftrqtdyw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.ehwqpu.com/gtlfpzxjll.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.quarkkingdee.top/gtoclwzpgz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.cashguo.top/gttantcjnu.html

[H02] finally / ensure 收尾
来源：http://hz.zhiwuduotai.top/gtkcttfcfk.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.svipenyu.cn/gtyajnauds.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jlsjyb.cn/gtrhchdntt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.snrcjt.cn/gtmcdkjrco.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jqgfzy.top/gttzpcibmi.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.ivvv.top/gtditqfhwe.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.dashuyun.cn/gtpgkvhqpn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.cucudq.cn/gtoiipfckq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yj202588.top/gtmojriidm.html

[H03] 主动抛出异常
来源：http://hz.kuanghao11.cn/gtvfqhbvbo.html

Py:   raise ValueError("错误信息")
来源：http://hz.zdqjudy.top/gtzskcfubb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jyoumei.cn/gtbjvwqkcu.html

JS:   throw new Error("错误信息");
来源：http://hz.316326.xyz/gtgggopkji.html

TS:   throw new Error("错误信息");
来源：http://hz.yj202588.top/gtspqmcvjo.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.tanke756.top/gtgpbjqzey.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.vqdsnc.cn/gtjggcxhqe.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.kuanghao11.cn/gtzwnctqfe.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.shanyushiyangkeji.top/gtgnseogmd.html

[H04] 自定义异常类型
来源：http://hz.shuidangran.top/gthczckuzo.html

Py:   class MyError(Exception): pass
来源：http://hz.wangdashe.top/gtdnephzfs.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.xinyue.icu/gtfthfnqut.html

JS:   class MyError extends Error {}
来源：http://hz.cqqwz.cn/gtqmvzhwuk.html

TS:   class MyError extends Error {}
来源：http://hz.daria6918.cn/gtmfietifk.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zhixingplan.top/gtuqucnuvy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.tanke756.top/gtfkdsvbqg.html

Ruby: class MyError < StandardError; end
来源：http://hz.zdqjudy.top/gtmmlpteks.html

C#:   class MyException : Exception {}
来源：http://hz.yj20258.top/gtnkoldyuh.html

[H05] 捕获特定类型
来源：http://hz.zhaomingkeji.xyz/gtmdkjumck.html

Py:   except ValueError as e:
来源：http://hz.shangyingyoupin.top/gtfuxjtauq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.ywan-chungtsiang.top/gteymsizml.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jyoumei.cn/gtqkxokddv.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.snrcjt.cn/gticoodjkb.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.9152youxi.cn/gtktiwgotr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.mhx1999.top/gtttqyctvu.html

Ruby: rescue ArgumentError => e
来源：http://hz.guannengcc.top/gttarijuzc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hysaishi.cn/gtzlddqolu.html

[H06] 可选值 / 空值安全访问
来源：http://hz.xziqi.cn/gtxkfodmfv.html


<!-- 参考信息 -->