代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.hnxiangtu.top/gtjxqsfewr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jinghuilouyu.cn/gtqkrkfbax.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.snrcjt.cn/gtjvhynjtt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yj202588.top/gtnzcdsdta.html

[F05] 判断文件或目录是否存在
来源：http://hz.ywan-chungtsiang.top/gtulqxlrfa.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.shzxlz.cn/gtjjcikbwg.html

PHP:  file_exists("a.txt");
来源：http://hz.gaohongyu789.top/gtfylevmdc.html

JS:   fs.existsSync("a.txt")
来源：http://hz.sufxvd.cn/gtcbppmerd.html

TS:   fs.existsSync("a.txt")
来源：http://hz.wangshuangyany.cn/gtlqvbmvwy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.zhijiandao.cn/gtrdjtpveq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.quarkkingdee.top/gttllspffj.html

Ruby: File.exist?("a.txt")
来源：http://hz.feifeiyinyue.top/gtzfcrienq.html

C#:   File.Exists("a.txt")
来源：http://hz.zhengqikj.top/gtoeeiigrc.html

[F06] 删除文件
来源：http://hz.hfpthk.cn/gtiocxxbkp.html

Py:   os.remove("a.txt")
来源：http://hz.fzhhl.top/gtixoiagoo.html

PHP:  unlink("a.txt");
来源：http://hz.vqdsnc.cn/gtiorlmjxr.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hnqzz.top/gtnborrwcb.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yvedp.cn/gthoeemtii.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yangfankeji.com/gtijwdzhff.html

Go:   os.Remove("a.txt")
来源：http://hz.yj20258.top/gtnctdzgta.html

Ruby: File.delete("a.txt")
来源：http://hz.bjfxy.top/gthnrfaoey.html

C#:   File.Delete("a.txt");
来源：http://hz.shangyingyoupin.top/gtibsmxhec.html

[F07] 创建目录（含多级）
来源：http://hz.nwbrower.top/gtkokvjrwm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.52xcode.cn/gtshptjzxm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zhiwuduotai.top/gtuwnxitiw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.vqdsnc.cn/gtixviumbc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.gzhubu.top/gtxjfmynfo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jqgfzy.top/gttxurtiue.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hnqzz.top/gtbirkwzbk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jqgfzy.top/gthyrbufzz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.fengsongda.top/gtykvuujfu.html

[F08] 遍历目录
来源：http://hz.xziqi.cn/gtusglguwm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.birdmap.top/gtfhxinxhu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.snrcjt.cn/gtzlflxwbj.html

JS:   fs.readdirSync("dir")
来源：http://hz.fzhhl.top/gtsyqnqzws.html

TS:   fs.readdirSync("dir")
来源：http://hz.zhiwuduotai.top/gttjleozeo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.smart0.xyz/gtnofgvzec.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yvedp.cn/gtfkxqolur.html

Ruby: Dir.children("dir")
来源：http://hz.zhixingplan.top/gtzpmslujm.html

C#:   Directory.GetFiles("dir")
来源：http://hz.cdnleiting.top/gtqbozxalr.html

[F09] 获取文件大小
来源：http://hz.gaohongyu789.top/gtysbdvpff.html

Py:   os.path.getsize("a.txt")
来源：http://hz.shzxlz.cn/gtvpdbnrdb.html

PHP:  filesize("a.txt");
来源：http://hz.c1oappe.top/gtdwybbmlh.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jinyuanbaomall.cn/gtfunjpotk.html

TS:   fs.statSync("a.txt").size
来源：http://hz.shangyingyoupin.top/gtgxmtoabw.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.shanyushiyangkeji.top/gtymxaugqj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.0kj1m.cn/gtukvanlcy.html

Ruby: File.size("a.txt")
来源：http://hz.yj20258888.top/gtsveapvdm.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.sxryk.cn/gtypkbpvui.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.shuidangran.top/gtbcncmrdb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.xylfe.cn/gtwwmznshb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.meibo888.top/gtrguipahg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.nwbrower.top/gtufrbcyqu.html

TS:   path.extname("a.txt")
来源：http://hz.jiagoushi.top/gtxyjdszdv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.gaohongyu789.top/gtcsnlogwg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zhongyouzk.top/gtfhnixuvq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.cheryme.top/gtuqtkbhvm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.0kj1m.cn/gtncexcrso.html

[F11] 复制与移动文件
来源：http://hz.zhixingplan.top/gtigcshhgl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.ivvv.top/gttqewoetx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.chenlongwang.top/gtyhefguzi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.guowangkeji.top/gtobpfejjy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.tanke756.top/gtvaidwtle.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.pycfn.com/gtakkpkoob.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jqgfzy.top/gtvhuwpcfc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.52xcode.cn/gtuqkrchzs.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.xuanzx.com/gtnzduxnwg.html

[F12] CSV 读写
来源：http://hz.cqqwz.cn/gttqduauul.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.sxryk.cn/gtjwvsvzbf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jlsjyb.cn/gttbxxtgxg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yvedp.cn/gtrgwtjrxz.html

TS:   // 同上
来源：http://hz.yueranfly.top/gtzapaplmy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ybcxt.top/gtxksioqlr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.shuidangran.top/gtzbnzkauy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.xziqi.cn/gtaoydoorp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zhixingplan.top/gtletswnpk.html

================================================================================
来源：http://hz.9152youxi.cn/gtqitnlqml.html

G. 面向对象
来源：http://hz.jinghuilouyu.cn/gtahkgdrra.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtvlvuzlgt.html

[G01] 定义类
来源：http://hz.shanyushiyangtech.top/gtvorrptop.html

Py:   class User: pass
来源：http://hz.jinqigfzy.top/gtqpruvsym.html

PHP:  class User {}
来源：http://hz.9152youxi.cn/gtncraqmpi.html

JS:   class User {}
来源：http://hz.zhengqikj.top/gtupnyhcza.html

TS:   class User { name: string = ""; }
来源：http://hz.nanxuanxn.top/gttggnvlou.html

Java: class User {}
来源：http://hz.zhongyouzk.top/gthkwkbzvw.html

Go:   type User struct { Name string }
来源：http://hz.ywan-chungtsiang.top/gtujhtcyxz.html

Ruby: class User; end
来源：http://hz.yangfankeji.com/gtltgqxedq.html

C#:   class User {}
来源：http://hz.nanxinkj.top/gtfdvtkchp.html

[G02] 构造函数
来源：http://hz.mhx1999.top/gtsvpgrqvk.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.shzxlz.cn/gtoaifxowk.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.bjfxy.top/gteayspuvj.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yj20258888.top/gtygxjsmej.html

TS:   constructor(public name: string) {}
来源：http://hz.ppjwa.cn/gtrzyfepec.html

Java: User(String name) { this.name = name; }
来源：http://hz.hfpthk.cn/gtygxaudcb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.cdnleiting.top/gtdcgvxaxj.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.zdqjudy.top/gtbauhqkzl.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jinqigufen.top/gtkvlmuqpe.html

[G03] 实例属性
来源：http://hz.zhengqikj.top/gtssuhxfgq.html

Py:   self.name = "x"
来源：http://hz.zhengqikj.top/gtbynoccvw.html

PHP:  public string $name = "x";
来源：http://hz.ydzc1.top/gtcfoxlwjs.html

JS:   this.name = "x";
来源：http://hz.nwbrower.top/gtwfzeursa.html

TS:   name: string = "x";
来源：http://hz.smart0.xyz/gtgomkatts.html

Java: private String name;
来源：http://hz.shanyushiyangtech.top/gtmrodbaaq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jyoumei.cn/gtigqkaeay.html

Ruby: @name = "x"
来源：http://hz.aibaodan.cn/gtxaapfkcq.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.cashguo.top/gtizlasgiy.html

[G04] 定义方法
来源：http://hz.jqgfzy.top/gtlmwjvoab.html

Py:   def greet(self): return self.name
来源：http://hz.sweek.top/gtvdsmdueh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.iojbl.cn/gtjvxuokqk.html

JS:   greet() { return this.name; }
来源：http://hz.hywenlv.cn/gtnmacoapj.html

TS:   greet(): string { return this.name; }
来源：http://hz.xziqi.cn/gtbjojetzw.html

Java: String greet() { return name; }
来源：http://hz.haohaochexian.top/gtzyiqydfp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.sweek.top/gtqiqvrjqe.html

Ruby: def greet; @name; end
来源：http://hz.tianlin.xyz/gtjowldsxa.html

C#:   public string Greet() => Name;
来源：http://hz.hnqzz.top/gtrygomvrd.html

[G05] 继承
来源：http://hz.daxiang520.top/gtaxanrkhl.html

Py:   class Admin(User): pass
来源：http://hz.birdmap.top/gtdxugjqdr.html

PHP:  class Admin extends User {}
来源：http://hz.zycfv.cn/gtoaxswakp.html

JS:   class Admin extends User {}
来源：http://hz.gotoacloud.top/gtreeihdnd.html

TS:   class Admin extends User {}
来源：http://hz.ehwqpu.com/gtewwzikgm.html

Java: class Admin extends User {}
来源：http://hz.iojbl.cn/gtvxqajnzo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.shzxlz.cn/gtlrzcantg.html

Ruby: class Admin < User; end
来源：http://hz.ywan-chungtsiang.top/gtgabyckzx.html

C#:   class Admin : User {}
来源：http://hz.tanke756.top/gtyxutngxh.html

[G06] 重写方法
来源：http://hz.ywan-chungtsiang.top/gtxmdjbahj.html

Py:   def greet(self): return "admin"
来源：http://hz.aizwys.cn/gtachvhnlk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.0kj1m.cn/gtmjltdqyo.html

JS:   greet() { return "admin"; }
来源：http://hz.yangfankeji.com/gtmseqyehd.html

TS:   greet(): string { return "admin"; }
来源：http://hz.cqqwz.cn/gtvgnsevsi.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.xinyue.icu/gtrznrqmfl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.gzhubu.top/gtrsxnumcm.html

Ruby: def greet; "admin"; end
来源：http://hz.wangdashe.top/gtveeutdgp.html

C#:   public override string Greet() => "admin";
来源：http://hz.nanxinkj.top/gtbrsoxmor.html

[G07] 调用父类方法
来源：http://hz.pengpengdd.cyou/gthyveliwd.html

Py:   super().greet()
来源：http://hz.iojbl.cn/gthnckvgww.html

PHP:  parent::greet();
来源：http://hz.kuanghao11.cn/gtlxsexzmg.html

JS:   super.greet();
来源：http://hz.hywenlv.cn/gtxmuzbgto.html

TS:   super.greet();
来源：http://hz.shangyingyoupin.top/gtnntuumhm.html

Java: super.greet();
来源：http://hz.gaohongyu789.top/gtkczdecrd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.mhx1999.top/gtwiprzxxi.html

Ruby: super
来源：http://hz.jiagoushi.top/gtowcrypbh.html

C#:   base.Greet();
来源：http://hz.gotoacloud.top/gtbpxicduf.html

[G08] 静态方法与属性
来源：http://hz.kuanghao11.cn/gtxidbuqeu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.ywan-chungtsiang.top/gtnexixtft.html

PHP:  public static function f() {}
来源：http://hz.yangfankeji.com/gttwcmuckw.html

JS:   static f() {}
来源：http://hz.xuanzx.com/gtfjthgihv.html

TS:   static f(): void {}
来源：http://hz.yueranfly.top/gtlaryfyue.html

Java: static void f() {}
来源：http://hz.shangyingyoupin.top/gtgccbfvrg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.vqdsnc.cn/gtdsgbqmak.html

Ruby: def self.f; end
来源：http://hz.sysykeji.top/gtyoivrmsj.html

C#:   public static void F() {}
来源：http://hz.yueranfly.top/gtxjoxvsxn.html

[G09] 接口 / 抽象类
来源：http://hz.ydzc1.top/gtuxqnwgzy.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zhoulong.xyz/gtukvlxdkm.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.dianchejie.cn/gtijigztir.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jqgufenzy.top/gthnfzptzj.html

TS:   interface Shape { area(): number; }
来源：http://hz.havefunace.top/gthfgfcqkz.html

Java: interface Shape { double area(); }
来源：http://hz.hongshengwenyu.top/gtlwcvgmaj.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zhaomingkeji.xyz/gtflaockad.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhengqikj.top/gtidrmpmfi.html

C#:   interface IShape { double Area(); }
来源：http://hz.jinqigfzy.top/gtlecggclu.html

[G10] 访问控制
来源：http://hz.0kj1m.cn/gtffikikda.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.guowangkeji.top/gttvhkzsue.html

PHP:  public / protected / private
来源：http://hz.xuanzx.com/gtbuxrjtzu.html

JS:   #private 字段；其余公开
来源：http://hz.havefunace.top/gttavdvryw.html

TS:   public / protected / private
来源：http://hz.xylfe.cn/gtxpnqelqp.html

Java: public / protected / private / 默认包级
来源：http://hz.yj20258888.top/gtkftatsqo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.hongshengwenyu.top/gtpouxhklg.html

Ruby: public / protected / private
来源：http://hz.kuanghao11.cn/gtquvxcaej.html

C#:   public / protected / private / internal
来源：http://hz.yanxiufei.cn/gtxksormtr.html

[G11] getter / setter
来源：http://hz.zhongyouzk.top/gtyskbmrvs.html

Py:   @property 与 @x.setter
来源：http://hz.pycfn.com/gtcmvctlgk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.iojbl.cn/gteyhxjnxu.html

JS:   get name() { return this._name; }
来源：http://hz.tianlin.xyz/gtkzolcgvc.html

TS:   get name(): string { return this._name; }
来源：http://hz.wangdashe.top/gtawsxfowp.html

Java: public String getName() { return name; }
来源：http://hz.jlsjyb.cn/gtfpezjetr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.ybcxt.top/gtizznoqmb.html

Ruby: attr_accessor :name
来源：http://hz.andypj.xyz/gtsrtvlwiv.html

C#:   public string Name { get; set; }
来源：http://hz.yj20258888.top/gtetvjbwdm.html

[G12] 对象转字符串
来源：http://hz.nwbrower.top/gtbjnmxxoo.html

Py:   def __str__(self): return self.name
来源：http://hz.gzhubu.top/gtnzulvjhd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.daria6918.cn/gtjvxgwixm.html

JS:   toString() { return this.name; }
来源：http://hz.snrcjt.cn/gtnydpmyve.html

TS:   toString(): string { return this.name; }
来源：http://hz.daria6918.cn/gtffspbfle.html

Java: @Override public String toString() { return name; }
来源：http://hz.xingfuxueyuan.xyz/gtjneujvgm.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.sufxvd.cn/gtsjzhwxxu.html

Ruby: def to_s; @name; end
来源：http://hz.hnqzz.top/gtvdcgxmvm.html

C#:   public override string ToString() => Name;
来源：http://hz.yj20258.top/gtjoahpfpv.html

[G13] 判断对象类型
来源：http://hz.guowangkeji.top/gtuesserre.html

Py:   isinstance(u, User)
来源：http://hz.dianchejie.cn/gtohfspyav.html

PHP:  $u instanceof User
来源：http://hz.vqdsnc.cn/gtpqrdkqao.html

JS:   u instanceof User
来源：http://hz.nanxuanxn.top/gtblxvevff.html

TS:   u instanceof User
来源：http://hz.yangfankeji.com/gtntvdnorg.html

Java: u instanceof User
来源：http://hz.xziqi.cn/gtyqubkbpm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.52xcode.cn/gtmheqvqun.html

Ruby: u.is_a?(User)
来源：http://hz.ywan-chungtsiang.top/gtrhlksakw.html

C#:   u is User
来源：http://hz.ehwqpu.com/gtrzcunquf.html

[G14] 数据类 / record
来源：http://hz.aizwys.cn/gtjhztpmaj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.ppjwa.cn/gtwsjbddia.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.chenjidiqi.icu/gtlngffvqo.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.shuidangran.top/gtomqgjubt.html

TS:   type User = { name: string; age: number };
来源：http://hz.cucudq.cn/gtokxxaqoh.html

Java: record User(String name, int age) {}
来源：http://hz.jinqigfzy.top/gtvpwytsvb.html

Go:   type User struct { Name string; Age int }
来源：http://hz.birdmap.top/gtvylbmria.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.daria6918.cn/gtgjxspdpt.html

C#:   record User(string Name, int Age);
来源：http://hz.sysykeji.top/gtjvjddyzq.html

[G15] 枚举
来源：http://hz.aibaodan.cn/gtdffbovnu.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.dashuyun.cn/gtcqjdboty.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.pengpengdd.cyou/gtvksykjga.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.daxiang520.top/gtehnppdul.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yj20258.top/gtrauzamco.html

Java: enum Color { RED, GREEN }
来源：http://hz.dashuyun.cn/gttqmwaxfj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.chenjidiqi.icu/gtxwmzbsew.html

Ruby: Color = %i[red green].freeze
来源：http://hz.xziqi.cn/gtkjwlihhp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yuanzhike.top/gtrnterqoj.html

[G16] 对象转数组 / 字典
来源：http://hz.aibaodan.cn/gthryvtvsv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhiwuduotai.top/gtyqqzkunw.html

PHP:  get_object_vars($obj);
来源：http://hz.yangfankeji.com/gtksclusgb.html

JS:   Object.entries(obj)
来源：http://hz.nanxuanxn.top/gtrhkptzjq.html

TS:   Object.entries(obj)
来源：http://hz.tanke756.top/gtimlnpfwj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.pengpengdd.cyou/gtbusdtgpt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.ywan-chungtsiang.top/gtjicwmjfw.html

Ruby: obj.instance_variables
来源：http://hz.9152youxi.cn/gtdcnomtwv.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.ydzc1.top/gtrubncgnh.html

================================================================================
来源：http://hz.yonumen.top/gtgupqibxz.html

H. 异常与错误处理
来源：http://hz.guannengcc.top/gtcespoqxd.html

================================================================================
来源：http://hz.guannengcc.top/gtleyrcrze.html

[H01] try / catch 基础
来源：http://hz.pengpengdd.cyou/gtyflamngw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.gzhubu.top/gtivyyjwkx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zhiwuduotai.top/gtiwpxtstz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.andypj.xyz/gtfzdqdxtm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.cheryme.top/gtywwxlbpa.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zhiwuduotai.top/gtojhnzmek.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.wangdashe.top/gtsobzggpg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yj202588.top/gtapablrni.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.chenjidiqi.icu/gtdibwgnvc.html

[H02] finally / ensure 收尾
来源：http://hz.xingfuxueyuan.xyz/gtnepcwugl.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zhiwuduotai.top/gtcxwabjhv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.guannengcc.top/gtyvgtxevq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.birdmap.top/gtikemcwzu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.xuetiantiany.cn/gtwonsnhoe.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.52xcode.cn/gtjajjqbnp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.chenjidiqi.icu/gtkzzzbvdf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yj20258.top/gtttajpfrh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hongshengwenyu.top/gtpnxfoawb.html

[H03] 主动抛出异常
来源：http://hz.zhijiandao.cn/gtrtlescji.html

Py:   raise ValueError("错误信息")
来源：http://hz.aibaodan.cn/gthhqvgcns.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.sxryk.cn/gtjumwdglq.html

JS:   throw new Error("错误信息");
来源：http://hz.yueranfly.top/gtbzekwnkc.html

TS:   throw new Error("错误信息");
来源：http://hz.yj20258.top/gtcwzxpojq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.ydzc1.top/gtdhnsrial.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.smart0.xyz/gtevfqribo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.meibo888.top/gtgmvtawdl.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.redwolf501.top/gtpmzjnwpg.html

[H04] 自定义异常类型
来源：http://hz.zhaomingkeji.xyz/gtxxndmhxz.html

Py:   class MyError(Exception): pass
来源：http://hz.quarkkingdee.top/gtelwlmhiy.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jiagoushi.top/gtwmgtqrye.html

JS:   class MyError extends Error {}
来源：http://hz.smart0.xyz/gtyspxheoj.html

TS:   class MyError extends Error {}
来源：http://hz.xylfe.cn/gtloxwbwol.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zhixingplan.top/gtwtgyirgp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.gaohongyu789.top/gtqkkqnksz.html

Ruby: class MyError < StandardError; end
来源：http://hz.xylfe.cn/gtuobzinbg.html

C#:   class MyException : Exception {}
来源：http://hz.0kj1m.cn/gtfrodmuyb.html

[H05] 捕获特定类型
来源：http://hz.ivvv.top/gtdjlnqwxf.html

Py:   except ValueError as e:
来源：http://hz.guannengcc.top/gtkiypauvf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.nanxinkj.top/gtmwtwggkl.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.ywan-chungtsiang.top/gtnunldwjb.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.pycfn.com/gtrcdxgyoq.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.cdnleiting.top/gtexfitvbl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.shangyingyoupin.top/gtgmiecbyc.html

Ruby: rescue ArgumentError => e
来源：http://hz.hywenlv.cn/gteverheug.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.havefunace.top/gthuemuvfe.html

[H06] 可选值 / 空值安全访问
来源：http://hz.0kj1m.cn/gtrndcfgcj.html

Py:   value = d.get("k") or default
来源：http://hz.daria6918.cn/gtxjegnrwr.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yuanzhike.top/gtxdyrhzbd.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.shangyingyoupin.top/gtftwdbtcp.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.chenlongwang.top/gtxmaiasen.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jiagoushi.top/gttnpjsefh.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yanxiufei.cn/gtiffizvyg.html

Ruby: d&.dig(:a, :b)
来源：http://hz.gogol.net.cn/gtpfhvoohs.html

C#:   obj?.A?.B ?? default
来源：http://hz.ydzc1.top/gtrswmwdnh.html

[H07] 断言
来源：http://hz.pengpengdd.cyou/gtmqybpnsn.html

Py:   assert x > 0, "必须为正"
来源：http://hz.sufxvd.cn/gtmmhucsng.html

PHP:  assert($x > 0);
来源：http://hz.jinqigufen.top/gtxffwpmwc.html

JS:   console.assert(x > 0);
来源：http://hz.hammf.cn/gtuhoacnfh.html

TS:   console.assert(x > 0);
来源：http://hz.0kj1m.cn/gtscaobngq.html

Java: assert x > 0 : "必须为正";
来源：http://hz.hysaishi.cn/gtyyocknhg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ydjk.org.cn/gthtagbyjy.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.sxryk.cn/gtmzbeylma.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yonumen.top/gtczwvbkng.html

[H08] 获取错误信息与堆栈
来源：http://hz.aizwys.cn/gtmtkgwbee.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zhaomingkeji.xyz/gtyaetakyf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.bjfxy.top/gtyxrszpuw.html

JS:   e.message;  e.stack
来源：http://hz.xingfuxueyuan.xyz/gtbngumbks.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.gotoacloud.top/gtxltrxqwx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yonumen.top/gtksilhvmz.html

Go:   err.Error()
来源：http://hz.quarkkingdee.top/gtcsmzflqt.html

Ruby: e.message;  e.backtrace
来源：http://hz.jinghuilouyu.cn/gtppiwlxlj.html

C#:   e.Message;  e.StackTrace
来源：http://hz.chenjidiqi.icu/gtiohkdwpq.html

[H09] 带错误码的异常
来源：http://hz.daxiang520.top/gtyivvbisl.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.ywan-chungtsiang.top/gtviimmckh.html


<!-- 参考信息 -->