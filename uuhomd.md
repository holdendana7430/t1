代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.pycfn.com/gtqnovngkh.html

================================================================================
来源：http://hz.chenzaomai.com/gtjsyhbmrs.html

F. 文件与目录
来源：http://hz.hnqzz.top/gtrudskcuz.html

================================================================================
来源：http://hz.yuxming.cn/gteyerqfgo.html

[F01] 读取整个文件
来源：http://hz.yangfankeji.com/gttooyrhbd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.tanke756.top/gtrbpnoowi.html

PHP:  file_get_contents("a.txt");
来源：http://hz.pycfn.com/gtidcbkits.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.kuanghao11.cn/gtdmbsyfru.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yonumen.top/gtyppyzutu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.tianlin.xyz/gtbqwxqdpy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yuxming.cn/gtqsnyycvs.html

Ruby: File.read("a.txt")
来源：http://hz.jqgufenzy.top/gtojbfosqy.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.aibaodan.cn/gtelzngdok.html

[F02] 逐行读取文件
来源：http://hz.gzhubu.top/gttmvfsozs.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zycfv.cn/gtsaofxhnw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yuanzhike.top/gturkjqcke.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.nanxuanxn.top/gtgfosmmwk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zycfv.cn/gthlzpsdxq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zhiwuduotai.top/gtpnijajoy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jqgfzy.top/gtgwfejapf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.xziqi.cn/gtevkhayes.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.gotoacloud.top/gtcvacphjw.html

[F03] 写入文件（覆盖）
来源：http://hz.gaohongyu789.top/gtzdvcpetd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.gotoacloud.top/gtfbcvfhhf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zdqjudy.top/gtlglqurlj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.birdmap.top/gtcrnoijyy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.feifeiyinyue.top/gttxeqssuz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.wangshuangyany.cn/gtnhluuteu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.xylfe.cn/gtnsmlovuz.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.sufxvd.cn/gtpbyhkyva.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.gogol.net.cn/gtlijrzxgv.html

[F04] 追加写入文件
来源：http://hz.jlsjyb.cn/gtyuctayqt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.52xcode.cn/gtcqtooxai.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.bjfxy.top/gtvpfhfojh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xinyue.icu/gtffqeqham.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yongpay.top/gthdsgrdei.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.hammf.cn/gtrgkzuvei.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.chenlongwang.top/gthcajvzyo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.hnxiangtu.top/gtzntntvnv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.shangyingyoupin.top/gtywafornp.html

[F05] 判断文件或目录是否存在
来源：http://hz.sxryk.cn/gtituqorjh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.xingfuxueyuan.xyz/gtewgwivpi.html

PHP:  file_exists("a.txt");
来源：http://hz.hysaishi.cn/gtnwlsliwu.html

JS:   fs.existsSync("a.txt")
来源：http://hz.pycfn.com/gtcxgbtqhr.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yj20258.top/gtrflzxtlp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yuxming.cn/gtnfqdmugt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.tanke756.top/gtaqgoerzi.html

Ruby: File.exist?("a.txt")
来源：http://hz.ydzc1.top/gtgbbfporf.html

C#:   File.Exists("a.txt")
来源：http://hz.yueranfly.top/gtewpivlhc.html

[F06] 删除文件
来源：http://hz.jinqigufen.top/gtgkrqyykg.html

Py:   os.remove("a.txt")
来源：http://hz.cqqwz.cn/gtpwvnnntk.html

PHP:  unlink("a.txt");
来源：http://hz.wangshuangyany.cn/gturpdbwbb.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.tanke756.top/gtsgrdpoxj.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jqgufenzy.top/gtgpxnzuxa.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.ehwqpu.com/gtdakfpgod.html

Go:   os.Remove("a.txt")
来源：http://hz.bjfxy.top/gtcbbsjitq.html

Ruby: File.delete("a.txt")
来源：http://hz.yangfankeji.com/gtllavjcgl.html

C#:   File.Delete("a.txt");
来源：http://hz.hysaishi.cn/gttconxivv.html

[F07] 创建目录（含多级）
来源：http://hz.hnxiangtu.top/gtavfxbhly.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.ywan-chungtsiang.top/gtrdsxhfcb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.xylfe.cn/gtprcrbttl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.c1oappe.top/gtgdeyehsp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhoulong.xyz/gtbnhbaoko.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yongpay.top/gtsozmibrf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.sweek.top/gtsdlvlgqi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jiagoushi.top/gtwapuzdiq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yj202588.top/gtlsgyplij.html

[F08] 遍历目录
来源：http://hz.tanke756.top/gtrrwmzzko.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.wangshuangyany.cn/gttszqjhio.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jiagoushi.top/gtgtjhbeau.html

JS:   fs.readdirSync("dir")
来源：http://hz.yj20258.top/gthtcfzxoe.html

TS:   fs.readdirSync("dir")
来源：http://hz.bjfxy.top/gtfzqwlfkn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jinqigufen.top/gtopadreag.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.daria6918.cn/gtjojkejcc.html

Ruby: Dir.children("dir")
来源：http://hz.xziqi.cn/gtmnarbwfu.html

C#:   Directory.GetFiles("dir")
来源：http://hz.hywenlv.cn/gtghswfokh.html

[F09] 获取文件大小
来源：http://hz.shuidangran.top/gturduplgy.html

Py:   os.path.getsize("a.txt")
来源：http://hz.cucudq.cn/gtbcltpern.html

PHP:  filesize("a.txt");
来源：http://hz.cdnleiting.top/gtwavtgygj.html

JS:   fs.statSync("a.txt").size
来源：http://hz.shangyingyoupin.top/gtoyvvgshf.html

TS:   fs.statSync("a.txt").size
来源：http://hz.52xcode.cn/gtaqdzzqlb.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.kuanghao11.cn/gtnwsbonir.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yueranfly.top/gtjhukalgg.html

Ruby: File.size("a.txt")
来源：http://hz.ehwqpu.com/gtayetrzwn.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.cashguo.top/gtukojrbbt.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.52xcode.cn/gtyhraetjz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.cheryme.top/gtxjghqdcn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.chenlongwang.top/gtzuwxvwfr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yueranfly.top/gtuezgbnct.html

TS:   path.extname("a.txt")
来源：http://hz.pengpengdd.cyou/gtbudiytju.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.hysaishi.cn/gtbolscuqx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.xylfe.cn/gtuxtkqwqx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yj202588.top/gtxeebpdyh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zycfv.cn/gtvkgdjjcx.html

[F11] 复制与移动文件
来源：http://hz.chenlongwang.top/gtntlsoyhz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yj202588.top/gthkqolspc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.316326.xyz/gtsuawrszv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.smart0.xyz/gtuajfbtiq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.tianlin.xyz/gtryfjaxlq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zycfv.cn/gtekdbkiai.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.shzxlz.cn/gtnvaclvrd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.nanxuanxn.top/gtzorlerpt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhongyouzk.top/gtfquwxygx.html

[F12] CSV 读写
来源：http://hz.xingfuxueyuan.xyz/gtakrrlqlu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.shzxlz.cn/gtpxmygidm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hywenlv.cn/gtqymhzuyd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.xinyue.icu/gtnhdrtaax.html

TS:   // 同上
来源：http://hz.nwbrower.top/gtrlewjpam.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.pycfn.com/gtdmlftndu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jlsjyb.cn/gtxcqjptsp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.9152youxi.cn/gtntykpmcy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.ppjwa.cn/gtzwumbabl.html

================================================================================
来源：http://hz.yj20258888.top/gtfvgxwgjf.html

G. 面向对象
来源：http://hz.ivvv.top/gtddgsjzgs.html

================================================================================
来源：http://hz.gzhubu.top/gtbrxulwdq.html

[G01] 定义类
来源：http://hz.zycfv.cn/gtqcfbxeaw.html

Py:   class User: pass
来源：http://hz.pengpengdd.cyou/gtdnqemlhp.html

PHP:  class User {}
来源：http://hz.chenjidiqi.icu/gtgeslqijd.html

JS:   class User {}
来源：http://hz.jianghu66.top/gtljynrpyh.html

TS:   class User { name: string = ""; }
来源：http://hz.zhoulong.xyz/gttiyaucty.html

Java: class User {}
来源：http://hz.xinyue.icu/gtawqzurxh.html

Go:   type User struct { Name string }
来源：http://hz.yj202588.top/gtpmrnngrz.html

Ruby: class User; end
来源：http://hz.guowangkeji.top/gtwxbuzyyy.html

C#:   class User {}
来源：http://hz.pycfn.com/gtwhlzjxuf.html

[G02] 构造函数
来源：http://hz.smart0.xyz/gtiglpvtxj.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.xinyue.icu/gtnjvbgbuk.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.c1oappe.top/gtwhvyeayl.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.tanke756.top/gtqycvavbs.html

TS:   constructor(public name: string) {}
来源：http://hz.gzhubu.top/gtgscescuq.html

Java: User(String name) { this.name = name; }
来源：http://hz.daxiang520.top/gtylkdmzps.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.nwbrower.top/gtxgmcjkww.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.xuetiantiany.cn/gthknkciaz.html

C#:   public User(string name) { Name = name; }
来源：http://hz.chenzaomai.com/gtjljtkyid.html

[G03] 实例属性
来源：http://hz.ppjwa.cn/gtorsfbnwm.html

Py:   self.name = "x"
来源：http://hz.kuanghao11.cn/gtfkxnfmgq.html

PHP:  public string $name = "x";
来源：http://hz.gogol.net.cn/gthhqpmehs.html

JS:   this.name = "x";
来源：http://hz.daria6918.cn/gtpoubmlpx.html

TS:   name: string = "x";
来源：http://hz.xuetiantiany.cn/gtwiizfocf.html

Java: private String name;
来源：http://hz.ehwqpu.com/gttvorkoak.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.tanke756.top/gttornaedx.html

Ruby: @name = "x"
来源：http://hz.yvedp.cn/gtrmqttblt.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.guannengcc.top/gtvkfzjapw.html

[G04] 定义方法
来源：http://hz.jqgufenzy.top/gtqblwnhrr.html

Py:   def greet(self): return self.name
来源：http://hz.cqqwz.cn/gtychprfog.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.0kj1m.cn/gtvqgwfmsm.html

JS:   greet() { return this.name; }
来源：http://hz.sysykeji.top/gtgggpdvuc.html

TS:   greet(): string { return this.name; }
来源：http://hz.jianghu66.top/gtnrfqytfp.html

Java: String greet() { return name; }
来源：http://hz.zhixingplan.top/gtvbwsmjvs.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.c1oappe.top/gtklsnumrl.html

Ruby: def greet; @name; end
来源：http://hz.fzhhl.top/gtywfnujkf.html

C#:   public string Greet() => Name;
来源：http://hz.daxiang520.top/gtxtkvdiox.html

[G05] 继承
来源：http://hz.haohaochexian.top/gtubgteihh.html

Py:   class Admin(User): pass
来源：http://hz.shuidangran.top/gtblbolazp.html

PHP:  class Admin extends User {}
来源：http://hz.fzhhl.top/gtunistfec.html

JS:   class Admin extends User {}
来源：http://hz.yonumen.top/gtljjwqgub.html

TS:   class Admin extends User {}
来源：http://hz.zhengqikj.top/gttnbychwq.html

Java: class Admin extends User {}
来源：http://hz.xylfe.cn/gtgfoqyjbm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zhengqikj.top/gtffqbfkzv.html

Ruby: class Admin < User; end
来源：http://hz.yongpay.top/gtyoqmnmpu.html

C#:   class Admin : User {}
来源：http://hz.havefunace.top/gtzzcrvhoy.html

[G06] 重写方法
来源：http://hz.cqqwz.cn/gtepcdjcgp.html

Py:   def greet(self): return "admin"
来源：http://hz.nanxinkj.top/gtcdxhrero.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ivvv.top/gtogkmnmtp.html

JS:   greet() { return "admin"; }
来源：http://hz.tian-w.cn/gthfywtqmb.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zhixingplan.top/gtbxhjazqh.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhijiandao.cn/gtlphbmmcx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yvedp.cn/gtpksuqmgg.html

Ruby: def greet; "admin"; end
来源：http://hz.yangfankeji.com/gtrpcsngrg.html

C#:   public override string Greet() => "admin";
来源：http://hz.wangshuangyany.cn/gtsvhfzlou.html

[G07] 调用父类方法
来源：http://hz.hnxiangtu.top/gtmpvxkjsw.html

Py:   super().greet()
来源：http://hz.jqgufenzy.top/gtrxaxsmcx.html

PHP:  parent::greet();
来源：http://hz.xziqi.cn/gtsgvwzzgb.html

JS:   super.greet();
来源：http://hz.yj20258.top/gtxmkqtywo.html

TS:   super.greet();
来源：http://hz.ydjk.org.cn/gtbxxbjwqi.html

Java: super.greet();
来源：http://hz.0kj1m.cn/gtuxkgotbw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jyoumei.cn/gtrwchbpge.html

Ruby: super
来源：http://hz.nanxinkj.top/gtugedqnnr.html

C#:   base.Greet();
来源：http://hz.hysaishi.cn/gtxrrupyqs.html

[G08] 静态方法与属性
来源：http://hz.dianchejie.cn/gttkiffqrj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.feifeiyinyue.top/gtnjrgwiyl.html

PHP:  public static function f() {}
来源：http://hz.fzhhl.top/gtlhulzkqg.html

JS:   static f() {}
来源：http://hz.0kj1m.cn/gtgqrgradx.html

TS:   static f(): void {}
来源：http://hz.gaohongyu789.top/gtoitwcjvg.html

Java: static void f() {}
来源：http://hz.yonumen.top/gtgyfsusbi.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.tianlin.xyz/gtunkqvonf.html

Ruby: def self.f; end
来源：http://hz.redwolf501.top/gtkexgnqbd.html

C#:   public static void F() {}
来源：http://hz.sysykeji.top/gtyoxfdmtb.html

[G09] 接口 / 抽象类
来源：http://hz.hysaishi.cn/gtxpwhowyt.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.iojbl.cn/gteywxmmkf.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jiagoushi.top/gtkuwjtcjw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.daria6918.cn/gteqlfirdg.html

TS:   interface Shape { area(): number; }
来源：http://hz.hnxiangtu.top/gtwxxuhzxt.html

Java: interface Shape { double area(); }
来源：http://hz.fzhhl.top/gtmmqcjgnc.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.bjfxy.top/gtzznzbmqr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.sxryk.cn/gtpghwcihm.html

C#:   interface IShape { double Area(); }
来源：http://hz.yuanzhike.top/gtfclsfcjs.html

[G10] 访问控制
来源：http://hz.chenlongwang.top/gtrbhzpiam.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.daria6918.cn/gtrqcydhfe.html

PHP:  public / protected / private
来源：http://hz.yj20258.top/gtsexigrgc.html

JS:   #private 字段；其余公开
来源：http://hz.jqgufenzy.top/gteuyxhciu.html

TS:   public / protected / private
来源：http://hz.dianchejie.cn/gttjxvotvz.html

Java: public / protected / private / 默认包级
来源：http://hz.yanxiufei.cn/gtozvgvihu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.c1oappe.top/gtzywirpje.html

Ruby: public / protected / private
来源：http://hz.jiagoushi.top/gtsptnqwhp.html

C#:   public / protected / private / internal
来源：http://hz.sysykeji.top/gtahwmcbld.html

[G11] getter / setter
来源：http://hz.bjfxy.top/gtwxfgjvdl.html

Py:   @property 与 @x.setter
来源：http://hz.jinqigufen.top/gtejgxzuau.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.meibo888.top/gtmklxyxgs.html

JS:   get name() { return this._name; }
来源：http://hz.mhx1999.top/gtjcerckam.html

TS:   get name(): string { return this._name; }
来源：http://hz.meibo888.top/gtdntakmln.html

Java: public String getName() { return name; }
来源：http://hz.52xcode.cn/gtwgybtfqa.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.vqdsnc.cn/gtzuxyflro.html

Ruby: attr_accessor :name
来源：http://hz.snrcjt.cn/gtufjozuof.html

C#:   public string Name { get; set; }
来源：http://hz.yuanzhike.top/gtuggsqsci.html

[G12] 对象转字符串
来源：http://hz.vqdsnc.cn/gtcdoalsfd.html

Py:   def __str__(self): return self.name
来源：http://hz.fengsongda.top/gtqbiemune.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.dashuyun.cn/gtwhdkklxk.html

JS:   toString() { return this.name; }
来源：http://hz.guannengcc.top/gtuwzpumso.html

TS:   toString(): string { return this.name; }
来源：http://hz.daxiang520.top/gtqudkkzad.html

Java: @Override public String toString() { return name; }
来源：http://hz.zhixingplan.top/gtrjnrrrdn.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.smart0.xyz/gttmrmytua.html

Ruby: def to_s; @name; end
来源：http://hz.zhoulong.xyz/gtlpvlxdst.html

C#:   public override string ToString() => Name;
来源：http://hz.yj202588.top/gtjetbhsxh.html

[G13] 判断对象类型
来源：http://hz.hywenlv.cn/gttjrsmrdv.html

Py:   isinstance(u, User)
来源：http://hz.ehwqpu.com/gttqdvwrie.html

PHP:  $u instanceof User
来源：http://hz.hammf.cn/gtmzuhjtaz.html

JS:   u instanceof User
来源：http://hz.pycfn.com/gtvntacehh.html

TS:   u instanceof User
来源：http://hz.ywan-chungtsiang.top/gtcfejqtra.html

Java: u instanceof User
来源：http://hz.gotoacloud.top/gtpixqzgue.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jianghu66.top/gttnzknpgr.html

Ruby: u.is_a?(User)
来源：http://hz.pengpengdd.cyou/gtoaywrujf.html

C#:   u is User
来源：http://hz.shangyingyoupin.top/gtrsiccnij.html

[G14] 数据类 / record
来源：http://hz.xziqi.cn/gteintibau.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yanxiufei.cn/gtiudrzjvh.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yongpay.top/gtwtnwspxv.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.feifeiyinyue.top/gtcqzrhptb.html

TS:   type User = { name: string; age: number };
来源：http://hz.cdnleiting.top/gtbjsaiiru.html

Java: record User(String name, int age) {}
来源：http://hz.pycfn.com/gtrczhucgf.html

Go:   type User struct { Name string; Age int }
来源：http://hz.dianchejie.cn/gtrmbptxnv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.sysykeji.top/gtymuyjvku.html

C#:   record User(string Name, int Age);
来源：http://hz.quarkkingdee.top/gtskuiuulz.html

[G15] 枚举
来源：http://hz.jinqigufen.top/gtxshtnrwd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jinyuanbaomall.cn/gthqjfysnm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.hongshengwenyu.top/gtskzoazdo.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.chenzaomai.com/gtppoiznho.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cheryme.top/gtwvatjofk.html

Java: enum Color { RED, GREEN }
来源：http://hz.guannengcc.top/gtlstmkqjf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jyoumei.cn/gtznmzwgqz.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zhengqikj.top/gtbwqkdvzr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xylfe.cn/gtgpbsdxid.html

[G16] 对象转数组 / 字典
来源：http://hz.tanke756.top/gtawasbgye.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.gogol.net.cn/gtmxtoolfg.html

PHP:  get_object_vars($obj);
来源：http://hz.nanxinkj.top/gtczdvwqav.html

JS:   Object.entries(obj)
来源：http://hz.yanxiufei.cn/gthjanzubt.html

TS:   Object.entries(obj)
来源：http://hz.yongpay.top/gtgiizmafu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.52xcode.cn/gtkugbzmiy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.nwbrower.top/gtzjtlfevk.html

Ruby: obj.instance_variables
来源：http://hz.jlsjyb.cn/gtclbrmleq.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.xingfuxueyuan.xyz/gtbngbvpaw.html

================================================================================
来源：http://hz.yj20258.top/gtuaiohhag.html

H. 异常与错误处理
来源：http://hz.shangyingyoupin.top/gtkxnhoems.html

================================================================================
来源：http://hz.9152youxi.cn/gtfuogycwh.html

[H01] try / catch 基础
来源：http://hz.yj202588.top/gtslmffrty.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.gotoacloud.top/gtgnudtsde.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.chenlongwang.top/gtexntitqd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.shangyingyoupin.top/gtsrvhzczd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.nanxinkj.top/gtjpnriucg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.gotoacloud.top/gtwlqotudq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zhoulong.xyz/gtoqfmfvoh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.nanxinkj.top/gtmoceautx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.9152youxi.cn/gtrndwcgys.html

[H02] finally / ensure 收尾
来源：http://hz.sufxvd.cn/gtknlxueji.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.aibaodan.cn/gtmafskowe.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.havefunace.top/gthjyozsdg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.ehwqpu.com/gtxpmzlufk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.cucudq.cn/gttlxfokyw.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.xuetiantiany.cn/gtaudgcpwi.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.shzxlz.cn/gtfxezbnky.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.hnqzz.top/gtrkbuwdnu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jyoumei.cn/gtpnxxyalt.html

[H03] 主动抛出异常
来源：http://hz.cdnleiting.top/gtetxawzzf.html

Py:   raise ValueError("错误信息")
来源：http://hz.pycfn.com/gtljaaueew.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.nanxinkj.top/gtgpdtriay.html

JS:   throw new Error("错误信息");
来源：http://hz.aizwys.cn/gtdxunnsnz.html

TS:   throw new Error("错误信息");
来源：http://hz.gogol.net.cn/gtgdhobkfa.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.smart0.xyz/gtrizrtfbu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.smart0.xyz/gtnayfstqd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jianghu66.top/gttefjlres.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yj20258888.top/gtikosnmux.html

[H04] 自定义异常类型
来源：http://hz.52xcode.cn/gtsrnksngg.html

Py:   class MyError(Exception): pass
来源：http://hz.xuanzx.com/gtcjryubqz.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.andypj.xyz/gtdgzjrfbf.html

JS:   class MyError extends Error {}
来源：http://hz.jiagoushi.top/gtnnbxjwkk.html

TS:   class MyError extends Error {}
来源：http://hz.hywenlv.cn/gtptorzrwq.html

Java: class MyException extends RuntimeException {}
来源：http://hz.fzhhl.top/gtwvspjoej.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.xuanzx.com/gtkjpqqzbh.html

Ruby: class MyError < StandardError; end
来源：http://hz.jqgufenzy.top/gtttmbweuf.html

C#:   class MyException : Exception {}
来源：http://hz.yj20258888.top/gtzsbphnoc.html

[H05] 捕获特定类型
来源：http://hz.gzhubu.top/gtpsgukqnz.html

Py:   except ValueError as e:
来源：http://hz.guannengcc.top/gtgcxsrdik.html


<!-- 参考信息 -->