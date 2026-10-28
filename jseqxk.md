代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.pycfn.com/gtbmrzonje.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.redwolf501.top/gtxslksrek.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.9152youxi.cn/gtpvcrpaje.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.pengpengdd.cyou/gtbrukfmmd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.c1oappe.top/gtokwjfgwv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.xingfuxueyuan.xyz/gtqaldmdvb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.svipenyu.cn/gtlmwywtng.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.ivvv.top/gtknmecbuj.html

[F05] 判断文件或目录是否存在
来源：http://hz.gaohongyu789.top/gtdlqbeltw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.meibo888.top/gtcddftffl.html

PHP:  file_exists("a.txt");
来源：http://hz.gotoacloud.top/gtanyyxkps.html

JS:   fs.existsSync("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtbcajluih.html

TS:   fs.existsSync("a.txt")
来源：http://hz.iojbl.cn/gtaoosifot.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yangfankeji.com/gttpqlvely.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zhixingplan.top/gtgjvcqzmb.html

Ruby: File.exist?("a.txt")
来源：http://hz.bjfxy.top/gtbiwtiqph.html

C#:   File.Exists("a.txt")
来源：http://hz.shangyingyoupin.top/gtvmabswit.html

[F06] 删除文件
来源：http://hz.hnxiangtu.top/gtimhypyxo.html

Py:   os.remove("a.txt")
来源：http://hz.hongshengwenyu.top/gtintrynff.html

PHP:  unlink("a.txt");
来源：http://hz.sysykeji.top/gtflubkwmy.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.kuanghao11.cn/gtgozrrpyu.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.quarkkingdee.top/gtbnafcwsh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.aizwys.cn/gtateiwmcd.html

Go:   os.Remove("a.txt")
来源：http://hz.hfpthk.cn/gtzwfondoh.html

Ruby: File.delete("a.txt")
来源：http://hz.zhijiandao.cn/gtfhotqfkk.html

C#:   File.Delete("a.txt");
来源：http://hz.gaohongyu789.top/gtxnnnxwis.html

[F07] 创建目录（含多级）
来源：http://hz.ppjwa.cn/gtrustuijz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hywenlv.cn/gtsdgmumfq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jiagoushi.top/gtgccwdvpg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.dashuyun.cn/gtfhxyahih.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cdnleiting.top/gtcxniqytv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hnqzz.top/gtipfmxenu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.nwbrower.top/gtwodwxczv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.haohaochexian.top/gtllcfqfkp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.chenjidiqi.icu/gthgjwpdpv.html

[F08] 遍历目录
来源：http://hz.havefunace.top/gtrxeuilii.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yonumen.top/gtlzmlcgzq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jqgfzy.top/gtbmcymwcz.html

JS:   fs.readdirSync("dir")
来源：http://hz.smart0.xyz/gteyxwsvtg.html

TS:   fs.readdirSync("dir")
来源：http://hz.havefunace.top/gtsiavbpqy.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.shangyingyoupin.top/gtnnqzwgzx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.birdmap.top/gtuzulpaih.html

Ruby: Dir.children("dir")
来源：http://hz.ywan-chungtsiang.top/gtobtgjysb.html

C#:   Directory.GetFiles("dir")
来源：http://hz.chenjidiqi.icu/gtdxsnfcyt.html

[F09] 获取文件大小
来源：http://hz.zdqjudy.top/gtilbednea.html

Py:   os.path.getsize("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtdccjcjcm.html

PHP:  filesize("a.txt");
来源：http://hz.aibaodan.cn/gtqcrchroq.html

JS:   fs.statSync("a.txt").size
来源：http://hz.cdnleiting.top/gtdwltvckc.html

TS:   fs.statSync("a.txt").size
来源：http://hz.hywenlv.cn/gtjmpdfugi.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.tanke756.top/gtuemewvon.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jqgfzy.top/gtyppaxhkw.html

Ruby: File.size("a.txt")
来源：http://hz.jinghuilouyu.cn/gtbvhqgnwq.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.hfpthk.cn/gtzsrljncw.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.havefunace.top/gtorpfjfxg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.gzhubu.top/gtkepqorih.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.ywan-chungtsiang.top/gtjotmdnwx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.sufxvd.cn/gtsjwlcsoy.html

TS:   path.extname("a.txt")
来源：http://hz.shuidangran.top/gtpvjsnjjx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.ivvv.top/gtbrxbmobr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.aizwys.cn/gtshevmpvr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.dashuyun.cn/gtdceadwwv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.shuidangran.top/gtqupqvqci.html

[F11] 复制与移动文件
来源：http://hz.meibo888.top/gtasjknfdb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.andypj.xyz/gtsaisrjkx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.cucudq.cn/gtxpnwlzti.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yuanzhike.top/gtqzbywzsx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xuanzx.com/gtatsgpiuc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.haohaochexian.top/gtiqilrqfu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.c1oappe.top/gtavbywsvy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.9152youxi.cn/gthaphlirx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhengqikj.top/gtpvgjqijr.html

[F12] CSV 读写
来源：http://hz.yj202588.top/gtfnsanewc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jinqigufen.top/gtxdovpsvf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.shanyushiyangtech.top/gtqmipxvld.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zhiwuduotai.top/gtuvjlflod.html

TS:   // 同上
来源：http://hz.cheryme.top/gtrmbadhiv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.pycfn.com/gtyreesruv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.guannengcc.top/gtvujorrrn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yj20258.top/gtixkmbfpe.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jqgfzy.top/gtztaulojo.html

================================================================================
来源：http://hz.ppjwa.cn/gtnldpesqc.html

G. 面向对象
来源：http://hz.meibo888.top/gtkdotmlja.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtrfqnrixl.html

[G01] 定义类
来源：http://hz.nwbrower.top/gtlavttpuj.html

Py:   class User: pass
来源：http://hz.shzxlz.cn/gtuqwxqdin.html

PHP:  class User {}
来源：http://hz.gzhubu.top/gtpkbzepqt.html

JS:   class User {}
来源：http://hz.yuanzhike.top/gtdhyhvtro.html

TS:   class User { name: string = ""; }
来源：http://hz.aibaodan.cn/gtmrttmrxx.html

Java: class User {}
来源：http://hz.ivvv.top/gtinlxemlz.html

Go:   type User struct { Name string }
来源：http://hz.zdqjudy.top/gtqpeyvsuz.html

Ruby: class User; end
来源：http://hz.c1oappe.top/gtymxkcbeg.html

C#:   class User {}
来源：http://hz.zycfv.cn/gtxbmktfpa.html

[G02] 构造函数
来源：http://hz.birdmap.top/gtdyhdptxm.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.meibo888.top/gtsqxmrbzh.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.cucudq.cn/gtjnrkicrt.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yuxming.cn/gtepmiedcx.html

TS:   constructor(public name: string) {}
来源：http://hz.jianghu66.top/gtkaxrltfb.html

Java: User(String name) { this.name = name; }
来源：http://hz.hammf.cn/gthfcnqzoj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.shzxlz.cn/gtvsixrevk.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.ybcxt.top/gtgsosacqv.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jyoumei.cn/gtzsdtvoyb.html

[G03] 实例属性
来源：http://hz.zdqjudy.top/gttzvihvao.html

Py:   self.name = "x"
来源：http://hz.xylfe.cn/gtcelodmne.html

PHP:  public string $name = "x";
来源：http://hz.ydzc1.top/gtpdkhrxia.html

JS:   this.name = "x";
来源：http://hz.xziqi.cn/gtnjmzzfyr.html

TS:   name: string = "x";
来源：http://hz.nanxuanxn.top/gtsgnyqatl.html

Java: private String name;
来源：http://hz.gzhubu.top/gtwcpgqrnr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.nanxuanxn.top/gtkrdfhrfe.html

Ruby: @name = "x"
来源：http://hz.yongpay.top/gtvwwctepc.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yvedp.cn/gttecjcrjb.html

[G04] 定义方法
来源：http://hz.dashuyun.cn/gtiemtrbyt.html

Py:   def greet(self): return self.name
来源：http://hz.haohaochexian.top/gtproighjs.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yvedp.cn/gtacjeljjn.html

JS:   greet() { return this.name; }
来源：http://hz.chenzaomai.com/gtvfnrvttv.html

TS:   greet(): string { return this.name; }
来源：http://hz.dashuyun.cn/gtcwvlhcdl.html

Java: String greet() { return name; }
来源：http://hz.jiagoushi.top/gthfljzsba.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.cucudq.cn/gtqkcidibj.html

Ruby: def greet; @name; end
来源：http://hz.bjfxy.top/gtkfijllbs.html

C#:   public string Greet() => Name;
来源：http://hz.jiagoushi.top/gtvilwnqfq.html

[G05] 继承
来源：http://hz.ehwqpu.com/gtqjdiwwdd.html

Py:   class Admin(User): pass
来源：http://hz.mhx1999.top/gtumzunpou.html

PHP:  class Admin extends User {}
来源：http://hz.yonumen.top/gtsxszsjoo.html

JS:   class Admin extends User {}
来源：http://hz.tian-w.cn/gtupqruyiv.html

TS:   class Admin extends User {}
来源：http://hz.zhengqikj.top/gtozahnlif.html

Java: class Admin extends User {}
来源：http://hz.jinqigufen.top/gtntwuaofp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hysaishi.cn/gtbflkfesd.html

Ruby: class Admin < User; end
来源：http://hz.cheryme.top/gtkkeqeefe.html

C#:   class Admin : User {}
来源：http://hz.cheryme.top/gtmdkzcyqt.html

[G06] 重写方法
来源：http://hz.tian-w.cn/gtqxajbvzp.html

Py:   def greet(self): return "admin"
来源：http://hz.wangshuangyany.cn/gtucoypszd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.hnqzz.top/gtbrgtajee.html

JS:   greet() { return "admin"; }
来源：http://hz.316326.xyz/gtvkgpmfis.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yj202588.top/gtnoevlfhh.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ydjk.org.cn/gtoqevbuqu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.daria6918.cn/gtyaczubsm.html

Ruby: def greet; "admin"; end
来源：http://hz.jinyuanbaomall.cn/gtbkdpjkyh.html

C#:   public override string Greet() => "admin";
来源：http://hz.yangfankeji.com/gtjumldvbc.html

[G07] 调用父类方法
来源：http://hz.guannengcc.top/gtejeccnwa.html

Py:   super().greet()
来源：http://hz.zhongyouzk.top/gtnsecjyhn.html

PHP:  parent::greet();
来源：http://hz.quarkkingdee.top/gthtlusimj.html

JS:   super.greet();
来源：http://hz.meibo888.top/gtzstackvg.html

TS:   super.greet();
来源：http://hz.316326.xyz/gtikzqhots.html

Java: super.greet();
来源：http://hz.yj202588.top/gtviawaxzd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.chenlongwang.top/gtzhxyzxzp.html

Ruby: super
来源：http://hz.gotoacloud.top/gtbomlvbaw.html

C#:   base.Greet();
来源：http://hz.tian-w.cn/gtyhgbfrfh.html

[G08] 静态方法与属性
来源：http://hz.havefunace.top/gttwlydbtl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.ppjwa.cn/gttxjxunik.html

PHP:  public static function f() {}
来源：http://hz.tanke756.top/gtrxdyyfya.html

JS:   static f() {}
来源：http://hz.tian-w.cn/gtzxcprfli.html

TS:   static f(): void {}
来源：http://hz.shuidangran.top/gtdmsftkhj.html

Java: static void f() {}
来源：http://hz.guannengcc.top/gtknxwvall.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.shangyingyoupin.top/gtwyioozqv.html

Ruby: def self.f; end
来源：http://hz.jinqigufen.top/gtytcmfhrq.html

C#:   public static void F() {}
来源：http://hz.hfpthk.cn/gtwfakjbfa.html

[G09] 接口 / 抽象类
来源：http://hz.yvedp.cn/gtuileqzzo.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.xuanzx.com/gtoegdhpft.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zhijiandao.cn/gtjyncuniq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.feifeiyinyue.top/gtdubntggq.html

TS:   interface Shape { area(): number; }
来源：http://hz.9152youxi.cn/gtflatyoys.html

Java: interface Shape { double area(); }
来源：http://hz.redwolf501.top/gtbdjzwgdl.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.daria6918.cn/gtssupzsok.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.guowangkeji.top/gtrotgfjme.html

C#:   interface IShape { double Area(); }
来源：http://hz.tianlin.xyz/gtfuythilz.html

[G10] 访问控制
来源：http://hz.0kj1m.cn/gtuvrijahi.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.chenjidiqi.icu/gtgrsjnrwn.html

PHP:  public / protected / private
来源：http://hz.yj20258888.top/gtovckbjsc.html

JS:   #private 字段；其余公开
来源：http://hz.xuetiantiany.cn/gtcimnqkod.html

TS:   public / protected / private
来源：http://hz.yanxiufei.cn/gtyibwifoj.html

Java: public / protected / private / 默认包级
来源：http://hz.vqdsnc.cn/gtobvieqnb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.guowangkeji.top/gtmndyuioe.html

Ruby: public / protected / private
来源：http://hz.vqdsnc.cn/gtbvxzwjnd.html

C#:   public / protected / private / internal
来源：http://hz.dashuyun.cn/gttrwbklhn.html

[G11] getter / setter
来源：http://hz.nanxuanxn.top/gturbdfmbg.html

Py:   @property 与 @x.setter
来源：http://hz.shanyushiyangtech.top/gteaxcnjng.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.andypj.xyz/gtbwuqedrn.html

JS:   get name() { return this._name; }
来源：http://hz.xuanzx.com/gtyiaqdwlp.html

TS:   get name(): string { return this._name; }
来源：http://hz.sxryk.cn/gtqydipqkl.html

Java: public String getName() { return name; }
来源：http://hz.gaohongyu789.top/gtydoaeucz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yuanzhike.top/gtjzfbomql.html

Ruby: attr_accessor :name
来源：http://hz.mhx1999.top/gtwucbvxga.html

C#:   public string Name { get; set; }
来源：http://hz.jinqigfzy.top/gtdpsbmjaf.html

[G12] 对象转字符串
来源：http://hz.xziqi.cn/gtkvzfypfa.html

Py:   def __str__(self): return self.name
来源：http://hz.xziqi.cn/gtwkrkuqop.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yuanzhike.top/gtffzxlfxx.html

JS:   toString() { return this.name; }
来源：http://hz.svipenyu.cn/gtisznavpd.html

TS:   toString(): string { return this.name; }
来源：http://hz.aizwys.cn/gtnxlzsmjr.html

Java: @Override public String toString() { return name; }
来源：http://hz.yj20258.top/gtvbvymuxe.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jinghuilouyu.cn/gtloihuqph.html

Ruby: def to_s; @name; end
来源：http://hz.chenzaomai.com/gtfbonbmdt.html

C#:   public override string ToString() => Name;
来源：http://hz.havefunace.top/gtqiionynd.html

[G13] 判断对象类型
来源：http://hz.havefunace.top/gttqpkxijf.html

Py:   isinstance(u, User)
来源：http://hz.yangfankeji.com/gtxntuqllb.html

PHP:  $u instanceof User
来源：http://hz.havefunace.top/gtjiyqqzzj.html

JS:   u instanceof User
来源：http://hz.redwolf501.top/gtmgmdkxzx.html

TS:   u instanceof User
来源：http://hz.xylfe.cn/gteestnljj.html

Java: u instanceof User
来源：http://hz.shzxlz.cn/gtufhgvioc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ywan-chungtsiang.top/gtakgezyyr.html

Ruby: u.is_a?(User)
来源：http://hz.shangyingyoupin.top/gtqvbsteqy.html

C#:   u is User
来源：http://hz.hysaishi.cn/gtdzxjydvi.html

[G14] 数据类 / record
来源：http://hz.hywenlv.cn/gtfnvlcrhs.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.ydzc1.top/gtwyvojhiq.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yvedp.cn/gtzevklnru.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.daxiang520.top/gtkqcucrsk.html

TS:   type User = { name: string; age: number };
来源：http://hz.tanke756.top/gtgtdfrvtu.html

Java: record User(String name, int age) {}
来源：http://hz.shanyushiyangkeji.top/gtxarhigag.html

Go:   type User struct { Name string; Age int }
来源：http://hz.pengpengdd.cyou/gtbvwpvpsb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.bjfxy.top/gtneavddbp.html

C#:   record User(string Name, int Age);
来源：http://hz.jinqigufen.top/gtrsyvgvpi.html

[G15] 枚举
来源：http://hz.andypj.xyz/gtzqkuuavf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.9152youxi.cn/gtvgcqotps.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.aizwys.cn/gtexjttioo.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.sufxvd.cn/gtiecxavvt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.haohaochexian.top/gtirzfbowa.html

Java: enum Color { RED, GREEN }
来源：http://hz.hfpthk.cn/gthnpnilei.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.shangyingyoupin.top/gtlzwyiewc.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ybcxt.top/gtbekllnbh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.nanxinkj.top/gtnwjmkmcc.html

[G16] 对象转数组 / 字典
来源：http://hz.9152youxi.cn/gtzbhsjqom.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.xuetiantiany.cn/gtgkteazha.html

PHP:  get_object_vars($obj);
来源：http://hz.guannengcc.top/gttmlpvija.html

JS:   Object.entries(obj)
来源：http://hz.ppjwa.cn/gtqcwjnvae.html

TS:   Object.entries(obj)
来源：http://hz.0kj1m.cn/gtnccemnvc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hammf.cn/gtizpswcnd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.cashguo.top/gtojmnkozl.html

Ruby: obj.instance_variables
来源：http://hz.jinyuanbaomall.cn/gttzcveidv.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yuxming.cn/gtxlbtzvsf.html

================================================================================
来源：http://hz.iojbl.cn/gtjtdpzkdy.html

H. 异常与错误处理
来源：http://hz.smart0.xyz/gtpkalngqu.html

================================================================================
来源：http://hz.fengsongda.top/gtsfkdnxvj.html

[H01] try / catch 基础
来源：http://hz.wangdashe.top/gtxazqgcsg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yonumen.top/gtmcmvidly.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.gaohongyu789.top/gtfwqudhxt.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jinqigfzy.top/gtwguufyrc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.shuidangran.top/gtzcclekei.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yonumen.top/gthrebqetv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.nwbrower.top/gtgwgdmthg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.hnqzz.top/gtmmbfbfei.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yonumen.top/gteadjnpxh.html

[H02] finally / ensure 收尾
来源：http://hz.sweek.top/gtnhhhbhkm.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jqgufenzy.top/gtmqqjbmae.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.cucudq.cn/gtictluipd.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.guannengcc.top/gtvlmfxewi.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.havefunace.top/gtlnmymxez.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.chenjidiqi.icu/gtngiyrccf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.iojbl.cn/gtzwnqfbao.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.sufxvd.cn/gtxsszbddh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.fengsongda.top/gtkpdrzxuy.html

[H03] 主动抛出异常
来源：http://hz.shanyushiyangtech.top/gtkdrvejcb.html

Py:   raise ValueError("错误信息")
来源：http://hz.wangdashe.top/gtybymsuua.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.mhx1999.top/gtcrqrugid.html

JS:   throw new Error("错误信息");
来源：http://hz.xuetiantiany.cn/gtdfetjqur.html

TS:   throw new Error("错误信息");
来源：http://hz.havefunace.top/gtcqybirgg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jinyuanbaomall.cn/gtelgzcbrj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.tian-w.cn/gtuuzmwxdv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.guannengcc.top/gtvwqiwbnr.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.gzhubu.top/gtarjvswyt.html

[H04] 自定义异常类型
来源：http://hz.nanxinkj.top/gtenalinqh.html

Py:   class MyError(Exception): pass
来源：http://hz.316326.xyz/gtlntbotio.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.9152youxi.cn/gtcejvfkgh.html

JS:   class MyError extends Error {}
来源：http://hz.jinyuanbaomall.cn/gtwvaxxtuk.html

TS:   class MyError extends Error {}
来源：http://hz.cqqwz.cn/gtmgfbbgzm.html

Java: class MyException extends RuntimeException {}
来源：http://hz.fzhhl.top/gtkclbviro.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.mhx1999.top/gtmjgkllpx.html

Ruby: class MyError < StandardError; end
来源：http://hz.guannengcc.top/gtbiphmkdx.html

C#:   class MyException : Exception {}
来源：http://hz.kuanghao11.cn/gtrcokxxet.html

[H05] 捕获特定类型
来源：http://hz.xinyue.icu/gtueyohrgj.html

Py:   except ValueError as e:
来源：http://hz.jinqigfzy.top/gtzahlwzde.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.kuanghao11.cn/gtjlffwthd.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.9152youxi.cn/gthkuzhxma.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jqgfzy.top/gtvvvowmyc.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.cashguo.top/gtpzbxvhwd.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.ehwqpu.com/gtufoivmae.html

Ruby: rescue ArgumentError => e
来源：http://hz.chenzaomai.com/gtoymduugu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.feifeiyinyue.top/gtnsjakirg.html

[H06] 可选值 / 空值安全访问
来源：http://hz.wangshuangyany.cn/gtzluhtooc.html

Py:   value = d.get("k") or default
来源：http://hz.pycfn.com/gttcpkmsik.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.bjfxy.top/gthejohfia.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.xuetiantiany.cn/gtjcqaskzh.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jyoumei.cn/gthzadgllm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ywan-chungtsiang.top/gtasqxaabf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.gaohongyu789.top/gtzujzhcjm.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yj20258.top/gticlboenn.html

C#:   obj?.A?.B ?? default
来源：http://hz.andypj.xyz/gtzgwyiuue.html

[H07] 断言
来源：http://hz.yueranfly.top/gtuauubfnp.html

Py:   assert x > 0, "必须为正"
来源：http://hz.quarkkingdee.top/gttqekgbru.html

PHP:  assert($x > 0);
来源：http://hz.snrcjt.cn/gtkzleeflc.html

JS:   console.assert(x > 0);
来源：http://hz.cdnleiting.top/gtlnusicyt.html

TS:   console.assert(x > 0);
来源：http://hz.ivvv.top/gthpbacutk.html

Java: assert x > 0 : "必须为正";
来源：http://hz.cqqwz.cn/gtglqiwzwp.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.xylfe.cn/gtifmxljac.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.svipenyu.cn/gtfcglwukf.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zhoulong.xyz/gtdftphqwn.html

[H08] 获取错误信息与堆栈
来源：http://hz.ydzc1.top/gtnrezzndg.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.sxryk.cn/gtxlqhfzox.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.cheryme.top/gtblnmnyjr.html

JS:   e.message;  e.stack
来源：http://hz.yongpay.top/gtplayhwjs.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.smart0.xyz/gtwpjyhayu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.chenzaomai.com/gtpuijmina.html

Go:   err.Error()
来源：http://hz.shanyushiyangkeji.top/gtxixnqflz.html


<!-- 参考信息 -->