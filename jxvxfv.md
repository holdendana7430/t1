代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.pycfn.com/gtqgdtkxtk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yonumen.top/gtloiasmgz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jinghuilouyu.cn/gthfblwmml.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.shuidangran.top/gtvhdifnxv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.ivvv.top/gtkydvjiqe.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.hongshengwenyu.top/gtqwmwpdgz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.shuidangran.top/gtxpadgohw.html

[F04] 追加写入文件
来源：http://hz.quarkkingdee.top/gtqbpncbbe.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.andypj.xyz/gtiramewen.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.fzhhl.top/gtizbdnqlm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shanyushiyangkeji.top/gtjgzqyrqm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.gogol.net.cn/gtuanraaje.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.ywan-chungtsiang.top/gtkpxhuqwa.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.bjfxy.top/gtjleekrtw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.hammf.cn/gtrrcoeepy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.sxryk.cn/gteewwgilo.html

[F05] 判断文件或目录是否存在
来源：http://hz.feifeiyinyue.top/gtwlvagpof.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zhixingplan.top/gtnfvbyibn.html

PHP:  file_exists("a.txt");
来源：http://hz.hysaishi.cn/gtcaqwollq.html

JS:   fs.existsSync("a.txt")
来源：http://hz.guannengcc.top/gtdmlngxjs.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yj202588.top/gtlofeqpcz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.fzhhl.top/gtisnarilc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.aizwys.cn/gtgxhgzteo.html

Ruby: File.exist?("a.txt")
来源：http://hz.guannengcc.top/gtswzdlkjn.html

C#:   File.Exists("a.txt")
来源：http://hz.kuanghao11.cn/gtnmpnatno.html

[F06] 删除文件
来源：http://hz.xziqi.cn/gtlswnwbyy.html

Py:   os.remove("a.txt")
来源：http://hz.birdmap.top/gtkryfcgaf.html

PHP:  unlink("a.txt");
来源：http://hz.daria6918.cn/gtwwbwmqju.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yongpay.top/gtyafxklnr.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.chenlongwang.top/gtrlsceqil.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.fzhhl.top/gttksuocci.html

Go:   os.Remove("a.txt")
来源：http://hz.sufxvd.cn/gtribslzpd.html

Ruby: File.delete("a.txt")
来源：http://hz.cqqwz.cn/gtuxdcfzlg.html

C#:   File.Delete("a.txt");
来源：http://hz.dashuyun.cn/gtitrfykyh.html

[F07] 创建目录（含多级）
来源：http://hz.fengsongda.top/gtvxntptbe.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.andypj.xyz/gtdcaxqvie.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.cashguo.top/gtjrhurkgn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.nanxinkj.top/gtflhttjeo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jinyuanbaomall.cn/gtcxnnfahz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yvedp.cn/gtyqanrdbg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.ivvv.top/gtchsnrxpy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.nanxinkj.top/gtkbwldgpu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zhijiandao.cn/gtbtclpdwf.html

[F08] 遍历目录
来源：http://hz.ivvv.top/gtqopceigq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.snrcjt.cn/gtyozznvuf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.bjfxy.top/gtppdarhgg.html

JS:   fs.readdirSync("dir")
来源：http://hz.cdnleiting.top/gtgwcxofso.html

TS:   fs.readdirSync("dir")
来源：http://hz.quarkkingdee.top/gtdnmxwpsg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zhaomingkeji.xyz/gtfjenydbz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.52xcode.cn/gtumsrwqha.html

Ruby: Dir.children("dir")
来源：http://hz.nwbrower.top/gtftkctqhm.html

C#:   Directory.GetFiles("dir")
来源：http://hz.dashuyun.cn/gtrimtatlw.html

[F09] 获取文件大小
来源：http://hz.gaohongyu789.top/gtjyayywbv.html

Py:   os.path.getsize("a.txt")
来源：http://hz.birdmap.top/gtellnnqww.html

PHP:  filesize("a.txt");
来源：http://hz.gaohongyu789.top/gtuzduvtzs.html

JS:   fs.statSync("a.txt").size
来源：http://hz.sxryk.cn/gtpwjrfema.html

TS:   fs.statSync("a.txt").size
来源：http://hz.nanxuanxn.top/gtgvykwlxt.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.ybcxt.top/gtuhobgenh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.9152youxi.cn/gtrqfglwrm.html

Ruby: File.size("a.txt")
来源：http://hz.hnqzz.top/gtitdawkea.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jqgfzy.top/gtnvchmeny.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.birdmap.top/gtsrjrfucb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.gaohongyu789.top/gtbvtrjgxz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.xuanzx.com/gtflvmlwbk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.ehwqpu.com/gtrgcwouup.html

TS:   path.extname("a.txt")
来源：http://hz.jianghu66.top/gtidzenywa.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.xuanzx.com/gtwgnwsoty.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.ehwqpu.com/gtwrjbbrbn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.sweek.top/gtyjqddexl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.xuanzx.com/gthgdyexku.html

[F11] 复制与移动文件
来源：http://hz.sweek.top/gtrvrrxikq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.gzhubu.top/gtollaqjci.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zycfv.cn/gtoadvseze.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yanxiufei.cn/gtcgzfcgtu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xuetiantiany.cn/gtlzqcsghu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.cashguo.top/gtugxoikrz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jqgfzy.top/gtkdvhlddb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.cdnleiting.top/gtyysoojmj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.nanxuanxn.top/gtbkgplgas.html

[F12] CSV 读写
来源：http://hz.smart0.xyz/gtyoowqvbv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xziqi.cn/gtvzclzfjz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.meibo888.top/gtnlwkylqw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.chenlongwang.top/gtwtnuvqwl.html

TS:   // 同上
来源：http://hz.cqqwz.cn/gttbldcnnf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.tanke756.top/gtvrrczcay.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.cdnleiting.top/gtbeqdlauq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.svipenyu.cn/gtoxtjnwwb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.pycfn.com/gtarykrbta.html

================================================================================
来源：http://hz.cqqwz.cn/gtpwclrtmv.html

G. 面向对象
来源：http://hz.yj20258888.top/gtfblikpji.html

================================================================================
来源：http://hz.ivvv.top/gtfyffyjvo.html

[G01] 定义类
来源：http://hz.kuanghao11.cn/gtveinodbq.html

Py:   class User: pass
来源：http://hz.shzxlz.cn/gtewphktoe.html

PHP:  class User {}
来源：http://hz.yj20258.top/gtcgqslsdf.html

JS:   class User {}
来源：http://hz.feifeiyinyue.top/gtqsirsmrv.html

TS:   class User { name: string = ""; }
来源：http://hz.cashguo.top/gtpfbweljg.html

Java: class User {}
来源：http://hz.yj20258888.top/gtcothfjwv.html

Go:   type User struct { Name string }
来源：http://hz.xylfe.cn/gthbwrgeth.html

Ruby: class User; end
来源：http://hz.ivvv.top/gtmmlqrkqu.html

C#:   class User {}
来源：http://hz.zycfv.cn/gtvlmirure.html

[G02] 构造函数
来源：http://hz.zhixingplan.top/gtzulvubdc.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhijiandao.cn/gtgccmjedf.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.aizwys.cn/gtopthjzlu.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.fzhhl.top/gtkkoimxuf.html

TS:   constructor(public name: string) {}
来源：http://hz.snrcjt.cn/gtbmzpwvfn.html

Java: User(String name) { this.name = name; }
来源：http://hz.yj20258888.top/gtptwfuamv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.mhx1999.top/gtivjhsxji.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.ppjwa.cn/gtirmjuvxm.html

C#:   public User(string name) { Name = name; }
来源：http://hz.sufxvd.cn/gtkraxmsfc.html

[G03] 实例属性
来源：http://hz.tianlin.xyz/gtwvxfvaae.html

Py:   self.name = "x"
来源：http://hz.jyoumei.cn/gtwkpqikxs.html

PHP:  public string $name = "x";
来源：http://hz.chenzaomai.com/gtwyvankbc.html

JS:   this.name = "x";
来源：http://hz.ppjwa.cn/gtrcdlotnl.html

TS:   name: string = "x";
来源：http://hz.gzhubu.top/gthlorpomu.html

Java: private String name;
来源：http://hz.yangfankeji.com/gtcrtwzxow.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.feifeiyinyue.top/gtkbsdkvtu.html

Ruby: @name = "x"
来源：http://hz.ywan-chungtsiang.top/gtafidtlem.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.daria6918.cn/gtzckntjkc.html

[G04] 定义方法
来源：http://hz.yangfankeji.com/gtqwvprymf.html

Py:   def greet(self): return self.name
来源：http://hz.cucudq.cn/gtapfggrxx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.9152youxi.cn/gtijywcnka.html

JS:   greet() { return this.name; }
来源：http://hz.jinqigfzy.top/gtizvdpnrf.html

TS:   greet(): string { return this.name; }
来源：http://hz.ydjk.org.cn/gtqoaopwqt.html

Java: String greet() { return name; }
来源：http://hz.guannengcc.top/gtqdijwfvu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.chenlongwang.top/gtyiucptkj.html

Ruby: def greet; @name; end
来源：http://hz.hammf.cn/gtivkogkmb.html

C#:   public string Greet() => Name;
来源：http://hz.feifeiyinyue.top/gtrjjahxdp.html

[G05] 继承
来源：http://hz.hysaishi.cn/gtadtivdtn.html

Py:   class Admin(User): pass
来源：http://hz.iojbl.cn/gtbbuceqgg.html

PHP:  class Admin extends User {}
来源：http://hz.ywan-chungtsiang.top/gtwycynldo.html

JS:   class Admin extends User {}
来源：http://hz.cqqwz.cn/gtycgaxabn.html

TS:   class Admin extends User {}
来源：http://hz.zhijiandao.cn/gtfrzckoxq.html

Java: class Admin extends User {}
来源：http://hz.hysaishi.cn/gtvmimokjs.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.iojbl.cn/gtipyqriut.html

Ruby: class Admin < User; end
来源：http://hz.pycfn.com/gtmuulkwhg.html

C#:   class Admin : User {}
来源：http://hz.hnxiangtu.top/gtpwhglarh.html

[G06] 重写方法
来源：http://hz.jqgfzy.top/gtapilbhsq.html

Py:   def greet(self): return "admin"
来源：http://hz.52xcode.cn/gtlvuzldqq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ppjwa.cn/gtwkeybqpw.html

JS:   greet() { return "admin"; }
来源：http://hz.jinyuanbaomall.cn/gtrrvqrqbn.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jinghuilouyu.cn/gtrzwmwqmi.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.redwolf501.top/gtoaccyhml.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jinqigufen.top/gtuwjrhpkl.html

Ruby: def greet; "admin"; end
来源：http://hz.shuidangran.top/gtcezepqsg.html

C#:   public override string Greet() => "admin";
来源：http://hz.dianchejie.cn/gtfzrhrykj.html

[G07] 调用父类方法
来源：http://hz.gzhubu.top/gtrzvuhgra.html

Py:   super().greet()
来源：http://hz.nanxuanxn.top/gtyosfykwr.html

PHP:  parent::greet();
来源：http://hz.zhixingplan.top/gtqrwqowyw.html

JS:   super.greet();
来源：http://hz.hnxiangtu.top/gtvjgnmvwb.html

TS:   super.greet();
来源：http://hz.jinqigufen.top/gtqoyhlpem.html

Java: super.greet();
来源：http://hz.shzxlz.cn/gtinlzxoed.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.chenlongwang.top/gtpocbrgnm.html

Ruby: super
来源：http://hz.xingfuxueyuan.xyz/gtdmventjv.html

C#:   base.Greet();
来源：http://hz.tian-w.cn/gtwccxajgi.html

[G08] 静态方法与属性
来源：http://hz.zhaomingkeji.xyz/gtfphlqumc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.shzxlz.cn/gtxezgpkbf.html

PHP:  public static function f() {}
来源：http://hz.chenzaomai.com/gtbztnawlc.html

JS:   static f() {}
来源：http://hz.tanke756.top/gtwkfewcmo.html

TS:   static f(): void {}
来源：http://hz.shzxlz.cn/gtjemunjmg.html

Java: static void f() {}
来源：http://hz.chenzaomai.com/gtxsqujfor.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jiagoushi.top/gtxnibmzwu.html

Ruby: def self.f; end
来源：http://hz.9152youxi.cn/gtksrdoaxu.html

C#:   public static void F() {}
来源：http://hz.jinqigufen.top/gtbrgeoglj.html

[G09] 接口 / 抽象类
来源：http://hz.hnqzz.top/gtwqraxjrn.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.pycfn.com/gtjjsjiqat.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.birdmap.top/gtviykhjcw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.kuanghao11.cn/gtktymwfwp.html

TS:   interface Shape { area(): number; }
来源：http://hz.ivvv.top/gtbauopick.html

Java: interface Shape { double area(); }
来源：http://hz.tianlin.xyz/gtzxrcfyes.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yj20258.top/gthoqacogh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.0kj1m.cn/gtqvdqfilx.html

C#:   interface IShape { double Area(); }
来源：http://hz.c1oappe.top/gtawknxktk.html

[G10] 访问控制
来源：http://hz.dianchejie.cn/gtqalunzud.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhaomingkeji.xyz/gtowfqmxlw.html

PHP:  public / protected / private
来源：http://hz.wangshuangyany.cn/gtddincjgu.html

JS:   #private 字段；其余公开
来源：http://hz.zdqjudy.top/gttxfyjudu.html

TS:   public / protected / private
来源：http://hz.ehwqpu.com/gtetuqbktl.html

Java: public / protected / private / 默认包级
来源：http://hz.yj202588.top/gtxgdynqie.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ehwqpu.com/gtteutyxnj.html

Ruby: public / protected / private
来源：http://hz.0kj1m.cn/gtokgfxsup.html

C#:   public / protected / private / internal
来源：http://hz.birdmap.top/gtqiswyzqj.html

[G11] getter / setter
来源：http://hz.hfpthk.cn/gtpbbsthyg.html

Py:   @property 与 @x.setter
来源：http://hz.yvedp.cn/gtrurznfqj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jinyuanbaomall.cn/gtmlynranc.html

JS:   get name() { return this._name; }
来源：http://hz.shuidangran.top/gtzpoyddop.html

TS:   get name(): string { return this._name; }
来源：http://hz.jinyuanbaomall.cn/gtnxridqet.html

Java: public String getName() { return name; }
来源：http://hz.sysykeji.top/gtsbbnbapc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.xylfe.cn/gtgvaigahv.html

Ruby: attr_accessor :name
来源：http://hz.yanxiufei.cn/gtmurgcrrb.html

C#:   public string Name { get; set; }
来源：http://hz.pengpengdd.cyou/gtomzmjxnu.html

[G12] 对象转字符串
来源：http://hz.yongpay.top/gtfocefpid.html

Py:   def __str__(self): return self.name
来源：http://hz.xziqi.cn/gtupdctppk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.chenlongwang.top/gtietuyxxo.html

JS:   toString() { return this.name; }
来源：http://hz.tianlin.xyz/gtinzsodgv.html

TS:   toString(): string { return this.name; }
来源：http://hz.kuanghao11.cn/gttyiyfegu.html

Java: @Override public String toString() { return name; }
来源：http://hz.bjfxy.top/gtjvzimfyt.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.hammf.cn/gtdyujtven.html

Ruby: def to_s; @name; end
来源：http://hz.smart0.xyz/gtttiqqfqd.html

C#:   public override string ToString() => Name;
来源：http://hz.feifeiyinyue.top/gtpcrunikc.html

[G13] 判断对象类型
来源：http://hz.guowangkeji.top/gtltdolbld.html

Py:   isinstance(u, User)
来源：http://hz.hfpthk.cn/gtkkerqbac.html

PHP:  $u instanceof User
来源：http://hz.xuetiantiany.cn/gtsuwajxkq.html

JS:   u instanceof User
来源：http://hz.daxiang520.top/gtbcmurmor.html

TS:   u instanceof User
来源：http://hz.hywenlv.cn/gtsdhmusau.html

Java: u instanceof User
来源：http://hz.zhiwuduotai.top/gthbxlzlai.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yuxming.cn/gtfvlimstb.html

Ruby: u.is_a?(User)
来源：http://hz.zhengqikj.top/gtmqsnokvk.html

C#:   u is User
来源：http://hz.zhoulong.xyz/gtnpfdpvwe.html

[G14] 数据类 / record
来源：http://hz.c1oappe.top/gtftbcqazi.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yj20258.top/gtbnsjmcxw.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.ivvv.top/gtkhxvywea.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.gzhubu.top/gtcxrpdjbx.html

TS:   type User = { name: string; age: number };
来源：http://hz.tian-w.cn/gteflqwkxb.html

Java: record User(String name, int age) {}
来源：http://hz.svipenyu.cn/gtvwsveirp.html

Go:   type User struct { Name string; Age int }
来源：http://hz.shanyushiyangkeji.top/gtkhmhvbjc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yj20258888.top/gtchoicweo.html

C#:   record User(string Name, int Age);
来源：http://hz.shanyushiyangtech.top/gtdfpnvsnm.html

[G15] 枚举
来源：http://hz.nwbrower.top/gtwzbtqbyy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.shanyushiyangtech.top/gtznsnxuey.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.snrcjt.cn/gttmrxdmhk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.sxryk.cn/gtcybogadg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.chenjidiqi.icu/gtixouemgw.html

Java: enum Color { RED, GREEN }
来源：http://hz.cheryme.top/gtgpxaagfp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.smart0.xyz/gtbfydijnn.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jqgufenzy.top/gtabqduykl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.andypj.xyz/gtcmjpgmuq.html

[G16] 对象转数组 / 字典
来源：http://hz.wangdashe.top/gtipknbuca.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.sxryk.cn/gtphgdflrx.html

PHP:  get_object_vars($obj);
来源：http://hz.hywenlv.cn/gtegoxabvp.html

JS:   Object.entries(obj)
来源：http://hz.0kj1m.cn/gtcpplwnpg.html

TS:   Object.entries(obj)
来源：http://hz.yj202588.top/gtspshdset.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.fzhhl.top/gtknkkmeou.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.shanyushiyangtech.top/gtwwpmcatn.html

Ruby: obj.instance_variables
来源：http://hz.tanke756.top/gtwywxhdzb.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.aibaodan.cn/gtwukdoliu.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtzjqadsck.html

H. 异常与错误处理
来源：http://hz.hywenlv.cn/gtbazhdxpp.html

================================================================================
来源：http://hz.hysaishi.cn/gtgliitfie.html

[H01] try / catch 基础
来源：http://hz.zhoulong.xyz/gtikznvyew.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.mhx1999.top/gteoluhldv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.cdnleiting.top/gteftyjveg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.tianlin.xyz/gtpdmnfemm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yuanzhike.top/gtvvyhvkyh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.dianchejie.cn/gtjqjmqudg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.fzhhl.top/gtegrvdsbg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.mhx1999.top/gtgffmjcdp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.gogol.net.cn/gtlcvpnfbt.html

[H02] finally / ensure 收尾
来源：http://hz.jqgfzy.top/gtcsbfunoc.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.pengpengdd.cyou/gtrsygdyqg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.tian-w.cn/gtqvpgcpmi.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.tanke756.top/gtfetzxfux.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.aizwys.cn/gtlybkvknq.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.c1oappe.top/gtifiacyhv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.chenlongwang.top/gtmnzslrog.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.chenzaomai.com/gtsaemknlh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.tanke756.top/gtewaiiaqc.html

[H03] 主动抛出异常
来源：http://hz.zhiwuduotai.top/gtpyeqvysu.html

Py:   raise ValueError("错误信息")
来源：http://hz.yongpay.top/gtfaylnnwf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yj20258.top/gtkuudjsty.html

JS:   throw new Error("错误信息");
来源：http://hz.hfpthk.cn/gttqwpbhrm.html

TS:   throw new Error("错误信息");
来源：http://hz.xinyue.icu/gtyypqjrbl.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zycfv.cn/gturnawfyf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.guowangkeji.top/gtetubqsds.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zhijiandao.cn/gtsyzgojun.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.wangshuangyany.cn/gtgorzvacb.html

[H04] 自定义异常类型
来源：http://hz.gotoacloud.top/gtiqaufwht.html

Py:   class MyError(Exception): pass
来源：http://hz.daria6918.cn/gtppaamcfl.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.chenlongwang.top/gtstrxrdvg.html

JS:   class MyError extends Error {}
来源：http://hz.wangdashe.top/gtzffgxftu.html

TS:   class MyError extends Error {}
来源：http://hz.jinqigfzy.top/gtvgqicyxk.html

Java: class MyException extends RuntimeException {}
来源：http://hz.xylfe.cn/gtontqiytv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zhengqikj.top/gtpenoqvwt.html

Ruby: class MyError < StandardError; end
来源：http://hz.xinyue.icu/gtfdydnbjt.html

C#:   class MyException : Exception {}
来源：http://hz.yj202588.top/gtupvzqunc.html

[H05] 捕获特定类型
来源：http://hz.chenlongwang.top/gtufkdhvsh.html

Py:   except ValueError as e:
来源：http://hz.chenzaomai.com/gtczjdwcpc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.ybcxt.top/gticyqbuhk.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.9152youxi.cn/gtudaclozc.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.ydzc1.top/gtsapzbocw.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.dashuyun.cn/gtlmxopptr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yanxiufei.cn/gtcerwiiee.html

Ruby: rescue ArgumentError => e
来源：http://hz.zycfv.cn/gtichofhix.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hnxiangtu.top/gtxhrhwtjp.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zhiwuduotai.top/gtjvylxnpe.html

Py:   value = d.get("k") or default
来源：http://hz.hammf.cn/gtvlqsrxye.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.nanxinkj.top/gtnhtbcspk.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.shuidangran.top/gtsrmnpkgt.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.hywenlv.cn/gtqxrxukkx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.tianlin.xyz/gtiewduzok.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.cucudq.cn/gtynwxachk.html

Ruby: d&.dig(:a, :b)
来源：http://hz.tianlin.xyz/gtrtthnvof.html

C#:   obj?.A?.B ?? default
来源：http://hz.hfpthk.cn/gtuglrvvkl.html

[H07] 断言
来源：http://hz.yuanzhike.top/gtbfgnloto.html

Py:   assert x > 0, "必须为正"
来源：http://hz.shanyushiyangtech.top/gtkiiklgac.html

PHP:  assert($x > 0);
来源：http://hz.jqgfzy.top/gtfmtlqgcz.html

JS:   console.assert(x > 0);
来源：http://hz.zhengqikj.top/gtcbfebdcd.html

TS:   console.assert(x > 0);
来源：http://hz.0kj1m.cn/gtuyzfwxzp.html

Java: assert x > 0 : "必须为正";
来源：http://hz.hnqzz.top/gtxgntlysr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.hfpthk.cn/gtiknnwifz.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.aizwys.cn/gtutinlhek.html


<!-- 参考信息 -->