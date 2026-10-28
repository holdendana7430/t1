代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yonumen.top/gtihzmisys.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhengqikj.top/gtjhkhklkq.html

[F03] 写入文件（覆盖）
来源：http://hz.zhaomingkeji.xyz/gtioxbvmqc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yuxming.cn/gtzrfpyihj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.0kj1m.cn/gtjkflbjjq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.tianlin.xyz/gtopniqlpg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.sufxvd.cn/gtdzfwopxq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.xinyue.icu/gtlcrczsas.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.sysykeji.top/gtrqncbcym.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yj202588.top/gthnivepmy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.cdnleiting.top/gttowfuihe.html

[F04] 追加写入文件
来源：http://hz.cheryme.top/gtijimyvfn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yj20258.top/gtvdhwkxtd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.haohaochexian.top/gtoijnwsjx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.pycfn.com/gtiedvejxf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yj20258.top/gticiwarhi.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.xuanzx.com/gtusvyuwjb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.xingfuxueyuan.xyz/gtmxbdcjxg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.hfpthk.cn/gthiaholnh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.c1oappe.top/gttjxmnvjn.html

[F05] 判断文件或目录是否存在
来源：http://hz.zhongyouzk.top/gtcrphkese.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zhaomingkeji.xyz/gtgmzhyklk.html

PHP:  file_exists("a.txt");
来源：http://hz.ybcxt.top/gtjdsxttbw.html

JS:   fs.existsSync("a.txt")
来源：http://hz.haohaochexian.top/gtzrfyoecm.html

TS:   fs.existsSync("a.txt")
来源：http://hz.sufxvd.cn/gthcoaxwlv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jqgfzy.top/gtfrjojiry.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.xylfe.cn/gtbheopowc.html

Ruby: File.exist?("a.txt")
来源：http://hz.guowangkeji.top/gttqnasynn.html

C#:   File.Exists("a.txt")
来源：http://hz.jiagoushi.top/gtwdlgtlyt.html

[F06] 删除文件
来源：http://hz.zhiwuduotai.top/gtbzleeevo.html

Py:   os.remove("a.txt")
来源：http://hz.xuanzx.com/gtuqczwsal.html

PHP:  unlink("a.txt");
来源：http://hz.hnqzz.top/gtroxuoaog.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.sxryk.cn/gtsjhprapr.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.smart0.xyz/gtzznmhwxv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.shanyushiyangtech.top/gtwvyhtbma.html

Go:   os.Remove("a.txt")
来源：http://hz.nanxinkj.top/gthttedlme.html

Ruby: File.delete("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtzpezalpz.html

C#:   File.Delete("a.txt");
来源：http://hz.xylfe.cn/gtksjxkpjj.html

[F07] 创建目录（含多级）
来源：http://hz.zycfv.cn/gtbbtgimpw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.xuetiantiany.cn/gtvhakexpw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.hammf.cn/gtsoxqyvsz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yj20258888.top/gtkqqdxrzm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ywan-chungtsiang.top/gtoijdfxnm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.xuanzx.com/gttfatpfzq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zhaomingkeji.xyz/gtcszrbjaf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zhongyouzk.top/gtytbugqqi.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.chenjidiqi.icu/gtshdeapgc.html

[F08] 遍历目录
来源：http://hz.ybcxt.top/gttlbeeuqr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.bjfxy.top/gtnpbhpzgs.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yueranfly.top/gtncptbspg.html

JS:   fs.readdirSync("dir")
来源：http://hz.jianghu66.top/gtpvmbnrsz.html

TS:   fs.readdirSync("dir")
来源：http://hz.meibo888.top/gtuwcjhqob.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.xuetiantiany.cn/gtqlcigesx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yongpay.top/gtdqskqhqo.html

Ruby: Dir.children("dir")
来源：http://hz.jiagoushi.top/gtbhjpegfw.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yj20258888.top/gtompuqdgf.html

[F09] 获取文件大小
来源：http://hz.ybcxt.top/gtizoswnub.html

Py:   os.path.getsize("a.txt")
来源：http://hz.nwbrower.top/gtqptqphwn.html

PHP:  filesize("a.txt");
来源：http://hz.jinqigfzy.top/gtrzygseau.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yuanzhike.top/gtxswufzol.html

TS:   fs.statSync("a.txt").size
来源：http://hz.mhx1999.top/gtsduzyotk.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zhaomingkeji.xyz/gtuvpghwud.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.andypj.xyz/gttqbzbunv.html

Ruby: File.size("a.txt")
来源：http://hz.yj20258888.top/gtlmxxfzef.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jinqigfzy.top/gtyfknjdyr.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.fzhhl.top/gtyfmpqygm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jyoumei.cn/gttfmwkxcn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.kuanghao11.cn/gtptaiydgl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yuanzhike.top/gtnjjdvace.html

TS:   path.extname("a.txt")
来源：http://hz.aizwys.cn/gtlfqcmfpr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.hnxiangtu.top/gtulbdcoxp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.gaohongyu789.top/gtxajmjnzq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jiagoushi.top/gtqhyfhxgp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.ydzc1.top/gtucukqwrj.html

[F11] 复制与移动文件
来源：http://hz.yj20258888.top/gtriblokgz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.cqqwz.cn/gtadwjkzca.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.sufxvd.cn/gtbkdxsrfp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jinyuanbaomall.cn/gttsdyznbl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.daria6918.cn/gtjtdrdmiw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.gogol.net.cn/gttcfhxdmw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.shuidangran.top/gtutczgsgr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.0kj1m.cn/gtraiezgng.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ydjk.org.cn/gturlmemoj.html

[F12] CSV 读写
来源：http://hz.haohaochexian.top/gtnelpbxfz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.316326.xyz/gtlvophorl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zhijiandao.cn/gtbwxkdutl.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.redwolf501.top/gttmoucpun.html

TS:   // 同上
来源：http://hz.yj20258888.top/gtlgeecpoi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.meibo888.top/gtsrssyljd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jinghuilouyu.cn/gtgyptzbdr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.havefunace.top/gtvirncpbi.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yuxming.cn/gtpownnkfg.html

================================================================================
来源：http://hz.hysaishi.cn/gtnnljtmbf.html

G. 面向对象
来源：http://hz.shanyushiyangkeji.top/gtzjeamylz.html

================================================================================
来源：http://hz.sxryk.cn/gtfwejkybf.html

[G01] 定义类
来源：http://hz.dianchejie.cn/gtflcnvynd.html

Py:   class User: pass
来源：http://hz.kuanghao11.cn/gtrtsjliyu.html

PHP:  class User {}
来源：http://hz.jianghu66.top/gtqjkntduk.html

JS:   class User {}
来源：http://hz.kuanghao11.cn/gtynuekuwz.html

TS:   class User { name: string = ""; }
来源：http://hz.xinyue.icu/gtsvtgcjew.html

Java: class User {}
来源：http://hz.hnxiangtu.top/gtklegnaeh.html

Go:   type User struct { Name string }
来源：http://hz.hnxiangtu.top/gtohsrqfrj.html

Ruby: class User; end
来源：http://hz.yonumen.top/gtbfdkqfsi.html

C#:   class User {}
来源：http://hz.gzhubu.top/gtjdhmwkje.html

[G02] 构造函数
来源：http://hz.0kj1m.cn/gtnmswxlkp.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.0kj1m.cn/gtikngjoui.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.cdnleiting.top/gtfhywbgie.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yanxiufei.cn/gtkgsveocp.html

TS:   constructor(public name: string) {}
来源：http://hz.hywenlv.cn/gtlquqhdua.html

Java: User(String name) { this.name = name; }
来源：http://hz.yangfankeji.com/gtcuikcrvu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hfpthk.cn/gtuzmhsnlf.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.aibaodan.cn/gtpqnknmod.html

C#:   public User(string name) { Name = name; }
来源：http://hz.gaohongyu789.top/gtqhfyygdz.html

[G03] 实例属性
来源：http://hz.zhoulong.xyz/gtyuycxlsj.html

Py:   self.name = "x"
来源：http://hz.52xcode.cn/gtzvohvfrp.html

PHP:  public string $name = "x";
来源：http://hz.hnxiangtu.top/gtvvpbteov.html

JS:   this.name = "x";
来源：http://hz.mhx1999.top/gtzivngczo.html

TS:   name: string = "x";
来源：http://hz.daria6918.cn/gtwgjqfjxo.html

Java: private String name;
来源：http://hz.vqdsnc.cn/gtrxqmizfq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yj20258888.top/gtaboigdxq.html

Ruby: @name = "x"
来源：http://hz.wangdashe.top/gthjemlrbt.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.mhx1999.top/gtqlppqzps.html

[G04] 定义方法
来源：http://hz.yueranfly.top/gtombpqwql.html

Py:   def greet(self): return self.name
来源：http://hz.redwolf501.top/gtwwlhdhug.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hywenlv.cn/gtefmqmsod.html

JS:   greet() { return this.name; }
来源：http://hz.dashuyun.cn/gtsuwcjiwz.html

TS:   greet(): string { return this.name; }
来源：http://hz.hnqzz.top/gthmmothpf.html

Java: String greet() { return name; }
来源：http://hz.zhijiandao.cn/gttjwbyivo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.gzhubu.top/gtnxzohjuw.html

Ruby: def greet; @name; end
来源：http://hz.jinghuilouyu.cn/gtjhgpiwmk.html

C#:   public string Greet() => Name;
来源：http://hz.ppjwa.cn/gtejfigxvy.html

[G05] 继承
来源：http://hz.gotoacloud.top/gthjmykmdz.html

Py:   class Admin(User): pass
来源：http://hz.zhoulong.xyz/gtqlmakugf.html

PHP:  class Admin extends User {}
来源：http://hz.jinyuanbaomall.cn/gtedpxfyce.html

JS:   class Admin extends User {}
来源：http://hz.jqgufenzy.top/gtgankbldl.html

TS:   class Admin extends User {}
来源：http://hz.yueranfly.top/gtwxfmxzxq.html

Java: class Admin extends User {}
来源：http://hz.shanyushiyangkeji.top/gtyixvhnxy.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hammf.cn/gtazcvarms.html

Ruby: class Admin < User; end
来源：http://hz.zhongyouzk.top/gttxoveekp.html

C#:   class Admin : User {}
来源：http://hz.daria6918.cn/gtkwbkptnb.html

[G06] 重写方法
来源：http://hz.ehwqpu.com/gtsotpckkf.html

Py:   def greet(self): return "admin"
来源：http://hz.xuanzx.com/gtqlrolmeo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.nwbrower.top/gtonqorhii.html

JS:   greet() { return "admin"; }
来源：http://hz.yvedp.cn/gtpmkmcnkz.html

TS:   greet(): string { return "admin"; }
来源：http://hz.shanyushiyangkeji.top/gtoydehvoi.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.guannengcc.top/gtzjxtbmtd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.sweek.top/gtwpozwfxq.html

Ruby: def greet; "admin"; end
来源：http://hz.hammf.cn/gtnlqqawds.html

C#:   public override string Greet() => "admin";
来源：http://hz.sufxvd.cn/gtcyogsboc.html

[G07] 调用父类方法
来源：http://hz.0kj1m.cn/gtoxdeubac.html

Py:   super().greet()
来源：http://hz.sufxvd.cn/gtrmgoffdk.html

PHP:  parent::greet();
来源：http://hz.fzhhl.top/gtjxidtbja.html

JS:   super.greet();
来源：http://hz.mhx1999.top/gtaqdidhtm.html

TS:   super.greet();
来源：http://hz.hnxiangtu.top/gtrkmoagzg.html

Java: super.greet();
来源：http://hz.jyoumei.cn/gtqwjqencl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zhijiandao.cn/gtkfwmhaey.html

Ruby: super
来源：http://hz.jqgfzy.top/gtwlylcver.html

C#:   base.Greet();
来源：http://hz.xylfe.cn/gtkpidbcby.html

[G08] 静态方法与属性
来源：http://hz.zhaomingkeji.xyz/gtfcrjjiuj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.daria6918.cn/gtztowlgqd.html

PHP:  public static function f() {}
来源：http://hz.mhx1999.top/gttbjsblly.html

JS:   static f() {}
来源：http://hz.sysykeji.top/gtxpzoazxk.html

TS:   static f(): void {}
来源：http://hz.yuxming.cn/gtsivdlgcg.html

Java: static void f() {}
来源：http://hz.sweek.top/gtrtbnedje.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.shuidangran.top/gtvafxodft.html

Ruby: def self.f; end
来源：http://hz.meibo888.top/gtxzginezy.html

C#:   public static void F() {}
来源：http://hz.xziqi.cn/gteaqxxnfh.html

[G09] 接口 / 抽象类
来源：http://hz.cashguo.top/gtcobutlte.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.quarkkingdee.top/gtkhlaslac.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ivvv.top/gtxkyxnkos.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.tanke756.top/gttwmjjcdf.html

TS:   interface Shape { area(): number; }
来源：http://hz.316326.xyz/gtdgbyzdwc.html

Java: interface Shape { double area(); }
来源：http://hz.feifeiyinyue.top/gtxkbjoppu.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yueranfly.top/gtmbgdppia.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.xuetiantiany.cn/gtqwcpybdd.html

C#:   interface IShape { double Area(); }
来源：http://hz.feifeiyinyue.top/gtmqyjklhv.html

[G10] 访问控制
来源：http://hz.hnqzz.top/gtdjpioqko.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jinyuanbaomall.cn/gtlkmyycbv.html

PHP:  public / protected / private
来源：http://hz.zhaomingkeji.xyz/gtfuanwlaj.html

JS:   #private 字段；其余公开
来源：http://hz.shuidangran.top/gtjqtahyxs.html

TS:   public / protected / private
来源：http://hz.c1oappe.top/gtgalmfjpi.html

Java: public / protected / private / 默认包级
来源：http://hz.jlsjyb.cn/gtpnjubhmy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.aizwys.cn/gtaiinznmb.html

Ruby: public / protected / private
来源：http://hz.yueranfly.top/gtgdvtfjfh.html

C#:   public / protected / private / internal
来源：http://hz.xuetiantiany.cn/gtlziqsijj.html

[G11] getter / setter
来源：http://hz.cashguo.top/gthastbtma.html

Py:   @property 与 @x.setter
来源：http://hz.chenjidiqi.icu/gtnwtuvugz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.tianlin.xyz/gttbqkfseg.html

JS:   get name() { return this._name; }
来源：http://hz.zhongyouzk.top/gtuyjagmbf.html

TS:   get name(): string { return this._name; }
来源：http://hz.zycfv.cn/gtcfuncjbj.html

Java: public String getName() { return name; }
来源：http://hz.andypj.xyz/gtoximvdbc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.kuanghao11.cn/gtyhltiybs.html

Ruby: attr_accessor :name
来源：http://hz.cashguo.top/gttguhpsvg.html

C#:   public string Name { get; set; }
来源：http://hz.0kj1m.cn/gtbdwujrot.html

[G12] 对象转字符串
来源：http://hz.andypj.xyz/gtazvrpash.html

Py:   def __str__(self): return self.name
来源：http://hz.9152youxi.cn/gtzpopreqv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yonumen.top/gtofkltfnv.html

JS:   toString() { return this.name; }
来源：http://hz.haohaochexian.top/gtrzztksvi.html

TS:   toString(): string { return this.name; }
来源：http://hz.chenlongwang.top/gtjvnploii.html

Java: @Override public String toString() { return name; }
来源：http://hz.sxryk.cn/gtkqdqwvok.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhengqikj.top/gtatxuplkt.html

Ruby: def to_s; @name; end
来源：http://hz.zdqjudy.top/gtpxaqczgv.html

C#:   public override string ToString() => Name;
来源：http://hz.daria6918.cn/gtcgdrawne.html

[G13] 判断对象类型
来源：http://hz.chenzaomai.com/gtypxtysgb.html

Py:   isinstance(u, User)
来源：http://hz.jinqigfzy.top/gtohnbspma.html

PHP:  $u instanceof User
来源：http://hz.sxryk.cn/gteacqoxlh.html

JS:   u instanceof User
来源：http://hz.shanyushiyangtech.top/gtoljmhnsb.html

TS:   u instanceof User
来源：http://hz.9152youxi.cn/gtvwwzuyab.html

Java: u instanceof User
来源：http://hz.jqgfzy.top/gthebgiewg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.aibaodan.cn/gtwrzslbjt.html

Ruby: u.is_a?(User)
来源：http://hz.chenzaomai.com/gtjhxqhigz.html

C#:   u is User
来源：http://hz.hywenlv.cn/gtlggtvgtl.html

[G14] 数据类 / record
来源：http://hz.jianghu66.top/gtxwkrflxh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.chenzaomai.com/gtscznnjzn.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.meibo888.top/gthvjhxwta.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.xylfe.cn/gthwgujfcd.html

TS:   type User = { name: string; age: number };
来源：http://hz.fzhhl.top/gtetxwmkod.html

Java: record User(String name, int age) {}
来源：http://hz.sxryk.cn/gtgrzmpfzh.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jianghu66.top/gtddffxxoq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.hnqzz.top/gtanoskorj.html

C#:   record User(string Name, int Age);
来源：http://hz.tanke756.top/gtbpdokyki.html

[G15] 枚举
来源：http://hz.zhaomingkeji.xyz/gtwrqzicnn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.guowangkeji.top/gthjtzvdbl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.kuanghao11.cn/gthvnnsyyk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zhongyouzk.top/gtmqfyowfx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cdnleiting.top/gtcvdlxjsf.html

Java: enum Color { RED, GREEN }
来源：http://hz.daria6918.cn/gtkiugdywg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ivvv.top/gtxknjyivj.html

Ruby: Color = %i[red green].freeze
来源：http://hz.tian-w.cn/gtywphbvlb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.daxiang520.top/gtplzeaatg.html

[G16] 对象转数组 / 字典
来源：http://hz.jinqigufen.top/gtmrxyzzvn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.316326.xyz/gtbnmebtki.html

PHP:  get_object_vars($obj);
来源：http://hz.jiagoushi.top/gtlhlwppmu.html

JS:   Object.entries(obj)
来源：http://hz.bjfxy.top/gthlbuhjcv.html

TS:   Object.entries(obj)
来源：http://hz.iojbl.cn/gtpcwzjiae.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.aizwys.cn/gtedsytugh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.shangyingyoupin.top/gtkkqrbhqv.html

Ruby: obj.instance_variables
来源：http://hz.sysykeji.top/gtdxwtxbpj.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yvedp.cn/gtlsnacvqa.html

================================================================================
来源：http://hz.jianghu66.top/gtljqhsezt.html

H. 异常与错误处理
来源：http://hz.yj20258.top/gtnswizvdh.html

================================================================================
来源：http://hz.yj202588.top/gtieokeywo.html

[H01] try / catch 基础
来源：http://hz.yj20258.top/gtykqqzkxn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.ydzc1.top/gtpbbshajy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ehwqpu.com/gttetnrfjf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.wangshuangyany.cn/gtmzqumfga.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yanxiufei.cn/gtwrpvoqmf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.cheryme.top/gtovgbqzmp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.shzxlz.cn/gttckmhcez.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.zhiwuduotai.top/gtejjgwxdw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.guowangkeji.top/gtthgnyigf.html

[H02] finally / ensure 收尾
来源：http://hz.andypj.xyz/gtxvzbamdw.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.cashguo.top/gtjqsnizoy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.9152youxi.cn/gtmunmpkqj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.aizwys.cn/gtwwgfhhah.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.guowangkeji.top/gtnbumpdnw.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.feifeiyinyue.top/gtzymqhzri.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hfpthk.cn/gtjyratcbn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.sysykeji.top/gtmomnaiur.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.kuanghao11.cn/gtynzwtams.html

[H03] 主动抛出异常
来源：http://hz.yonumen.top/gtjntmyogw.html

Py:   raise ValueError("错误信息")
来源：http://hz.zhongyouzk.top/gtxljmzonh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zhengqikj.top/gtmhregamp.html

JS:   throw new Error("错误信息");
来源：http://hz.daxiang520.top/gtlgqknatv.html

TS:   throw new Error("错误信息");
来源：http://hz.sweek.top/gtcfediufa.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.guannengcc.top/gtooxbwrae.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.ydjk.org.cn/gtecivlddg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.shuidangran.top/gtcufahaxv.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.ydjk.org.cn/gtqptrwcge.html

[H04] 自定义异常类型
来源：http://hz.sweek.top/gttgyxgreh.html

Py:   class MyError(Exception): pass
来源：http://hz.ivvv.top/gtjhcpwymr.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.wangdashe.top/gtfdqolfew.html

JS:   class MyError extends Error {}
来源：http://hz.sysykeji.top/gtzodtjpyd.html

TS:   class MyError extends Error {}
来源：http://hz.zhixingplan.top/gtxdcjakoe.html

Java: class MyException extends RuntimeException {}
来源：http://hz.tanke756.top/gtsaxidfxy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.hnqzz.top/gtshfeajsn.html

Ruby: class MyError < StandardError; end
来源：http://hz.xuanzx.com/gtxydhutgn.html

C#:   class MyException : Exception {}
来源：http://hz.9152youxi.cn/gtvttstpzc.html

[H05] 捕获特定类型
来源：http://hz.yvedp.cn/gtcsuwascf.html

Py:   except ValueError as e:
来源：http://hz.xuanzx.com/gtlavomovp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jinqigfzy.top/gtlmmvflnk.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.dashuyun.cn/gtuetjrcid.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.redwolf501.top/gtpzhxhtkn.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yuanzhike.top/gtivwkxwmz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.xuetiantiany.cn/gtpbfwflcw.html

Ruby: rescue ArgumentError => e
来源：http://hz.yj202588.top/gtyavbkqlj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hfpthk.cn/gthptdbtku.html

[H06] 可选值 / 空值安全访问
来源：http://hz.vqdsnc.cn/gthrhetmwv.html

Py:   value = d.get("k") or default
来源：http://hz.316326.xyz/gtjwfbdijj.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yuanzhike.top/gtszwrnkam.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.9152youxi.cn/gtmzgsjrmo.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yuanzhike.top/gtwqrkhlhx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.svipenyu.cn/gtmwysanti.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.nwbrower.top/gtkysnsosx.html

Ruby: d&.dig(:a, :b)
来源：http://hz.feifeiyinyue.top/gtycydibda.html

C#:   obj?.A?.B ?? default
来源：http://hz.jinghuilouyu.cn/gtkwmqrspe.html

[H07] 断言
来源：http://hz.ehwqpu.com/gtcerxvwux.html

Py:   assert x > 0, "必须为正"
来源：http://hz.ehwqpu.com/gtcgirpkqk.html

PHP:  assert($x > 0);
来源：http://hz.chenjidiqi.icu/gtpadaiadg.html

JS:   console.assert(x > 0);
来源：http://hz.yuxming.cn/gtuuumgrlz.html


<!-- 参考信息 -->