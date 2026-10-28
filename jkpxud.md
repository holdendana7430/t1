代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.ydzc1.top/gtefrechxf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.redwolf501.top/gtfblxdzlc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.pycfn.com/gtleiibypw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jinghuilouyu.cn/gtyrzijmai.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jinyuanbaomall.cn/gtghqbkcga.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yongpay.top/gtkbavudqs.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yangfankeji.com/gtvpswhmqq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.chenjidiqi.icu/gtkuqgdajs.html

[F05] 判断文件或目录是否存在
来源：http://hz.bjfxy.top/gtyablitwa.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.shuidangran.top/gthjukqqmz.html

PHP:  file_exists("a.txt");
来源：http://hz.jinqigufen.top/gtmcczpzrk.html

JS:   fs.existsSync("a.txt")
来源：http://hz.cdnleiting.top/gtxeofczrr.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yvedp.cn/gtyzmdrjwh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.guannengcc.top/gtjgmtdigi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.daxiang520.top/gtkkexbuiw.html

Ruby: File.exist?("a.txt")
来源：http://hz.tian-w.cn/gtxptemnes.html

C#:   File.Exists("a.txt")
来源：http://hz.aizwys.cn/gtgyodpezw.html

[F06] 删除文件
来源：http://hz.shanyushiyangkeji.top/gtartsllic.html

Py:   os.remove("a.txt")
来源：http://hz.birdmap.top/gtjcrfwabe.html

PHP:  unlink("a.txt");
来源：http://hz.iojbl.cn/gtyiezjkbj.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.xziqi.cn/gtyjzehfwo.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.vqdsnc.cn/gtbunfpdtv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yanxiufei.cn/gthivdeanv.html

Go:   os.Remove("a.txt")
来源：http://hz.hammf.cn/gtoobxgsog.html

Ruby: File.delete("a.txt")
来源：http://hz.wangdashe.top/gtayahfoso.html

C#:   File.Delete("a.txt");
来源：http://hz.52xcode.cn/gtreztitqo.html

[F07] 创建目录（含多级）
来源：http://hz.zhongyouzk.top/gtsqwsikxa.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.pycfn.com/gtoxcgdzke.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.hnxiangtu.top/gtyxyxzkzl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jianghu66.top/gtplwrlcxp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yongpay.top/gthiulomuc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yj20258888.top/gttmxjcpyi.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.ywan-chungtsiang.top/gtvsoxvrky.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yueranfly.top/gtzzlysqzr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.nanxuanxn.top/gtbvpastak.html

[F08] 遍历目录
来源：http://hz.jyoumei.cn/gtaptbriuo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.ydjk.org.cn/gtnesfdxvq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.hysaishi.cn/gtobwhbohn.html

JS:   fs.readdirSync("dir")
来源：http://hz.jinqigufen.top/gtqrpcxeer.html

TS:   fs.readdirSync("dir")
来源：http://hz.pengpengdd.cyou/gtomhptjen.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jqgufenzy.top/gtpohjhlwu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.xuanzx.com/gtsahwkyte.html

Ruby: Dir.children("dir")
来源：http://hz.mhx1999.top/gtsvzxsmhx.html

C#:   Directory.GetFiles("dir")
来源：http://hz.shanyushiyangtech.top/gtprzedmts.html

[F09] 获取文件大小
来源：http://hz.nanxuanxn.top/gtqdyqvvil.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zhixingplan.top/gtsxcwlrww.html

PHP:  filesize("a.txt");
来源：http://hz.sweek.top/gtjlvpukww.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jiagoushi.top/gtijttjews.html

TS:   fs.statSync("a.txt").size
来源：http://hz.havefunace.top/gtimhmlhrj.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.hfpthk.cn/gtvqluoldz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zhixingplan.top/gtgcxifvox.html

Ruby: File.size("a.txt")
来源：http://hz.jqgufenzy.top/gtbxhvkkfw.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.andypj.xyz/gtuwyribem.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jinghuilouyu.cn/gtrylnjjhg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jyoumei.cn/gtlecvnngs.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yonumen.top/gtgaudkrzx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.dianchejie.cn/gtpzqlqhbo.html

TS:   path.extname("a.txt")
来源：http://hz.svipenyu.cn/gtpzearswv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jyoumei.cn/gtmswvrgbd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.ivvv.top/gtfsblrxfc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jqgfzy.top/gtytfzxrvp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.fzhhl.top/gtnjsvxhoi.html

[F11] 复制与移动文件
来源：http://hz.mhx1999.top/gthkhkfkkq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.hfpthk.cn/gtzgklpcvx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.shzxlz.cn/gtkrldzvyh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.iojbl.cn/gtdvjlmprv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xuanzx.com/gtvfehrehs.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.316326.xyz/gtbmmszwre.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.guowangkeji.top/gtvhbhoonw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.xuetiantiany.cn/gtuuvjanft.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.nwbrower.top/gtruubsjiz.html

[F12] CSV 读写
来源：http://hz.hongshengwenyu.top/gthdjzkvwd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.cheryme.top/gtbtoeqtlr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zdqjudy.top/gtkumxzoaq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.hongshengwenyu.top/gtdmfzltgd.html

TS:   // 同上
来源：http://hz.yonumen.top/gtlnojolww.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yuanzhike.top/gtzkswufdj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.xinyue.icu/gtvfpggvhq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.xingfuxueyuan.xyz/gtlurqrpnt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.daria6918.cn/gtcqybdfdz.html

================================================================================
来源：http://hz.zhixingplan.top/gtrbhhiqmv.html

G. 面向对象
来源：http://hz.shzxlz.cn/gtctymgsib.html

================================================================================
来源：http://hz.hfpthk.cn/gtpafzxawa.html

[G01] 定义类
来源：http://hz.sufxvd.cn/gtxswqfrmb.html

Py:   class User: pass
来源：http://hz.sweek.top/gtjgckjhfp.html

PHP:  class User {}
来源：http://hz.tianlin.xyz/gtzdbbwimh.html

JS:   class User {}
来源：http://hz.hnqzz.top/gtgajpizev.html

TS:   class User { name: string = ""; }
来源：http://hz.zhaomingkeji.xyz/gtfpysezqv.html

Java: class User {}
来源：http://hz.jinqigufen.top/gtodnkctbr.html

Go:   type User struct { Name string }
来源：http://hz.birdmap.top/gtwmmchhge.html

Ruby: class User; end
来源：http://hz.xuetiantiany.cn/gtofwtkyfi.html

C#:   class User {}
来源：http://hz.zhongyouzk.top/gttmgvmfbv.html

[G02] 构造函数
来源：http://hz.jinghuilouyu.cn/gtktjwcfux.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yvedp.cn/gtdnspwzpb.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.chenlongwang.top/gtifdkbcos.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.52xcode.cn/gthyewjoia.html

TS:   constructor(public name: string) {}
来源：http://hz.yuanzhike.top/gtpimyuvuz.html

Java: User(String name) { this.name = name; }
来源：http://hz.gotoacloud.top/gthkshbrko.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hammf.cn/gttvlwrsey.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.52xcode.cn/gtdftydynz.html

C#:   public User(string name) { Name = name; }
来源：http://hz.xziqi.cn/gtdcammich.html

[G03] 实例属性
来源：http://hz.jinyuanbaomall.cn/gtcuxyqjol.html

Py:   self.name = "x"
来源：http://hz.shzxlz.cn/gtkduhhezn.html

PHP:  public string $name = "x";
来源：http://hz.zhijiandao.cn/gtrrdboavb.html

JS:   this.name = "x";
来源：http://hz.daxiang520.top/gthnsgqbrt.html

TS:   name: string = "x";
来源：http://hz.cheryme.top/gtyphsllbn.html

Java: private String name;
来源：http://hz.cdnleiting.top/gtprnetdge.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.ivvv.top/gteehknufw.html

Ruby: @name = "x"
来源：http://hz.yvedp.cn/gtjpumxvwa.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jlsjyb.cn/gtszhdwwhh.html

[G04] 定义方法
来源：http://hz.yueranfly.top/gtdiotqood.html

Py:   def greet(self): return self.name
来源：http://hz.fengsongda.top/gtyiivyfit.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.fzhhl.top/gtaplalzhv.html

JS:   greet() { return this.name; }
来源：http://hz.cdnleiting.top/gtzgcfylfb.html

TS:   greet(): string { return this.name; }
来源：http://hz.ppjwa.cn/gtwoxktwgj.html

Java: String greet() { return name; }
来源：http://hz.vqdsnc.cn/gtndthdzsl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.kuanghao11.cn/gttvhjnxmh.html

Ruby: def greet; @name; end
来源：http://hz.havefunace.top/gtdhiedxbp.html

C#:   public string Greet() => Name;
来源：http://hz.daria6918.cn/gthxpnhfji.html

[G05] 继承
来源：http://hz.zhixingplan.top/gthdsmohpa.html

Py:   class Admin(User): pass
来源：http://hz.dashuyun.cn/gtobqlwccd.html

PHP:  class Admin extends User {}
来源：http://hz.9152youxi.cn/gtvavqsgzn.html

JS:   class Admin extends User {}
来源：http://hz.havefunace.top/gtnjbuqyyr.html

TS:   class Admin extends User {}
来源：http://hz.xingfuxueyuan.xyz/gtiadqfids.html

Java: class Admin extends User {}
来源：http://hz.yanxiufei.cn/gtxgvofhsd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ywan-chungtsiang.top/gthujjvkoe.html

Ruby: class Admin < User; end
来源：http://hz.shangyingyoupin.top/gtxbpicxqj.html

C#:   class Admin : User {}
来源：http://hz.shuidangran.top/gtqbncxmou.html

[G06] 重写方法
来源：http://hz.chenlongwang.top/gthxzqsbwv.html

Py:   def greet(self): return "admin"
来源：http://hz.iojbl.cn/gtborffhde.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.xylfe.cn/gtbypsnoed.html

JS:   greet() { return "admin"; }
来源：http://hz.nanxuanxn.top/gttezudwqh.html

TS:   greet(): string { return "admin"; }
来源：http://hz.cucudq.cn/gtdbkgjtqz.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.cheryme.top/gtpleaueob.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.dianchejie.cn/gtlexnifgv.html

Ruby: def greet; "admin"; end
来源：http://hz.hfpthk.cn/gtzwxssgvv.html

C#:   public override string Greet() => "admin";
来源：http://hz.0kj1m.cn/gtnxqauley.html

[G07] 调用父类方法
来源：http://hz.jinqigufen.top/gtysxqhfby.html

Py:   super().greet()
来源：http://hz.jinyuanbaomall.cn/gtoazqqoep.html

PHP:  parent::greet();
来源：http://hz.jyoumei.cn/gtflobixxp.html

JS:   super.greet();
来源：http://hz.yangfankeji.com/gtewzwauom.html

TS:   super.greet();
来源：http://hz.yanxiufei.cn/gtgmecnkpa.html

Java: super.greet();
来源：http://hz.cdnleiting.top/gtvpvccxdu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.nanxuanxn.top/gtlxcsonuc.html

Ruby: super
来源：http://hz.haohaochexian.top/gtayrqgrps.html

C#:   base.Greet();
来源：http://hz.gaohongyu789.top/gtsqgasixg.html

[G08] 静态方法与属性
来源：http://hz.snrcjt.cn/gtetsthrdb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.xylfe.cn/gtgllvxikm.html

PHP:  public static function f() {}
来源：http://hz.kuanghao11.cn/gtjxsvirkr.html

JS:   static f() {}
来源：http://hz.gotoacloud.top/gtwsbchmrh.html

TS:   static f(): void {}
来源：http://hz.kuanghao11.cn/gttzxizhqw.html

Java: static void f() {}
来源：http://hz.gogol.net.cn/gtlzzxnrfu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.wangshuangyany.cn/gtqjzlgrfk.html

Ruby: def self.f; end
来源：http://hz.feifeiyinyue.top/gtfmiyarti.html

C#:   public static void F() {}
来源：http://hz.cucudq.cn/gtoeboumrz.html

[G09] 接口 / 抽象类
来源：http://hz.havefunace.top/gtfbujvtaj.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.smart0.xyz/gtvrnvudyn.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.cheryme.top/gtxadjcwzh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.9152youxi.cn/gtuxsvumvd.html

TS:   interface Shape { area(): number; }
来源：http://hz.shzxlz.cn/gtylldjrcv.html

Java: interface Shape { double area(); }
来源：http://hz.wangdashe.top/gtrowdpekr.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.ivvv.top/gtxkpucmkm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.ehwqpu.com/gtzlzjdyqb.html

C#:   interface IShape { double Area(); }
来源：http://hz.tian-w.cn/gtddvzmlqd.html

[G10] 访问控制
来源：http://hz.gotoacloud.top/gtldltbtds.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.vqdsnc.cn/gtgewkkumt.html

PHP:  public / protected / private
来源：http://hz.hysaishi.cn/gtuwfvsalb.html

JS:   #private 字段；其余公开
来源：http://hz.zdqjudy.top/gtgbgotljx.html

TS:   public / protected / private
来源：http://hz.xinyue.icu/gtfmqobkyo.html

Java: public / protected / private / 默认包级
来源：http://hz.gaohongyu789.top/gtbduzbxcd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.gotoacloud.top/gtlsqjpdjx.html

Ruby: public / protected / private
来源：http://hz.zhongyouzk.top/gtazarcinp.html

C#:   public / protected / private / internal
来源：http://hz.tian-w.cn/gteubvuonm.html

[G11] getter / setter
来源：http://hz.daxiang520.top/gtaszpgrap.html

Py:   @property 与 @x.setter
来源：http://hz.jinghuilouyu.cn/gtqnkumnln.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.smart0.xyz/gticoxddjn.html

JS:   get name() { return this._name; }
来源：http://hz.xuetiantiany.cn/gtddtcrbpm.html

TS:   get name(): string { return this._name; }
来源：http://hz.daxiang520.top/gtxnybzbaa.html

Java: public String getName() { return name; }
来源：http://hz.52xcode.cn/gtdtpkwvgj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.fzhhl.top/gttphekfdm.html

Ruby: attr_accessor :name
来源：http://hz.cucudq.cn/gtfgfpxrbd.html

C#:   public string Name { get; set; }
来源：http://hz.fengsongda.top/gtactjalsz.html

[G12] 对象转字符串
来源：http://hz.yj202588.top/gtxeeqnmbq.html

Py:   def __str__(self): return self.name
来源：http://hz.jqgufenzy.top/gtrvflyyiz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ydjk.org.cn/gtlgwqzmtm.html

JS:   toString() { return this.name; }
来源：http://hz.sxryk.cn/gtirhivwsw.html

TS:   toString(): string { return this.name; }
来源：http://hz.smart0.xyz/gtaojwirdb.html

Java: @Override public String toString() { return name; }
来源：http://hz.xingfuxueyuan.xyz/gtybxbuibo.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jlsjyb.cn/gtqzihhmwd.html

Ruby: def to_s; @name; end
来源：http://hz.cqqwz.cn/gtnynyngxe.html

C#:   public override string ToString() => Name;
来源：http://hz.aizwys.cn/gtrtucenou.html

[G13] 判断对象类型
来源：http://hz.yj20258888.top/gtcxhncgcv.html

Py:   isinstance(u, User)
来源：http://hz.nanxuanxn.top/gtfjebikcs.html

PHP:  $u instanceof User
来源：http://hz.yanxiufei.cn/gtoadbbdio.html

JS:   u instanceof User
来源：http://hz.shangyingyoupin.top/gtkjmdebws.html

TS:   u instanceof User
来源：http://hz.52xcode.cn/gtrbsjkwud.html

Java: u instanceof User
来源：http://hz.aibaodan.cn/gtqmxkaanc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.kuanghao11.cn/gtccmmfhbp.html

Ruby: u.is_a?(User)
来源：http://hz.jinghuilouyu.cn/gtvxsovjxu.html

C#:   u is User
来源：http://hz.shanyushiyangkeji.top/gtpoqiaojo.html

[G14] 数据类 / record
来源：http://hz.zdqjudy.top/gtasspxkjb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jqgufenzy.top/gtighgxzmr.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.bjfxy.top/gtsfnjeopb.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.kuanghao11.cn/gtickixsvy.html

TS:   type User = { name: string; age: number };
来源：http://hz.chenzaomai.com/gtcxzolnuj.html

Java: record User(String name, int age) {}
来源：http://hz.nwbrower.top/gtskfzqmxa.html

Go:   type User struct { Name string; Age int }
来源：http://hz.shuidangran.top/gtqlnwxiew.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yongpay.top/gtjdrvyyst.html

C#:   record User(string Name, int Age);
来源：http://hz.dianchejie.cn/gtuxxouxjx.html

[G15] 枚举
来源：http://hz.chenlongwang.top/gtljfxjeqj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.cashguo.top/gtpmfkhips.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.gogol.net.cn/gtpyxfegfs.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.shanyushiyangkeji.top/gtilniprgg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jlsjyb.cn/gtploevsbj.html

Java: enum Color { RED, GREEN }
来源：http://hz.ydzc1.top/gtdrqrfier.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yuxming.cn/gtddzobaej.html

Ruby: Color = %i[red green].freeze
来源：http://hz.kuanghao11.cn/gtcdcftsrq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.316326.xyz/gtpxysaukf.html

[G16] 对象转数组 / 字典
来源：http://hz.birdmap.top/gtrkxinjnb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jinyuanbaomall.cn/gtwdrwyrgf.html

PHP:  get_object_vars($obj);
来源：http://hz.chenzaomai.com/gtymjmfayv.html

JS:   Object.entries(obj)
来源：http://hz.dashuyun.cn/gthplkyobh.html

TS:   Object.entries(obj)
来源：http://hz.chenzaomai.com/gtjyyxkrty.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yuxming.cn/gtuefrgtfn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.feifeiyinyue.top/gtqijjvaym.html

Ruby: obj.instance_variables
来源：http://hz.xziqi.cn/gtysuakzqv.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jiagoushi.top/gtemjgzhvv.html

================================================================================
来源：http://hz.fzhhl.top/gthojnofii.html

H. 异常与错误处理
来源：http://hz.c1oappe.top/gtwrrcxrak.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtdmtxcbaz.html

[H01] try / catch 基础
来源：http://hz.andypj.xyz/gtvttblpsu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yongpay.top/gthlohxggy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hnxiangtu.top/gtbehuzczk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.kuanghao11.cn/gtrejzswbj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.ehwqpu.com/gtvglhwapt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.chenlongwang.top/gtelcodtzz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jinqigfzy.top/gtmwrzunmm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.bjfxy.top/gtuomczfjv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.xziqi.cn/gtvoallokb.html

[H02] finally / ensure 收尾
来源：http://hz.cheryme.top/gtpatwqryj.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.cqqwz.cn/gtspnnnrha.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jqgufenzy.top/gtjjwyonon.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jinqigfzy.top/gtbwovqmwi.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.snrcjt.cn/gtpzikhaed.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.birdmap.top/gttlukgfuo.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.shanyushiyangkeji.top/gtpiraeozp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.mhx1999.top/gtvhayowep.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.svipenyu.cn/gtimlzpnfi.html

[H03] 主动抛出异常
来源：http://hz.yangfankeji.com/gtxgsntclr.html

Py:   raise ValueError("错误信息")
来源：http://hz.sxryk.cn/gtntikuijd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.fengsongda.top/gtrzfwlgjg.html

JS:   throw new Error("错误信息");
来源：http://hz.zycfv.cn/gtyrlhddke.html

TS:   throw new Error("错误信息");
来源：http://hz.vqdsnc.cn/gtwzveghsu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.cheryme.top/gtcwzvfrxn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.cqqwz.cn/gtgadlzwra.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.tanke756.top/gtyduptwnx.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.vqdsnc.cn/gtqnrhockm.html

[H04] 自定义异常类型
来源：http://hz.tanke756.top/gtuehfatqz.html

Py:   class MyError(Exception): pass
来源：http://hz.zhongyouzk.top/gttigcqglp.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.chenlongwang.top/gtynphwsgi.html

JS:   class MyError extends Error {}
来源：http://hz.hysaishi.cn/gteuewauvy.html

TS:   class MyError extends Error {}
来源：http://hz.ivvv.top/gtdpvyohwx.html

Java: class MyException extends RuntimeException {}
来源：http://hz.havefunace.top/gtexofmsep.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.aizwys.cn/gtqajwjucz.html

Ruby: class MyError < StandardError; end
来源：http://hz.haohaochexian.top/gtplfisugo.html

C#:   class MyException : Exception {}
来源：http://hz.nwbrower.top/gtgharsgoi.html

[H05] 捕获特定类型
来源：http://hz.shanyushiyangkeji.top/gtcpidsftr.html

Py:   except ValueError as e:
来源：http://hz.chenzaomai.com/gtrmnngcmp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yueranfly.top/gthmdkjrzq.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.smart0.xyz/gtjflkguwv.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.smart0.xyz/gtiyzjihgg.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yuanzhike.top/gtasnababh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yongpay.top/gtvqqyigpi.html

Ruby: rescue ArgumentError => e
来源：http://hz.vqdsnc.cn/gttdwwqnat.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.daxiang520.top/gtasnhzrsx.html

[H06] 可选值 / 空值安全访问
来源：http://hz.tianlin.xyz/gtykxjymbf.html

Py:   value = d.get("k") or default
来源：http://hz.zycfv.cn/gttuslgexg.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.nanxuanxn.top/gtaypgfwpf.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.andypj.xyz/gtethmjidi.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.xinyue.icu/gtzaglxlzz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ybcxt.top/gtaxwekifo.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.xylfe.cn/gtlfkuftye.html

Ruby: d&.dig(:a, :b)
来源：http://hz.chenjidiqi.icu/gtoqqnipsi.html

C#:   obj?.A?.B ?? default
来源：http://hz.nanxuanxn.top/gttyixkxpo.html

[H07] 断言
来源：http://hz.havefunace.top/gtjoxvnbqa.html

Py:   assert x > 0, "必须为正"
来源：http://hz.ehwqpu.com/gtsyofqzwx.html

PHP:  assert($x > 0);
来源：http://hz.yj20258888.top/gtbavnbngx.html

JS:   console.assert(x > 0);
来源：http://hz.gogol.net.cn/gtkougybtj.html

TS:   console.assert(x > 0);
来源：http://hz.aizwys.cn/gttqlrwzkd.html

Java: assert x > 0 : "必须为正";
来源：http://hz.cqqwz.cn/gtgbbmpndu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.chenzaomai.com/gtonachuij.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hongshengwenyu.top/gtmhemgjni.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zdqjudy.top/gttilogkjc.html

[H08] 获取错误信息与堆栈
来源：http://hz.shanyushiyangtech.top/gtsajulwwd.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.hongshengwenyu.top/gtkgbcfofk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.nanxuanxn.top/gtpuaticum.html

JS:   e.message;  e.stack
来源：http://hz.fzhhl.top/gtbcjggzdg.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.shanyushiyangkeji.top/gtkbtkrrms.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.dianchejie.cn/gtcvodwusr.html

Go:   err.Error()
来源：http://hz.shangyingyoupin.top/gtmbnsvgmc.html


<!-- 参考信息 -->