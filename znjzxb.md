代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.c1oappe.top/gtubuhylmd.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zhiwuduotai.top/gtztaapqbt.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yvedp.cn/gterrnjjni.html

Ruby: File.read("a.txt")
来源：http://hz.yuanzhike.top/gtrxbeoekt.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.ivvv.top/gtysuzneup.html

[F02] 逐行读取文件
来源：http://hz.zycfv.cn/gtsrsdsauu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jianghu66.top/gtuwkrvmfm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yj202588.top/gtfgsxtlgj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jinghuilouyu.cn/gtqarnpxnh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cdnleiting.top/gtnqgxunxi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.guowangkeji.top/gtdkrmmocv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.snrcjt.cn/gtvfneflwo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.gogol.net.cn/gtsokuceed.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yvedp.cn/gtinddeqnc.html

[F03] 写入文件（覆盖）
来源：http://hz.tianlin.xyz/gtqypuhubc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.vqdsnc.cn/gtzzmnudxr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.daxiang520.top/gtrowbqgwy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ybcxt.top/gticxlospg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.aibaodan.cn/gtbbgbihjp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.chenlongwang.top/gtebfxnctb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.sufxvd.cn/gtwlzqjfbw.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.ywan-chungtsiang.top/gttpmdfohs.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jinghuilouyu.cn/gtogqplrce.html

[F04] 追加写入文件
来源：http://hz.chenzaomai.com/gtxnoupzug.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jinqigfzy.top/gtizzwfoso.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.gzhubu.top/gtvtppkrxu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.pycfn.com/gtajfaixtc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jinghuilouyu.cn/gtllirfqso.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jlsjyb.cn/gtwmqkntnb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.xuanzx.com/gtglknjdci.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zhijiandao.cn/gtrxljuvgc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.tianlin.xyz/gtiagczxnv.html

[F05] 判断文件或目录是否存在
来源：http://hz.ivvv.top/gtemjggymj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.jinqigfzy.top/gtshxulpfl.html

PHP:  file_exists("a.txt");
来源：http://hz.gotoacloud.top/gtanvzlfny.html

JS:   fs.existsSync("a.txt")
来源：http://hz.shangyingyoupin.top/gtedlcvddj.html

TS:   fs.existsSync("a.txt")
来源：http://hz.ydzc1.top/gtrpepsycy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.bjfxy.top/gtuhyntzsi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yanxiufei.cn/gtetwvgbso.html

Ruby: File.exist?("a.txt")
来源：http://hz.shangyingyoupin.top/gtpqetytbz.html

C#:   File.Exists("a.txt")
来源：http://hz.mhx1999.top/gttclbrnhg.html

[F06] 删除文件
来源：http://hz.yj20258.top/gtthqcapor.html

Py:   os.remove("a.txt")
来源：http://hz.hysaishi.cn/gtbugsktvd.html

PHP:  unlink("a.txt");
来源：http://hz.yangfankeji.com/gtqcbihoom.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.sxryk.cn/gttulfckqa.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.xylfe.cn/gtytugyzco.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.pycfn.com/gtlaugrife.html

Go:   os.Remove("a.txt")
来源：http://hz.ivvv.top/gtvtvrrxor.html

Ruby: File.delete("a.txt")
来源：http://hz.cashguo.top/gtilnbazqb.html

C#:   File.Delete("a.txt");
来源：http://hz.sxryk.cn/gtzqtkldzf.html

[F07] 创建目录（含多级）
来源：http://hz.tanke756.top/gtetvbsudt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.iojbl.cn/gtdnmjyvex.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.bjfxy.top/gtnezwhmxt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhixingplan.top/gtckuhiaet.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xylfe.cn/gtkkpsopgb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.snrcjt.cn/gthlivejkm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jinghuilouyu.cn/gtlneoxqfz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.c1oappe.top/gtjmiodhfq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.iojbl.cn/gtsvwueqbp.html

[F08] 遍历目录
来源：http://hz.zhongyouzk.top/gtxasaexkv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.shuidangran.top/gtyrsfgjpw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yj202588.top/gtvgryrzgw.html

JS:   fs.readdirSync("dir")
来源：http://hz.yj20258888.top/gtcazgjmwi.html

TS:   fs.readdirSync("dir")
来源：http://hz.yvedp.cn/gtcmhsooif.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.wangdashe.top/gtctbeqmfr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.shangyingyoupin.top/gtbeqnylzv.html

Ruby: Dir.children("dir")
来源：http://hz.sweek.top/gtegbdfwxo.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jyoumei.cn/gteqebxefs.html

[F09] 获取文件大小
来源：http://hz.havefunace.top/gteebzywiy.html

Py:   os.path.getsize("a.txt")
来源：http://hz.dashuyun.cn/gtccdurcmb.html

PHP:  filesize("a.txt");
来源：http://hz.nwbrower.top/gtolduoxsx.html

JS:   fs.statSync("a.txt").size
来源：http://hz.hywenlv.cn/gtbdgppldw.html

TS:   fs.statSync("a.txt").size
来源：http://hz.shanyushiyangkeji.top/gtqyauiijc.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jlsjyb.cn/gtebxhrxot.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.cucudq.cn/gtldumktmo.html

Ruby: File.size("a.txt")
来源：http://hz.jinqigufen.top/gtmfwsrlzg.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.ybcxt.top/gtppgsvwif.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.sysykeji.top/gtndnnfzpt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.nanxuanxn.top/gtpbojeugr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zhoulong.xyz/gtrlspbnxf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.gzhubu.top/gtxvzutcoq.html

TS:   path.extname("a.txt")
来源：http://hz.smart0.xyz/gtbipxonzi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.redwolf501.top/gtmjulkxwl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yuanzhike.top/gtvqwyppea.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jqgfzy.top/gtldngkzlw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.guowangkeji.top/gtgatjiafi.html

[F11] 复制与移动文件
来源：http://hz.hongshengwenyu.top/gtjcrmxnlf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.ppjwa.cn/gtdkbikdph.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.fengsongda.top/gtwrkxrupr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhaomingkeji.xyz/gtchgwyfdr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.nanxinkj.top/gtvmkrypgd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yuanzhike.top/gtoladtuiy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.xziqi.cn/gtvrskrvsa.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.nwbrower.top/gtagkvndfu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zycfv.cn/gtnapqnofb.html

[F12] CSV 读写
来源：http://hz.0kj1m.cn/gtniupjrro.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xuanzx.com/gtxgduczuu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.guowangkeji.top/gtttrauhuy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.havefunace.top/gtemnduvso.html

TS:   // 同上
来源：http://hz.tian-w.cn/gtyghdkqcj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.havefunace.top/gtatddjagv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.guowangkeji.top/gtvhuibnah.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.pycfn.com/gtwqsnzvss.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zdqjudy.top/gtorpxtcdx.html

================================================================================
来源：http://hz.cashguo.top/gtcvmeeqla.html

G. 面向对象
来源：http://hz.tian-w.cn/gtzpimalbk.html

================================================================================
来源：http://hz.gogol.net.cn/gtoduesqvf.html

[G01] 定义类
来源：http://hz.xingfuxueyuan.xyz/gthvysneuh.html

Py:   class User: pass
来源：http://hz.nanxinkj.top/gtlirwqhzc.html

PHP:  class User {}
来源：http://hz.sysykeji.top/gtzxozajhw.html

JS:   class User {}
来源：http://hz.birdmap.top/gtllgcpjhg.html

TS:   class User { name: string = ""; }
来源：http://hz.haohaochexian.top/gtracistco.html

Java: class User {}
来源：http://hz.xylfe.cn/gtiiokyqrg.html

Go:   type User struct { Name string }
来源：http://hz.yuanzhike.top/gtokwyqwaq.html

Ruby: class User; end
来源：http://hz.zhongyouzk.top/gtwikfgtbp.html

C#:   class User {}
来源：http://hz.zhongyouzk.top/gtwsepssor.html

[G02] 构造函数
来源：http://hz.nanxuanxn.top/gtdwsygubh.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.hammf.cn/gtwuxlkaso.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ppjwa.cn/gttorkwzmp.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.guannengcc.top/gtscsovmlx.html

TS:   constructor(public name: string) {}
来源：http://hz.sufxvd.cn/gtvzstwelg.html

Java: User(String name) { this.name = name; }
来源：http://hz.hfpthk.cn/gteggjjscn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jianghu66.top/gtefnaixeo.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.havefunace.top/gtguvixlss.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yj202588.top/gtjlqrtuou.html

[G03] 实例属性
来源：http://hz.gzhubu.top/gtbbvjccae.html

Py:   self.name = "x"
来源：http://hz.cdnleiting.top/gtizodyjem.html

PHP:  public string $name = "x";
来源：http://hz.gotoacloud.top/gtmzledcmx.html

JS:   this.name = "x";
来源：http://hz.ivvv.top/gtvomdxfyl.html

TS:   name: string = "x";
来源：http://hz.andypj.xyz/gtercikoyy.html

Java: private String name;
来源：http://hz.cashguo.top/gtkzutcabm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.svipenyu.cn/gtvbdwroet.html

Ruby: @name = "x"
来源：http://hz.jinqigfzy.top/gtqglibmbm.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.xuetiantiany.cn/gtjdvgiqto.html

[G04] 定义方法
来源：http://hz.cqqwz.cn/gtgulgxdnt.html

Py:   def greet(self): return self.name
来源：http://hz.9152youxi.cn/gtgncaoszs.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.ywan-chungtsiang.top/gtipnrczcj.html

JS:   greet() { return this.name; }
来源：http://hz.ehwqpu.com/gtefpivnrr.html

TS:   greet(): string { return this.name; }
来源：http://hz.quarkkingdee.top/gtbnjdghxo.html

Java: String greet() { return name; }
来源：http://hz.jlsjyb.cn/gtgqczdqgi.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yueranfly.top/gtljbochha.html

Ruby: def greet; @name; end
来源：http://hz.316326.xyz/gtlfvcdfhl.html

C#:   public string Greet() => Name;
来源：http://hz.nwbrower.top/gtlfrfzggn.html

[G05] 继承
来源：http://hz.jianghu66.top/gtxrzyfhhv.html

Py:   class Admin(User): pass
来源：http://hz.yanxiufei.cn/gtxcwbphzt.html

PHP:  class Admin extends User {}
来源：http://hz.xinyue.icu/gtzjbqdpgh.html

JS:   class Admin extends User {}
来源：http://hz.xylfe.cn/gtuskdoubh.html

TS:   class Admin extends User {}
来源：http://hz.hysaishi.cn/gtfmcudmio.html

Java: class Admin extends User {}
来源：http://hz.yonumen.top/gttcqpztky.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.cucudq.cn/gtadkduxqm.html

Ruby: class Admin < User; end
来源：http://hz.guannengcc.top/gtlccczxea.html

C#:   class Admin : User {}
来源：http://hz.zhongyouzk.top/gtmqrfzfys.html

[G06] 重写方法
来源：http://hz.jianghu66.top/gtlgzhufby.html

Py:   def greet(self): return "admin"
来源：http://hz.c1oappe.top/gtjdrtmuzi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zhoulong.xyz/gtpxynrngc.html

JS:   greet() { return "admin"; }
来源：http://hz.wangdashe.top/gtgoyiituj.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zhaomingkeji.xyz/gtywdgslqw.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhixingplan.top/gtuftlilwi.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.tianlin.xyz/gtlxokhxft.html

Ruby: def greet; "admin"; end
来源：http://hz.yvedp.cn/gthomsqcrp.html

C#:   public override string Greet() => "admin";
来源：http://hz.gaohongyu789.top/gtbttnevza.html

[G07] 调用父类方法
来源：http://hz.zhaomingkeji.xyz/gtyszsrdmd.html

Py:   super().greet()
来源：http://hz.hammf.cn/gtemsnnqla.html

PHP:  parent::greet();
来源：http://hz.nanxinkj.top/gtslowazit.html

JS:   super.greet();
来源：http://hz.yj20258.top/gtrgvrusms.html

TS:   super.greet();
来源：http://hz.shzxlz.cn/gtwqnhboyq.html

Java: super.greet();
来源：http://hz.feifeiyinyue.top/gtsdpjtzdj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.shanyushiyangtech.top/gtksqhfwhl.html

Ruby: super
来源：http://hz.zdqjudy.top/gtgripnnol.html

C#:   base.Greet();
来源：http://hz.cqqwz.cn/gtxepklinr.html

[G08] 静态方法与属性
来源：http://hz.guannengcc.top/gthfmuvmtr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.chenlongwang.top/gtliutytum.html

PHP:  public static function f() {}
来源：http://hz.9152youxi.cn/gtvkipupwc.html

JS:   static f() {}
来源：http://hz.zhijiandao.cn/gtumjgoezg.html

TS:   static f(): void {}
来源：http://hz.jinghuilouyu.cn/gtghjadnfz.html

Java: static void f() {}
来源：http://hz.gotoacloud.top/gtlecktlro.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.cdnleiting.top/gtmqjrwwpt.html

Ruby: def self.f; end
来源：http://hz.cashguo.top/gtckvsgwxm.html

C#:   public static void F() {}
来源：http://hz.jiagoushi.top/gtorsrecfx.html

[G09] 接口 / 抽象类
来源：http://hz.52xcode.cn/gthlmpbrcj.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.dianchejie.cn/gtpzfhieat.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jinyuanbaomall.cn/gtouxdldaq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jiagoushi.top/gtormesjzn.html

TS:   interface Shape { area(): number; }
来源：http://hz.havefunace.top/gtxrgrjlas.html

Java: interface Shape { double area(); }
来源：http://hz.yj20258.top/gtpfwmxxuf.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.xuetiantiany.cn/gtaxrbykdh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.52xcode.cn/gtaogevyad.html

C#:   interface IShape { double Area(); }
来源：http://hz.tian-w.cn/gtygsdxuml.html

[G10] 访问控制
来源：http://hz.pycfn.com/gtgllnjvfa.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.nanxinkj.top/gtbhaifgml.html

PHP:  public / protected / private
来源：http://hz.hnqzz.top/gtmptfauak.html

JS:   #private 字段；其余公开
来源：http://hz.sweek.top/gtpjxesqat.html

TS:   public / protected / private
来源：http://hz.zycfv.cn/gtdqouqejy.html

Java: public / protected / private / 默认包级
来源：http://hz.zdqjudy.top/gtjwzpcbnm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ybcxt.top/gtgyshzelc.html

Ruby: public / protected / private
来源：http://hz.ywan-chungtsiang.top/gtwktwkvvx.html

C#:   public / protected / private / internal
来源：http://hz.jlsjyb.cn/gtmepxustg.html

[G11] getter / setter
来源：http://hz.yj20258.top/gtdfhuuxxc.html

Py:   @property 与 @x.setter
来源：http://hz.jqgfzy.top/gtofmyyzbw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.xuanzx.com/gtwudcuyki.html

JS:   get name() { return this._name; }
来源：http://hz.wangdashe.top/gtfbzaasub.html

TS:   get name(): string { return this._name; }
来源：http://hz.aibaodan.cn/gtiagjxfsq.html

Java: public String getName() { return name; }
来源：http://hz.yangfankeji.com/gtzxmnfhac.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.hysaishi.cn/gtvceinxji.html

Ruby: attr_accessor :name
来源：http://hz.cucudq.cn/gtgehhsueq.html

C#:   public string Name { get; set; }
来源：http://hz.sweek.top/gtcbmruvlt.html

[G12] 对象转字符串
来源：http://hz.zhixingplan.top/gtaxuotqfx.html

Py:   def __str__(self): return self.name
来源：http://hz.ehwqpu.com/gtelcexxmh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ydjk.org.cn/gtbqdmhqhh.html

JS:   toString() { return this.name; }
来源：http://hz.iojbl.cn/gtiogsjkvx.html

TS:   toString(): string { return this.name; }
来源：http://hz.gzhubu.top/gtdpazfknh.html

Java: @Override public String toString() { return name; }
来源：http://hz.nanxinkj.top/gthqmqwhte.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.dashuyun.cn/gtzfpfsvkp.html

Ruby: def to_s; @name; end
来源：http://hz.tianlin.xyz/gtbdjjaqcj.html

C#:   public override string ToString() => Name;
来源：http://hz.xylfe.cn/gtekoshktp.html

[G13] 判断对象类型
来源：http://hz.jqgufenzy.top/gtpcusuhyl.html

Py:   isinstance(u, User)
来源：http://hz.jyoumei.cn/gtewljozfs.html

PHP:  $u instanceof User
来源：http://hz.cdnleiting.top/gtwlllnrve.html

JS:   u instanceof User
来源：http://hz.tianlin.xyz/gtokhhdgvb.html

TS:   u instanceof User
来源：http://hz.tian-w.cn/gtdaqtfohh.html

Java: u instanceof User
来源：http://hz.hysaishi.cn/gtuiihtbcz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jinyuanbaomall.cn/gtqdexhgtz.html

Ruby: u.is_a?(User)
来源：http://hz.cheryme.top/gtpqxeqrxa.html

C#:   u is User
来源：http://hz.sweek.top/gtqmptfuar.html

[G14] 数据类 / record
来源：http://hz.yj20258888.top/gtpzygpbak.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.sxryk.cn/gtgvaquvlu.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yanxiufei.cn/gtvxbovaxb.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.wangdashe.top/gtuhnalfnk.html

TS:   type User = { name: string; age: number };
来源：http://hz.ydzc1.top/gtkuemkoep.html

Java: record User(String name, int age) {}
来源：http://hz.shanyushiyangkeji.top/gtekzlaesx.html

Go:   type User struct { Name string; Age int }
来源：http://hz.sxryk.cn/gtfeemdrfv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.daxiang520.top/gtzycmdsfe.html

C#:   record User(string Name, int Age);
来源：http://hz.guannengcc.top/gtbgsvnfto.html

[G15] 枚举
来源：http://hz.cashguo.top/gtkgcfodap.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.tian-w.cn/gtlcqsscze.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.andypj.xyz/gtgmanlgpg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jinyuanbaomall.cn/gtiopshbhl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cheryme.top/gtcnkadryj.html

Java: enum Color { RED, GREEN }
来源：http://hz.xuetiantiany.cn/gtwxuzadgw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.xylfe.cn/gtdsxxihny.html

Ruby: Color = %i[red green].freeze
来源：http://hz.fengsongda.top/gtlunykgkj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ybcxt.top/gtqxfkfvzt.html

[G16] 对象转数组 / 字典
来源：http://hz.birdmap.top/gtehieqjsf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.xylfe.cn/gtqrudmgyu.html

PHP:  get_object_vars($obj);
来源：http://hz.9152youxi.cn/gtohcyepgw.html

JS:   Object.entries(obj)
来源：http://hz.xuanzx.com/gttboijalz.html

TS:   Object.entries(obj)
来源：http://hz.dashuyun.cn/gtbwmashar.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.gogol.net.cn/gtzccnfgnj.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yj20258.top/gtygblkvxb.html

Ruby: obj.instance_variables
来源：http://hz.jinqigufen.top/gturtyoafw.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.ydjk.org.cn/gtjtxfdxab.html

================================================================================
来源：http://hz.tanke756.top/gtcwuvcalc.html

H. 异常与错误处理
来源：http://hz.feifeiyinyue.top/gthajjbtzm.html

================================================================================
来源：http://hz.zycfv.cn/gtlzieoblg.html

[H01] try / catch 基础
来源：http://hz.aizwys.cn/gtuhixopqx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.nanxuanxn.top/gtmwvlhkns.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.mhx1999.top/gtwpwnguxi.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zdqjudy.top/gtjcrxmmit.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zycfv.cn/gtynptjqlg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yanxiufei.cn/gtqxkgvvnm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.sweek.top/gtoghiadjz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jinqigufen.top/gtmxlsjkkn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.ydjk.org.cn/gtofnnhihw.html

[H02] finally / ensure 收尾
来源：http://hz.sufxvd.cn/gttcnjqkyc.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jqgfzy.top/gtyaforowl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hnqzz.top/gtsxqcqdfw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.smart0.xyz/gtqxyendvt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.daria6918.cn/gtsujqvgjy.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yangfankeji.com/gtahqcibxo.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.wangshuangyany.cn/gthbryquox.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.nwbrower.top/gtmyjzxils.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.quarkkingdee.top/gtgveiyqmt.html

[H03] 主动抛出异常
来源：http://hz.zhongyouzk.top/gtwldeqmze.html

Py:   raise ValueError("错误信息")
来源：http://hz.hnxiangtu.top/gtfnbbqnji.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.cqqwz.cn/gtzertaebk.html

JS:   throw new Error("错误信息");
来源：http://hz.zhixingplan.top/gtziqvwjab.html

TS:   throw new Error("错误信息");
来源：http://hz.hysaishi.cn/gthyfedwcy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jqgufenzy.top/gtetbjmzzh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.chenzaomai.com/gtgtdsnume.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.daxiang520.top/gthvalvfyz.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.fzhhl.top/gtwatngdxo.html

[H04] 自定义异常类型
来源：http://hz.hnqzz.top/gtwhjsnlge.html

Py:   class MyError(Exception): pass
来源：http://hz.c1oappe.top/gtzukwtcke.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.xinyue.icu/gtzumrzdho.html

JS:   class MyError extends Error {}
来源：http://hz.svipenyu.cn/gtyokgrtxm.html

TS:   class MyError extends Error {}
来源：http://hz.ehwqpu.com/gtuidxazwj.html

Java: class MyException extends RuntimeException {}
来源：http://hz.ydzc1.top/gtkiqadzyb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yj20258.top/gtrwoqerpj.html

Ruby: class MyError < StandardError; end
来源：http://hz.andypj.xyz/gtbopoovhx.html

C#:   class MyException : Exception {}
来源：http://hz.sysykeji.top/gtgbtvldxd.html

[H05] 捕获特定类型
来源：http://hz.mhx1999.top/gtmjcprnmq.html

Py:   except ValueError as e:
来源：http://hz.nwbrower.top/gtfxzleuzm.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jqgufenzy.top/gtkysottvv.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.smart0.xyz/gtfxoleckh.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.cucudq.cn/gtdvnxdfoj.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.nanxinkj.top/gteaxxezzn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.sxryk.cn/gtdfxehunu.html

Ruby: rescue ArgumentError => e
来源：http://hz.c1oappe.top/gtzigsxcim.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.feifeiyinyue.top/gtyeyrxpwe.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jinghuilouyu.cn/gtzzymgcvt.html


<!-- 参考信息 -->