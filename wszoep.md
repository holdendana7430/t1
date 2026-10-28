代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.pycfn.com/gtnydrnjqt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.fzhhl.top/gtgrroxomq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xinyue.icu/gtulqjyafi.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.ydjk.org.cn/gtcktzhihf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.pycfn.com/gtdalxxtte.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.316326.xyz/gtlnkmfwzo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.wangdashe.top/gtwhtheake.html

[F04] 追加写入文件
来源：http://hz.xziqi.cn/gtsfclbpmh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.shzxlz.cn/gtsuxobesn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yj20258.top/gtjqgnuaej.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.smart0.xyz/gtivhfqhik.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.316326.xyz/gtyuatzyhd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.cheryme.top/gtqywojigi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.sxryk.cn/gtfmpswxpz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.chenzaomai.com/gtzuunrbkp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jqgfzy.top/gtyrobpfmc.html

[F05] 判断文件或目录是否存在
来源：http://hz.shangyingyoupin.top/gtbgtkytrd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.andypj.xyz/gtweatxcuz.html

PHP:  file_exists("a.txt");
来源：http://hz.pengpengdd.cyou/gthvbyjitc.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jianghu66.top/gtgezqrbzp.html

TS:   fs.existsSync("a.txt")
来源：http://hz.iojbl.cn/gtbjrohojj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hywenlv.cn/gthlermnrv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ywan-chungtsiang.top/gtuqreudej.html

Ruby: File.exist?("a.txt")
来源：http://hz.yj20258888.top/gtyuaqzdzr.html

C#:   File.Exists("a.txt")
来源：http://hz.ybcxt.top/gtphclbvhq.html

[F06] 删除文件
来源：http://hz.jinqigfzy.top/gttevkuhov.html

Py:   os.remove("a.txt")
来源：http://hz.hywenlv.cn/gtyhawhbqt.html

PHP:  unlink("a.txt");
来源：http://hz.9152youxi.cn/gtlbmhzsuf.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.aizwys.cn/gtfvueflpw.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yonumen.top/gtlehflmuj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhongyouzk.top/gtbddfvmtq.html

Go:   os.Remove("a.txt")
来源：http://hz.jianghu66.top/gtxnunqxej.html

Ruby: File.delete("a.txt")
来源：http://hz.ppjwa.cn/gtoznrdikg.html

C#:   File.Delete("a.txt");
来源：http://hz.sysykeji.top/gtoglbywmu.html

[F07] 创建目录（含多级）
来源：http://hz.yangfankeji.com/gtilfskjbk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.snrcjt.cn/gteglhxybn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yongpay.top/gthuiwqxtw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yj202588.top/gtehephupw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yonumen.top/gtpwgeilpi.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jinqigufen.top/gttklyhjws.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.ydjk.org.cn/gtequrnbcu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yanxiufei.cn/gtyzcawyij.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.daxiang520.top/gtqpevvtno.html

[F08] 遍历目录
来源：http://hz.jianghu66.top/gtgzqejquh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.shzxlz.cn/gtzhvupuyy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.xylfe.cn/gtepkcdsbf.html

JS:   fs.readdirSync("dir")
来源：http://hz.hammf.cn/gtybfbrmkp.html

TS:   fs.readdirSync("dir")
来源：http://hz.hnqzz.top/gthivnhvkd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.shanyushiyangtech.top/gtabdugxkv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.shangyingyoupin.top/gtbwcfaycx.html

Ruby: Dir.children("dir")
来源：http://hz.jyoumei.cn/gtlwahfzzb.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jlsjyb.cn/gtpbycbwko.html

[F09] 获取文件大小
来源：http://hz.yvedp.cn/gtgjtzivkj.html

Py:   os.path.getsize("a.txt")
来源：http://hz.svipenyu.cn/gtgchkhozw.html

PHP:  filesize("a.txt");
来源：http://hz.yangfankeji.com/gtfyzgwrbb.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zhaomingkeji.xyz/gtxauxbssr.html

TS:   fs.statSync("a.txt").size
来源：http://hz.ydjk.org.cn/gtiwasylrx.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jqgfzy.top/gtygpekydn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.fengsongda.top/gtochoblia.html

Ruby: File.size("a.txt")
来源：http://hz.havefunace.top/gtnaddtwzb.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.zhoulong.xyz/gtznuhdztj.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jinqigfzy.top/gtfkuetpcp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.mhx1999.top/gtfuecykfo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zhijiandao.cn/gtymlerfvw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.shuidangran.top/gtvqicezeb.html

TS:   path.extname("a.txt")
来源：http://hz.hfpthk.cn/gtznjnmyki.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.sweek.top/gtcdvvhagi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.ydzc1.top/gttgatnowr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.0kj1m.cn/gtxomtysey.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.shzxlz.cn/gtybdhjvmb.html

[F11] 复制与移动文件
来源：http://hz.tian-w.cn/gttjlkradh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.pengpengdd.cyou/gtshennraa.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.hammf.cn/gtrlwicibr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shzxlz.cn/gttfunzoso.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shanyushiyangkeji.top/gtodquqayy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.ehwqpu.com/gtwrpfnstp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.tian-w.cn/gtzvdovoqf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.aizwys.cn/gtsfzdilmm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.daria6918.cn/gtilvgysgv.html

[F12] CSV 读写
来源：http://hz.shzxlz.cn/gtmhhnnwky.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yuxming.cn/gttiuxxxjv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.xuanzx.com/gtqnugbnjb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.xuetiantiany.cn/gtpycjjdvq.html

TS:   // 同上
来源：http://hz.yanxiufei.cn/gtridzfhey.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yangfankeji.com/gtjoolikbn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.ppjwa.cn/gtsruyvzqb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ybcxt.top/gtrsrzimrm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.cheryme.top/gteojvkwew.html

================================================================================
来源：http://hz.vqdsnc.cn/gtvymaotyr.html

G. 面向对象
来源：http://hz.sxryk.cn/gtjlgxikkl.html

================================================================================
来源：http://hz.ydjk.org.cn/gtpihsbyjn.html

[G01] 定义类
来源：http://hz.pengpengdd.cyou/gtwxbyibqo.html

Py:   class User: pass
来源：http://hz.zhiwuduotai.top/gtdfzotwuy.html

PHP:  class User {}
来源：http://hz.shangyingyoupin.top/gtqerqbyyq.html

JS:   class User {}
来源：http://hz.jiagoushi.top/gtpyogmsct.html

TS:   class User { name: string = ""; }
来源：http://hz.hfpthk.cn/gtswkercwx.html

Java: class User {}
来源：http://hz.yj20258888.top/gtwfweashq.html

Go:   type User struct { Name string }
来源：http://hz.nanxuanxn.top/gtjpesszer.html

Ruby: class User; end
来源：http://hz.jiagoushi.top/gtaiygifya.html

C#:   class User {}
来源：http://hz.nanxinkj.top/gtuwktdjpz.html

[G02] 构造函数
来源：http://hz.zdqjudy.top/gtrmldgoex.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.gaohongyu789.top/gtlirlqksp.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.tianlin.xyz/gtbhsnizdn.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.iojbl.cn/gtjhpyjohl.html

TS:   constructor(public name: string) {}
来源：http://hz.haohaochexian.top/gtkypqzxaa.html

Java: User(String name) { this.name = name; }
来源：http://hz.zhongyouzk.top/gtdohilpzk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yuanzhike.top/gtlhvrsspp.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.pengpengdd.cyou/gtsxtpcvuk.html

C#:   public User(string name) { Name = name; }
来源：http://hz.gzhubu.top/gtxngezhem.html

[G03] 实例属性
来源：http://hz.sxryk.cn/gtsotzwvir.html

Py:   self.name = "x"
来源：http://hz.ppjwa.cn/gteaguuuuw.html

PHP:  public string $name = "x";
来源：http://hz.sufxvd.cn/gtymfhxriy.html

JS:   this.name = "x";
来源：http://hz.snrcjt.cn/gtldljiprq.html

TS:   name: string = "x";
来源：http://hz.yuanzhike.top/gtnfrxdjgy.html

Java: private String name;
来源：http://hz.shanyushiyangkeji.top/gtyvnlqbim.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hfpthk.cn/gtlxrpntwo.html

Ruby: @name = "x"
来源：http://hz.hongshengwenyu.top/gthihmsnlv.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hnxiangtu.top/gttbhqfccg.html

[G04] 定义方法
来源：http://hz.ydzc1.top/gtfxrgckry.html

Py:   def greet(self): return self.name
来源：http://hz.9152youxi.cn/gtuvyqvmnd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.shzxlz.cn/gtzxeergdp.html

JS:   greet() { return this.name; }
来源：http://hz.nanxinkj.top/gtixqvwuuo.html

TS:   greet(): string { return this.name; }
来源：http://hz.shzxlz.cn/gtfjzpqamj.html

Java: String greet() { return name; }
来源：http://hz.gzhubu.top/gtzowlrjcx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.kuanghao11.cn/gtjbrvkjrz.html

Ruby: def greet; @name; end
来源：http://hz.cdnleiting.top/gtptmccczx.html

C#:   public string Greet() => Name;
来源：http://hz.hysaishi.cn/gtngjtobvv.html

[G05] 继承
来源：http://hz.9152youxi.cn/gtwlxpdnhi.html

Py:   class Admin(User): pass
来源：http://hz.svipenyu.cn/gtxdzlsoky.html

PHP:  class Admin extends User {}
来源：http://hz.hywenlv.cn/gtnbxtmzku.html

JS:   class Admin extends User {}
来源：http://hz.kuanghao11.cn/gtkxotbwnw.html

TS:   class Admin extends User {}
来源：http://hz.ydjk.org.cn/gtspmgaloa.html

Java: class Admin extends User {}
来源：http://hz.xylfe.cn/gtwzqeisgs.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.shzxlz.cn/gtyqsdswtr.html

Ruby: class Admin < User; end
来源：http://hz.hysaishi.cn/gtbyntxbsg.html

C#:   class Admin : User {}
来源：http://hz.52xcode.cn/gtifevgtic.html

[G06] 重写方法
来源：http://hz.tian-w.cn/gtpftiutha.html

Py:   def greet(self): return "admin"
来源：http://hz.zhaomingkeji.xyz/gtsayodzne.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yonumen.top/gtukfzfgou.html

JS:   greet() { return "admin"; }
来源：http://hz.yongpay.top/gtffxcjams.html

TS:   greet(): string { return "admin"; }
来源：http://hz.ydjk.org.cn/gtgutaccio.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jianghu66.top/gtrikxvhcu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yueranfly.top/gtryovugdm.html

Ruby: def greet; "admin"; end
来源：http://hz.cucudq.cn/gtdmapczie.html

C#:   public override string Greet() => "admin";
来源：http://hz.shangyingyoupin.top/gtqwosukdm.html

[G07] 调用父类方法
来源：http://hz.nanxuanxn.top/gtwjqysgvz.html

Py:   super().greet()
来源：http://hz.snrcjt.cn/gtolmirbmn.html

PHP:  parent::greet();
来源：http://hz.svipenyu.cn/gtdqpgbnsq.html

JS:   super.greet();
来源：http://hz.nanxinkj.top/gtuujrmrzn.html

TS:   super.greet();
来源：http://hz.yj202588.top/gtuhfhtcbb.html

Java: super.greet();
来源：http://hz.ehwqpu.com/gtllihkobv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.sxryk.cn/gtkczkdwsb.html

Ruby: super
来源：http://hz.yueranfly.top/gtxwcygjnw.html

C#:   base.Greet();
来源：http://hz.zhengqikj.top/gtbrhruaex.html

[G08] 静态方法与属性
来源：http://hz.zdqjudy.top/gtmivwblhy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.gogol.net.cn/gtfudzjhmn.html

PHP:  public static function f() {}
来源：http://hz.pengpengdd.cyou/gtbbfejgyj.html

JS:   static f() {}
来源：http://hz.xingfuxueyuan.xyz/gtvkkfoamb.html

TS:   static f(): void {}
来源：http://hz.shuidangran.top/gttsnclzrq.html

Java: static void f() {}
来源：http://hz.daria6918.cn/gtbyxdeiso.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.hywenlv.cn/gtsdhqadvk.html

Ruby: def self.f; end
来源：http://hz.zhixingplan.top/gtywrexsni.html

C#:   public static void F() {}
来源：http://hz.andypj.xyz/gtjkxcdqja.html

[G09] 接口 / 抽象类
来源：http://hz.andypj.xyz/gtudppccfa.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.daria6918.cn/gtpkzkchvt.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.pycfn.com/gtmknmgxtp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.tian-w.cn/gtpuypwutu.html

TS:   interface Shape { area(): number; }
来源：http://hz.zhixingplan.top/gthcghxbqs.html

Java: interface Shape { double area(); }
来源：http://hz.guowangkeji.top/gtjeqvdeea.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.ppjwa.cn/gtippatogg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.gogol.net.cn/gtlievqgql.html

C#:   interface IShape { double Area(); }
来源：http://hz.ywan-chungtsiang.top/gtkovhwxce.html

[G10] 访问控制
来源：http://hz.zhijiandao.cn/gthleujrje.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.ivvv.top/gtpmmpbgzz.html

PHP:  public / protected / private
来源：http://hz.52xcode.cn/gtntejlwie.html

JS:   #private 字段；其余公开
来源：http://hz.xuetiantiany.cn/gtgttjjufl.html

TS:   public / protected / private
来源：http://hz.yangfankeji.com/gtcudakkkw.html

Java: public / protected / private / 默认包级
来源：http://hz.yangfankeji.com/gtlvnddifw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.quarkkingdee.top/gtayhreqxp.html

Ruby: public / protected / private
来源：http://hz.daria6918.cn/gtjmsacjeq.html

C#:   public / protected / private / internal
来源：http://hz.hnqzz.top/gtvlvlvjho.html

[G11] getter / setter
来源：http://hz.sysykeji.top/gtxqdsocvy.html

Py:   @property 与 @x.setter
来源：http://hz.pycfn.com/gtbjxahqis.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.fzhhl.top/gtcrkgttaa.html

JS:   get name() { return this._name; }
来源：http://hz.havefunace.top/gttchsrrgn.html

TS:   get name(): string { return this._name; }
来源：http://hz.daria6918.cn/gtrewbhxnw.html

Java: public String getName() { return name; }
来源：http://hz.wangdashe.top/gtuwvoovla.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.aizwys.cn/gtzqljqtpn.html

Ruby: attr_accessor :name
来源：http://hz.yj20258.top/gtkdunxnsz.html

C#:   public string Name { get; set; }
来源：http://hz.zhaomingkeji.xyz/gtwbxvfzmm.html

[G12] 对象转字符串
来源：http://hz.xingfuxueyuan.xyz/gtyppxzrxx.html

Py:   def __str__(self): return self.name
来源：http://hz.xingfuxueyuan.xyz/gthqrxglkx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.0kj1m.cn/gtbfaxecba.html

JS:   toString() { return this.name; }
来源：http://hz.zhengqikj.top/gtvmlbznai.html

TS:   toString(): string { return this.name; }
来源：http://hz.c1oappe.top/gthxqvkkdz.html

Java: @Override public String toString() { return name; }
来源：http://hz.meibo888.top/gtoiiaazbi.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.iojbl.cn/gtumpngheu.html

Ruby: def to_s; @name; end
来源：http://hz.xuetiantiany.cn/gtqvfpulkc.html

C#:   public override string ToString() => Name;
来源：http://hz.shzxlz.cn/gtdrajkobd.html

[G13] 判断对象类型
来源：http://hz.hammf.cn/gtolruidyd.html

Py:   isinstance(u, User)
来源：http://hz.mhx1999.top/gtdtcnbmtr.html

PHP:  $u instanceof User
来源：http://hz.havefunace.top/gtbzpyhwpg.html

JS:   u instanceof User
来源：http://hz.zhengqikj.top/gtbwgmuskl.html

TS:   u instanceof User
来源：http://hz.zycfv.cn/gttfwegmvc.html

Java: u instanceof User
来源：http://hz.zhengqikj.top/gtktodyilm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.fengsongda.top/gtpnwruhns.html

Ruby: u.is_a?(User)
来源：http://hz.chenjidiqi.icu/gtdsrkzthk.html

C#:   u is User
来源：http://hz.guannengcc.top/gtpywuybsm.html

[G14] 数据类 / record
来源：http://hz.wangdashe.top/gtujpawcij.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.sufxvd.cn/gtrlgmfezf.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.9152youxi.cn/gtrutueegp.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.ppjwa.cn/gtqunaucan.html

TS:   type User = { name: string; age: number };
来源：http://hz.zhoulong.xyz/gtytqjvmgh.html

Java: record User(String name, int age) {}
来源：http://hz.sufxvd.cn/gtpxyzhidz.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yueranfly.top/gtcvzfotmr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.andypj.xyz/gtyivdxefz.html

C#:   record User(string Name, int Age);
来源：http://hz.tian-w.cn/gtdfudzxjf.html

[G15] 枚举
来源：http://hz.gotoacloud.top/gtoysnnojw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.wangdashe.top/gtcdurpnqw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.chenjidiqi.icu/gtibunueeq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yj202588.top/gtkxlyophn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.chenlongwang.top/gtudcjzchi.html

Java: enum Color { RED, GREEN }
来源：http://hz.yueranfly.top/gtfyxhnlkq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zhijiandao.cn/gtuwuqmwaf.html

Ruby: Color = %i[red green].freeze
来源：http://hz.0kj1m.cn/gtyuvbksdo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jinghuilouyu.cn/gttjgojtoj.html

[G16] 对象转数组 / 字典
来源：http://hz.xinyue.icu/gtzltlzgqi.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.meibo888.top/gtbdwjukas.html

PHP:  get_object_vars($obj);
来源：http://hz.fzhhl.top/gtzxvnpnri.html

JS:   Object.entries(obj)
来源：http://hz.zhengqikj.top/gtezwuavdq.html

TS:   Object.entries(obj)
来源：http://hz.jyoumei.cn/gtiemklydc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hnxiangtu.top/gtnjaauvnq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.wangdashe.top/gtllgpledy.html

Ruby: obj.instance_variables
来源：http://hz.zhengqikj.top/gtnxlxsnqu.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yj20258.top/gtvpecffvu.html

================================================================================
来源：http://hz.svipenyu.cn/gtwnnoysei.html

H. 异常与错误处理
来源：http://hz.sxryk.cn/gtealheflu.html

================================================================================
来源：http://hz.xylfe.cn/gtulgyldim.html

[H01] try / catch 基础
来源：http://hz.zhengqikj.top/gtwafjquze.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.xinyue.icu/gthbqtegng.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jyoumei.cn/gtwhdqqwly.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.sweek.top/gtniollkdq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jinyuanbaomall.cn/gtqomovjqk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.dashuyun.cn/gtemwhksov.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.ydzc1.top/gtzbjwhpkj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yj202588.top/gtnhixoahf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.ydjk.org.cn/gtdmfkvluy.html

[H02] finally / ensure 收尾
来源：http://hz.52xcode.cn/gtqhyqnoew.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.sweek.top/gtcglezxgs.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.shangyingyoupin.top/gtnxzoodnt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.pycfn.com/gttxvxshzm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ydzc1.top/gtarkmjfui.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.kuanghao11.cn/gthgmclhvp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.xylfe.cn/gtrdramgtm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.smart0.xyz/gtiwwhytzh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yongpay.top/gtbledujbp.html

[H03] 主动抛出异常
来源：http://hz.tian-w.cn/gtfrqnpfht.html

Py:   raise ValueError("错误信息")
来源：http://hz.shzxlz.cn/gtcxxbxwxl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zhijiandao.cn/gtwadrmowl.html

JS:   throw new Error("错误信息");
来源：http://hz.c1oappe.top/gtljmhqprx.html

TS:   throw new Error("错误信息");
来源：http://hz.jinyuanbaomall.cn/gtcnmowgzm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhengqikj.top/gtfidztyax.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hongshengwenyu.top/gtkhfattes.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.bjfxy.top/gtkxxquwsd.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.shanyushiyangtech.top/gtlistddqv.html

[H04] 自定义异常类型
来源：http://hz.zhengqikj.top/gtkxzgksfj.html

Py:   class MyError(Exception): pass
来源：http://hz.shangyingyoupin.top/gtpopmqzpx.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.ppjwa.cn/gtexixfvjl.html

JS:   class MyError extends Error {}
来源：http://hz.wangshuangyany.cn/gtsqgqlzgq.html

TS:   class MyError extends Error {}
来源：http://hz.yongpay.top/gtpxhaxinc.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jyoumei.cn/gtqlukosjx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.tianlin.xyz/gthcesegbh.html

Ruby: class MyError < StandardError; end
来源：http://hz.52xcode.cn/gtgzyotsex.html

C#:   class MyException : Exception {}
来源：http://hz.daria6918.cn/gtyguakkud.html

[H05] 捕获特定类型
来源：http://hz.yuanzhike.top/gtpbwuefhu.html

Py:   except ValueError as e:
来源：http://hz.gotoacloud.top/gtfnbmtdmf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.shuidangran.top/gtzfbhufhy.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.iojbl.cn/gtcbyqrypa.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.ydzc1.top/gtlgandmsz.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.cdnleiting.top/gtwcrwuqkz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.ivvv.top/gtztiwgqny.html

Ruby: rescue ArgumentError => e
来源：http://hz.ydjk.org.cn/gtypthwkjg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.guannengcc.top/gtuwuwntzj.html

[H06] 可选值 / 空值安全访问
来源：http://hz.smart0.xyz/gttyazakov.html

Py:   value = d.get("k") or default
来源：http://hz.xziqi.cn/gtgwgonflh.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.xinyue.icu/gtbbrfwysv.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.snrcjt.cn/gtqehcpbzp.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zhoulong.xyz/gtbircoozf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.hywenlv.cn/gtlwetkbtr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.cheryme.top/gtkuvqlrmr.html

Ruby: d&.dig(:a, :b)
来源：http://hz.tian-w.cn/gtmoivcblk.html

C#:   obj?.A?.B ?? default
来源：http://hz.cashguo.top/gtssinsvsk.html

[H07] 断言
来源：http://hz.jqgufenzy.top/gtlcbkmduq.html

Py:   assert x > 0, "必须为正"
来源：http://hz.smart0.xyz/gtlkxsonlg.html

PHP:  assert($x > 0);
来源：http://hz.daxiang520.top/gtffxgoysr.html

JS:   console.assert(x > 0);
来源：http://hz.hysaishi.cn/gtqzburjga.html

TS:   console.assert(x > 0);
来源：http://hz.yj20258.top/gtzszsfyor.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jianghu66.top/gtfvsezpks.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.316326.xyz/gtmzuampgj.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhengqikj.top/gtwrmcaukx.html


<!-- 参考信息 -->