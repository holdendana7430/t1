代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://hz.nwbrower.top/gtmquxryhr.html

[F02] 逐行读取文件
来源：http://hz.0kj1m.cn/gtyctmqsqd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yvedp.cn/gtnmchlsoz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.gotoacloud.top/gtnqzwipjs.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jlsjyb.cn/gtytpnorno.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hfpthk.cn/gtwtxxoudq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.kuanghao11.cn/gtmpjokkmc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.gogol.net.cn/gtiniiszte.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yongpay.top/gtxhuxmsbd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.hysaishi.cn/gtnhjgffij.html

[F03] 写入文件（覆盖）
来源：http://hz.svipenyu.cn/gtohhveakl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.pycfn.com/gtvuktqocd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.wangdashe.top/gtbdtsprda.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.chenzaomai.com/gtmhrcqqxn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.haohaochexian.top/gthezfdrmp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.wangshuangyany.cn/gtovitpbqa.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.cdnleiting.top/gtpfdyhsnl.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.smart0.xyz/gtuxaxqjvm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.iojbl.cn/gtnmhiojhq.html

[F04] 追加写入文件
来源：http://hz.nwbrower.top/gtvzagsqbm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yuanzhike.top/gtceijnpah.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.xylfe.cn/gtxbejkcrn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shuidangran.top/gtlpsrdlrp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hnxiangtu.top/gttwlbmsjq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.smart0.xyz/gtcdxcyrtz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yonumen.top/gtsvqifihg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.pengpengdd.cyou/gtgikasjig.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.shanyushiyangkeji.top/gtnvpvrttb.html

[F05] 判断文件或目录是否存在
来源：http://hz.jqgufenzy.top/gtlmlkgzps.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.jqgfzy.top/gtnmimbslg.html

PHP:  file_exists("a.txt");
来源：http://hz.meibo888.top/gtfbsupukm.html

JS:   fs.existsSync("a.txt")
来源：http://hz.gogol.net.cn/gtroccgauk.html

TS:   fs.existsSync("a.txt")
来源：http://hz.hywenlv.cn/gtcdqybyuc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.zhijiandao.cn/gtkqyvvzal.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.cucudq.cn/gtbesxgjwh.html

Ruby: File.exist?("a.txt")
来源：http://hz.hfpthk.cn/gtzicchoal.html

C#:   File.Exists("a.txt")
来源：http://hz.wangshuangyany.cn/gtwxidqflp.html

[F06] 删除文件
来源：http://hz.xylfe.cn/gtuwxyyqnd.html

Py:   os.remove("a.txt")
来源：http://hz.xziqi.cn/gtlsaqqtuy.html

PHP:  unlink("a.txt");
来源：http://hz.ybcxt.top/gtwhemfxci.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yj20258888.top/gtpmyzaeuv.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.svipenyu.cn/gtqidcnsco.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jinqigufen.top/gtvsejmqfk.html

Go:   os.Remove("a.txt")
来源：http://hz.hammf.cn/gtyrorcczx.html

Ruby: File.delete("a.txt")
来源：http://hz.tian-w.cn/gtfeirmsms.html

C#:   File.Delete("a.txt");
来源：http://hz.xuetiantiany.cn/gtmcjjettn.html

[F07] 创建目录（含多级）
来源：http://hz.redwolf501.top/gteojnkgdf.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hongshengwenyu.top/gtuqeqiubw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.pycfn.com/gtwdwsphyo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hfpthk.cn/gtxrlvcblp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.gzhubu.top/gtetwdzmrv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.xuetiantiany.cn/gtjqythcnk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yj20258.top/gtvvxvgckw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.shanyushiyangtech.top/gtsjbbhfbp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jyoumei.cn/gtictdkcll.html

[F08] 遍历目录
来源：http://hz.jyoumei.cn/gtilkxjlln.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.jinghuilouyu.cn/gtokacycad.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.gzhubu.top/gtqfeordmb.html

JS:   fs.readdirSync("dir")
来源：http://hz.ydjk.org.cn/gtrxpoaivj.html

TS:   fs.readdirSync("dir")
来源：http://hz.jyoumei.cn/gtupnyqxwn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.daria6918.cn/gtjsnjxwyk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.nanxinkj.top/gtfqoshfuc.html

Ruby: Dir.children("dir")
来源：http://hz.ppjwa.cn/gtraxrpdtf.html

C#:   Directory.GetFiles("dir")
来源：http://hz.bjfxy.top/gtzjdwlbzz.html

[F09] 获取文件大小
来源：http://hz.cashguo.top/gtglspmajk.html

Py:   os.path.getsize("a.txt")
来源：http://hz.aibaodan.cn/gtqmdnvxax.html

PHP:  filesize("a.txt");
来源：http://hz.jinqigufen.top/gtufdrwdno.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yj20258888.top/gtrbsixoar.html

TS:   fs.statSync("a.txt").size
来源：http://hz.guannengcc.top/gtzpqbhulj.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.ybcxt.top/gtseqaclqw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jiagoushi.top/gtrerfzbnj.html

Ruby: File.size("a.txt")
来源：http://hz.316326.xyz/gtzpugvqti.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.gogol.net.cn/gtyopbpuvv.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.nanxinkj.top/gtpsbbfyee.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.ivvv.top/gtpokrguxi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.guannengcc.top/gtspzjwoct.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.hongshengwenyu.top/gtijhrgdeu.html

TS:   path.extname("a.txt")
来源：http://hz.fengsongda.top/gtomwkxxlg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.ywan-chungtsiang.top/gtansbpywa.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.cqqwz.cn/gtyhwyqlcs.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.havefunace.top/gtsqyubvru.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.aizwys.cn/gtfsyttocr.html

[F11] 复制与移动文件
来源：http://hz.haohaochexian.top/gtcajcbxlb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.bjfxy.top/gtlbxikubh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.sweek.top/gtatwenbtt.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sysykeji.top/gtiwlmtbqz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yueranfly.top/gtgbyzkcsg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.pengpengdd.cyou/gtoaafnymv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yuanzhike.top/gtzlpzvlps.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yj202588.top/gtwbceclmw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jiagoushi.top/gtdqjujgxn.html

[F12] CSV 读写
来源：http://hz.gaohongyu789.top/gtxbxgpaeu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yj202588.top/gtdfcmnmsz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.gogol.net.cn/gtovfeqzuz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zhengqikj.top/gtkjizopki.html

TS:   // 同上
来源：http://hz.jiagoushi.top/gtheajlzae.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.c1oappe.top/gtbnshbdjc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zycfv.cn/gtwjovfxyz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.aibaodan.cn/gtwablbswa.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.gzhubu.top/gtcmwfduhm.html

================================================================================
来源：http://hz.ppjwa.cn/gttacmhoin.html

G. 面向对象
来源：http://hz.gzhubu.top/gtlkggyeeq.html

================================================================================
来源：http://hz.fengsongda.top/gtiligtjto.html

[G01] 定义类
来源：http://hz.zdqjudy.top/gteielilsm.html

Py:   class User: pass
来源：http://hz.jinghuilouyu.cn/gtcvbtupie.html

PHP:  class User {}
来源：http://hz.xziqi.cn/gtpybjxqpl.html

JS:   class User {}
来源：http://hz.jinghuilouyu.cn/gtsdephmtb.html

TS:   class User { name: string = ""; }
来源：http://hz.cheryme.top/gtpatvywrn.html

Java: class User {}
来源：http://hz.xylfe.cn/gtbxeqnsus.html

Go:   type User struct { Name string }
来源：http://hz.shanyushiyangkeji.top/gtqqhgswup.html

Ruby: class User; end
来源：http://hz.aibaodan.cn/gtyqhlziiq.html

C#:   class User {}
来源：http://hz.jianghu66.top/gtdppqwwvu.html

[G02] 构造函数
来源：http://hz.xylfe.cn/gtlrdmgkwo.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhiwuduotai.top/gtrrnwhzfc.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.feifeiyinyue.top/gtmpirdxmf.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.hywenlv.cn/gtnlmqxbed.html

TS:   constructor(public name: string) {}
来源：http://hz.xziqi.cn/gtrrmcawmv.html

Java: User(String name) { this.name = name; }
来源：http://hz.dashuyun.cn/gtleandpie.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.fzhhl.top/gtjgnpidrj.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.gogol.net.cn/gtbcmyyeve.html

C#:   public User(string name) { Name = name; }
来源：http://hz.tianlin.xyz/gtayylmipc.html

[G03] 实例属性
来源：http://hz.bjfxy.top/gtzcyjvepb.html

Py:   self.name = "x"
来源：http://hz.yuxming.cn/gtpgurgcdv.html

PHP:  public string $name = "x";
来源：http://hz.shanyushiyangkeji.top/gtmmxdjosl.html

JS:   this.name = "x";
来源：http://hz.pengpengdd.cyou/gtctmfcglf.html

TS:   name: string = "x";
来源：http://hz.xuanzx.com/gtoxzyqnpy.html

Java: private String name;
来源：http://hz.xuetiantiany.cn/gtvqoasdde.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.ywan-chungtsiang.top/gtivhwbkit.html

Ruby: @name = "x"
来源：http://hz.zdqjudy.top/gtnqtefktx.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.xylfe.cn/gtzgzqtzch.html

[G04] 定义方法
来源：http://hz.jianghu66.top/gtsliuhzfw.html

Py:   def greet(self): return self.name
来源：http://hz.yj20258888.top/gtewxdcmns.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yvedp.cn/gtpcvltbxn.html

JS:   greet() { return this.name; }
来源：http://hz.316326.xyz/gtkfmuklku.html

TS:   greet(): string { return this.name; }
来源：http://hz.sweek.top/gtsxhbbzwz.html

Java: String greet() { return name; }
来源：http://hz.hnxiangtu.top/gttivheags.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hnqzz.top/gtyupyiocc.html

Ruby: def greet; @name; end
来源：http://hz.chenjidiqi.icu/gtfjtlrtle.html

C#:   public string Greet() => Name;
来源：http://hz.zhoulong.xyz/gtcegzqiuw.html

[G05] 继承
来源：http://hz.wangshuangyany.cn/gtrgkqpvfa.html

Py:   class Admin(User): pass
来源：http://hz.jqgufenzy.top/gtpquwzxni.html

PHP:  class Admin extends User {}
来源：http://hz.quarkkingdee.top/gtovoglmde.html

JS:   class Admin extends User {}
来源：http://hz.zhixingplan.top/gtrsjapmlh.html

TS:   class Admin extends User {}
来源：http://hz.pengpengdd.cyou/gtrbmzvlwo.html

Java: class Admin extends User {}
来源：http://hz.yonumen.top/gtzgymwwkz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ywan-chungtsiang.top/gtlwymugny.html

Ruby: class Admin < User; end
来源：http://hz.yanxiufei.cn/gttujugqtx.html

C#:   class Admin : User {}
来源：http://hz.smart0.xyz/gtndmzbegx.html

[G06] 重写方法
来源：http://hz.sxryk.cn/gtzjygjqrz.html

Py:   def greet(self): return "admin"
来源：http://hz.zhijiandao.cn/gtheqxdlfy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.guannengcc.top/gtqyfrsrxv.html

JS:   greet() { return "admin"; }
来源：http://hz.ehwqpu.com/gtntvwddhn.html

TS:   greet(): string { return "admin"; }
来源：http://hz.daxiang520.top/gtqmnyjhul.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhengqikj.top/gtvyztezua.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.daria6918.cn/gthpdycjon.html

Ruby: def greet; "admin"; end
来源：http://hz.wangshuangyany.cn/gttkijgfox.html

C#:   public override string Greet() => "admin";
来源：http://hz.tianlin.xyz/gtfvpdupyr.html

[G07] 调用父类方法
来源：http://hz.316326.xyz/gtekohgziq.html

Py:   super().greet()
来源：http://hz.redwolf501.top/gtcrbfpunj.html

PHP:  parent::greet();
来源：http://hz.svipenyu.cn/gtyorgugfd.html

JS:   super.greet();
来源：http://hz.yueranfly.top/gtyqrpqkic.html

TS:   super.greet();
来源：http://hz.snrcjt.cn/gtwjlblzjm.html

Java: super.greet();
来源：http://hz.ybcxt.top/gtcznxjhol.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.smart0.xyz/gtsqjsgkwo.html

Ruby: super
来源：http://hz.hywenlv.cn/gtsixzilca.html

C#:   base.Greet();
来源：http://hz.zhaomingkeji.xyz/gtjwwlwxmk.html

[G08] 静态方法与属性
来源：http://hz.tianlin.xyz/gtnslzfjkz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.cdnleiting.top/gtxbmjqvog.html

PHP:  public static function f() {}
来源：http://hz.aibaodan.cn/gtxalkfetq.html

JS:   static f() {}
来源：http://hz.zdqjudy.top/gtzertgteq.html

TS:   static f(): void {}
来源：http://hz.tanke756.top/gtyzpikfqn.html

Java: static void f() {}
来源：http://hz.zhongyouzk.top/gtktcumqbw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yj20258.top/gtellxprlk.html

Ruby: def self.f; end
来源：http://hz.ydjk.org.cn/gtpnknskob.html

C#:   public static void F() {}
来源：http://hz.zhengqikj.top/gtxmzpyymy.html

[G09] 接口 / 抽象类
来源：http://hz.yueranfly.top/gtcmacwcsi.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.9152youxi.cn/gtlccitcrt.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.aizwys.cn/gtcyieeilp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.sufxvd.cn/gtmxilpwhm.html

TS:   interface Shape { area(): number; }
来源：http://hz.hfpthk.cn/gtdipuxrcl.html

Java: interface Shape { double area(); }
来源：http://hz.jinyuanbaomall.cn/gtqifpwmzn.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.52xcode.cn/gtztaikxuu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.wangshuangyany.cn/gtmnticxib.html

C#:   interface IShape { double Area(); }
来源：http://hz.0kj1m.cn/gtmyscrvnz.html

[G10] 访问控制
来源：http://hz.quarkkingdee.top/gtkzvozvuj.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.chenlongwang.top/gtgaophbze.html

PHP:  public / protected / private
来源：http://hz.shzxlz.cn/gthikcneex.html

JS:   #private 字段；其余公开
来源：http://hz.feifeiyinyue.top/gtzkmvhqrh.html

TS:   public / protected / private
来源：http://hz.xuetiantiany.cn/gtymhyssyk.html

Java: public / protected / private / 默认包级
来源：http://hz.havefunace.top/gtyjxvnrce.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yongpay.top/gtujdtpyxi.html

Ruby: public / protected / private
来源：http://hz.cdnleiting.top/gtqhhheidx.html

C#:   public / protected / private / internal
来源：http://hz.quarkkingdee.top/gtcexceggz.html

[G11] getter / setter
来源：http://hz.jyoumei.cn/gtrkzoljhr.html

Py:   @property 与 @x.setter
来源：http://hz.xylfe.cn/gtcphwsfch.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yvedp.cn/gtuzxmygqg.html

JS:   get name() { return this._name; }
来源：http://hz.ehwqpu.com/gtdhwuyhrk.html

TS:   get name(): string { return this._name; }
来源：http://hz.tanke756.top/gtwhqlpngx.html

Java: public String getName() { return name; }
来源：http://hz.zhaomingkeji.xyz/gtgnwwbdoy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.aizwys.cn/gttnfszuwe.html

Ruby: attr_accessor :name
来源：http://hz.jinqigufen.top/gtbxvpsljz.html

C#:   public string Name { get; set; }
来源：http://hz.xuanzx.com/gtmkkvfllr.html

[G12] 对象转字符串
来源：http://hz.yongpay.top/gtywaunljm.html

Py:   def __str__(self): return self.name
来源：http://hz.xziqi.cn/gtyzapiweo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.quarkkingdee.top/gtwqlwjknk.html

JS:   toString() { return this.name; }
来源：http://hz.andypj.xyz/gtadchgktx.html

TS:   toString(): string { return this.name; }
来源：http://hz.jiagoushi.top/gtlmobbtsp.html

Java: @Override public String toString() { return name; }
来源：http://hz.feifeiyinyue.top/gtdvzwjczk.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.kuanghao11.cn/gtvcdmeecj.html

Ruby: def to_s; @name; end
来源：http://hz.chenlongwang.top/gtblpuqtsj.html

C#:   public override string ToString() => Name;
来源：http://hz.dashuyun.cn/gtjlhaemni.html

[G13] 判断对象类型
来源：http://hz.c1oappe.top/gttmupwnzj.html

Py:   isinstance(u, User)
来源：http://hz.wangdashe.top/gtwqqjwcbr.html

PHP:  $u instanceof User
来源：http://hz.jianghu66.top/gtamtdzgjo.html

JS:   u instanceof User
来源：http://hz.feifeiyinyue.top/gtokzgqiea.html

TS:   u instanceof User
来源：http://hz.tianlin.xyz/gtricerbuj.html

Java: u instanceof User
来源：http://hz.ehwqpu.com/gtwordthyh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.xinyue.icu/gtccxpiexw.html

Ruby: u.is_a?(User)
来源：http://hz.bjfxy.top/gtpecxvpcp.html

C#:   u is User
来源：http://hz.jlsjyb.cn/gtghqqsaox.html

[G14] 数据类 / record
来源：http://hz.yvedp.cn/gtoerlyaqa.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.gaohongyu789.top/gtnvrvhsrz.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yueranfly.top/gtyxzznzir.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jianghu66.top/gtbmpepiaa.html

TS:   type User = { name: string; age: number };
来源：http://hz.nanxinkj.top/gtuqgycokz.html

Java: record User(String name, int age) {}
来源：http://hz.chenlongwang.top/gtlgntyvoz.html

Go:   type User struct { Name string; Age int }
来源：http://hz.ivvv.top/gtaxhmmdwm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.hongshengwenyu.top/gtftpvmrgt.html

C#:   record User(string Name, int Age);
来源：http://hz.andypj.xyz/gtazvlwayw.html

[G15] 枚举
来源：http://hz.tianlin.xyz/gtxwtkmkfe.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.sxryk.cn/gtsfibdnam.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.shuidangran.top/gtrzxwhhil.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hysaishi.cn/gtlmvmwktf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.52xcode.cn/gtajygcqiu.html

Java: enum Color { RED, GREEN }
来源：http://hz.shzxlz.cn/gthiiknvou.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.vqdsnc.cn/gtjpftsibq.html

Ruby: Color = %i[red green].freeze
来源：http://hz.chenjidiqi.icu/gtunxnnwfv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hnxiangtu.top/gtrwdhuzkz.html

[G16] 对象转数组 / 字典
来源：http://hz.hammf.cn/gtpyygquud.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.sufxvd.cn/gtmrsctngm.html

PHP:  get_object_vars($obj);
来源：http://hz.kuanghao11.cn/gtuauyfyss.html

JS:   Object.entries(obj)
来源：http://hz.zhiwuduotai.top/gtyxyviinb.html

TS:   Object.entries(obj)
来源：http://hz.9152youxi.cn/gtkxjhxcux.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jqgufenzy.top/gtzfklnuqs.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yj20258.top/gtmumedmds.html

Ruby: obj.instance_variables
来源：http://hz.hfpthk.cn/gtuutzfprn.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.shanyushiyangtech.top/gtpjxwgboe.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtqulwwder.html

H. 异常与错误处理
来源：http://hz.bjfxy.top/gtmboeukgf.html

================================================================================
来源：http://hz.nwbrower.top/gtyrdduqvw.html

[H01] try / catch 基础
来源：http://hz.xziqi.cn/gtyoluvmpk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.xuetiantiany.cn/gtslwyjpsz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yj202588.top/gttqljlvhn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.haohaochexian.top/gtwsrvmrrw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.birdmap.top/gtjhveyixy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.feifeiyinyue.top/gtjnnwflom.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zhengqikj.top/gtenfqzqvz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.nanxinkj.top/gthczuzwbf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.xziqi.cn/gtahmopzvs.html

[H02] finally / ensure 收尾
来源：http://hz.svipenyu.cn/gteffjiurx.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.hongshengwenyu.top/gtfraxqtvh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.316326.xyz/gtggmrzktp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yanxiufei.cn/gthuzetzqm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.aizwys.cn/gtqxhbgayp.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yueranfly.top/gtqgqirbcj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.sxryk.cn/gtewcucrdr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jinghuilouyu.cn/gttgrrrfqq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.gzhubu.top/gtovusjoji.html

[H03] 主动抛出异常
来源：http://hz.dianchejie.cn/gtovkpciwp.html

Py:   raise ValueError("错误信息")
来源：http://hz.pengpengdd.cyou/gtqfevuwuo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.ydzc1.top/gtazyoocqc.html

JS:   throw new Error("错误信息");
来源：http://hz.shangyingyoupin.top/gtlzbmjovv.html

TS:   throw new Error("错误信息");
来源：http://hz.snrcjt.cn/gtixicpnhc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.redwolf501.top/gtrnftlsuj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hammf.cn/gtjtorikpk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.xziqi.cn/gtrexyzbcm.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.shanyushiyangkeji.top/gtmwktcsel.html

[H04] 自定义异常类型
来源：http://hz.hammf.cn/gtlfjvkgdr.html

Py:   class MyError(Exception): pass
来源：http://hz.jlsjyb.cn/gtshgulvie.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.xylfe.cn/gtnrtxhcan.html

JS:   class MyError extends Error {}
来源：http://hz.nwbrower.top/gtjkmigqtp.html

TS:   class MyError extends Error {}
来源：http://hz.hammf.cn/gtboysavil.html

Java: class MyException extends RuntimeException {}
来源：http://hz.kuanghao11.cn/gtknebyfvy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.nanxuanxn.top/gtubrqiqir.html

Ruby: class MyError < StandardError; end
来源：http://hz.tanke756.top/gteakzxteb.html

C#:   class MyException : Exception {}
来源：http://hz.zhijiandao.cn/gtiopgjgld.html

[H05] 捕获特定类型
来源：http://hz.ywan-chungtsiang.top/gtunkvisqw.html

Py:   except ValueError as e:
来源：http://hz.redwolf501.top/gtgmbjifxs.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yuanzhike.top/gtyqrxygtr.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jinyuanbaomall.cn/gtrwibxova.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.chenjidiqi.icu/gthebaczlw.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yanxiufei.cn/gtmgpdtwni.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hongshengwenyu.top/gtylihbcmp.html

Ruby: rescue ArgumentError => e
来源：http://hz.yonumen.top/gtaqqqoehl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.ehwqpu.com/gtrtpzgygh.html

[H06] 可选值 / 空值安全访问
来源：http://hz.pycfn.com/gtexgzecct.html

Py:   value = d.get("k") or default
来源：http://hz.bjfxy.top/gtvrfazujp.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.iojbl.cn/gtjnfsgrje.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.gogol.net.cn/gtefkhiahg.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zhaomingkeji.xyz/gtkcrikcsc.html


<!-- 参考信息 -->