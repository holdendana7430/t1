代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yj202588.top/gttoqbiquy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yueranfly.top/gtpsngpzme.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.nanxinkj.top/gtsflospzx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.chenjidiqi.icu/gteaygmbbf.html

[F05] 判断文件或目录是否存在
来源：http://hz.feifeiyinyue.top/gtqaxkoycf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yonumen.top/gtzkgqkawj.html

PHP:  file_exists("a.txt");
来源：http://hz.yongpay.top/gthcrvgfgc.html

JS:   fs.existsSync("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtbtvezgiy.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yangfankeji.com/gtynvmzzyj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jinqigfzy.top/gtiphbtlfn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zhiwuduotai.top/gtppekytmr.html

Ruby: File.exist?("a.txt")
来源：http://hz.cqqwz.cn/gtcetslkmc.html

C#:   File.Exists("a.txt")
来源：http://hz.kuanghao11.cn/gtdrboxtas.html

[F06] 删除文件
来源：http://hz.sufxvd.cn/gtwfzbbtol.html

Py:   os.remove("a.txt")
来源：http://hz.yueranfly.top/gttaadnljs.html

PHP:  unlink("a.txt");
来源：http://hz.xziqi.cn/gtzefnmcti.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.gaohongyu789.top/gtwljxyafd.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtpzjdudqa.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jinghuilouyu.cn/gtdifngacl.html

Go:   os.Remove("a.txt")
来源：http://hz.guowangkeji.top/gtmhsejiiq.html

Ruby: File.delete("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtfjaerfuq.html

C#:   File.Delete("a.txt");
来源：http://hz.nwbrower.top/gthccwhxct.html

[F07] 创建目录（含多级）
来源：http://hz.fzhhl.top/gtasitvblx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jinghuilouyu.cn/gtprbqusbf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.feifeiyinyue.top/gtjpgatmua.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jinqigfzy.top/gtchsgkzae.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.gzhubu.top/gttnxojcvt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.dashuyun.cn/gtiaeogzlo.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.gzhubu.top/gthuuuzasb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.dianchejie.cn/gtuykkpsqg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.dianchejie.cn/gtfzfhgiyk.html

[F08] 遍历目录
来源：http://hz.cucudq.cn/gtuajbldof.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.xingfuxueyuan.xyz/gtjhluluue.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.fzhhl.top/gtusuhavmh.html

JS:   fs.readdirSync("dir")
来源：http://hz.ydjk.org.cn/gtawqftpuu.html

TS:   fs.readdirSync("dir")
来源：http://hz.shuidangran.top/gtospqiepx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.dianchejie.cn/gtmtyfzxqb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zdqjudy.top/gtdyueqxuj.html

Ruby: Dir.children("dir")
来源：http://hz.c1oappe.top/gtolfsqory.html

C#:   Directory.GetFiles("dir")
来源：http://hz.vqdsnc.cn/gtqwcnbssr.html

[F09] 获取文件大小
来源：http://hz.chenlongwang.top/gtgxxotabs.html

Py:   os.path.getsize("a.txt")
来源：http://hz.dashuyun.cn/gtnopsoezn.html

PHP:  filesize("a.txt");
来源：http://hz.yueranfly.top/gtgffgtqtx.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zhiwuduotai.top/gttbtpjzhe.html

TS:   fs.statSync("a.txt").size
来源：http://hz.hfpthk.cn/gtfzlodmox.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.pengpengdd.cyou/gtivfrkkja.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.ivvv.top/gtupkmybjs.html

Ruby: File.size("a.txt")
来源：http://hz.xuanzx.com/gtddljolfp.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.tianlin.xyz/gtxbjvplyq.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.bjfxy.top/gtgijkdvfq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.smart0.xyz/gtjxqaieoy.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.shanyushiyangkeji.top/gtlwwafwtk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.wangdashe.top/gtdxjgnbot.html

TS:   path.extname("a.txt")
来源：http://hz.zdqjudy.top/gtfbbstfhd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yueranfly.top/gtnmyqkmbm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.hysaishi.cn/gtesgqcvwz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.guannengcc.top/gtrrjkfkkg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.sweek.top/gtizmorxnn.html

[F11] 复制与移动文件
来源：http://hz.iojbl.cn/gtlifxpxuw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zycfv.cn/gtnswxaool.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jyoumei.cn/gtnchhfjca.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.snrcjt.cn/gtiagleysv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.guannengcc.top/gtibuwpctu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zhoulong.xyz/gtnqchykhw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.hywenlv.cn/gtojfsychg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.ywan-chungtsiang.top/gtqujjaqnn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.fengsongda.top/gtgbyjbmeb.html

[F12] CSV 读写
来源：http://hz.hammf.cn/gtpakdfzpo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.shuidangran.top/gtkwxaurbd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.mhx1999.top/gtrwpwegjz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.xziqi.cn/gtqtjztsha.html

TS:   // 同上
来源：http://hz.zhongyouzk.top/gtgbdcknil.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.gotoacloud.top/gtfgvobysl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.shangyingyoupin.top/gtloisysnm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.tian-w.cn/gtnoakgbxd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.sufxvd.cn/gtofofctez.html

================================================================================
来源：http://hz.yangfankeji.com/gtclfjplxo.html

G. 面向对象
来源：http://hz.vqdsnc.cn/gthrhovjdu.html

================================================================================
来源：http://hz.fzhhl.top/gtpqzqsxbk.html

[G01] 定义类
来源：http://hz.pycfn.com/gtwtrfxfzd.html

Py:   class User: pass
来源：http://hz.fengsongda.top/gtgevptmpc.html

PHP:  class User {}
来源：http://hz.dianchejie.cn/gtkfexinpa.html

JS:   class User {}
来源：http://hz.yonumen.top/gtqxystqgr.html

TS:   class User { name: string = ""; }
来源：http://hz.zhiwuduotai.top/gtwlrxyaxz.html

Java: class User {}
来源：http://hz.ydjk.org.cn/gtdixeewzd.html

Go:   type User struct { Name string }
来源：http://hz.316326.xyz/gthwqaqhij.html

Ruby: class User; end
来源：http://hz.9152youxi.cn/gtrkncrdcd.html

C#:   class User {}
来源：http://hz.jlsjyb.cn/gtxfcblvtv.html

[G02] 构造函数
来源：http://hz.nanxinkj.top/gtzwrkjiua.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yj20258.top/gtnaaojxkt.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ppjwa.cn/gtltutwoop.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.hongshengwenyu.top/gtwjgntnzb.html

TS:   constructor(public name: string) {}
来源：http://hz.haohaochexian.top/gtsdnptvvc.html

Java: User(String name) { this.name = name; }
来源：http://hz.ivvv.top/gtsdxqbwau.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.xinyue.icu/gtpufjswdu.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.dianchejie.cn/gtpegkppxn.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jinqigfzy.top/gtjsdkqmqt.html

[G03] 实例属性
来源：http://hz.ybcxt.top/gtcdfyedcm.html

Py:   self.name = "x"
来源：http://hz.snrcjt.cn/gtnpqiiplg.html

PHP:  public string $name = "x";
来源：http://hz.9152youxi.cn/gtuaiipzkx.html

JS:   this.name = "x";
来源：http://hz.hysaishi.cn/gtpqnungeo.html

TS:   name: string = "x";
来源：http://hz.meibo888.top/gtdaroyxrl.html

Java: private String name;
来源：http://hz.jinghuilouyu.cn/gtcowinsin.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yj20258888.top/gtcndfuzkn.html

Ruby: @name = "x"
来源：http://hz.dianchejie.cn/gtnqfkynlc.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hnqzz.top/gttlzqnbfx.html

[G04] 定义方法
来源：http://hz.ivvv.top/gtssrvihwx.html

Py:   def greet(self): return self.name
来源：http://hz.9152youxi.cn/gtljxvsets.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.xylfe.cn/gtxiavxvjr.html

JS:   greet() { return this.name; }
来源：http://hz.gzhubu.top/gtbopiojyn.html

TS:   greet(): string { return this.name; }
来源：http://hz.sxryk.cn/gtcwiljuwj.html

Java: String greet() { return name; }
来源：http://hz.iojbl.cn/gthxairmlq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.mhx1999.top/gtfgtevsdv.html

Ruby: def greet; @name; end
来源：http://hz.hnxiangtu.top/gtqluyylig.html

C#:   public string Greet() => Name;
来源：http://hz.jinghuilouyu.cn/gtmdqpqzzi.html

[G05] 继承
来源：http://hz.zdqjudy.top/gtoxlkxbns.html

Py:   class Admin(User): pass
来源：http://hz.chenjidiqi.icu/gtoprffivo.html

PHP:  class Admin extends User {}
来源：http://hz.quarkkingdee.top/gthrtmoenc.html

JS:   class Admin extends User {}
来源：http://hz.xziqi.cn/gtauhbetub.html

TS:   class Admin extends User {}
来源：http://hz.pengpengdd.cyou/gtyufnfhbo.html

Java: class Admin extends User {}
来源：http://hz.zhiwuduotai.top/gtxbiwswqw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.shzxlz.cn/gtnwpdhrxu.html

Ruby: class Admin < User; end
来源：http://hz.jinghuilouyu.cn/gtmyzalwqn.html

C#:   class Admin : User {}
来源：http://hz.pycfn.com/gtxbdinklo.html

[G06] 重写方法
来源：http://hz.mhx1999.top/gtbguuqcuf.html

Py:   def greet(self): return "admin"
来源：http://hz.chenzaomai.com/gtxdzjanof.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jinyuanbaomall.cn/gtjxbllgbc.html

JS:   greet() { return "admin"; }
来源：http://hz.gzhubu.top/gtmnwyjhfv.html

TS:   greet(): string { return "admin"; }
来源：http://hz.ppjwa.cn/gtzqzqkuoh.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.sweek.top/gthobngvlt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.nwbrower.top/gtsxrnvbva.html

Ruby: def greet; "admin"; end
来源：http://hz.meibo888.top/gtpwapsvxf.html

C#:   public override string Greet() => "admin";
来源：http://hz.nanxuanxn.top/gtvsuaqzav.html

[G07] 调用父类方法
来源：http://hz.xuetiantiany.cn/gtupkwczpg.html

Py:   super().greet()
来源：http://hz.zhiwuduotai.top/gtyghoahxj.html

PHP:  parent::greet();
来源：http://hz.ppjwa.cn/gtmoshducd.html

JS:   super.greet();
来源：http://hz.zhixingplan.top/gtjqakuybk.html

TS:   super.greet();
来源：http://hz.kuanghao11.cn/gtifjrvovo.html

Java: super.greet();
来源：http://hz.yuanzhike.top/gttvmeyzvv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.shzxlz.cn/gtylptspau.html

Ruby: super
来源：http://hz.shangyingyoupin.top/gtgiyxmagn.html

C#:   base.Greet();
来源：http://hz.zhixingplan.top/gthfilyuft.html

[G08] 静态方法与属性
来源：http://hz.cashguo.top/gtxbjwhmdx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.sxryk.cn/gttuofiizo.html

PHP:  public static function f() {}
来源：http://hz.redwolf501.top/gtxefyblok.html

JS:   static f() {}
来源：http://hz.zhiwuduotai.top/gtqzgsygwv.html

TS:   static f(): void {}
来源：http://hz.nanxuanxn.top/gtgkiwgbxh.html

Java: static void f() {}
来源：http://hz.zhoulong.xyz/gtnwoxiuaw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jinghuilouyu.cn/gttfppbzto.html

Ruby: def self.f; end
来源：http://hz.ydzc1.top/gtjpvjbmeg.html

C#:   public static void F() {}
来源：http://hz.sxryk.cn/gtdjxbxhot.html

[G09] 接口 / 抽象类
来源：http://hz.ydjk.org.cn/gtnouuyoyg.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zhoulong.xyz/gtjgjdkirh.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.fzhhl.top/gtvvbtdspz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yj202588.top/gtkeioiwjr.html

TS:   interface Shape { area(): number; }
来源：http://hz.jyoumei.cn/gttxmiibql.html

Java: interface Shape { double area(); }
来源：http://hz.yj20258.top/gtbldurtaf.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.52xcode.cn/gtkgdqsren.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jianghu66.top/gtguwwzpxk.html

C#:   interface IShape { double Area(); }
来源：http://hz.9152youxi.cn/gtyxabctnv.html

[G10] 访问控制
来源：http://hz.gaohongyu789.top/gtichivzbl.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.0kj1m.cn/gtgpqutfto.html

PHP:  public / protected / private
来源：http://hz.dashuyun.cn/gttpokzvzp.html

JS:   #private 字段；其余公开
来源：http://hz.316326.xyz/gtxbsrxkvj.html

TS:   public / protected / private
来源：http://hz.daria6918.cn/gtxxgmkepc.html

Java: public / protected / private / 默认包级
来源：http://hz.yj202588.top/gtlfbtsxer.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.wangshuangyany.cn/gtpzpzcjtq.html

Ruby: public / protected / private
来源：http://hz.yvedp.cn/gtvinyuwjz.html

C#:   public / protected / private / internal
来源：http://hz.ivvv.top/gtrgowwmks.html

[G11] getter / setter
来源：http://hz.yj20258.top/gtoktaiowr.html

Py:   @property 与 @x.setter
来源：http://hz.hysaishi.cn/gtsqoctyhr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.kuanghao11.cn/gtyytleyof.html

JS:   get name() { return this._name; }
来源：http://hz.jinyuanbaomall.cn/gtvnxwxmwo.html

TS:   get name(): string { return this._name; }
来源：http://hz.guowangkeji.top/gtfxerdvmh.html

Java: public String getName() { return name; }
来源：http://hz.yj20258.top/gtvenmgiau.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.gaohongyu789.top/gtzaoxtaxp.html

Ruby: attr_accessor :name
来源：http://hz.shzxlz.cn/gtixxrbzri.html

C#:   public string Name { get; set; }
来源：http://hz.meibo888.top/gtjtwxdipe.html

[G12] 对象转字符串
来源：http://hz.fengsongda.top/gtqtyxetln.html

Py:   def __str__(self): return self.name
来源：http://hz.cucudq.cn/gtclzwanfh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yonumen.top/gttoucwskd.html

JS:   toString() { return this.name; }
来源：http://hz.jinghuilouyu.cn/gtsprnarnj.html

TS:   toString(): string { return this.name; }
来源：http://hz.yj20258.top/gthbcktrcc.html

Java: @Override public String toString() { return name; }
来源：http://hz.hysaishi.cn/gtmyzxhboc.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.c1oappe.top/gtoocxsols.html

Ruby: def to_s; @name; end
来源：http://hz.dianchejie.cn/gtijiypfyr.html

C#:   public override string ToString() => Name;
来源：http://hz.nwbrower.top/gtbzeyashx.html

[G13] 判断对象类型
来源：http://hz.zhongyouzk.top/gtblohdfwx.html

Py:   isinstance(u, User)
来源：http://hz.yj20258.top/gtzntqhkfm.html

PHP:  $u instanceof User
来源：http://hz.hnqzz.top/gtzbwqpaad.html

JS:   u instanceof User
来源：http://hz.tanke756.top/gtjlrxxcaq.html

TS:   u instanceof User
来源：http://hz.yangfankeji.com/gtqkhgmuon.html

Java: u instanceof User
来源：http://hz.ivvv.top/gtmahloxrl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yj20258888.top/gtygybslvk.html

Ruby: u.is_a?(User)
来源：http://hz.zycfv.cn/gtukebgtpn.html

C#:   u is User
来源：http://hz.guowangkeji.top/gtfuhmdpil.html

[G14] 数据类 / record
来源：http://hz.snrcjt.cn/gtfncqudpg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.fzhhl.top/gthxbwhgwz.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.hongshengwenyu.top/gtyqadggmu.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jinqigufen.top/gtwezditbl.html

TS:   type User = { name: string; age: number };
来源：http://hz.c1oappe.top/gtmvofnwfa.html

Java: record User(String name, int age) {}
来源：http://hz.guannengcc.top/gtibdxcthz.html

Go:   type User struct { Name string; Age int }
来源：http://hz.iojbl.cn/gtnxhkqsrk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.sweek.top/gtsarnedlh.html

C#:   record User(string Name, int Age);
来源：http://hz.shuidangran.top/gtlznfeauv.html

[G15] 枚举
来源：http://hz.jinghuilouyu.cn/gtjgzbicfd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jinqigufen.top/gtdzqejhcr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.xuanzx.com/gteqxrjwuq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hongshengwenyu.top/gtgnsllvat.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jianghu66.top/gtvpfhjhue.html

Java: enum Color { RED, GREEN }
来源：http://hz.zhengqikj.top/gtomjkjxyr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.shuidangran.top/gteahvacel.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jiagoushi.top/gtvvdmafhx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.nanxinkj.top/gtdlwaldjx.html

[G16] 对象转数组 / 字典
来源：http://hz.shuidangran.top/gtzjlenpkj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.shanyushiyangtech.top/gtnczmihms.html

PHP:  get_object_vars($obj);
来源：http://hz.zdqjudy.top/gtqtxzwrif.html

JS:   Object.entries(obj)
来源：http://hz.hammf.cn/gtshnlqcaf.html

TS:   Object.entries(obj)
来源：http://hz.zhiwuduotai.top/gtfagrpbhv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.nwbrower.top/gtznupqjlf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.cucudq.cn/gtlqaauicu.html

Ruby: obj.instance_variables
来源：http://hz.yanxiufei.cn/gtolxvkini.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.ydzc1.top/gtutkzsssl.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtwqqtforz.html

H. 异常与错误处理
来源：http://hz.zhaomingkeji.xyz/gthncnkoar.html

================================================================================
来源：http://hz.zhoulong.xyz/gttfbuyufu.html

[H01] try / catch 基础
来源：http://hz.gotoacloud.top/gtwiuxelqa.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.ehwqpu.com/gtcpclzmtr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.kuanghao11.cn/gtjbfsozil.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.sufxvd.cn/gtcrpfpiol.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.tian-w.cn/gtucfpgewh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jqgufenzy.top/gtntmnnrhk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jiagoushi.top/gtokiwgjji.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ehwqpu.com/gtxyqhduoh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.nwbrower.top/gtzrcwuhrc.html

[H02] finally / ensure 收尾
来源：http://hz.hnqzz.top/gtovajlfqy.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.sysykeji.top/gtxtpiebja.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.andypj.xyz/gtwbhqojha.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.fengsongda.top/gtnyirfvxq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.sxryk.cn/gtoqmxaald.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.sysykeji.top/gtvwxmrqep.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.cucudq.cn/gtpifwtpdb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.sysykeji.top/gtlbgjibcu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yueranfly.top/gtkjhbjxmq.html

[H03] 主动抛出异常
来源：http://hz.ehwqpu.com/gtvbgsdmaz.html

Py:   raise ValueError("错误信息")
来源：http://hz.yueranfly.top/gtxagmtalb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.meibo888.top/gtidnhcuxu.html

JS:   throw new Error("错误信息");
来源：http://hz.wangshuangyany.cn/gtoahwkmov.html

TS:   throw new Error("错误信息");
来源：http://hz.yonumen.top/gtonmwclvu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.cashguo.top/gtbdjulckx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.gaohongyu789.top/gtrzqyngmb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.0kj1m.cn/gtjxpebnbe.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.ydjk.org.cn/gtizeqbuzz.html

[H04] 自定义异常类型
来源：http://hz.vqdsnc.cn/gtycedwbdt.html

Py:   class MyError(Exception): pass
来源：http://hz.gogol.net.cn/gtuuidnqjk.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.cheryme.top/gtnskkxbmj.html

JS:   class MyError extends Error {}
来源：http://hz.sysykeji.top/gtullsgpmb.html

TS:   class MyError extends Error {}
来源：http://hz.aizwys.cn/gtmvwlqtoo.html

Java: class MyException extends RuntimeException {}
来源：http://hz.aibaodan.cn/gtnglrprpj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zhongyouzk.top/gtqejbvyhr.html

Ruby: class MyError < StandardError; end
来源：http://hz.hongshengwenyu.top/gtpbdvkoqj.html

C#:   class MyException : Exception {}
来源：http://hz.sweek.top/gtgtkcjmpl.html

[H05] 捕获特定类型
来源：http://hz.gogol.net.cn/gtypahhdaf.html

Py:   except ValueError as e:
来源：http://hz.redwolf501.top/gttqkykbvn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhijiandao.cn/gthmvedeyu.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.cqqwz.cn/gtcmczesxs.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yvedp.cn/gtbqctjuvn.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zycfv.cn/gtlpvewjzq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.shzxlz.cn/gtwxdvdkau.html

Ruby: rescue ArgumentError => e
来源：http://hz.pengpengdd.cyou/gthidakgml.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.quarkkingdee.top/gtnupncuhq.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zhongyouzk.top/gtngiaeznn.html

Py:   value = d.get("k") or default
来源：http://hz.quarkkingdee.top/gtqlvwneha.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.guannengcc.top/gtrpmssldu.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jqgufenzy.top/gtqhtwytxi.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jianghu66.top/gtibtvulhn.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.vqdsnc.cn/gtrppileds.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.cqqwz.cn/gtcryfpwvs.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhoulong.xyz/gtjiehhoru.html

C#:   obj?.A?.B ?? default
来源：http://hz.xingfuxueyuan.xyz/gtrxiobjgj.html

[H07] 断言
来源：http://hz.ivvv.top/gtyjixhbky.html

Py:   assert x > 0, "必须为正"
来源：http://hz.chenzaomai.com/gtvwbceseb.html

PHP:  assert($x > 0);
来源：http://hz.aizwys.cn/gtlinqrbdf.html

JS:   console.assert(x > 0);
来源：http://hz.jinyuanbaomall.cn/gtxoewlfkg.html

TS:   console.assert(x > 0);
来源：http://hz.redwolf501.top/gtmojiwyhh.html

Java: assert x > 0 : "必须为正";
来源：http://hz.daxiang520.top/gtuofzmwid.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.c1oappe.top/gtiuuqwijw.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.ehwqpu.com/gtoyowhdez.html

C#:   Debug.Assert(x > 0);
来源：http://hz.ydzc1.top/gteygmnxgv.html

[H08] 获取错误信息与堆栈
来源：http://hz.zhiwuduotai.top/gtjieznuwe.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.wangshuangyany.cn/gtzwpnpvpf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yj20258.top/gtuyfjpbrx.html

JS:   e.message;  e.stack
来源：http://hz.pycfn.com/gtoxvovwjn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.fzhhl.top/gtgjkihtrv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.smart0.xyz/gtfybyorsl.html

Go:   err.Error()
来源：http://hz.yueranfly.top/gtppmmeucl.html

Ruby: e.message;  e.backtrace
来源：http://hz.zhongyouzk.top/gtxlwfszii.html

C#:   e.Message;  e.StackTrace
来源：http://hz.tian-w.cn/gtpqgqmgss.html

[H09] 带错误码的异常
来源：http://hz.ybcxt.top/gtcjkuyxss.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.sweek.top/gtkimgbwox.html


<!-- 参考信息 -->