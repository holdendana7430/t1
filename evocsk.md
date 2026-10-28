代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.mhx1999.top/gtycfyptjp.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yangfankeji.com/gtrmhamicd.html

[F03] 写入文件（覆盖）
来源：http://hz.aizwys.cn/gtuksndwmx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.chenjidiqi.icu/gtyzzqrimk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.0kj1m.cn/gtgglywxir.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.guannengcc.top/gtlbwcjkis.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yuxming.cn/gtrcjleczz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.52xcode.cn/gtcnjffttk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.shanyushiyangkeji.top/gtsgmmmgzt.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.pengpengdd.cyou/gtdjvqjitf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.daxiang520.top/gtzppuvgiy.html

[F04] 追加写入文件
来源：http://hz.316326.xyz/gtgfrdxyua.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.aizwys.cn/gtlvscxccb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.tian-w.cn/gtcbdslvzd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.svipenyu.cn/gtqxfnadzc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.mhx1999.top/gtcjgvgqrs.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jinqigufen.top/gtqdwxjloh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.ybcxt.top/gtuavglqmf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.snrcjt.cn/gtqxrhxtaz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yueranfly.top/gtbfjpsaub.html

[F05] 判断文件或目录是否存在
来源：http://hz.dianchejie.cn/gtpzlnfhtz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.shanyushiyangtech.top/gtvesfmyfb.html

PHP:  file_exists("a.txt");
来源：http://hz.dianchejie.cn/gtwilbusdq.html

JS:   fs.existsSync("a.txt")
来源：http://hz.zhoulong.xyz/gtlhncvgyf.html

TS:   fs.existsSync("a.txt")
来源：http://hz.dashuyun.cn/gtjgekmpie.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.gogol.net.cn/gtgicribft.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.gzhubu.top/gtzuctvklr.html

Ruby: File.exist?("a.txt")
来源：http://hz.hysaishi.cn/gtgxjojevo.html

C#:   File.Exists("a.txt")
来源：http://hz.chenzaomai.com/gtnasyyhrc.html

[F06] 删除文件
来源：http://hz.bjfxy.top/gtupfnpkth.html

Py:   os.remove("a.txt")
来源：http://hz.gaohongyu789.top/gtkjfgmyxa.html

PHP:  unlink("a.txt");
来源：http://hz.jianghu66.top/gtqalyksnd.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtkltmvlrw.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.sweek.top/gttiixpgtv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.c1oappe.top/gtldvexerc.html

Go:   os.Remove("a.txt")
来源：http://hz.zhengqikj.top/gthtvlgexs.html

Ruby: File.delete("a.txt")
来源：http://hz.sweek.top/gtevkrivaq.html

C#:   File.Delete("a.txt");
来源：http://hz.yanxiufei.cn/gttauwyhfp.html

[F07] 创建目录（含多级）
来源：http://hz.wangdashe.top/gtdbgiehql.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.bjfxy.top/gtvnhmyeln.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.sysykeji.top/gthockyzba.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.smart0.xyz/gttvtzkuza.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.aibaodan.cn/gtncberiwv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yongpay.top/gtzallepkd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.vqdsnc.cn/gtybjrrpvp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.quarkkingdee.top/gtqjcojgll.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.tian-w.cn/gtravlryol.html

[F08] 遍历目录
来源：http://hz.meibo888.top/gtnnkqhqsi.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.hysaishi.cn/gtjuhsdznf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.birdmap.top/gthwgpaicm.html

JS:   fs.readdirSync("dir")
来源：http://hz.aizwys.cn/gtavifptcu.html

TS:   fs.readdirSync("dir")
来源：http://hz.chenjidiqi.icu/gtegdoklnl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.cqqwz.cn/gtdjxkffgm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yuanzhike.top/gtbagidkie.html

Ruby: Dir.children("dir")
来源：http://hz.yongpay.top/gteevxdwtl.html

C#:   Directory.GetFiles("dir")
来源：http://hz.shanyushiyangkeji.top/gtwuwjcxbo.html

[F09] 获取文件大小
来源：http://hz.316326.xyz/gtcmvcpvmq.html

Py:   os.path.getsize("a.txt")
来源：http://hz.gogol.net.cn/gtclruiivv.html

PHP:  filesize("a.txt");
来源：http://hz.shuidangran.top/gtuhttqvht.html

JS:   fs.statSync("a.txt").size
来源：http://hz.xingfuxueyuan.xyz/gtgjebtuyh.html

TS:   fs.statSync("a.txt").size
来源：http://hz.xingfuxueyuan.xyz/gtlgnopwfw.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.sysykeji.top/gtaokeizgv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.52xcode.cn/gtqdzxtlag.html

Ruby: File.size("a.txt")
来源：http://hz.birdmap.top/gtacxwwmng.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.52xcode.cn/gtaaewtxyu.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hysaishi.cn/gtpneprukz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.pengpengdd.cyou/gtdiwrmsyz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.nwbrower.top/gthluierxc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.quarkkingdee.top/gtmwvoknxt.html

TS:   path.extname("a.txt")
来源：http://hz.yonumen.top/gtszpmarym.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.xuanzx.com/gtdutzkvcm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.vqdsnc.cn/gtxtjlvzud.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.ybcxt.top/gtqvjyxpte.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.hongshengwenyu.top/gtfccfenel.html

[F11] 复制与移动文件
来源：http://hz.ppjwa.cn/gtkhockcmz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.ydjk.org.cn/gtdawpacpz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.hywenlv.cn/gtijhcjwzn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shuidangran.top/gtdbzrhbvn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zdqjudy.top/gtaoftrkut.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.0kj1m.cn/gtlhzuugbu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.snrcjt.cn/gttctnxzyn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jiagoushi.top/gtivllnigb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.cheryme.top/gtheqflhrs.html

[F12] CSV 读写
来源：http://hz.gotoacloud.top/gtswuadgfv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.nwbrower.top/gtveyifltk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.guowangkeji.top/gtvezffekq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zhiwuduotai.top/gtnwuftznd.html

TS:   // 同上
来源：http://hz.sxryk.cn/gthyqsyumj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.pycfn.com/gtdhcsvvek.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.meibo888.top/gtwtzmgwej.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.gzhubu.top/gtkexbomxa.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.chenjidiqi.icu/gtngrzfjrl.html

================================================================================
来源：http://hz.gaohongyu789.top/gtuppyusjk.html

G. 面向对象
来源：http://hz.fzhhl.top/gtfrrvwayk.html

================================================================================
来源：http://hz.shuidangran.top/gtizalyewy.html

[G01] 定义类
来源：http://hz.andypj.xyz/gthbkcvwhx.html

Py:   class User: pass
来源：http://hz.cdnleiting.top/gtsdmecyta.html

PHP:  class User {}
来源：http://hz.gaohongyu789.top/gtmgxsuryv.html

JS:   class User {}
来源：http://hz.mhx1999.top/gtqwcagjcj.html

TS:   class User { name: string = ""; }
来源：http://hz.xuanzx.com/gtihwgojrx.html

Java: class User {}
来源：http://hz.dashuyun.cn/gtpbbsxosv.html

Go:   type User struct { Name string }
来源：http://hz.ybcxt.top/gtmbillted.html

Ruby: class User; end
来源：http://hz.smart0.xyz/gtyntwnibd.html

C#:   class User {}
来源：http://hz.sufxvd.cn/gtupgfqsvt.html

[G02] 构造函数
来源：http://hz.bjfxy.top/gtncjyymvm.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.sysykeji.top/gtxpjoflkl.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hnxiangtu.top/gtobaawida.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.ppjwa.cn/gtegrgfnhq.html

TS:   constructor(public name: string) {}
来源：http://hz.gotoacloud.top/gtothnqqgj.html

Java: User(String name) { this.name = name; }
来源：http://hz.cheryme.top/gtpkactwcx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.ppjwa.cn/gtjaydqhjb.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.svipenyu.cn/gtdbjgppgz.html

C#:   public User(string name) { Name = name; }
来源：http://hz.cdnleiting.top/gtjrpzwklt.html

[G03] 实例属性
来源：http://hz.yangfankeji.com/gtduetrxth.html

Py:   self.name = "x"
来源：http://hz.birdmap.top/gtkzyjxuis.html

PHP:  public string $name = "x";
来源：http://hz.hongshengwenyu.top/gtufjcefhx.html

JS:   this.name = "x";
来源：http://hz.tanke756.top/gtrfyzoufp.html

TS:   name: string = "x";
来源：http://hz.ybcxt.top/gtylmkttxz.html

Java: private String name;
来源：http://hz.daxiang520.top/gtauokextu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.wangshuangyany.cn/gtbabpcoyb.html

Ruby: @name = "x"
来源：http://hz.xinyue.icu/gtsslbdbes.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.guowangkeji.top/gtyzgobjhf.html

[G04] 定义方法
来源：http://hz.9152youxi.cn/gttyucxpby.html

Py:   def greet(self): return self.name
来源：http://hz.jqgfzy.top/gtrfgizqao.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.ivvv.top/gttmqjowfa.html

JS:   greet() { return this.name; }
来源：http://hz.aizwys.cn/gtbgxoixwx.html

TS:   greet(): string { return this.name; }
来源：http://hz.ydzc1.top/gtxehcmxvs.html

Java: String greet() { return name; }
来源：http://hz.xziqi.cn/gtvmrlstky.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.cdnleiting.top/gtiwbcfgkl.html

Ruby: def greet; @name; end
来源：http://hz.yangfankeji.com/gtzvldtzbf.html

C#:   public string Greet() => Name;
来源：http://hz.yangfankeji.com/gtomsfkmfi.html

[G05] 继承
来源：http://hz.ydjk.org.cn/gtmnvzhmog.html

Py:   class Admin(User): pass
来源：http://hz.iojbl.cn/gtnxjsiwyl.html

PHP:  class Admin extends User {}
来源：http://hz.chenlongwang.top/gtfwilvdws.html

JS:   class Admin extends User {}
来源：http://hz.xuetiantiany.cn/gtlluqtgca.html

TS:   class Admin extends User {}
来源：http://hz.bjfxy.top/gtfvhgxnpx.html

Java: class Admin extends User {}
来源：http://hz.aibaodan.cn/gtmpuozcqm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yuanzhike.top/gtoclszaeo.html

Ruby: class Admin < User; end
来源：http://hz.guannengcc.top/gtbiiauqeb.html

C#:   class Admin : User {}
来源：http://hz.xylfe.cn/gtktmsjauv.html

[G06] 重写方法
来源：http://hz.yj20258.top/gtmwjaxijx.html

Py:   def greet(self): return "admin"
来源：http://hz.guowangkeji.top/gtqhbzrnvx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.52xcode.cn/gtbuoylpti.html

JS:   greet() { return "admin"; }
来源：http://hz.gaohongyu789.top/gtvjjvuewc.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hnxiangtu.top/gteyxgluhb.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.tanke756.top/gtookabhez.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.chenjidiqi.icu/gtksjjzqba.html

Ruby: def greet; "admin"; end
来源：http://hz.daxiang520.top/gtrwbaornl.html

C#:   public override string Greet() => "admin";
来源：http://hz.ivvv.top/gtkqyghewe.html

[G07] 调用父类方法
来源：http://hz.mhx1999.top/gtkpmzdoei.html

Py:   super().greet()
来源：http://hz.shzxlz.cn/gtyvknhdaj.html

PHP:  parent::greet();
来源：http://hz.hnxiangtu.top/gtcjczzkca.html

JS:   super.greet();
来源：http://hz.jyoumei.cn/gtttqypjwz.html

TS:   super.greet();
来源：http://hz.zhijiandao.cn/gtpezlbcma.html

Java: super.greet();
来源：http://hz.xinyue.icu/gtnnfgjsxg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.tian-w.cn/gtpnqqswfi.html

Ruby: super
来源：http://hz.c1oappe.top/gtmctoiqtf.html

C#:   base.Greet();
来源：http://hz.zhixingplan.top/gtljexmblv.html

[G08] 静态方法与属性
来源：http://hz.hnqzz.top/gtnzmdwnxa.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.sweek.top/gtpdgtaoni.html

PHP:  public static function f() {}
来源：http://hz.cqqwz.cn/gtbbbdocza.html

JS:   static f() {}
来源：http://hz.svipenyu.cn/gtykpsgmjn.html

TS:   static f(): void {}
来源：http://hz.sysykeji.top/gtchzwgduq.html

Java: static void f() {}
来源：http://hz.xuanzx.com/gtizvtdadz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.shanyushiyangtech.top/gtbluwepsk.html

Ruby: def self.f; end
来源：http://hz.xingfuxueyuan.xyz/gttruygnuc.html

C#:   public static void F() {}
来源：http://hz.xuanzx.com/gtjriogosn.html

[G09] 接口 / 抽象类
来源：http://hz.zhijiandao.cn/gtrjvttytd.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.snrcjt.cn/gtukxusxyz.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.hywenlv.cn/gtpzktwmsy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.pycfn.com/gtxaywnayv.html

TS:   interface Shape { area(): number; }
来源：http://hz.gaohongyu789.top/gtwjvdhpkh.html

Java: interface Shape { double area(); }
来源：http://hz.chenlongwang.top/gtfwduamdh.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yuanzhike.top/gtvmpjdtda.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.ivvv.top/gtvdxkqmzs.html

C#:   interface IShape { double Area(); }
来源：http://hz.wangshuangyany.cn/gtfmjoujjy.html

[G10] 访问控制
来源：http://hz.hnqzz.top/gtcambpvjd.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yueranfly.top/gtpanrizzl.html

PHP:  public / protected / private
来源：http://hz.chenzaomai.com/gttfvngsiu.html

JS:   #private 字段；其余公开
来源：http://hz.dianchejie.cn/gtpahlozsc.html

TS:   public / protected / private
来源：http://hz.dashuyun.cn/gtvrqbusdx.html

Java: public / protected / private / 默认包级
来源：http://hz.dianchejie.cn/gtjwfebdog.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.hongshengwenyu.top/gtmlyzpxri.html

Ruby: public / protected / private
来源：http://hz.nanxinkj.top/gtpzijwskl.html

C#:   public / protected / private / internal
来源：http://hz.nanxinkj.top/gtfnsxoobx.html

[G11] getter / setter
来源：http://hz.mhx1999.top/gtlgjmmtvv.html

Py:   @property 与 @x.setter
来源：http://hz.andypj.xyz/gtaburblax.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.svipenyu.cn/gtlqlfzzwn.html

JS:   get name() { return this._name; }
来源：http://hz.cheryme.top/gtybktbepv.html

TS:   get name(): string { return this._name; }
来源：http://hz.haohaochexian.top/gtwvalymnk.html

Java: public String getName() { return name; }
来源：http://hz.svipenyu.cn/gtbgcdnnze.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.havefunace.top/gtcznuilms.html

Ruby: attr_accessor :name
来源：http://hz.yueranfly.top/gtjodlatqi.html

C#:   public string Name { get; set; }
来源：http://hz.yanxiufei.cn/gtrdhuhlwa.html

[G12] 对象转字符串
来源：http://hz.nanxinkj.top/gtxfylianm.html

Py:   def __str__(self): return self.name
来源：http://hz.redwolf501.top/gtovxrwtab.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.wangdashe.top/gtoanhghjk.html

JS:   toString() { return this.name; }
来源：http://hz.zhijiandao.cn/gtqnoqjbpz.html

TS:   toString(): string { return this.name; }
来源：http://hz.ywan-chungtsiang.top/gtsobvooyi.html

Java: @Override public String toString() { return name; }
来源：http://hz.gotoacloud.top/gtvreyeatq.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yonumen.top/gtfjkcgehl.html

Ruby: def to_s; @name; end
来源：http://hz.ppjwa.cn/gtoihcbajd.html

C#:   public override string ToString() => Name;
来源：http://hz.hfpthk.cn/gtdjdbxary.html

[G13] 判断对象类型
来源：http://hz.yj20258.top/gtfnkzxcct.html

Py:   isinstance(u, User)
来源：http://hz.cheryme.top/gtmhdzrraa.html

PHP:  $u instanceof User
来源：http://hz.jqgfzy.top/gttblsgoub.html

JS:   u instanceof User
来源：http://hz.fzhhl.top/gtadzgzzoe.html

TS:   u instanceof User
来源：http://hz.jinqigfzy.top/gtbqcyuucu.html

Java: u instanceof User
来源：http://hz.aibaodan.cn/gttwmrjpfi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.tian-w.cn/gtuwidteve.html

Ruby: u.is_a?(User)
来源：http://hz.jinqigfzy.top/gtjqhmosfb.html

C#:   u is User
来源：http://hz.ybcxt.top/gtmzjczinm.html

[G14] 数据类 / record
来源：http://hz.ydjk.org.cn/gtwuqyqtqn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.fengsongda.top/gtrdinduhg.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.52xcode.cn/gtqbrpwdhm.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jianghu66.top/gteuvonvdh.html

TS:   type User = { name: string; age: number };
来源：http://hz.xuanzx.com/gtrnwnoopc.html

Java: record User(String name, int age) {}
来源：http://hz.sufxvd.cn/gtemjzfail.html

Go:   type User struct { Name string; Age int }
来源：http://hz.aibaodan.cn/gtccuvmpjf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.shzxlz.cn/gtgshgnayp.html

C#:   record User(string Name, int Age);
来源：http://hz.jinghuilouyu.cn/gtknccathy.html

[G15] 枚举
来源：http://hz.zhijiandao.cn/gttaplveey.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zhoulong.xyz/gtgysfdmtj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.xziqi.cn/gtoxptcoje.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.ywan-chungtsiang.top/gtifkydcjm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.9152youxi.cn/gtryndjyft.html

Java: enum Color { RED, GREEN }
来源：http://hz.nanxinkj.top/gtlegmvcha.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.9152youxi.cn/gtjeivaxbl.html

Ruby: Color = %i[red green].freeze
来源：http://hz.fzhhl.top/gtryqerato.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.tanke756.top/gtumoukxhx.html

[G16] 对象转数组 / 字典
来源：http://hz.ybcxt.top/gtdyutkril.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhengqikj.top/gthhjqeini.html

PHP:  get_object_vars($obj);
来源：http://hz.yueranfly.top/gtaqcezazi.html

JS:   Object.entries(obj)
来源：http://hz.hnxiangtu.top/gtnmiwnphu.html

TS:   Object.entries(obj)
来源：http://hz.zhijiandao.cn/gtqvmypjhw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.guowangkeji.top/gtpxlintmu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hfpthk.cn/gtzzecxtbd.html

Ruby: obj.instance_variables
来源：http://hz.yj202588.top/gtvfjglxnx.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.316326.xyz/gtdfhcquxa.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtppxfycvn.html

H. 异常与错误处理
来源：http://hz.xziqi.cn/gtjybapwsn.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtmsyogdhw.html

[H01] try / catch 基础
来源：http://hz.cucudq.cn/gtepjidhjf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.hnqzz.top/gtgvjptupl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.xuanzx.com/gtkcpibwmm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.xuanzx.com/gtkbuuwxxe.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.shanyushiyangkeji.top/gtwgnkwhou.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.316326.xyz/gtzzpwnflk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.9152youxi.cn/gthjueutpu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.mhx1999.top/gtthgrvloz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zdqjudy.top/gtkldksbwc.html

[H02] finally / ensure 收尾
来源：http://hz.xuetiantiany.cn/gtytbnvdvm.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.cqqwz.cn/gtewyarswr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhengqikj.top/gtbqzltzow.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zycfv.cn/gtielwbjwp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.feifeiyinyue.top/gtbkytzfnp.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.52xcode.cn/gtecioshjl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hnqzz.top/gtfafekgxu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ydjk.org.cn/gtmclvdixh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.fengsongda.top/gtbpvhfljw.html

[H03] 主动抛出异常
来源：http://hz.tian-w.cn/gtfqgibfju.html

Py:   raise ValueError("错误信息")
来源：http://hz.52xcode.cn/gtntpprwyo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.xuetiantiany.cn/gtqfxsdyds.html

JS:   throw new Error("错误信息");
来源：http://hz.feifeiyinyue.top/gtgsromdme.html

TS:   throw new Error("错误信息");
来源：http://hz.nanxinkj.top/gtqvvgrlac.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.fengsongda.top/gtelomuipt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.xuanzx.com/gtvdakjmyt.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.tanke756.top/gtuqofbesc.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.ywan-chungtsiang.top/gtshumbmhf.html

[H04] 自定义异常类型
来源：http://hz.shanyushiyangtech.top/gttgmzjzqj.html

Py:   class MyError(Exception): pass
来源：http://hz.gogol.net.cn/gthvujedip.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zhiwuduotai.top/gtvtbcxlze.html

JS:   class MyError extends Error {}
来源：http://hz.yvedp.cn/gtcyudxcqz.html

TS:   class MyError extends Error {}
来源：http://hz.shanyushiyangtech.top/gtplfrqszf.html

Java: class MyException extends RuntimeException {}
来源：http://hz.havefunace.top/gtepczgbco.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ywan-chungtsiang.top/gtspwnyezi.html

Ruby: class MyError < StandardError; end
来源：http://hz.ydzc1.top/gtgjrnmibm.html

C#:   class MyException : Exception {}
来源：http://hz.shzxlz.cn/gtuqlxsyij.html

[H05] 捕获特定类型
来源：http://hz.hysaishi.cn/gtsdhmjsxj.html

Py:   except ValueError as e:
来源：http://hz.shuidangran.top/gtgocvzrzp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.gogol.net.cn/gtxekqntbh.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.ppjwa.cn/gtqfozsqvv.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yonumen.top/gttjptlmhj.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.9152youxi.cn/gtmfmxbqpw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.xingfuxueyuan.xyz/gtjsqjpjbn.html

Ruby: rescue ArgumentError => e
来源：http://hz.birdmap.top/gtomhraajm.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jinqigufen.top/gtdihgbvee.html

[H06] 可选值 / 空值安全访问
来源：http://hz.shangyingyoupin.top/gtriyntqdw.html

Py:   value = d.get("k") or default
来源：http://hz.redwolf501.top/gtksepycor.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yvedp.cn/gtameznxep.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zhongyouzk.top/gtestvilgb.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.daxiang520.top/gtylbfmdde.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jinqigfzy.top/gtjxsouqmk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.ydzc1.top/gtyzbrkxse.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jlsjyb.cn/gthmotdnpa.html

C#:   obj?.A?.B ?? default
来源：http://hz.shuidangran.top/gtdunclubu.html

[H07] 断言
来源：http://hz.xinyue.icu/gtjagslygi.html

Py:   assert x > 0, "必须为正"
来源：http://hz.316326.xyz/gtlddfllah.html

PHP:  assert($x > 0);
来源：http://hz.jiagoushi.top/gtbnlpskal.html

JS:   console.assert(x > 0);
来源：http://hz.316326.xyz/gtheasxvmj.html


<!-- 参考信息 -->