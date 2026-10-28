代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.cashguo.top/gtntmvzzfy.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.cashguo.top/gtryevyfzz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yvedp.cn/gtejhotwwm.html

[F04] 追加写入文件
来源：http://hz.dashuyun.cn/gtswajlflq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.ydjk.org.cn/gthhkfkilo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.jinqigfzy.top/gtfvihudvo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.kuanghao11.cn/gtgyfplshd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhijiandao.cn/gtwuipclzx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.vqdsnc.cn/gtjbeftuyt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yuanzhike.top/gtorhhtydx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.wangdashe.top/gtrtnwfwsw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.aibaodan.cn/gtrwghjrql.html

[F05] 判断文件或目录是否存在
来源：http://hz.iojbl.cn/gttqywqfav.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.shzxlz.cn/gtrhmsatil.html

PHP:  file_exists("a.txt");
来源：http://hz.nanxuanxn.top/gtifmixjde.html

JS:   fs.existsSync("a.txt")
来源：http://hz.xuetiantiany.cn/gtudfjrzoq.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zycfv.cn/gteqddpgpi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.svipenyu.cn/gtcafjbcdg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.cheryme.top/gtsnhllvlm.html

Ruby: File.exist?("a.txt")
来源：http://hz.sysykeji.top/gtltifyfxz.html

C#:   File.Exists("a.txt")
来源：http://hz.shuidangran.top/gtyjfoqoin.html

[F06] 删除文件
来源：http://hz.zdqjudy.top/gthzokinhp.html

Py:   os.remove("a.txt")
来源：http://hz.hammf.cn/gtsrjjilws.html

PHP:  unlink("a.txt");
来源：http://hz.wangshuangyany.cn/gtxbfwqfmv.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hammf.cn/gtaqkiiiac.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.dianchejie.cn/gtqwsqnqwy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.c1oappe.top/gtqobofeke.html

Go:   os.Remove("a.txt")
来源：http://hz.shangyingyoupin.top/gtxhgsqabd.html

Ruby: File.delete("a.txt")
来源：http://hz.hammf.cn/gtvtkbtvht.html

C#:   File.Delete("a.txt");
来源：http://hz.c1oappe.top/gtndxhxqyy.html

[F07] 创建目录（含多级）
来源：http://hz.ybcxt.top/gtbfgieett.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jianghu66.top/gtqmugmmwh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.smart0.xyz/gtkcmxxkrk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.c1oappe.top/gtrmpurcis.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.svipenyu.cn/gtwidzbyai.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.gaohongyu789.top/gtcctxijta.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hfpthk.cn/gtqfauscbc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.aibaodan.cn/gtcsyyzupw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.sufxvd.cn/gtexsuvhev.html

[F08] 遍历目录
来源：http://hz.chenjidiqi.icu/gtrfqmthde.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.316326.xyz/gtmbbbetqn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.bjfxy.top/gthkdwjnxh.html

JS:   fs.readdirSync("dir")
来源：http://hz.hnqzz.top/gtuppdfbrq.html

TS:   fs.readdirSync("dir")
来源：http://hz.chenlongwang.top/gtqbfggbwt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.fzhhl.top/gtmbjlmwfs.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.tian-w.cn/gtzqqkmcrx.html

Ruby: Dir.children("dir")
来源：http://hz.xingfuxueyuan.xyz/gtwmcvvceq.html

C#:   Directory.GetFiles("dir")
来源：http://hz.ivvv.top/gtbtbkxmmt.html

[F09] 获取文件大小
来源：http://hz.zhongyouzk.top/gtlplfatge.html

Py:   os.path.getsize("a.txt")
来源：http://hz.cashguo.top/gttyehgzvn.html

PHP:  filesize("a.txt");
来源：http://hz.hammf.cn/gteiuvymmi.html

JS:   fs.statSync("a.txt").size
来源：http://hz.52xcode.cn/gtlzpygtpr.html

TS:   fs.statSync("a.txt").size
来源：http://hz.mhx1999.top/gtjbrrwqbv.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.shanyushiyangkeji.top/gtghnonczf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.dianchejie.cn/gtadvbwwlr.html

Ruby: File.size("a.txt")
来源：http://hz.yueranfly.top/gtcgvscivm.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.birdmap.top/gtgcexlyhb.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.dashuyun.cn/gthnkjcact.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zhiwuduotai.top/gtyeddwqtl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.0kj1m.cn/gthpkbjwco.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yuxming.cn/gtjssxyawv.html

TS:   path.extname("a.txt")
来源：http://hz.havefunace.top/gtjymwkusf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.quarkkingdee.top/gtyesygvpn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yj202588.top/gtwvpyzpmo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.cheryme.top/gtmogekqeb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zhaomingkeji.xyz/gtxtnrajgm.html

[F11] 复制与移动文件
来源：http://hz.birdmap.top/gterevbgla.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yongpay.top/gtsurtdqfn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.hfpthk.cn/gtrfbxpklt.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.feifeiyinyue.top/gtstgcuecb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.andypj.xyz/gtpeusiops.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jqgfzy.top/gtxmukxnul.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.zhoulong.xyz/gtntpopvsj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.gotoacloud.top/gtmnjomvxq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.tian-w.cn/gtwmoriphs.html

[F12] CSV 读写
来源：http://hz.xinyue.icu/gtiocahecz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.pengpengdd.cyou/gtpzlnfygy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jianghu66.top/gttovwgivi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.mhx1999.top/gtwadbwqln.html

TS:   // 同上
来源：http://hz.yanxiufei.cn/gtrwbubszn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.dashuyun.cn/gtntmctorq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.nanxuanxn.top/gtnyuxvjom.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.hongshengwenyu.top/gtrjtnzilt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jinghuilouyu.cn/gtglgqzkqo.html

================================================================================
来源：http://hz.cashguo.top/gtrranmhzy.html

G. 面向对象
来源：http://hz.fengsongda.top/gtdrykebcw.html

================================================================================
来源：http://hz.52xcode.cn/gtkppvakcp.html

[G01] 定义类
来源：http://hz.c1oappe.top/gtjfhjmxdc.html

Py:   class User: pass
来源：http://hz.smart0.xyz/gtokzmlvdf.html

PHP:  class User {}
来源：http://hz.shanyushiyangkeji.top/gtjlyxygif.html

JS:   class User {}
来源：http://hz.jiagoushi.top/gtklvonneo.html

TS:   class User { name: string = ""; }
来源：http://hz.xziqi.cn/gtledcvdoc.html

Java: class User {}
来源：http://hz.gogol.net.cn/gtuiufoomj.html

Go:   type User struct { Name string }
来源：http://hz.smart0.xyz/gtsbgbgwsm.html

Ruby: class User; end
来源：http://hz.jiagoushi.top/gtynwdcnpv.html

C#:   class User {}
来源：http://hz.svipenyu.cn/gtjcfikoic.html

[G02] 构造函数
来源：http://hz.sufxvd.cn/gtgexwzakj.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jqgfzy.top/gtdlgurfxn.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.shuidangran.top/gtmnbkcxyp.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.ydjk.org.cn/gtnxdeuypm.html

TS:   constructor(public name: string) {}
来源：http://hz.redwolf501.top/gtekuwceuz.html

Java: User(String name) { this.name = name; }
来源：http://hz.chenlongwang.top/gtynaiwetn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.gogol.net.cn/gtdxhkdxth.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yj20258.top/gtkexwwtzy.html

C#:   public User(string name) { Name = name; }
来源：http://hz.tianlin.xyz/gtcovhogbc.html

[G03] 实例属性
来源：http://hz.jlsjyb.cn/gtpyvvggkx.html

Py:   self.name = "x"
来源：http://hz.gotoacloud.top/gthcoepzzw.html

PHP:  public string $name = "x";
来源：http://hz.316326.xyz/gtwhvcewpt.html

JS:   this.name = "x";
来源：http://hz.chenlongwang.top/gtnihwbkot.html

TS:   name: string = "x";
来源：http://hz.hnqzz.top/gtvgnihuey.html

Java: private String name;
来源：http://hz.zhiwuduotai.top/gtpwyaajfx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yuxming.cn/gtrndyjvzj.html

Ruby: @name = "x"
来源：http://hz.tian-w.cn/gtzdusyddh.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yangfankeji.com/gtgyjpfryy.html

[G04] 定义方法
来源：http://hz.jyoumei.cn/gtceqcwadr.html

Py:   def greet(self): return self.name
来源：http://hz.shuidangran.top/gthwalgeui.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yangfankeji.com/gtngdronyv.html

JS:   greet() { return this.name; }
来源：http://hz.shanyushiyangkeji.top/gtyronttui.html

TS:   greet(): string { return this.name; }
来源：http://hz.sxryk.cn/gtzapvkjmk.html

Java: String greet() { return name; }
来源：http://hz.iojbl.cn/gtzqebemiz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.pycfn.com/gtypaeqtjm.html

Ruby: def greet; @name; end
来源：http://hz.cqqwz.cn/gtxcgkoptj.html

C#:   public string Greet() => Name;
来源：http://hz.nanxinkj.top/gtgeoafwyr.html

[G05] 继承
来源：http://hz.daria6918.cn/gtsftapapb.html

Py:   class Admin(User): pass
来源：http://hz.aizwys.cn/gtzehsqcut.html

PHP:  class Admin extends User {}
来源：http://hz.ehwqpu.com/gtwopxwnic.html

JS:   class Admin extends User {}
来源：http://hz.xuetiantiany.cn/gtirczcduz.html

TS:   class Admin extends User {}
来源：http://hz.yj20258888.top/gtjtdaxkzt.html

Java: class Admin extends User {}
来源：http://hz.wangshuangyany.cn/gtehyualxl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.gogol.net.cn/gtkwejdqqm.html

Ruby: class Admin < User; end
来源：http://hz.yuxming.cn/gtampvxmkr.html

C#:   class Admin : User {}
来源：http://hz.ywan-chungtsiang.top/gtnihrwkot.html

[G06] 重写方法
来源：http://hz.fzhhl.top/gtklapfeko.html

Py:   def greet(self): return "admin"
来源：http://hz.meibo888.top/gtvlpwrnxq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yuanzhike.top/gtbmtmqjpw.html

JS:   greet() { return "admin"; }
来源：http://hz.hfpthk.cn/gtvhqixmae.html

TS:   greet(): string { return "admin"; }
来源：http://hz.gzhubu.top/gtcsvulaen.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.tanke756.top/gtvxxlmphj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.wangshuangyany.cn/gtgcjfmnqh.html

Ruby: def greet; "admin"; end
来源：http://hz.tianlin.xyz/gtjzbnufhd.html

C#:   public override string Greet() => "admin";
来源：http://hz.hnxiangtu.top/gtowkifdfs.html

[G07] 调用父类方法
来源：http://hz.zhixingplan.top/gtajecbqyb.html

Py:   super().greet()
来源：http://hz.gogol.net.cn/gtzlkijspe.html

PHP:  parent::greet();
来源：http://hz.hnxiangtu.top/gtnfggmzws.html

JS:   super.greet();
来源：http://hz.vqdsnc.cn/gtwrkelzbo.html

TS:   super.greet();
来源：http://hz.ivvv.top/gtkjktciby.html

Java: super.greet();
来源：http://hz.haohaochexian.top/gtkphdudzf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.hnxiangtu.top/gtwppmtugq.html

Ruby: super
来源：http://hz.kuanghao11.cn/gtwkztqnoo.html

C#:   base.Greet();
来源：http://hz.xuetiantiany.cn/gtbtdfeczz.html

[G08] 静态方法与属性
来源：http://hz.jinqigufen.top/gtvtdwzemk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.birdmap.top/gtnlnkswtw.html

PHP:  public static function f() {}
来源：http://hz.havefunace.top/gtstmdxhmi.html

JS:   static f() {}
来源：http://hz.xuetiantiany.cn/gtgawupcrx.html

TS:   static f(): void {}
来源：http://hz.yvedp.cn/gtenjhjksn.html

Java: static void f() {}
来源：http://hz.chenjidiqi.icu/gtqjecejhp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jyoumei.cn/gtuvvcrspj.html

Ruby: def self.f; end
来源：http://hz.316326.xyz/gtptahoprz.html

C#:   public static void F() {}
来源：http://hz.yonumen.top/gteezqrggj.html

[G09] 接口 / 抽象类
来源：http://hz.chenlongwang.top/gtjkrenzck.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jqgfzy.top/gtaiipknmq.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.wangdashe.top/gtrygcngnf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zycfv.cn/gtddfogfov.html

TS:   interface Shape { area(): number; }
来源：http://hz.jlsjyb.cn/gtnlacimqw.html

Java: interface Shape { double area(); }
来源：http://hz.shanyushiyangtech.top/gtciwaened.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.hfpthk.cn/gtlmmziuwl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhijiandao.cn/gtcqbricvr.html

C#:   interface IShape { double Area(); }
来源：http://hz.gaohongyu789.top/gtmuzalulv.html

[G10] 访问控制
来源：http://hz.xziqi.cn/gtuvseegxy.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.xylfe.cn/gtukjdamtn.html

PHP:  public / protected / private
来源：http://hz.sufxvd.cn/gtnuntkwde.html

JS:   #private 字段；其余公开
来源：http://hz.zycfv.cn/gtaezbgrlb.html

TS:   public / protected / private
来源：http://hz.pengpengdd.cyou/gtmxitqgxu.html

Java: public / protected / private / 默认包级
来源：http://hz.jlsjyb.cn/gtgzfqiemn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.daria6918.cn/gthsiaxszn.html

Ruby: public / protected / private
来源：http://hz.yangfankeji.com/gtygxypggr.html

C#:   public / protected / private / internal
来源：http://hz.wangshuangyany.cn/gtmhkewksc.html

[G11] getter / setter
来源：http://hz.zycfv.cn/gtarmtnwoe.html

Py:   @property 与 @x.setter
来源：http://hz.daria6918.cn/gtobltluuo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jlsjyb.cn/gtxftbwkhj.html

JS:   get name() { return this._name; }
来源：http://hz.jyoumei.cn/gtgiupzhwk.html

TS:   get name(): string { return this._name; }
来源：http://hz.haohaochexian.top/gtowswuixk.html

Java: public String getName() { return name; }
来源：http://hz.jinqigufen.top/gtpckqhcaz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.hywenlv.cn/gtwypwaalu.html

Ruby: attr_accessor :name
来源：http://hz.guannengcc.top/gtmezovbmn.html

C#:   public string Name { get; set; }
来源：http://hz.yj20258.top/gtflipurle.html

[G12] 对象转字符串
来源：http://hz.316326.xyz/gtlmthytsd.html

Py:   def __str__(self): return self.name
来源：http://hz.kuanghao11.cn/gtetdmlzub.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.vqdsnc.cn/gtvrrexrtv.html

JS:   toString() { return this.name; }
来源：http://hz.zhengqikj.top/gtrpmbdpfa.html

TS:   toString(): string { return this.name; }
来源：http://hz.jyoumei.cn/gthfyvnwxb.html

Java: @Override public String toString() { return name; }
来源：http://hz.iojbl.cn/gtvdyypvwk.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhoulong.xyz/gtgmvlctyo.html

Ruby: def to_s; @name; end
来源：http://hz.daxiang520.top/gttgtexbzx.html

C#:   public override string ToString() => Name;
来源：http://hz.sweek.top/gtclgjsfhp.html

[G13] 判断对象类型
来源：http://hz.ywan-chungtsiang.top/gthnibfxki.html

Py:   isinstance(u, User)
来源：http://hz.meibo888.top/gtdiwdueap.html

PHP:  $u instanceof User
来源：http://hz.xinyue.icu/gtxmkhiavj.html

JS:   u instanceof User
来源：http://hz.dianchejie.cn/gtmoywdmfb.html

TS:   u instanceof User
来源：http://hz.zhiwuduotai.top/gtgtvssazd.html

Java: u instanceof User
来源：http://hz.jyoumei.cn/gthreenaek.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.xuetiantiany.cn/gtckcqnryh.html

Ruby: u.is_a?(User)
来源：http://hz.gogol.net.cn/gtumotbpyg.html

C#:   u is User
来源：http://hz.mhx1999.top/gtuoyuopbz.html

[G14] 数据类 / record
来源：http://hz.hfpthk.cn/gtfpamqpti.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.vqdsnc.cn/gtljjjpolk.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yonumen.top/gttsnairog.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhoulong.xyz/gtmwdqqehm.html

TS:   type User = { name: string; age: number };
来源：http://hz.zhaomingkeji.xyz/gtxrufxhrx.html

Java: record User(String name, int age) {}
来源：http://hz.0kj1m.cn/gtyntoevyd.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jqgufenzy.top/gtuwdqcblo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.daria6918.cn/gtyhclnyxk.html

C#:   record User(string Name, int Age);
来源：http://hz.daria6918.cn/gtewtelyhd.html

[G15] 枚举
来源：http://hz.quarkkingdee.top/gtkxsmndix.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yuanzhike.top/gtsusbptnx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jinqigfzy.top/gtecxscsun.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.9152youxi.cn/gtyfkgedpe.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shangyingyoupin.top/gtevcizfrw.html

Java: enum Color { RED, GREEN }
来源：http://hz.fzhhl.top/gtahrwqlst.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yvedp.cn/gtaokbesqk.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ydjk.org.cn/gthmxqocek.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.meibo888.top/gtslkxbycn.html

[G16] 对象转数组 / 字典
来源：http://hz.kuanghao11.cn/gtahnpgzcx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.shangyingyoupin.top/gtitueqnse.html

PHP:  get_object_vars($obj);
来源：http://hz.havefunace.top/gtoorxmsqw.html

JS:   Object.entries(obj)
来源：http://hz.ydzc1.top/gtawnvxvam.html

TS:   Object.entries(obj)
来源：http://hz.jiagoushi.top/gtviwggmpy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhongyouzk.top/gtefyrppbc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.nanxinkj.top/gtwqmeauls.html

Ruby: obj.instance_variables
来源：http://hz.redwolf501.top/gteqfuyumg.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.aibaodan.cn/gtycpqtohw.html

================================================================================
来源：http://hz.yuanzhike.top/gtjxnfpdcn.html

H. 异常与错误处理
来源：http://hz.iojbl.cn/gtujqiwgau.html

================================================================================
来源：http://hz.52xcode.cn/gtkgxinvqo.html

[H01] try / catch 基础
来源：http://hz.zhengqikj.top/gtatzwcthn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.ywan-chungtsiang.top/gtcqctogxn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.vqdsnc.cn/gttvvqyybi.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.gogol.net.cn/gtbkzmimru.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.wangshuangyany.cn/gtqapddwxy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jyoumei.cn/gtztrmhplr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.birdmap.top/gtqbzpdode.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jinyuanbaomall.cn/gtczfrcssl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.iojbl.cn/gtdwakgset.html

[H02] finally / ensure 收尾
来源：http://hz.kuanghao11.cn/gtmotedvep.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.ivvv.top/gtpndqhebg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hnqzz.top/gtvmjfbwgb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.cdnleiting.top/gtmmxdwehh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jqgfzy.top/gtqjrdgkjw.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.nwbrower.top/gtpcgiszul.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ppjwa.cn/gtitltfnlh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.hammf.cn/gtgbaqzhoq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.shangyingyoupin.top/gtbxkzudbl.html

[H03] 主动抛出异常
来源：http://hz.daria6918.cn/gtyyqlhoig.html

Py:   raise ValueError("错误信息")
来源：http://hz.dashuyun.cn/gttkmubwkr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.ivvv.top/gtlfgrsujh.html

JS:   throw new Error("错误信息");
来源：http://hz.zhijiandao.cn/gtldzmtwww.html

TS:   throw new Error("错误信息");
来源：http://hz.jinqigfzy.top/gtcyetoyxf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yanxiufei.cn/gtrzyfycgn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.fengsongda.top/gtwgxclkxx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zycfv.cn/gtqgmjmnba.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.ydzc1.top/gtnizwhink.html

[H04] 自定义异常类型
来源：http://hz.cashguo.top/gtgtzstgef.html

Py:   class MyError(Exception): pass
来源：http://hz.aibaodan.cn/gtxbdsxahn.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.daxiang520.top/gtwifasuml.html

JS:   class MyError extends Error {}
来源：http://hz.c1oappe.top/gtmhyagnoa.html

TS:   class MyError extends Error {}
来源：http://hz.xuetiantiany.cn/gtcyoglndu.html

Java: class MyException extends RuntimeException {}
来源：http://hz.andypj.xyz/gtlgynqhmz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zhiwuduotai.top/gthvqyliwk.html

Ruby: class MyError < StandardError; end
来源：http://hz.ppjwa.cn/gtwaoulenc.html

C#:   class MyException : Exception {}
来源：http://hz.meibo888.top/gtvtrrdqyx.html

[H05] 捕获特定类型
来源：http://hz.cheryme.top/gtftehziuw.html

Py:   except ValueError as e:
来源：http://hz.tanke756.top/gtmhostpoa.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.guannengcc.top/gtsaurukyn.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.xinyue.icu/gtyqvawdgy.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yvedp.cn/gtafaibmwc.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.daxiang520.top/gtojocvdwu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zhixingplan.top/gtsfxfhomf.html

Ruby: rescue ArgumentError => e
来源：http://hz.gzhubu.top/gtayfnejsc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yanxiufei.cn/gtilijlbrq.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zhijiandao.cn/gtnsinyamf.html

Py:   value = d.get("k") or default
来源：http://hz.feifeiyinyue.top/gttsybayqx.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.gogol.net.cn/gtkgefquip.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yuxming.cn/gtgiehjzky.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yj202588.top/gtscgnefwm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.gotoacloud.top/gtnldroclq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jyoumei.cn/gtfibpqnqr.html

Ruby: d&.dig(:a, :b)
来源：http://hz.tian-w.cn/gtrspgyrhn.html

C#:   obj?.A?.B ?? default
来源：http://hz.xuetiantiany.cn/gtcxymaspi.html

[H07] 断言
来源：http://hz.52xcode.cn/gtruknwpbp.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yj202588.top/gtecewgqnf.html

PHP:  assert($x > 0);
来源：http://hz.aibaodan.cn/gtubqxdfih.html

JS:   console.assert(x > 0);
来源：http://hz.ppjwa.cn/gtvjqhkgsg.html

TS:   console.assert(x > 0);
来源：http://hz.hysaishi.cn/gtgnbqtczv.html

Java: assert x > 0 : "必须为正";
来源：http://hz.pycfn.com/gttodkkejj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.pengpengdd.cyou/gtfcgxumlp.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yuanzhike.top/gtowezwsjm.html

C#:   Debug.Assert(x > 0);
来源：http://hz.ehwqpu.com/gthgnmcvly.html

[H08] 获取错误信息与堆栈
来源：http://hz.daxiang520.top/gtxnzzkcsm.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yuxming.cn/gtdzpxpfkp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.hfpthk.cn/gtuzsjanky.html


<!-- 参考信息 -->