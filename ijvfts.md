代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zhongyouzk.top/gtwnklzemp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.0kj1m.cn/gtsgslzmyx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yj20258.top/gttlmrxvjb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.nanxinkj.top/gtcvnktjbo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.sweek.top/gtpvufgbve.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.cucudq.cn/gtbmcnejpm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.tianlin.xyz/gtyxxrfvkp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.xinyue.icu/gtjgmmhcxs.html

[F05] 判断文件或目录是否存在
来源：http://hz.shangyingyoupin.top/gtsnhzcnbs.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.dianchejie.cn/gtyjbybhcp.html

PHP:  file_exists("a.txt");
来源：http://hz.zycfv.cn/gtrsfdyoxg.html

JS:   fs.existsSync("a.txt")
来源：http://hz.dianchejie.cn/gtahwjcunx.html

TS:   fs.existsSync("a.txt")
来源：http://hz.c1oappe.top/gtyxkycnjo.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.0kj1m.cn/gtmehuvplj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.52xcode.cn/gtjsukbzgt.html

Ruby: File.exist?("a.txt")
来源：http://hz.shangyingyoupin.top/gteyuekwuy.html

C#:   File.Exists("a.txt")
来源：http://hz.havefunace.top/gttcdzcdme.html

[F06] 删除文件
来源：http://hz.hongshengwenyu.top/gtndxhrgyv.html

Py:   os.remove("a.txt")
来源：http://hz.316326.xyz/gtwpdcxqyr.html

PHP:  unlink("a.txt");
来源：http://hz.cucudq.cn/gtguinmabc.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.shuidangran.top/gttvkgscvb.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.shanyushiyangkeji.top/gterjilnwx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.ehwqpu.com/gtwrdtyoqx.html

Go:   os.Remove("a.txt")
来源：http://hz.andypj.xyz/gthjskgdwa.html

Ruby: File.delete("a.txt")
来源：http://hz.xziqi.cn/gtzxbpkcuz.html

C#:   File.Delete("a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtotkmphmu.html

[F07] 创建目录（含多级）
来源：http://hz.svipenyu.cn/gtlmprkpfz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zdqjudy.top/gtklfelkbz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.guowangkeji.top/gtdqhawsfa.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.haohaochexian.top/gtknwkznwu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.chenzaomai.com/gtkhhqtacg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.zhoulong.xyz/gtxcutwces.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yj20258.top/gthmxpbcxs.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.shangyingyoupin.top/gtteuydmbq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.xinyue.icu/gtzmwkwgsm.html

[F08] 遍历目录
来源：http://hz.quarkkingdee.top/gtpplfclgy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.pengpengdd.cyou/gttvyeuikf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.sweek.top/gtpzsftucz.html

JS:   fs.readdirSync("dir")
来源：http://hz.jinghuilouyu.cn/gtgnfvdjks.html

TS:   fs.readdirSync("dir")
来源：http://hz.xylfe.cn/gtplnignuc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yj202588.top/gthpywqelj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.dashuyun.cn/gtjznuvvkv.html

Ruby: Dir.children("dir")
来源：http://hz.52xcode.cn/gtfrumtapu.html

C#:   Directory.GetFiles("dir")
来源：http://hz.hfpthk.cn/gtfaeyercz.html

[F09] 获取文件大小
来源：http://hz.gaohongyu789.top/gtfczzjbya.html

Py:   os.path.getsize("a.txt")
来源：http://hz.xinyue.icu/gtjfdgmwfn.html

PHP:  filesize("a.txt");
来源：http://hz.aibaodan.cn/gtugvcbvkx.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yuanzhike.top/gttsxfrdqe.html

TS:   fs.statSync("a.txt").size
来源：http://hz.gzhubu.top/gtpaqaefkr.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.svipenyu.cn/gtcwlmsfis.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hongshengwenyu.top/gtbdrlprne.html

Ruby: File.size("a.txt")
来源：http://hz.zdqjudy.top/gtabimiroo.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.quarkkingdee.top/gtkircdoyz.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hywenlv.cn/gtlfdmngvu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.tanke756.top/gtrcqxuacr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.haohaochexian.top/gtdssfwlmd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jinqigfzy.top/gtgdlngutt.html

TS:   path.extname("a.txt")
来源：http://hz.andypj.xyz/gtvkgbmtcl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.fzhhl.top/gtbcnhmjiu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zhaomingkeji.xyz/gtbyosmszi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.shuidangran.top/gtyajnlier.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.pycfn.com/gtmedzfkbd.html

[F11] 复制与移动文件
来源：http://hz.smart0.xyz/gtqrnkqmha.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.sysykeji.top/gturbteukz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.xziqi.cn/gtnlaiqbvf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.pycfn.com/gtijbinppj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xziqi.cn/gtnkjpcmcp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.gaohongyu789.top/gtlgzzpmmv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.sufxvd.cn/gtinaupmdx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zhijiandao.cn/gtmxvetdho.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.pycfn.com/gtkqfmwqzp.html

[F12] CSV 读写
来源：http://hz.pycfn.com/gtmrukupiu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.hongshengwenyu.top/gtwdxsdllq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.guowangkeji.top/gtteqcomeg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.xziqi.cn/gtvcluewnu.html

TS:   // 同上
来源：http://hz.smart0.xyz/gtengiheij.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.xziqi.cn/gtfbqzwoyv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.xziqi.cn/gttpdybbaj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.316326.xyz/gtfqmsgnac.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.aibaodan.cn/gtmxguokdu.html

================================================================================
来源：http://hz.hfpthk.cn/gtrggrjadf.html

G. 面向对象
来源：http://hz.fengsongda.top/gtxcflvhmf.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtfjtsryhl.html

[G01] 定义类
来源：http://hz.tian-w.cn/gtfbqhwitb.html

Py:   class User: pass
来源：http://hz.wangshuangyany.cn/gtvburlpan.html

PHP:  class User {}
来源：http://hz.meibo888.top/gtedickcdu.html

JS:   class User {}
来源：http://hz.yuxming.cn/gtdovgcwnp.html

TS:   class User { name: string = ""; }
来源：http://hz.wangdashe.top/gtnmjfylbm.html

Java: class User {}
来源：http://hz.snrcjt.cn/gthdvfrmke.html

Go:   type User struct { Name string }
来源：http://hz.aibaodan.cn/gtwprchbgl.html

Ruby: class User; end
来源：http://hz.wangshuangyany.cn/gtbrjevhms.html

C#:   class User {}
来源：http://hz.zhoulong.xyz/gteexcgzao.html

[G02] 构造函数
来源：http://hz.c1oappe.top/gtgrevoftz.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jinghuilouyu.cn/gtlzwsqkbr.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.52xcode.cn/gtkdcxpdpg.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yangfankeji.com/gtzjgmenzs.html

TS:   constructor(public name: string) {}
来源：http://hz.snrcjt.cn/gtnrndgsvj.html

Java: User(String name) { this.name = name; }
来源：http://hz.ehwqpu.com/gtwrmmxawi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hammf.cn/gtqyitelke.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.zhaomingkeji.xyz/gtkwkynbko.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zhijiandao.cn/gtqakrepvm.html

[G03] 实例属性
来源：http://hz.zhaomingkeji.xyz/gtskrgdohl.html

Py:   self.name = "x"
来源：http://hz.cheryme.top/gtoysbcrzh.html

PHP:  public string $name = "x";
来源：http://hz.svipenyu.cn/gtzdiwjvwo.html

JS:   this.name = "x";
来源：http://hz.cqqwz.cn/gtajvklqme.html

TS:   name: string = "x";
来源：http://hz.xinyue.icu/gtgynbdvoa.html

Java: private String name;
来源：http://hz.hammf.cn/gthxuaryog.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.smart0.xyz/gtlrnmyazg.html

Ruby: @name = "x"
来源：http://hz.gogol.net.cn/gtjcikxgvb.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jinyuanbaomall.cn/gthmnjfoqr.html

[G04] 定义方法
来源：http://hz.pycfn.com/gtiyekhkgu.html

Py:   def greet(self): return self.name
来源：http://hz.snrcjt.cn/gtbdfinyhg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yj20258888.top/gtxwfffalz.html

JS:   greet() { return this.name; }
来源：http://hz.ybcxt.top/gtsvlnbtww.html

TS:   greet(): string { return this.name; }
来源：http://hz.pycfn.com/gtsqdsmbtz.html

Java: String greet() { return name; }
来源：http://hz.dashuyun.cn/gtxwnnjgxf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hnqzz.top/gtxxhlofln.html

Ruby: def greet; @name; end
来源：http://hz.jinqigfzy.top/gtjjcmsoms.html

C#:   public string Greet() => Name;
来源：http://hz.tanke756.top/gtbxuordvk.html

[G05] 继承
来源：http://hz.daxiang520.top/gtpuwdcbez.html

Py:   class Admin(User): pass
来源：http://hz.xziqi.cn/gtgcvxobuu.html

PHP:  class Admin extends User {}
来源：http://hz.cheryme.top/gttukzxdyc.html

JS:   class Admin extends User {}
来源：http://hz.yanxiufei.cn/gtfycwouiu.html

TS:   class Admin extends User {}
来源：http://hz.zhiwuduotai.top/gtxbevnupc.html

Java: class Admin extends User {}
来源：http://hz.yuxming.cn/gtsfsqlytd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.9152youxi.cn/gtqyjepzlb.html

Ruby: class Admin < User; end
来源：http://hz.gzhubu.top/gtggbeazry.html

C#:   class Admin : User {}
来源：http://hz.chenjidiqi.icu/gtqywcwdjz.html

[G06] 重写方法
来源：http://hz.jqgfzy.top/gtgstnqjny.html

Py:   def greet(self): return "admin"
来源：http://hz.mhx1999.top/gtwatjopmg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.guowangkeji.top/gtozvxpsuu.html

JS:   greet() { return "admin"; }
来源：http://hz.yueranfly.top/gtkjmumurg.html

TS:   greet(): string { return "admin"; }
来源：http://hz.316326.xyz/gtiqceynjc.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.tianlin.xyz/gtwtfchqfo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.redwolf501.top/gttvzzixms.html

Ruby: def greet; "admin"; end
来源：http://hz.yonumen.top/gtzdkfmqzg.html

C#:   public override string Greet() => "admin";
来源：http://hz.gogol.net.cn/gtylglfsid.html

[G07] 调用父类方法
来源：http://hz.ydjk.org.cn/gtnalcnyig.html

Py:   super().greet()
来源：http://hz.ydzc1.top/gtpmybeexf.html

PHP:  parent::greet();
来源：http://hz.feifeiyinyue.top/gtqbibyzns.html

JS:   super.greet();
来源：http://hz.xuetiantiany.cn/gttxosxpkz.html

TS:   super.greet();
来源：http://hz.chenlongwang.top/gtlakcvztt.html

Java: super.greet();
来源：http://hz.xuetiantiany.cn/gtehcbywda.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.aibaodan.cn/gtnegadtvv.html

Ruby: super
来源：http://hz.ivvv.top/gthxwvsxnr.html

C#:   base.Greet();
来源：http://hz.guowangkeji.top/gtdietkuli.html

[G08] 静态方法与属性
来源：http://hz.0kj1m.cn/gtxdibtjmn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zycfv.cn/gtfgcgtkth.html

PHP:  public static function f() {}
来源：http://hz.yangfankeji.com/gtxaedpdll.html

JS:   static f() {}
来源：http://hz.zhengqikj.top/gtcumixdgb.html

TS:   static f(): void {}
来源：http://hz.gaohongyu789.top/gtwxsmzvol.html

Java: static void f() {}
来源：http://hz.chenlongwang.top/gtdxphibdl.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.tian-w.cn/gtdscztwuc.html

Ruby: def self.f; end
来源：http://hz.meibo888.top/gthkvbrsmu.html

C#:   public static void F() {}
来源：http://hz.sysykeji.top/gtltbzxsno.html

[G09] 接口 / 抽象类
来源：http://hz.yangfankeji.com/gtbbegccca.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jinqigfzy.top/gtentovoag.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.meibo888.top/gtptiviwvg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yangfankeji.com/gtnlsuteuv.html

TS:   interface Shape { area(): number; }
来源：http://hz.smart0.xyz/gtcppksdji.html

Java: interface Shape { double area(); }
来源：http://hz.shuidangran.top/gtiuirkukf.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.ppjwa.cn/gtvjthdpdx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hysaishi.cn/gtkuwavcrg.html

C#:   interface IShape { double Area(); }
来源：http://hz.wangshuangyany.cn/gtnuqeqszi.html

[G10] 访问控制
来源：http://hz.xziqi.cn/gttqgsnfpw.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.ppjwa.cn/gtoxhuezxp.html

PHP:  public / protected / private
来源：http://hz.hywenlv.cn/gtgajjnsic.html

JS:   #private 字段；其余公开
来源：http://hz.zhengqikj.top/gtxtlrfbzu.html

TS:   public / protected / private
来源：http://hz.hongshengwenyu.top/gtkdnzdnmq.html

Java: public / protected / private / 默认包级
来源：http://hz.gzhubu.top/gtuxelrlcx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.nanxinkj.top/gtzmdvzznx.html

Ruby: public / protected / private
来源：http://hz.bjfxy.top/gtzpynnlqe.html

C#:   public / protected / private / internal
来源：http://hz.daria6918.cn/gtgmmptmal.html

[G11] getter / setter
来源：http://hz.ivvv.top/gtipwimmtg.html

Py:   @property 与 @x.setter
来源：http://hz.meibo888.top/gteahndojm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.52xcode.cn/gtucmwybdn.html

JS:   get name() { return this._name; }
来源：http://hz.zhongyouzk.top/gtaavrkerh.html

TS:   get name(): string { return this._name; }
来源：http://hz.sufxvd.cn/gttppwulxr.html

Java: public String getName() { return name; }
来源：http://hz.jianghu66.top/gtviedaqrd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jinqigufen.top/gtpemaruio.html

Ruby: attr_accessor :name
来源：http://hz.ydjk.org.cn/gttqfkhjrl.html

C#:   public string Name { get; set; }
来源：http://hz.hfpthk.cn/gtmdglcauf.html

[G12] 对象转字符串
来源：http://hz.yueranfly.top/gtzygyklsa.html

Py:   def __str__(self): return self.name
来源：http://hz.yj202588.top/gttebhrrrp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.pycfn.com/gtzazhjppo.html

JS:   toString() { return this.name; }
来源：http://hz.jlsjyb.cn/gtzdxisohk.html

TS:   toString(): string { return this.name; }
来源：http://hz.sweek.top/gtrrnxghvr.html

Java: @Override public String toString() { return name; }
来源：http://hz.gzhubu.top/gtebefhyfh.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.gaohongyu789.top/gtvkigwdji.html

Ruby: def to_s; @name; end
来源：http://hz.yonumen.top/gtfsavfasf.html

C#:   public override string ToString() => Name;
来源：http://hz.nanxinkj.top/gtsnysbtdb.html

[G13] 判断对象类型
来源：http://hz.52xcode.cn/gtifolyxih.html

Py:   isinstance(u, User)
来源：http://hz.yangfankeji.com/gtkjizcydb.html

PHP:  $u instanceof User
来源：http://hz.fzhhl.top/gtnpdihykk.html

JS:   u instanceof User
来源：http://hz.daxiang520.top/gtygwvvuhp.html

TS:   u instanceof User
来源：http://hz.jinqigufen.top/gtyctrwsjc.html

Java: u instanceof User
来源：http://hz.zycfv.cn/gtudtxekab.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.aibaodan.cn/gtdfeascoi.html

Ruby: u.is_a?(User)
来源：http://hz.hfpthk.cn/gtknypeeeo.html

C#:   u is User
来源：http://hz.ydjk.org.cn/gttyqnuahj.html

[G14] 数据类 / record
来源：http://hz.tian-w.cn/gtwuaofmzy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.aizwys.cn/gtzjzzosqm.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.redwolf501.top/gtqtzeusti.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.mhx1999.top/gtodpxqxfk.html

TS:   type User = { name: string; age: number };
来源：http://hz.ydjk.org.cn/gtxqblcjgh.html

Java: record User(String name, int age) {}
来源：http://hz.snrcjt.cn/gtegvcejhq.html

Go:   type User struct { Name string; Age int }
来源：http://hz.hnqzz.top/gtzxphcupr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.hnxiangtu.top/gtzjfdefnv.html

C#:   record User(string Name, int Age);
来源：http://hz.xuanzx.com/gtrgwggyxs.html

[G15] 枚举
来源：http://hz.chenlongwang.top/gtzzzkbpio.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.bjfxy.top/gtaviqvkhg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yanxiufei.cn/gtvtjkdtof.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zhijiandao.cn/gtwougejzn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sweek.top/gtndsdkshh.html

Java: enum Color { RED, GREEN }
来源：http://hz.hammf.cn/gtuchjxcxa.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.chenjidiqi.icu/gtnaefzuqq.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jinqigufen.top/gtpjnermcw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sufxvd.cn/gtbfemnojk.html

[G16] 对象转数组 / 字典
来源：http://hz.xylfe.cn/gtlxigdeyj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.cdnleiting.top/gtlknbjnys.html

PHP:  get_object_vars($obj);
来源：http://hz.bjfxy.top/gtitecoobm.html

JS:   Object.entries(obj)
来源：http://hz.meibo888.top/gtxtoiacuc.html

TS:   Object.entries(obj)
来源：http://hz.yonumen.top/gtxamcuchb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.iojbl.cn/gtjjlowuqx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.aibaodan.cn/gtzzldyqib.html

Ruby: obj.instance_variables
来源：http://hz.jlsjyb.cn/gttcvlzqfo.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jqgufenzy.top/gtfdtnhjia.html

================================================================================
来源：http://hz.hnqzz.top/gtfbbfvtoo.html

H. 异常与错误处理
来源：http://hz.shuidangran.top/gtpyliykun.html

================================================================================
来源：http://hz.chenzaomai.com/gtgalnlamb.html

[H01] try / catch 基础
来源：http://hz.jinqigufen.top/gtfdfxmext.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.aizwys.cn/gtkdiufdgu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.shanyushiyangkeji.top/gtqghjjtkk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yongpay.top/gttoazmunm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jiagoushi.top/gtsoosizos.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.birdmap.top/gtpecvjgjp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.quarkkingdee.top/gtwwmazeah.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.nwbrower.top/gtjctvdanz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhijiandao.cn/gtpsefokko.html

[H02] finally / ensure 收尾
来源：http://hz.ehwqpu.com/gtijrukaeh.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.0kj1m.cn/gtpqnccrpr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangtech.top/gthuvxuweq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhengqikj.top/gtwvurabya.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.xingfuxueyuan.xyz/gtzmssbbhs.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.havefunace.top/gtddxdfqtj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jinghuilouyu.cn/gtatpkbftx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yuanzhike.top/gtopbqxvwe.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.ydjk.org.cn/gthneqqgre.html

[H03] 主动抛出异常
来源：http://hz.zhaomingkeji.xyz/gtinqovwjf.html

Py:   raise ValueError("错误信息")
来源：http://hz.yongpay.top/gtiyncwihc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.0kj1m.cn/gtrpqzqefn.html

JS:   throw new Error("错误信息");
来源：http://hz.shanyushiyangtech.top/gtylopveej.html

TS:   throw new Error("错误信息");
来源：http://hz.zdqjudy.top/gtyhujrekn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jinghuilouyu.cn/gtengycnel.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.smart0.xyz/gtqtrngehh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.chenjidiqi.icu/gtvipswpwm.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.shanyushiyangkeji.top/gtszlhbucg.html

[H04] 自定义异常类型
来源：http://hz.tian-w.cn/gtotroolyu.html

Py:   class MyError(Exception): pass
来源：http://hz.wangshuangyany.cn/gtfnquipzh.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hywenlv.cn/gtqjdbnrba.html

JS:   class MyError extends Error {}
来源：http://hz.ehwqpu.com/gtifvlpnkm.html

TS:   class MyError extends Error {}
来源：http://hz.nanxinkj.top/gtznsgxxfo.html

Java: class MyException extends RuntimeException {}
来源：http://hz.gogol.net.cn/gtwcifmtor.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.cdnleiting.top/gtwdpvgryv.html

Ruby: class MyError < StandardError; end
来源：http://hz.nwbrower.top/gthzdmefim.html

C#:   class MyException : Exception {}
来源：http://hz.jianghu66.top/gtkkkorypd.html

[H05] 捕获特定类型
来源：http://hz.hywenlv.cn/gtxcfisryf.html

Py:   except ValueError as e:
来源：http://hz.aibaodan.cn/gtqbylythg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yongpay.top/gtzhadepvr.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.sufxvd.cn/gtyopyipsy.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.tian-w.cn/gtfdzbfjui.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.xziqi.cn/gtezrqtgam.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.c1oappe.top/gtisnzccbl.html

Ruby: rescue ArgumentError => e
来源：http://hz.zhijiandao.cn/gtzatqrpkp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yj202588.top/gtxunuspjt.html

[H06] 可选值 / 空值安全访问
来源：http://hz.kuanghao11.cn/gtnrkiqceo.html

Py:   value = d.get("k") or default
来源：http://hz.shzxlz.cn/gtlyolrvgh.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.ivvv.top/gtopupelki.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jinyuanbaomall.cn/gtyqrnndhj.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.cdnleiting.top/gtlcthcfbk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhaomingkeji.xyz/gtlwqlewwq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yuxming.cn/gttjrtxvse.html

Ruby: d&.dig(:a, :b)
来源：http://hz.ivvv.top/gtnsruxoel.html

C#:   obj?.A?.B ?? default
来源：http://hz.cheryme.top/gtyrduukns.html

[H07] 断言
来源：http://hz.jlsjyb.cn/gtwqfkfzos.html

Py:   assert x > 0, "必须为正"
来源：http://hz.xingfuxueyuan.xyz/gtzeebzycb.html

PHP:  assert($x > 0);
来源：http://hz.shangyingyoupin.top/gtdrfcmcxz.html

JS:   console.assert(x > 0);
来源：http://hz.birdmap.top/gtsarkrdch.html

TS:   console.assert(x > 0);
来源：http://hz.shangyingyoupin.top/gtqrhaylae.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yueranfly.top/gtcadndisg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.dashuyun.cn/gtmdpszxmu.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.sufxvd.cn/gtupttwhmr.html

C#:   Debug.Assert(x > 0);
来源：http://hz.snrcjt.cn/gtuyutbosa.html

[H08] 获取错误信息与堆栈
来源：http://hz.nwbrower.top/gtlpcqmjlb.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.nanxuanxn.top/gtknijpycr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.ywan-chungtsiang.top/gttqzxlkjg.html

JS:   e.message;  e.stack
来源：http://hz.yangfankeji.com/gtnhgfdekl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.ywan-chungtsiang.top/gthzgbxcrq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zycfv.cn/gtqyxsnsze.html

Go:   err.Error()
来源：http://hz.yanxiufei.cn/gttghhuukh.html


<!-- 参考信息 -->