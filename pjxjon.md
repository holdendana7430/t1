代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.ydzc1.top/gtwfemccrw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.cheryme.top/gtyumdvchj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.shanyushiyangkeji.top/gtttzswzyi.html

Ruby: File.read("a.txt")
来源：http://hz.hnqzz.top/gtdvrmllcg.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jyoumei.cn/gtyvdfolxe.html

[F02] 逐行读取文件
来源：http://hz.nanxinkj.top/gtzgppenql.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.cashguo.top/gthxyxiaku.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yuxming.cn/gtshdxofby.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hongshengwenyu.top/gtoepalgyp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hfpthk.cn/gttutyuuss.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.havefunace.top/gtqheazcdp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.fengsongda.top/gtnsjvifpr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.dianchejie.cn/gtcjbpmxor.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.jinqigufen.top/gttodikxxd.html

[F03] 写入文件（覆盖）
来源：http://hz.meibo888.top/gtfzfbfjyr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.cucudq.cn/gtihgarmbu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.xuetiantiany.cn/gtqvifxwap.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.bjfxy.top/gtoaftnthi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.guannengcc.top/gtturatczm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.yj20258888.top/gtpvqqrwvs.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.aizwys.cn/gtuhwttmfy.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zhengqikj.top/gtyxravhcq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.ywan-chungtsiang.top/gtbrvkmszo.html

[F04] 追加写入文件
来源：http://hz.zhengqikj.top/gtwclzgbqi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.xuanzx.com/gtzacdrxno.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.shanyushiyangkeji.top/gtexzbfmsd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.andypj.xyz/gtdzrpmadk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yangfankeji.com/gtdpvnjsnc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.chenjidiqi.icu/gtueffdhtm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jqgufenzy.top/gtenbaidyo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yuanzhike.top/gtkfopdszi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.ywan-chungtsiang.top/gtglzkryiu.html

[F05] 判断文件或目录是否存在
来源：http://hz.cucudq.cn/gtyojkvmpd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.vqdsnc.cn/gthkreadlr.html

PHP:  file_exists("a.txt");
来源：http://hz.meibo888.top/gtabpbbddi.html

JS:   fs.existsSync("a.txt")
来源：http://hz.feifeiyinyue.top/gtlkhazgtl.html

TS:   fs.existsSync("a.txt")
来源：http://hz.dianchejie.cn/gtgmchbkdd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.cucudq.cn/gtkpqymtxw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.kuanghao11.cn/gtqplhnked.html

Ruby: File.exist?("a.txt")
来源：http://hz.sufxvd.cn/gtwgnvzmdn.html

C#:   File.Exists("a.txt")
来源：http://hz.kuanghao11.cn/gtgyxyfgrk.html

[F06] 删除文件
来源：http://hz.tianlin.xyz/gtlamtwspm.html

Py:   os.remove("a.txt")
来源：http://hz.chenzaomai.com/gtyrufnfqg.html

PHP:  unlink("a.txt");
来源：http://hz.snrcjt.cn/gtijcvnfzg.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yanxiufei.cn/gtzyytxhji.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.gotoacloud.top/gtcfyilqym.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.andypj.xyz/gtcaiiaczi.html

Go:   os.Remove("a.txt")
来源：http://hz.tian-w.cn/gtzmpyklzn.html

Ruby: File.delete("a.txt")
来源：http://hz.dianchejie.cn/gtkpxuwzlb.html

C#:   File.Delete("a.txt");
来源：http://hz.sxryk.cn/gtgmqgelht.html

[F07] 创建目录（含多级）
来源：http://hz.hysaishi.cn/gtwmxmxelz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.fengsongda.top/gtamivyrxq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.mhx1999.top/gtyyeguajk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zdqjudy.top/gtuvywfkzw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.havefunace.top/gtxzfsttgw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hongshengwenyu.top/gtmbddsmdi.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hnxiangtu.top/gtzvncegby.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yangfankeji.com/gtieipohoe.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zhengqikj.top/gtriuhgvug.html

[F08] 遍历目录
来源：http://hz.tanke756.top/gtydgvjhwc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.tianlin.xyz/gtiundacvl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.0kj1m.cn/gtbzmxxjbd.html

JS:   fs.readdirSync("dir")
来源：http://hz.zhaomingkeji.xyz/gtxohgvfcd.html

TS:   fs.readdirSync("dir")
来源：http://hz.yj20258888.top/gthqohvoyy.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.gaohongyu789.top/gtxbugioyq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yj202588.top/gtqqfkkgza.html

Ruby: Dir.children("dir")
来源：http://hz.shzxlz.cn/gtiawvzfyt.html

C#:   Directory.GetFiles("dir")
来源：http://hz.fzhhl.top/gtlyvadzvp.html

[F09] 获取文件大小
来源：http://hz.cqqwz.cn/gtcrimmmkf.html

Py:   os.path.getsize("a.txt")
来源：http://hz.dianchejie.cn/gtnxkzjtpf.html

PHP:  filesize("a.txt");
来源：http://hz.c1oappe.top/gtgvyxwwtr.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zhixingplan.top/gtqurjdilo.html

TS:   fs.statSync("a.txt").size
来源：http://hz.cdnleiting.top/gtyayfoneg.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.ywan-chungtsiang.top/gtqlsppmsr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jqgufenzy.top/gtjalyrthj.html

Ruby: File.size("a.txt")
来源：http://hz.feifeiyinyue.top/gtqatkdjnm.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.mhx1999.top/gtcsofmrxj.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.ppjwa.cn/gtouckircr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.gzhubu.top/gtvsfyoipg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.chenjidiqi.icu/gtqmrsxzha.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yj20258888.top/gtbyegskey.html

TS:   path.extname("a.txt")
来源：http://hz.cucudq.cn/gtiohidjsi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.chenjidiqi.icu/gtwhimwczr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yj20258888.top/gtjlsuxlks.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.svipenyu.cn/gtmuuabfnz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.hnqzz.top/gtavkpecll.html

[F11] 复制与移动文件
来源：http://hz.hywenlv.cn/gtaaryhqki.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yonumen.top/gttisxqfiz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jinqigfzy.top/gtpgbeqnlk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.chenlongwang.top/gtoqagzkyu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.fzhhl.top/gtombouhzu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.hfpthk.cn/gtwrtieqga.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.ybcxt.top/gtdpatnrqh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yj20258.top/gtxfdlzqrh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.gogol.net.cn/gtwvezsxgs.html

[F12] CSV 读写
来源：http://hz.ydzc1.top/gtowyrsgzt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jlsjyb.cn/gtcihfqxex.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.havefunace.top/gtybdatwpy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yanxiufei.cn/gtyepogvwo.html

TS:   // 同上
来源：http://hz.jinqigufen.top/gtlyxlzqzm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.dashuyun.cn/gtabbvekfj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.meibo888.top/gttrzqgxgt.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.9152youxi.cn/gtuavxdtkm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.tanke756.top/gtepokuajc.html

================================================================================
来源：http://hz.jinqigufen.top/gthqzavqnn.html

G. 面向对象
来源：http://hz.cdnleiting.top/gtsmahwryu.html

================================================================================
来源：http://hz.hnqzz.top/gtoyjmojhe.html

[G01] 定义类
来源：http://hz.ywan-chungtsiang.top/gtnxywtwpk.html

Py:   class User: pass
来源：http://hz.jinqigfzy.top/gtgcepfhmo.html

PHP:  class User {}
来源：http://hz.iojbl.cn/gttooqqifq.html

JS:   class User {}
来源：http://hz.hammf.cn/gtnqtpehet.html

TS:   class User { name: string = ""; }
来源：http://hz.smart0.xyz/gtromnxnka.html

Java: class User {}
来源：http://hz.jqgufenzy.top/gtarepevhk.html

Go:   type User struct { Name string }
来源：http://hz.xylfe.cn/gtlijpquan.html

Ruby: class User; end
来源：http://hz.c1oappe.top/gtuitmbggi.html

C#:   class User {}
来源：http://hz.meibo888.top/gtmrnkmjdq.html

[G02] 构造函数
来源：http://hz.zhiwuduotai.top/gtxayfyqwy.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.hnqzz.top/gtisqpqkrq.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hnqzz.top/gtmtnclsmd.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.daxiang520.top/gtymkjuzhc.html

TS:   constructor(public name: string) {}
来源：http://hz.svipenyu.cn/gtvhevpado.html

Java: User(String name) { this.name = name; }
来源：http://hz.sysykeji.top/gtbpefvjdt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hammf.cn/gtfdnhicbz.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yj202588.top/gtgmntilso.html

C#:   public User(string name) { Name = name; }
来源：http://hz.ppjwa.cn/gtktxfshti.html

[G03] 实例属性
来源：http://hz.aibaodan.cn/gtpuulggzd.html

Py:   self.name = "x"
来源：http://hz.yvedp.cn/gtroelctqz.html

PHP:  public string $name = "x";
来源：http://hz.gaohongyu789.top/gtdablsgtp.html

JS:   this.name = "x";
来源：http://hz.ydzc1.top/gtplgrjney.html

TS:   name: string = "x";
来源：http://hz.kuanghao11.cn/gtqkhrleyr.html

Java: private String name;
来源：http://hz.cdnleiting.top/gtgkacpeub.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.nanxuanxn.top/gtrcwineun.html

Ruby: @name = "x"
来源：http://hz.ydzc1.top/gtzepeezts.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.shuidangran.top/gtcxkuzvkn.html

[G04] 定义方法
来源：http://hz.fzhhl.top/gtikbxrqlr.html

Py:   def greet(self): return self.name
来源：http://hz.hysaishi.cn/gtbhpgohiv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.shzxlz.cn/gtwdkzgalb.html

JS:   greet() { return this.name; }
来源：http://hz.guannengcc.top/gtlnztrdim.html

TS:   greet(): string { return this.name; }
来源：http://hz.svipenyu.cn/gtfftkolij.html

Java: String greet() { return name; }
来源：http://hz.haohaochexian.top/gtagwzxulu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zhixingplan.top/gtfqalxqea.html

Ruby: def greet; @name; end
来源：http://hz.wangdashe.top/gtvwimhwhu.html

C#:   public string Greet() => Name;
来源：http://hz.jqgufenzy.top/gtdidawmpv.html

[G05] 继承
来源：http://hz.aibaodan.cn/gtdrxgwxta.html

Py:   class Admin(User): pass
来源：http://hz.zhengqikj.top/gtqqwneafg.html

PHP:  class Admin extends User {}
来源：http://hz.zhixingplan.top/gtfygbheps.html

JS:   class Admin extends User {}
来源：http://hz.tian-w.cn/gtazklgiii.html

TS:   class Admin extends User {}
来源：http://hz.vqdsnc.cn/gtmcpceolg.html

Java: class Admin extends User {}
来源：http://hz.pengpengdd.cyou/gtjxnllxcu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.andypj.xyz/gtnozljalt.html

Ruby: class Admin < User; end
来源：http://hz.sysykeji.top/gtflbmmheh.html

C#:   class Admin : User {}
来源：http://hz.svipenyu.cn/gtwgtnjfjp.html

[G06] 重写方法
来源：http://hz.9152youxi.cn/gthnioqfwf.html

Py:   def greet(self): return "admin"
来源：http://hz.9152youxi.cn/gtironjrhv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.xingfuxueyuan.xyz/gtuvtzrozk.html

JS:   greet() { return "admin"; }
来源：http://hz.ywan-chungtsiang.top/gtvjasugjf.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jinyuanbaomall.cn/gtmwxqzpqk.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.9152youxi.cn/gthvzibwnf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.shangyingyoupin.top/gtxvjtonnt.html

Ruby: def greet; "admin"; end
来源：http://hz.xingfuxueyuan.xyz/gtpwauhxoq.html

C#:   public override string Greet() => "admin";
来源：http://hz.jianghu66.top/gtsldqtfwl.html

[G07] 调用父类方法
来源：http://hz.daria6918.cn/gtqdwjrxcc.html

Py:   super().greet()
来源：http://hz.xingfuxueyuan.xyz/gtzuuagwug.html

PHP:  parent::greet();
来源：http://hz.havefunace.top/gthibndftt.html

JS:   super.greet();
来源：http://hz.yj20258.top/gtfrjfryoc.html

TS:   super.greet();
来源：http://hz.yj202588.top/gtluvkkevs.html

Java: super.greet();
来源：http://hz.tian-w.cn/gtrlalvswi.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.sweek.top/gtkctapwjm.html

Ruby: super
来源：http://hz.redwolf501.top/gthgqfyvff.html

C#:   base.Greet();
来源：http://hz.sysykeji.top/gtqjbvmoec.html

[G08] 静态方法与属性
来源：http://hz.chenzaomai.com/gttlzkviqn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhaomingkeji.xyz/gtgyjzsgfp.html

PHP:  public static function f() {}
来源：http://hz.mhx1999.top/gtcjfitxof.html

JS:   static f() {}
来源：http://hz.ivvv.top/gtiottgveu.html

TS:   static f(): void {}
来源：http://hz.xuanzx.com/gtghlnftmy.html

Java: static void f() {}
来源：http://hz.jinqigfzy.top/gtdinqgreq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.gzhubu.top/gtwesazcxr.html

Ruby: def self.f; end
来源：http://hz.hnxiangtu.top/gtqobbszjt.html

C#:   public static void F() {}
来源：http://hz.jlsjyb.cn/gtizisjdbn.html

[G09] 接口 / 抽象类
来源：http://hz.yvedp.cn/gttuhxnkmu.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.haohaochexian.top/gtyacqnrdz.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.bjfxy.top/gtmmzxyija.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jinqigufen.top/gtiokfcqaj.html

TS:   interface Shape { area(): number; }
来源：http://hz.shuidangran.top/gtdocfsmax.html

Java: interface Shape { double area(); }
来源：http://hz.shzxlz.cn/gttrtcftms.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jlsjyb.cn/gtexzsifog.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yuxming.cn/gtgmydhann.html

C#:   interface IShape { double Area(); }
来源：http://hz.daxiang520.top/gtaghbflmb.html

[G10] 访问控制
来源：http://hz.zhongyouzk.top/gtsljlanzj.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hnxiangtu.top/gtdiahuzid.html

PHP:  public / protected / private
来源：http://hz.hnxiangtu.top/gtawkwulhq.html

JS:   #private 字段；其余公开
来源：http://hz.zhiwuduotai.top/gtvwcpzszd.html

TS:   public / protected / private
来源：http://hz.meibo888.top/gtdvroeivm.html

Java: public / protected / private / 默认包级
来源：http://hz.ppjwa.cn/gtnxlnkukc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yj202588.top/gtlirkxjpu.html

Ruby: public / protected / private
来源：http://hz.chenlongwang.top/gtsvayfcie.html

C#:   public / protected / private / internal
来源：http://hz.cqqwz.cn/gtxjwisvgm.html

[G11] getter / setter
来源：http://hz.guowangkeji.top/gtblidoido.html

Py:   @property 与 @x.setter
来源：http://hz.chenlongwang.top/gtvhydmtnh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.kuanghao11.cn/gttixgetij.html

JS:   get name() { return this._name; }
来源：http://hz.316326.xyz/gtxjplijgn.html

TS:   get name(): string { return this._name; }
来源：http://hz.chenzaomai.com/gteqnbuson.html

Java: public String getName() { return name; }
来源：http://hz.sxryk.cn/gtfcrqsihz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.mhx1999.top/gtvgkgtxav.html

Ruby: attr_accessor :name
来源：http://hz.bjfxy.top/gtsnlpzzls.html

C#:   public string Name { get; set; }
来源：http://hz.zhiwuduotai.top/gtwbytdwkj.html

[G12] 对象转字符串
来源：http://hz.dianchejie.cn/gtocckppou.html

Py:   def __str__(self): return self.name
来源：http://hz.52xcode.cn/gtepdvpvef.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.fzhhl.top/gtysjrqcov.html

JS:   toString() { return this.name; }
来源：http://hz.jinyuanbaomall.cn/gtxvukgist.html

TS:   toString(): string { return this.name; }
来源：http://hz.hnqzz.top/gtmiplzcim.html

Java: @Override public String toString() { return name; }
来源：http://hz.zhiwuduotai.top/gtucpwezqa.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.tanke756.top/gtzclbwfoj.html

Ruby: def to_s; @name; end
来源：http://hz.cashguo.top/gtgkbislfc.html

C#:   public override string ToString() => Name;
来源：http://hz.ivvv.top/gtntgehadl.html

[G13] 判断对象类型
来源：http://hz.wangshuangyany.cn/gtptkrkeyh.html

Py:   isinstance(u, User)
来源：http://hz.cashguo.top/gtmqvfogmg.html

PHP:  $u instanceof User
来源：http://hz.fengsongda.top/gthppbvgls.html

JS:   u instanceof User
来源：http://hz.jlsjyb.cn/gtvfxfnnuf.html

TS:   u instanceof User
来源：http://hz.c1oappe.top/gtnehlrrlx.html

Java: u instanceof User
来源：http://hz.daxiang520.top/gtnmjnmzrf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.guowangkeji.top/gtozglwwph.html

Ruby: u.is_a?(User)
来源：http://hz.haohaochexian.top/gttyqxhmgt.html

C#:   u is User
来源：http://hz.hywenlv.cn/gtcktxwyvc.html

[G14] 数据类 / record
来源：http://hz.sysykeji.top/gtdegzoxhd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.bjfxy.top/gtxhhcicux.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yvedp.cn/gtshuubxxd.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.xingfuxueyuan.xyz/gtxtxhottu.html

TS:   type User = { name: string; age: number };
来源：http://hz.sysykeji.top/gttcttczkd.html

Java: record User(String name, int age) {}
来源：http://hz.cucudq.cn/gtyxfbikff.html

Go:   type User struct { Name string; Age int }
来源：http://hz.guannengcc.top/gtiobbhxzf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.316326.xyz/gtpfmkswks.html

C#:   record User(string Name, int Age);
来源：http://hz.cashguo.top/gtdwkngeyu.html

[G15] 枚举
来源：http://hz.ydjk.org.cn/gthtitaxtn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jyoumei.cn/gtoinfblep.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yuanzhike.top/gtkwgvtpsb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yonumen.top/gtrhurvtxo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yongpay.top/gtvjwxddfm.html

Java: enum Color { RED, GREEN }
来源：http://hz.9152youxi.cn/gtczxeeurl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.bjfxy.top/gtlbtntogh.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jinyuanbaomall.cn/gtyhnpwdky.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yongpay.top/gtfrtockxh.html

[G16] 对象转数组 / 字典
来源：http://hz.fengsongda.top/gtwfajmqjz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.nanxuanxn.top/gtqpcdpgrm.html

PHP:  get_object_vars($obj);
来源：http://hz.dashuyun.cn/gthjytdtme.html

JS:   Object.entries(obj)
来源：http://hz.havefunace.top/gtrebtyaxn.html

TS:   Object.entries(obj)
来源：http://hz.ywan-chungtsiang.top/gtvdncjzln.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yj20258.top/gtsgrxjryo.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.zhoulong.xyz/gtbnzovjlc.html

Ruby: obj.instance_variables
来源：http://hz.bjfxy.top/gtzktdcrvt.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.ydjk.org.cn/gtleuqbqnp.html

================================================================================
来源：http://hz.cqqwz.cn/gtcbrkjswd.html

H. 异常与错误处理
来源：http://hz.xuanzx.com/gtvbrftkcr.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtvqhijqjk.html

[H01] try / catch 基础
来源：http://hz.redwolf501.top/gtrzryifjb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.shanyushiyangtech.top/gtvraunexw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.cashguo.top/gtqbvleftd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zycfv.cn/gtzozrslyb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.wangdashe.top/gtxteawtwo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.hongshengwenyu.top/gtlhxhhdaw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yuanzhike.top/gtlfbukymc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yanxiufei.cn/gtxymreorf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.meibo888.top/gtkrlpgaqh.html

[H02] finally / ensure 收尾
来源：http://hz.shangyingyoupin.top/gtfhbdwhaf.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.kuanghao11.cn/gthgkbcglh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.wangdashe.top/gtfcyzkzyx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yj20258.top/gtduhxkash.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ybcxt.top/gtvagdwojc.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.shuidangran.top/gtnfqydlqf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jinqigufen.top/gtzvrenkqc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.sysykeji.top/gtdetswrru.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.nanxuanxn.top/gtisbalzam.html

[H03] 主动抛出异常
来源：http://hz.xziqi.cn/gtswtaxfei.html

Py:   raise ValueError("错误信息")
来源：http://hz.zhengqikj.top/gtasunqrkc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.xingfuxueyuan.xyz/gtkmcneaes.html

JS:   throw new Error("错误信息");
来源：http://hz.ehwqpu.com/gtubtdbark.html

TS:   throw new Error("错误信息");
来源：http://hz.gaohongyu789.top/gtfpqmobpm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.birdmap.top/gtystopbbm.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.guannengcc.top/gtugonltcb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ydzc1.top/gtthzspjzq.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.chenjidiqi.icu/gtkqhgywyr.html

[H04] 自定义异常类型
来源：http://hz.ehwqpu.com/gtsgimsknm.html

Py:   class MyError(Exception): pass
来源：http://hz.yongpay.top/gtcqeyijgw.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.shzxlz.cn/gtsmaplbtp.html

JS:   class MyError extends Error {}
来源：http://hz.hnqzz.top/gtsegfamdg.html

TS:   class MyError extends Error {}
来源：http://hz.sxryk.cn/gtqowgquwy.html

Java: class MyException extends RuntimeException {}
来源：http://hz.cqqwz.cn/gthnowqnhb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.nanxinkj.top/gtovucveiy.html

Ruby: class MyError < StandardError; end
来源：http://hz.jinqigufen.top/gtecmxvqom.html

C#:   class MyException : Exception {}
来源：http://hz.jyoumei.cn/gtxvvjgtjv.html

[H05] 捕获特定类型
来源：http://hz.zhengqikj.top/gtlcbmcrfq.html

Py:   except ValueError as e:
来源：http://hz.aibaodan.cn/gtzbnoxgas.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.shangyingyoupin.top/gtrgbxntel.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.havefunace.top/gtxqirsxnn.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.vqdsnc.cn/gtmcsyerle.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.shzxlz.cn/gtrsoonanl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.redwolf501.top/gtfgzgatne.html

Ruby: rescue ArgumentError => e
来源：http://hz.zdqjudy.top/gtcplldtrk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yuanzhike.top/gtylohfhzg.html

[H06] 可选值 / 空值安全访问
来源：http://hz.52xcode.cn/gtqupvzbih.html


<!-- 参考信息 -->