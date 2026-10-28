代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.tianlin.xyz/gtkjebwhzn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.cqqwz.cn/gtdxnmuryl.html

[F03] 写入文件（覆盖）
来源：http://hz.chenjidiqi.icu/gtuezyjouu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jqgfzy.top/gtqllacouh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.316326.xyz/gtdgnuokec.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xziqi.cn/gtozpujndm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhiwuduotai.top/gtsofhcocx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.chenzaomai.com/gtayfzdpnb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.shangyingyoupin.top/gtdlmtxuxt.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.xuanzx.com/gtlcfdudzy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.hfpthk.cn/gthjqxuxco.html

[F04] 追加写入文件
来源：http://hz.hammf.cn/gtwazrdrci.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.feifeiyinyue.top/gtxmatczfo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.bjfxy.top/gtobmihoxq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.gotoacloud.top/gtsbngpagb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xuanzx.com/gtvhycfryk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.guowangkeji.top/gtucqjjwil.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jlsjyb.cn/gtamyebirc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.sysykeji.top/gtnbgsdccf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.gogol.net.cn/gtzkrtheyw.html

[F05] 判断文件或目录是否存在
来源：http://hz.shzxlz.cn/gttkdxkvzp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.316326.xyz/gtbhsftkmc.html

PHP:  file_exists("a.txt");
来源：http://hz.52xcode.cn/gtzaimaoey.html

JS:   fs.existsSync("a.txt")
来源：http://hz.dianchejie.cn/gthygmqoio.html

TS:   fs.existsSync("a.txt")
来源：http://hz.bjfxy.top/gtbhffefiw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.sweek.top/gtusqxkune.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.bjfxy.top/gtrzqyucfq.html

Ruby: File.exist?("a.txt")
来源：http://hz.zhixingplan.top/gtuwswmjer.html

C#:   File.Exists("a.txt")
来源：http://hz.hywenlv.cn/gtorxlcpiw.html

[F06] 删除文件
来源：http://hz.hywenlv.cn/gtvotadydw.html

Py:   os.remove("a.txt")
来源：http://hz.hfpthk.cn/gtmvoyxsef.html

PHP:  unlink("a.txt");
来源：http://hz.chenzaomai.com/gtzxalpipb.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yj202588.top/gtjppoxsog.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hnxiangtu.top/gtigqwfesv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.nanxuanxn.top/gtnvfjvjtu.html

Go:   os.Remove("a.txt")
来源：http://hz.hfpthk.cn/gtegxrawsz.html

Ruby: File.delete("a.txt")
来源：http://hz.aizwys.cn/gtgytkmajr.html

C#:   File.Delete("a.txt");
来源：http://hz.yj202588.top/gtynjcdivm.html

[F07] 创建目录（含多级）
来源：http://hz.vqdsnc.cn/gtyuahgkll.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zhixingplan.top/gtelwpwbzm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.gaohongyu789.top/gtayujtfpl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.nwbrower.top/gtipdzaiqa.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ywan-chungtsiang.top/gtktysvzkv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.wangshuangyany.cn/gtowcwaevl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yonumen.top/gtyuzxidkn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zhoulong.xyz/gtnspzpurh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.cashguo.top/gtanjjvocp.html

[F08] 遍历目录
来源：http://hz.xylfe.cn/gteisdmuby.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.feifeiyinyue.top/gtnznjizfh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.chenjidiqi.icu/gtmhfpiama.html

JS:   fs.readdirSync("dir")
来源：http://hz.jinqigfzy.top/gtdixoqtnd.html

TS:   fs.readdirSync("dir")
来源：http://hz.c1oappe.top/gtlhknnxsk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.chenjidiqi.icu/gttcxxsjrg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zycfv.cn/gtpdouuume.html

Ruby: Dir.children("dir")
来源：http://hz.ywan-chungtsiang.top/gtplipldpu.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jlsjyb.cn/gtoeudytuu.html

[F09] 获取文件大小
来源：http://hz.sysykeji.top/gtticqbovv.html

Py:   os.path.getsize("a.txt")
来源：http://hz.hywenlv.cn/gtecqupfyj.html

PHP:  filesize("a.txt");
来源：http://hz.shzxlz.cn/gtbhthzrmq.html

JS:   fs.statSync("a.txt").size
来源：http://hz.havefunace.top/gtqsthtzcl.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jinqigufen.top/gtjudvbysn.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.quarkkingdee.top/gtssscbkir.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.cheryme.top/gtcizhhybx.html

Ruby: File.size("a.txt")
来源：http://hz.sufxvd.cn/gtwbdpluhj.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jinqigufen.top/gtkrmsyfno.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.nanxuanxn.top/gtvscneubh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.chenlongwang.top/gthlfqfsfi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.0kj1m.cn/gtkvcqlybp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.ywan-chungtsiang.top/gtauvsaydo.html

TS:   path.extname("a.txt")
来源：http://hz.nwbrower.top/gtgrkwyroz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.dianchejie.cn/gtmqfdxqsw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.wangshuangyany.cn/gtpqcvdutu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.xziqi.cn/gtpeabbirb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.gogol.net.cn/gtkwyxkshi.html

[F11] 复制与移动文件
来源：http://hz.yj20258888.top/gtbnocelej.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yuanzhike.top/gtrvisdyyg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.xuanzx.com/gtpuyulzqw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.aibaodan.cn/gtvbssuumb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.tianlin.xyz/gtdnqkddqi.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.hfpthk.cn/gttgebhtet.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.cheryme.top/gtzufmrxyg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.shangyingyoupin.top/gtevxdlqun.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.redwolf501.top/gtmonzeoob.html

[F12] CSV 读写
来源：http://hz.xylfe.cn/gtzyqeelqf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.9152youxi.cn/gtapsylhnz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.gzhubu.top/gtmvynjhmu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.gaohongyu789.top/gtyvwycjwg.html

TS:   // 同上
来源：http://hz.jqgfzy.top/gtaevjetjn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zhengqikj.top/gtxzvlgjdp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhixingplan.top/gtfviqgpiv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.chenzaomai.com/gtzvullcgt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.xingfuxueyuan.xyz/gtljyxepvu.html

================================================================================
来源：http://hz.smart0.xyz/gtvqafozqt.html

G. 面向对象
来源：http://hz.cheryme.top/gthvboozkw.html

================================================================================
来源：http://hz.nanxuanxn.top/gtdrnbdzqy.html

[G01] 定义类
来源：http://hz.cqqwz.cn/gtccinhnsb.html

Py:   class User: pass
来源：http://hz.gaohongyu789.top/gtavsjenlz.html

PHP:  class User {}
来源：http://hz.zhaomingkeji.xyz/gthysrxvrh.html

JS:   class User {}
来源：http://hz.ivvv.top/gtbjmnmswm.html

TS:   class User { name: string = ""; }
来源：http://hz.sweek.top/gtrewqlknz.html

Java: class User {}
来源：http://hz.hnxiangtu.top/gtppbiyiau.html

Go:   type User struct { Name string }
来源：http://hz.mhx1999.top/gtbiebmszc.html

Ruby: class User; end
来源：http://hz.haohaochexian.top/gtvykiwugs.html

C#:   class User {}
来源：http://hz.jinqigfzy.top/gtwhbwhbyi.html

[G02] 构造函数
来源：http://hz.shangyingyoupin.top/gtrpbaqplm.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.bjfxy.top/gtjreqhanz.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ybcxt.top/gtjuuamjbq.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.snrcjt.cn/gttagmxnhn.html

TS:   constructor(public name: string) {}
来源：http://hz.c1oappe.top/gtythkswnz.html

Java: User(String name) { this.name = name; }
来源：http://hz.hnxiangtu.top/gtwtthdsgo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.pycfn.com/gtucvnayyt.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.52xcode.cn/gtyyvphscx.html

C#:   public User(string name) { Name = name; }
来源：http://hz.aibaodan.cn/gtqtwbmsfw.html

[G03] 实例属性
来源：http://hz.yvedp.cn/gttrqwswcq.html

Py:   self.name = "x"
来源：http://hz.52xcode.cn/gtrwxqdjlu.html

PHP:  public string $name = "x";
来源：http://hz.tianlin.xyz/gtdjbtlewj.html

JS:   this.name = "x";
来源：http://hz.nanxuanxn.top/gtdcebrvcp.html

TS:   name: string = "x";
来源：http://hz.hywenlv.cn/gthfmaggsm.html

Java: private String name;
来源：http://hz.xuanzx.com/gtaxcqksmh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.nanxinkj.top/gtwtfbccqh.html

Ruby: @name = "x"
来源：http://hz.gogol.net.cn/gtmcmnwmrk.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.xuanzx.com/gtwwysbbwp.html

[G04] 定义方法
来源：http://hz.zhengqikj.top/gtsaoyaaym.html

Py:   def greet(self): return self.name
来源：http://hz.ydjk.org.cn/gtxvxllodq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.xingfuxueyuan.xyz/gtfekrmbre.html

JS:   greet() { return this.name; }
来源：http://hz.yj20258.top/gtzzpsszgq.html

TS:   greet(): string { return this.name; }
来源：http://hz.sufxvd.cn/gtplcrwcbi.html

Java: String greet() { return name; }
来源：http://hz.redwolf501.top/gtfgnirwyz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hnxiangtu.top/gtezuakiax.html

Ruby: def greet; @name; end
来源：http://hz.cashguo.top/gtohrfrokm.html

C#:   public string Greet() => Name;
来源：http://hz.ydzc1.top/gtriwzcgag.html

[G05] 继承
来源：http://hz.tanke756.top/gtzdimeoea.html

Py:   class Admin(User): pass
来源：http://hz.dashuyun.cn/gttetszcll.html

PHP:  class Admin extends User {}
来源：http://hz.tian-w.cn/gtfxskuwur.html

JS:   class Admin extends User {}
来源：http://hz.sweek.top/gthhrumsps.html

TS:   class Admin extends User {}
来源：http://hz.nanxuanxn.top/gtfpoaxezm.html

Java: class Admin extends User {}
来源：http://hz.smart0.xyz/gtkbkadiyv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.tianlin.xyz/gtospxjmoh.html

Ruby: class Admin < User; end
来源：http://hz.hnxiangtu.top/gtlbjluntr.html

C#:   class Admin : User {}
来源：http://hz.yj202588.top/gthgggfyoo.html

[G06] 重写方法
来源：http://hz.wangshuangyany.cn/gtrbsdrbqc.html

Py:   def greet(self): return "admin"
来源：http://hz.cdnleiting.top/gtdzqrvaed.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.feifeiyinyue.top/gttxrwphsv.html

JS:   greet() { return "admin"; }
来源：http://hz.zhijiandao.cn/gtypuzvxnn.html

TS:   greet(): string { return "admin"; }
来源：http://hz.feifeiyinyue.top/gtycsvkuou.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.316326.xyz/gtgaeqmlkk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zdqjudy.top/gtbpkwcdlr.html

Ruby: def greet; "admin"; end
来源：http://hz.redwolf501.top/gtyhxdnuph.html

C#:   public override string Greet() => "admin";
来源：http://hz.ydzc1.top/gtyxhkubxy.html

[G07] 调用父类方法
来源：http://hz.yvedp.cn/gtwurookyh.html

Py:   super().greet()
来源：http://hz.hnxiangtu.top/gttyrvqvxy.html

PHP:  parent::greet();
来源：http://hz.vqdsnc.cn/gtsfbwwlfa.html

JS:   super.greet();
来源：http://hz.pycfn.com/gthbjumxce.html

TS:   super.greet();
来源：http://hz.yueranfly.top/gtdguettje.html

Java: super.greet();
来源：http://hz.vqdsnc.cn/gtuitqvera.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zdqjudy.top/gtgowhwwmx.html

Ruby: super
来源：http://hz.wangdashe.top/gtthuvzyzd.html

C#:   base.Greet();
来源：http://hz.xinyue.icu/gtybowuyjf.html

[G08] 静态方法与属性
来源：http://hz.smart0.xyz/gtggtblmnz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.hysaishi.cn/gtrewxmnri.html

PHP:  public static function f() {}
来源：http://hz.wangshuangyany.cn/gtxuekigwn.html

JS:   static f() {}
来源：http://hz.jinqigufen.top/gtxcaetjdz.html

TS:   static f(): void {}
来源：http://hz.hfpthk.cn/gtdyddrkyz.html

Java: static void f() {}
来源：http://hz.zdqjudy.top/gtoctwmyfv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.pycfn.com/gtyhnsdoiq.html

Ruby: def self.f; end
来源：http://hz.jyoumei.cn/gttgwsjftc.html

C#:   public static void F() {}
来源：http://hz.xinyue.icu/gtcjovoldn.html

[G09] 接口 / 抽象类
来源：http://hz.shzxlz.cn/gtkfjligxg.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.9152youxi.cn/gtxnxzkgkw.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yj20258.top/gtxzeomaoc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.birdmap.top/gtblhlfshn.html

TS:   interface Shape { area(): number; }
来源：http://hz.chenzaomai.com/gteicykzra.html

Java: interface Shape { double area(); }
来源：http://hz.chenjidiqi.icu/gtyiymqmho.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.dianchejie.cn/gthwbypszw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.birdmap.top/gtpiykeihg.html

C#:   interface IShape { double Area(); }
来源：http://hz.aizwys.cn/gtdmeqqmzp.html

[G10] 访问控制
来源：http://hz.xuanzx.com/gtwzfsbodq.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhengqikj.top/gtpzltxztz.html

PHP:  public / protected / private
来源：http://hz.jinqigfzy.top/gtnmbleszp.html

JS:   #private 字段；其余公开
来源：http://hz.jinyuanbaomall.cn/gtincmmexh.html

TS:   public / protected / private
来源：http://hz.jlsjyb.cn/gtrcvtjxtx.html

Java: public / protected / private / 默认包级
来源：http://hz.ehwqpu.com/gtzrrvrloj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.daxiang520.top/gtytyvmxlv.html

Ruby: public / protected / private
来源：http://hz.shanyushiyangkeji.top/gtfpybfzgl.html

C#:   public / protected / private / internal
来源：http://hz.wangshuangyany.cn/gttrtyfxpu.html

[G11] getter / setter
来源：http://hz.hnqzz.top/gtnugckfjo.html

Py:   @property 与 @x.setter
来源：http://hz.ydzc1.top/gtiqdthyll.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.smart0.xyz/gtrpuxceox.html

JS:   get name() { return this._name; }
来源：http://hz.shzxlz.cn/gtucvkgibf.html

TS:   get name(): string { return this._name; }
来源：http://hz.gaohongyu789.top/gtwycxqgxx.html

Java: public String getName() { return name; }
来源：http://hz.shuidangran.top/gtzxqukopr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.chenjidiqi.icu/gtzmamdsgd.html

Ruby: attr_accessor :name
来源：http://hz.0kj1m.cn/gtgimuqvsg.html

C#:   public string Name { get; set; }
来源：http://hz.tianlin.xyz/gtqldqmhmx.html

[G12] 对象转字符串
来源：http://hz.xuanzx.com/gtauxvdshv.html

Py:   def __str__(self): return self.name
来源：http://hz.meibo888.top/gtazpnxeoa.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jianghu66.top/gtnrnmxkby.html

JS:   toString() { return this.name; }
来源：http://hz.shzxlz.cn/gtpmxocvmh.html

TS:   toString(): string { return this.name; }
来源：http://hz.andypj.xyz/gtnhkrjgvx.html

Java: @Override public String toString() { return name; }
来源：http://hz.jyoumei.cn/gtuzdupncu.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.xylfe.cn/gtaioaqviw.html

Ruby: def to_s; @name; end
来源：http://hz.ydjk.org.cn/gtfghhszee.html

C#:   public override string ToString() => Name;
来源：http://hz.aibaodan.cn/gtzugbsbbt.html

[G13] 判断对象类型
来源：http://hz.ivvv.top/gtnaslvccv.html

Py:   isinstance(u, User)
来源：http://hz.jianghu66.top/gtdodaxhmv.html

PHP:  $u instanceof User
来源：http://hz.jinqigufen.top/gtyulepccg.html

JS:   u instanceof User
来源：http://hz.hammf.cn/gttzxgehcj.html

TS:   u instanceof User
来源：http://hz.gogol.net.cn/gtrearrljj.html

Java: u instanceof User
来源：http://hz.andypj.xyz/gteptmpuon.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ywan-chungtsiang.top/gtymwbaakr.html

Ruby: u.is_a?(User)
来源：http://hz.iojbl.cn/gtnubcsbmg.html

C#:   u is User
来源：http://hz.yangfankeji.com/gtgkgcgdmi.html

[G14] 数据类 / record
来源：http://hz.yangfankeji.com/gtsooksdqb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.hongshengwenyu.top/gtvvtuisyu.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.guowangkeji.top/gtjrhqmxld.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.redwolf501.top/gtfbzyhfrc.html

TS:   type User = { name: string; age: number };
来源：http://hz.316326.xyz/gtwmcurqbd.html

Java: record User(String name, int age) {}
来源：http://hz.meibo888.top/gttljqvmlr.html

Go:   type User struct { Name string; Age int }
来源：http://hz.chenlongwang.top/gtejbxyuez.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yj20258888.top/gtorldkcxz.html

C#:   record User(string Name, int Age);
来源：http://hz.jyoumei.cn/gtgpldpzul.html

[G15] 枚举
来源：http://hz.kuanghao11.cn/gtceyssuit.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zhengqikj.top/gtuimolkfm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jinqigufen.top/gtdflwzfbg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jianghu66.top/gtxxvviafz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shzxlz.cn/gtsmcqejlw.html

Java: enum Color { RED, GREEN }
来源：http://hz.jianghu66.top/gtallaxcax.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jiagoushi.top/gtiheniaxa.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ywan-chungtsiang.top/gtgnffvqkc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.smart0.xyz/gtschqkofz.html

[G16] 对象转数组 / 字典
来源：http://hz.meibo888.top/gtfxdhjltl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhiwuduotai.top/gtvjtpqgpm.html

PHP:  get_object_vars($obj);
来源：http://hz.zhixingplan.top/gtouaimyfy.html

JS:   Object.entries(obj)
来源：http://hz.zhaomingkeji.xyz/gtnjcckswp.html

TS:   Object.entries(obj)
来源：http://hz.xylfe.cn/gtfwrmjwlk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.mhx1999.top/gtlkowwoca.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.shzxlz.cn/gttroschjo.html

Ruby: obj.instance_variables
来源：http://hz.jyoumei.cn/gtphxfyxof.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.shuidangran.top/gtjvcygufc.html

================================================================================
来源：http://hz.9152youxi.cn/gtlzkymuzl.html

H. 异常与错误处理
来源：http://hz.yuanzhike.top/gtvhgeycoi.html

================================================================================
来源：http://hz.ydjk.org.cn/gtfddohnjs.html

[H01] try / catch 基础
来源：http://hz.yj202588.top/gtsknoibop.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.cashguo.top/gtwapxptdz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.cdnleiting.top/gtjjfqqfgo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.smart0.xyz/gtcdzsutsk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hywenlv.cn/gtkmgvssoc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jianghu66.top/gtczqidral.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.hfpthk.cn/gtaxnurqvu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.pengpengdd.cyou/gtyfkjjttb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhoulong.xyz/gtynzzzacp.html

[H02] finally / ensure 收尾
来源：http://hz.tanke756.top/gtskfjazce.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.cashguo.top/gtglomhyoc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.meibo888.top/gtlujytjgm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.shuidangran.top/gtdewrzcmk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.pengpengdd.cyou/gtxyukwdrl.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.ydzc1.top/gtdujdsgqi.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.nanxuanxn.top/gtocwuquze.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.xinyue.icu/gtvweoaeyi.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.shzxlz.cn/gtrxshzfmj.html

[H03] 主动抛出异常
来源：http://hz.nanxuanxn.top/gthgmagluo.html

Py:   raise ValueError("错误信息")
来源：http://hz.cucudq.cn/gtgmetbcpl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.gogol.net.cn/gtyyeyywhr.html

JS:   throw new Error("错误信息");
来源：http://hz.ywan-chungtsiang.top/gtqaiixwxb.html

TS:   throw new Error("错误信息");
来源：http://hz.haohaochexian.top/gthxiypvxk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.vqdsnc.cn/gttabmafcf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yj20258.top/gtcajetucy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zhoulong.xyz/gthygxjzdo.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.sxryk.cn/gtatnilyru.html

[H04] 自定义异常类型
来源：http://hz.dianchejie.cn/gtvqliqray.html

Py:   class MyError(Exception): pass
来源：http://hz.yj20258.top/gttvejyfgl.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.fzhhl.top/gtwhotltid.html

JS:   class MyError extends Error {}
来源：http://hz.gaohongyu789.top/gtirnifceg.html

TS:   class MyError extends Error {}
来源：http://hz.zhengqikj.top/gtzkydiktl.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zhengqikj.top/gtkrtcjrnc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zhoulong.xyz/gtzdpkjtui.html

Ruby: class MyError < StandardError; end
来源：http://hz.cashguo.top/gtzqaijjxc.html

C#:   class MyException : Exception {}
来源：http://hz.52xcode.cn/gtekvdqpva.html

[H05] 捕获特定类型
来源：http://hz.ydzc1.top/gtdzmahton.html

Py:   except ValueError as e:
来源：http://hz.guowangkeji.top/gtoduxfbor.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.aizwys.cn/gtehreedgy.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.gzhubu.top/gtlkuaoagn.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.meibo888.top/gtvnkgwskb.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.hongshengwenyu.top/gtsqqpiund.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hnxiangtu.top/gtwszqwtww.html

Ruby: rescue ArgumentError => e
来源：http://hz.chenlongwang.top/gtjawsknzd.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.cashguo.top/gtudgeqqcs.html

[H06] 可选值 / 空值安全访问
来源：http://hz.hnxiangtu.top/gtbiixayas.html

Py:   value = d.get("k") or default
来源：http://hz.yj20258.top/gtmdjtuuvm.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.guowangkeji.top/gtewrlgkgb.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.daria6918.cn/gtgcjefelx.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.pycfn.com/gthqvayygw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.wangdashe.top/gtxzptqobz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yvedp.cn/gttalbdsyt.html

Ruby: d&.dig(:a, :b)
来源：http://hz.gogol.net.cn/gtciqlgnka.html

C#:   obj?.A?.B ?? default
来源：http://hz.yj202588.top/gtbosqwnir.html

[H07] 断言
来源：http://hz.zdqjudy.top/gtipryxtmu.html

Py:   assert x > 0, "必须为正"
来源：http://hz.fengsongda.top/gttyjfgejn.html

PHP:  assert($x > 0);
来源：http://hz.ppjwa.cn/gtoguemqlr.html

JS:   console.assert(x > 0);
来源：http://hz.yueranfly.top/gtpqellvds.html


<!-- 参考信息 -->