代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.shangyingyoupin.top/gtgjeeijci.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.tianlin.xyz/gtkskqelah.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yj202588.top/gtrwwjbvgy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cqqwz.cn/gtqluxbtzu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.gotoacloud.top/gttrdpbyvz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.hongshengwenyu.top/gthbyvmiou.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yongpay.top/gttjomvdvz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.xuetiantiany.cn/gtfsbstiyl.html

[F05] 判断文件或目录是否存在
来源：http://hz.tanke756.top/gtmvyvivwt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.cucudq.cn/gtrxsabnyf.html

PHP:  file_exists("a.txt");
来源：http://hz.cucudq.cn/gtbwbglini.html

JS:   fs.existsSync("a.txt")
来源：http://hz.nanxinkj.top/gtenvtotax.html

TS:   fs.existsSync("a.txt")
来源：http://hz.9152youxi.cn/gtqgfspegs.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.zhoulong.xyz/gtwoapuqyt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yanxiufei.cn/gtahprtyit.html

Ruby: File.exist?("a.txt")
来源：http://hz.yj20258888.top/gtetfxletc.html

C#:   File.Exists("a.txt")
来源：http://hz.jinqigfzy.top/gtpbsqhlzt.html

[F06] 删除文件
来源：http://hz.chenjidiqi.icu/gtslpiofxe.html

Py:   os.remove("a.txt")
来源：http://hz.hnxiangtu.top/gtqvxwsbif.html

PHP:  unlink("a.txt");
来源：http://hz.andypj.xyz/gtdxydpewh.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.cashguo.top/gthkwrzqnj.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yanxiufei.cn/gtrevjpfxb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.sweek.top/gtukywahss.html

Go:   os.Remove("a.txt")
来源：http://hz.yangfankeji.com/gtbbqvbiqd.html

Ruby: File.delete("a.txt")
来源：http://hz.birdmap.top/gtecdblilf.html

C#:   File.Delete("a.txt");
来源：http://hz.c1oappe.top/gttzmdqjpu.html

[F07] 创建目录（含多级）
来源：http://hz.52xcode.cn/gtbsvednmt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.xuetiantiany.cn/gtpevghucb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zhiwuduotai.top/gtynvbgoxm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.9152youxi.cn/gtydceqipi.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jqgufenzy.top/gtsimanfie.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.zhijiandao.cn/gtwaryvhwn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hnxiangtu.top/gtdrawlhzv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.iojbl.cn/gtrbbfjnls.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.xziqi.cn/gtllnhsfsn.html

[F08] 遍历目录
来源：http://hz.shzxlz.cn/gtsusefzyd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.xuetiantiany.cn/gtncexdrgs.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.chenzaomai.com/gtxyvunkda.html

JS:   fs.readdirSync("dir")
来源：http://hz.havefunace.top/gthnioqdyo.html

TS:   fs.readdirSync("dir")
来源：http://hz.cdnleiting.top/gtcmbxhbyd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.ywan-chungtsiang.top/gtqptngexd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.sweek.top/gtxmwsioan.html

Ruby: Dir.children("dir")
来源：http://hz.gotoacloud.top/gtuxfilyho.html

C#:   Directory.GetFiles("dir")
来源：http://hz.tian-w.cn/gtmlibmzxm.html

[F09] 获取文件大小
来源：http://hz.hnqzz.top/gtiycoeyvv.html

Py:   os.path.getsize("a.txt")
来源：http://hz.cdnleiting.top/gthzvfjzsc.html

PHP:  filesize("a.txt");
来源：http://hz.xuetiantiany.cn/gtjhrmumos.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yueranfly.top/gtjmlwpaav.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jianghu66.top/gtpvvuaqqo.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.sysykeji.top/gtjfsmngrn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.gogol.net.cn/gttyxxlksr.html

Ruby: File.size("a.txt")
来源：http://hz.hnxiangtu.top/gtzvyxrmvm.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.xingfuxueyuan.xyz/gtvljtlkoi.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hongshengwenyu.top/gtbqldsawd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yonumen.top/gtduxmdijp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.nanxinkj.top/gtnydpytuf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jianghu66.top/gtuulrkgsc.html

TS:   path.extname("a.txt")
来源：http://hz.shanyushiyangtech.top/gtutvxqhyf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.hnqzz.top/gtfwdclwbc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.pycfn.com/gtsaopzipd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.pycfn.com/gtzidbaxqu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.xuanzx.com/gtxjbaydgl.html

[F11] 复制与移动文件
来源：http://hz.316326.xyz/gtfqejiimc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zhongyouzk.top/gtucdhzrub.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yongpay.top/gtyxppgxxw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.nanxinkj.top/gtembudsau.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sweek.top/gtfngxdbkw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jiagoushi.top/gtjufdklln.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.gzhubu.top/gtcnxrmcwf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.shuidangran.top/gtjnaniuti.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.xuanzx.com/gtiuzmbuat.html

[F12] CSV 读写
来源：http://hz.yj202588.top/gtydiwmbat.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.ydjk.org.cn/gtauutdawt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.vqdsnc.cn/gtmbjspjoc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.ppjwa.cn/gtfcnzgctf.html

TS:   // 同上
来源：http://hz.snrcjt.cn/gtexgumgny.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ehwqpu.com/gtmdpdvjzm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhijiandao.cn/gtrmnqglcs.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.guannengcc.top/gtvvbpitub.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.nanxinkj.top/gtsvpwdxym.html

================================================================================
来源：http://hz.haohaochexian.top/gtvqyuzmzt.html

G. 面向对象
来源：http://hz.shanyushiyangkeji.top/gtgjkoiucu.html

================================================================================
来源：http://hz.xuanzx.com/gtfntybgdu.html

[G01] 定义类
来源：http://hz.chenlongwang.top/gtshyrqbtw.html

Py:   class User: pass
来源：http://hz.nwbrower.top/gthusyueys.html

PHP:  class User {}
来源：http://hz.yanxiufei.cn/gthlpxgkyt.html

JS:   class User {}
来源：http://hz.sufxvd.cn/gthqzxegrj.html

TS:   class User { name: string = ""; }
来源：http://hz.sufxvd.cn/gtchgesrac.html

Java: class User {}
来源：http://hz.cucudq.cn/gtjharchsx.html

Go:   type User struct { Name string }
来源：http://hz.jinyuanbaomall.cn/gtzrufixpb.html

Ruby: class User; end
来源：http://hz.316326.xyz/gtjwwkgvjn.html

C#:   class User {}
来源：http://hz.jianghu66.top/gtaswwambu.html

[G02] 构造函数
来源：http://hz.feifeiyinyue.top/gtylmfydyz.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.xuetiantiany.cn/gtdggtgwzm.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.nanxuanxn.top/gtgvyipsgb.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.0kj1m.cn/gtftlkvmrt.html

TS:   constructor(public name: string) {}
来源：http://hz.zhengqikj.top/gtsgrdyojw.html

Java: User(String name) { this.name = name; }
来源：http://hz.tian-w.cn/gtpvmejqum.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zycfv.cn/gtqvawjmzd.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.hywenlv.cn/gtxknjymxi.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jqgfzy.top/gtvqzfjbyb.html

[G03] 实例属性
来源：http://hz.hnxiangtu.top/gtvscmflgm.html

Py:   self.name = "x"
来源：http://hz.haohaochexian.top/gtocxgziqm.html

PHP:  public string $name = "x";
来源：http://hz.yj20258.top/gtdopbcszm.html

JS:   this.name = "x";
来源：http://hz.fengsongda.top/gtqyseaumw.html

TS:   name: string = "x";
来源：http://hz.yanxiufei.cn/gtymfvkbcq.html

Java: private String name;
来源：http://hz.jinghuilouyu.cn/gtmcferqya.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.bjfxy.top/gtxjoauueb.html

Ruby: @name = "x"
来源：http://hz.jinqigfzy.top/gtclhdsyzg.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.tanke756.top/gtczzaqgwz.html

[G04] 定义方法
来源：http://hz.sysykeji.top/gtcvivhofv.html

Py:   def greet(self): return self.name
来源：http://hz.jinghuilouyu.cn/gtqhioueqb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jlsjyb.cn/gtjapxazsj.html

JS:   greet() { return this.name; }
来源：http://hz.zhaomingkeji.xyz/gtouoxmklm.html

TS:   greet(): string { return this.name; }
来源：http://hz.redwolf501.top/gtomdyhhfl.html

Java: String greet() { return name; }
来源：http://hz.shuidangran.top/gtbscqmyba.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jyoumei.cn/gtsioytbxh.html

Ruby: def greet; @name; end
来源：http://hz.haohaochexian.top/gthohurxgw.html

C#:   public string Greet() => Name;
来源：http://hz.jinyuanbaomall.cn/gtcdnithzl.html

[G05] 继承
来源：http://hz.jinqigfzy.top/gthrjrecpw.html

Py:   class Admin(User): pass
来源：http://hz.jqgfzy.top/gtwcynggdd.html

PHP:  class Admin extends User {}
来源：http://hz.jiagoushi.top/gtyxurfxmo.html

JS:   class Admin extends User {}
来源：http://hz.shzxlz.cn/gtgydwwizf.html

TS:   class Admin extends User {}
来源：http://hz.ydjk.org.cn/gtfdiqeqwy.html

Java: class Admin extends User {}
来源：http://hz.tianlin.xyz/gtggnnmuje.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.vqdsnc.cn/gtsrptsncx.html

Ruby: class Admin < User; end
来源：http://hz.cheryme.top/gtcrfzhlea.html

C#:   class Admin : User {}
来源：http://hz.zhiwuduotai.top/gtyibcxopy.html

[G06] 重写方法
来源：http://hz.xylfe.cn/gtphuwzmny.html

Py:   def greet(self): return "admin"
来源：http://hz.chenzaomai.com/gtrcxygqto.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jyoumei.cn/gtwqxheese.html

JS:   greet() { return "admin"; }
来源：http://hz.c1oappe.top/gthzlrgxxj.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zhongyouzk.top/gtpeuiwgvq.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hammf.cn/gtbntdbpuc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.nanxuanxn.top/gtckuzbymy.html

Ruby: def greet; "admin"; end
来源：http://hz.52xcode.cn/gtwukylgmg.html

C#:   public override string Greet() => "admin";
来源：http://hz.bjfxy.top/gtmgeqmsyl.html

[G07] 调用父类方法
来源：http://hz.cdnleiting.top/gtnbdzcswz.html

Py:   super().greet()
来源：http://hz.xylfe.cn/gtrmnuqevz.html

PHP:  parent::greet();
来源：http://hz.yj20258888.top/gtllkdyqsf.html

JS:   super.greet();
来源：http://hz.jqgfzy.top/gtlkfubloq.html

TS:   super.greet();
来源：http://hz.ehwqpu.com/gtedcndomj.html

Java: super.greet();
来源：http://hz.hnqzz.top/gtcgnocwny.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yvedp.cn/gtjxblvckb.html

Ruby: super
来源：http://hz.birdmap.top/gtdaajpvei.html

C#:   base.Greet();
来源：http://hz.jiagoushi.top/gtzcximtic.html

[G08] 静态方法与属性
来源：http://hz.meibo888.top/gtlctckkap.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.ydjk.org.cn/gtcloeqzek.html

PHP:  public static function f() {}
来源：http://hz.havefunace.top/gtibqayfyx.html

JS:   static f() {}
来源：http://hz.xziqi.cn/gtfcqnndaq.html

TS:   static f(): void {}
来源：http://hz.hywenlv.cn/gtrcxbslfz.html

Java: static void f() {}
来源：http://hz.xuanzx.com/gtdnqidvkj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.sysykeji.top/gtiunolrki.html

Ruby: def self.f; end
来源：http://hz.gotoacloud.top/gtoikgaeas.html

C#:   public static void F() {}
来源：http://hz.daxiang520.top/gtcskuianr.html

[G09] 接口 / 抽象类
来源：http://hz.vqdsnc.cn/gtylkmyabw.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.ydzc1.top/gtlnjiqoyj.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.daxiang520.top/gtszktiqzz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ehwqpu.com/gtewdsvxal.html

TS:   interface Shape { area(): number; }
来源：http://hz.aibaodan.cn/gtxqpvagsq.html

Java: interface Shape { double area(); }
来源：http://hz.shuidangran.top/gthzooojoo.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.ydjk.org.cn/gtlkzlczac.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hfpthk.cn/gtwjquolsm.html

C#:   interface IShape { double Area(); }
来源：http://hz.yj20258888.top/gtfxsngpeb.html

[G10] 访问控制
来源：http://hz.ywan-chungtsiang.top/gtonegpomd.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.chenlongwang.top/gtxsnemcoe.html

PHP:  public / protected / private
来源：http://hz.dashuyun.cn/gtwouokgqk.html

JS:   #private 字段；其余公开
来源：http://hz.daxiang520.top/gtjfedtzpp.html

TS:   public / protected / private
来源：http://hz.yuanzhike.top/gtohuexobi.html

Java: public / protected / private / 默认包级
来源：http://hz.zycfv.cn/gtvdqkukdr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhijiandao.cn/gtgmkskrli.html

Ruby: public / protected / private
来源：http://hz.hfpthk.cn/gtidbwucwf.html

C#:   public / protected / private / internal
来源：http://hz.sxryk.cn/gtajsbpbdb.html

[G11] getter / setter
来源：http://hz.52xcode.cn/gteivelfyl.html

Py:   @property 与 @x.setter
来源：http://hz.zdqjudy.top/gtiqlystcq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.ppjwa.cn/gtwinttdzr.html

JS:   get name() { return this._name; }
来源：http://hz.yuanzhike.top/gtidtjvgnq.html

TS:   get name(): string { return this._name; }
来源：http://hz.dianchejie.cn/gttpuoqvuf.html

Java: public String getName() { return name; }
来源：http://hz.zhoulong.xyz/gtwjokjdjz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.tian-w.cn/gtshmwoxfx.html

Ruby: attr_accessor :name
来源：http://hz.daxiang520.top/gtiuqabkfo.html

C#:   public string Name { get; set; }
来源：http://hz.hongshengwenyu.top/gtrvcnfqbm.html

[G12] 对象转字符串
来源：http://hz.dashuyun.cn/gtteiwmvan.html

Py:   def __str__(self): return self.name
来源：http://hz.guowangkeji.top/gtnaqtuvlb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.feifeiyinyue.top/gtnnmuhoth.html

JS:   toString() { return this.name; }
来源：http://hz.daria6918.cn/gtyaerfovp.html

TS:   toString(): string { return this.name; }
来源：http://hz.316326.xyz/gtcyxodfhk.html

Java: @Override public String toString() { return name; }
来源：http://hz.zhiwuduotai.top/gtomjpgnzk.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yvedp.cn/gtpzzeyeyt.html

Ruby: def to_s; @name; end
来源：http://hz.birdmap.top/gtibojdssw.html

C#:   public override string ToString() => Name;
来源：http://hz.zhongyouzk.top/gtscsqhwnf.html

[G13] 判断对象类型
来源：http://hz.daxiang520.top/gtbxkxvanm.html

Py:   isinstance(u, User)
来源：http://hz.quarkkingdee.top/gtxfmvlufj.html

PHP:  $u instanceof User
来源：http://hz.zhijiandao.cn/gtomrjeuuh.html

JS:   u instanceof User
来源：http://hz.zhoulong.xyz/gtyvtiteri.html

TS:   u instanceof User
来源：http://hz.jinqigfzy.top/gtogvcfylw.html

Java: u instanceof User
来源：http://hz.mhx1999.top/gtcoqqckba.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.sysykeji.top/gtosabwrmj.html

Ruby: u.is_a?(User)
来源：http://hz.tanke756.top/gtngptstpc.html

C#:   u is User
来源：http://hz.xziqi.cn/gthnmjnanl.html

[G14] 数据类 / record
来源：http://hz.cheryme.top/gtvwpnxqgz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.cdnleiting.top/gttxfsinup.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jyoumei.cn/gtweuihhgs.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.hysaishi.cn/gtklwqmmyi.html

TS:   type User = { name: string; age: number };
来源：http://hz.ywan-chungtsiang.top/gtjflazmrj.html

Java: record User(String name, int age) {}
来源：http://hz.yongpay.top/gtbbtniemg.html

Go:   type User struct { Name string; Age int }
来源：http://hz.ywan-chungtsiang.top/gtyenfpgiw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.birdmap.top/gtxajiqptl.html

C#:   record User(string Name, int Age);
来源：http://hz.hnqzz.top/gtljjndddh.html

[G15] 枚举
来源：http://hz.yonumen.top/gtdnnmuwpw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.xinyue.icu/gtwnfpbabq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.shangyingyoupin.top/gtcgfybhte.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.nwbrower.top/gtfbmljyua.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jiagoushi.top/gtjznadbsi.html

Java: enum Color { RED, GREEN }
来源：http://hz.sweek.top/gtsvifaubm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ivvv.top/gtvnayblao.html

Ruby: Color = %i[red green].freeze
来源：http://hz.shzxlz.cn/gtakrywzzq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.kuanghao11.cn/gtundmvhby.html

[G16] 对象转数组 / 字典
来源：http://hz.jinghuilouyu.cn/gtkdevrxty.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.hnqzz.top/gtosntfovj.html

PHP:  get_object_vars($obj);
来源：http://hz.ybcxt.top/gtdtohtwgi.html

JS:   Object.entries(obj)
来源：http://hz.gzhubu.top/gtllrkycyg.html

TS:   Object.entries(obj)
来源：http://hz.guannengcc.top/gtmqibstlb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yangfankeji.com/gtzqzkkryb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.feifeiyinyue.top/gtckbrvmcf.html

Ruby: obj.instance_variables
来源：http://hz.bjfxy.top/gtjqzukrdb.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.smart0.xyz/gtsniysgsg.html

================================================================================
来源：http://hz.hfpthk.cn/gtsofkmpme.html

H. 异常与错误处理
来源：http://hz.gotoacloud.top/gtdqnoxmyv.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gthzuhcruf.html

[H01] try / catch 基础
来源：http://hz.jinqigufen.top/gtpneebxsr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.sysykeji.top/gtcubvbhhx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.cdnleiting.top/gtvjogyomn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.chenlongwang.top/gtpyhqimzw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.sysykeji.top/gtqjqpzqlb.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jinyuanbaomall.cn/gtqiadjdlq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jyoumei.cn/gtpvhujnzh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ywan-chungtsiang.top/gteteesspn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.ywan-chungtsiang.top/gtoptcwaty.html

[H02] finally / ensure 收尾
来源：http://hz.cashguo.top/gtyqsgbtar.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.xuetiantiany.cn/gtpnkzjhta.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zdqjudy.top/gthslbyitx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.svipenyu.cn/gtsfblxkqt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.daxiang520.top/gtpgtwtnwx.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.daria6918.cn/gtgtkjgbyp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.xingfuxueyuan.xyz/gtrocjilio.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.zhengqikj.top/gtnwornrij.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jqgfzy.top/gtmzfajsos.html

[H03] 主动抛出异常
来源：http://hz.daria6918.cn/gtzslzrcia.html

Py:   raise ValueError("错误信息")
来源：http://hz.dashuyun.cn/gtvqqaglto.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yj20258.top/gthxqpjwty.html

JS:   throw new Error("错误信息");
来源：http://hz.jiagoushi.top/gtuhvsmdeq.html

TS:   throw new Error("错误信息");
来源：http://hz.hywenlv.cn/gtsyohrjbk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.9152youxi.cn/gtvvfyjrfe.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.andypj.xyz/gtmbsukbvm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yj20258888.top/gtfndkhsjp.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yangfankeji.com/gtlgzbshuw.html

[H04] 自定义异常类型
来源：http://hz.jinyuanbaomall.cn/gtzeiiwdkp.html

Py:   class MyError(Exception): pass
来源：http://hz.tianlin.xyz/gtvghhpdpc.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zhijiandao.cn/gtvdhwwedv.html

JS:   class MyError extends Error {}
来源：http://hz.316326.xyz/gtwbvpvtnq.html

TS:   class MyError extends Error {}
来源：http://hz.nanxuanxn.top/gtdppbznqq.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jiagoushi.top/gtjoszbkzl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.chenzaomai.com/gtcudpitoh.html

Ruby: class MyError < StandardError; end
来源：http://hz.gaohongyu789.top/gtlkopqxsr.html

C#:   class MyException : Exception {}
来源：http://hz.chenzaomai.com/gtlepxyhvp.html

[H05] 捕获特定类型
来源：http://hz.snrcjt.cn/gtgmmztfbx.html

Py:   except ValueError as e:
来源：http://hz.gogol.net.cn/gtoqlaurna.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.ywan-chungtsiang.top/gtcbrmqbvr.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.wangshuangyany.cn/gtqxxbbuoe.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.0kj1m.cn/gtyniphvjn.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhixingplan.top/gtuwbzsskk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hnxiangtu.top/gtkbjbxvuc.html

Ruby: rescue ArgumentError => e
来源：http://hz.jyoumei.cn/gtyzssghvp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.aibaodan.cn/gtzhjyswjt.html

[H06] 可选值 / 空值安全访问
来源：http://hz.dianchejie.cn/gtddyuodlz.html

Py:   value = d.get("k") or default
来源：http://hz.wangdashe.top/gtqriqnbnb.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.ywan-chungtsiang.top/gtvpmihlyd.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.redwolf501.top/gtfviezjnc.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.xziqi.cn/gtvhdrdlmd.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yj202588.top/gtawusjpzf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.dianchejie.cn/gtmmumrwzp.html

Ruby: d&.dig(:a, :b)
来源：http://hz.meibo888.top/gthzzweeyp.html

C#:   obj?.A?.B ?? default
来源：http://hz.shanyushiyangkeji.top/gtgcqiayug.html

[H07] 断言
来源：http://hz.wangdashe.top/gtlwqebcnx.html

Py:   assert x > 0, "必须为正"
来源：http://hz.gogol.net.cn/gtdmvryirk.html

PHP:  assert($x > 0);
来源：http://hz.tanke756.top/gtcravkwsl.html

JS:   console.assert(x > 0);
来源：http://hz.316326.xyz/gtafhhumaj.html

TS:   console.assert(x > 0);
来源：http://hz.aibaodan.cn/gtbjbqraks.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jqgfzy.top/gthktbkjma.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yj202588.top/gtzkikntlf.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.chenjidiqi.icu/gtaqlxkpib.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zdqjudy.top/gtuhztjgqb.html

[H08] 获取错误信息与堆栈
来源：http://hz.yueranfly.top/gtdbbsfuvu.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.52xcode.cn/gtkqnpfflk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.feifeiyinyue.top/gtwzpduipk.html

JS:   e.message;  e.stack
来源：http://hz.tianlin.xyz/gtgkeompot.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.nanxuanxn.top/gtmpukojsq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.chenjidiqi.icu/gtckflfucv.html

Go:   err.Error()
来源：http://hz.sweek.top/gtcsxudsnn.html


<!-- 参考信息 -->