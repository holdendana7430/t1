代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.cqqwz.cn/gtignigeky.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.zhengqikj.top/gtuhmnxvhi.html

[F03] 写入文件（覆盖）
来源：http://hz.jinyuanbaomall.cn/gtajhlyxsn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.sweek.top/gtfwmzyxdm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.hfpthk.cn/gtawxjpfoi.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cheryme.top/gtldfmmuxf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xinyue.icu/gtarlhchaf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.fengsongda.top/gtaonoazoj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jqgfzy.top/gtmkkbngxf.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yvedp.cn/gtbnbnujro.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.0kj1m.cn/gtbjwqfqao.html

[F04] 追加写入文件
来源：http://hz.yj202588.top/gtkzjdglfn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.shuidangran.top/gtbgdmehon.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.hywenlv.cn/gtzcpvfulw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ivvv.top/gtrkownpzp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yj202588.top/gtphubsmzy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.snrcjt.cn/gtjhpryops.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.cheryme.top/gtgdbuqxor.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.xingfuxueyuan.xyz/gtkudfqhrw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.zhoulong.xyz/gtjhqgkpsd.html

[F05] 判断文件或目录是否存在
来源：http://hz.yuxming.cn/gtnsvpivkq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.daxiang520.top/gtfvnujksi.html

PHP:  file_exists("a.txt");
来源：http://hz.iojbl.cn/gtsuzyaiid.html

JS:   fs.existsSync("a.txt")
来源：http://hz.wangshuangyany.cn/gtxmadqofb.html

TS:   fs.existsSync("a.txt")
来源：http://hz.ydjk.org.cn/gtgpkctgwf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jlsjyb.cn/gttpyebtdz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.snrcjt.cn/gtuschmlnd.html

Ruby: File.exist?("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtotowxcvz.html

C#:   File.Exists("a.txt")
来源：http://hz.birdmap.top/gtntpwdxnz.html

[F06] 删除文件
来源：http://hz.yj20258.top/gtqcimmruq.html

Py:   os.remove("a.txt")
来源：http://hz.ydjk.org.cn/gtiybmgbif.html

PHP:  unlink("a.txt");
来源：http://hz.jyoumei.cn/gtwqoqaonr.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yangfankeji.com/gtyffxncox.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.gogol.net.cn/gtwantjdpq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.gzhubu.top/gtaareylrt.html

Go:   os.Remove("a.txt")
来源：http://hz.ywan-chungtsiang.top/gttvmpmxki.html

Ruby: File.delete("a.txt")
来源：http://hz.shanyushiyangtech.top/gtetjtqfzs.html

C#:   File.Delete("a.txt");
来源：http://hz.yj20258.top/gtcmhmsgla.html

[F07] 创建目录（含多级）
来源：http://hz.nwbrower.top/gtalwueecp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yuanzhike.top/gtsvwcfyxn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jlsjyb.cn/gtemdpsisb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.gaohongyu789.top/gtqnneuvah.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.haohaochexian.top/gtbkbhbaxj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.nwbrower.top/gtcewpvdlr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zhoulong.xyz/gttnoddutp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.daria6918.cn/gtdnadakrk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.haohaochexian.top/gtyguuwbga.html

[F08] 遍历目录
来源：http://hz.sysykeji.top/gtsytswubi.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.316326.xyz/gtuefsflnh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.smart0.xyz/gtlsgrhvkc.html

JS:   fs.readdirSync("dir")
来源：http://hz.cashguo.top/gtfedgjzuh.html

TS:   fs.readdirSync("dir")
来源：http://hz.pengpengdd.cyou/gtzroaabti.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zhongyouzk.top/gtctdqggzi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.cashguo.top/gtfxwgbkuj.html

Ruby: Dir.children("dir")
来源：http://hz.zhongyouzk.top/gthgmsvymh.html

C#:   Directory.GetFiles("dir")
来源：http://hz.wangdashe.top/gtcuulhhdu.html

[F09] 获取文件大小
来源：http://hz.dashuyun.cn/gthzurfepv.html

Py:   os.path.getsize("a.txt")
来源：http://hz.fzhhl.top/gtunqtgwax.html

PHP:  filesize("a.txt");
来源：http://hz.ehwqpu.com/gtcrcdqyjh.html

JS:   fs.statSync("a.txt").size
来源：http://hz.dashuyun.cn/gtwqymszpa.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zhaomingkeji.xyz/gtqxjhwvta.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.iojbl.cn/gtrhccexgy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yangfankeji.com/gtgcdustyl.html

Ruby: File.size("a.txt")
来源：http://hz.xinyue.icu/gtsctoedyy.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.bjfxy.top/gtbtlbetax.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.havefunace.top/gtgwgnujws.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.guowangkeji.top/gtwukranpp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.daria6918.cn/gtiyaqbhft.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.feifeiyinyue.top/gttdzlqflz.html

TS:   path.extname("a.txt")
来源：http://hz.guowangkeji.top/gtvzbrmiim.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.mhx1999.top/gtdezhbprv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.cdnleiting.top/gtvykqdsut.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.gzhubu.top/gtoflrvuez.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.0kj1m.cn/gtpvntknrz.html

[F11] 复制与移动文件
来源：http://hz.zdqjudy.top/gtnzwjrxys.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.tian-w.cn/gtoybuqhab.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.pycfn.com/gtvuoerxxw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.daxiang520.top/gtqjrywaxi.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sysykeji.top/gtbxxugfvd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yueranfly.top/gtqxdzptlk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.cqqwz.cn/gttzqnyipq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.feifeiyinyue.top/gtssyeztft.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.gaohongyu789.top/gtvebljfcp.html

[F12] CSV 读写
来源：http://hz.zhiwuduotai.top/gtksswgqgf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.gotoacloud.top/gtspizqspl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.ehwqpu.com/gtdnphlnvp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zdqjudy.top/gtkopuhael.html

TS:   // 同上
来源：http://hz.hysaishi.cn/gtwuxbtywn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.dashuyun.cn/gtaxiaoflk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.meibo888.top/gtzkhmucwq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jinqigufen.top/gthrfsobwr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yj20258.top/gtjoephrlb.html

================================================================================
来源：http://hz.jinqigufen.top/gtfkbeaalp.html

G. 面向对象
来源：http://hz.jyoumei.cn/gtberypztj.html

================================================================================
来源：http://hz.yj20258888.top/gtzmfgrkvq.html

[G01] 定义类
来源：http://hz.ppjwa.cn/gtmcwfiunn.html

Py:   class User: pass
来源：http://hz.zycfv.cn/gtihatdpme.html

PHP:  class User {}
来源：http://hz.hfpthk.cn/gttyohxghl.html

JS:   class User {}
来源：http://hz.zhaomingkeji.xyz/gtytoehepg.html

TS:   class User { name: string = ""; }
来源：http://hz.jinghuilouyu.cn/gticinylov.html

Java: class User {}
来源：http://hz.redwolf501.top/gtauptwryj.html

Go:   type User struct { Name string }
来源：http://hz.zhixingplan.top/gtrloycuwa.html

Ruby: class User; end
来源：http://hz.yj20258.top/gtbjsutnzp.html

C#:   class User {}
来源：http://hz.gotoacloud.top/gtrigwzjkg.html

[G02] 构造函数
来源：http://hz.ppjwa.cn/gttgolgefv.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.cqqwz.cn/gtkmnqxjsv.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.wangdashe.top/gtzudwqxjx.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.ydjk.org.cn/gthughjsjk.html

TS:   constructor(public name: string) {}
来源：http://hz.yonumen.top/gtjnsttjng.html

Java: User(String name) { this.name = name; }
来源：http://hz.shzxlz.cn/gtnguspnbp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zhixingplan.top/gtxkbreync.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.vqdsnc.cn/gtaxrgvbnk.html

C#:   public User(string name) { Name = name; }
来源：http://hz.birdmap.top/gtbqsqlaty.html

[G03] 实例属性
来源：http://hz.pengpengdd.cyou/gttdfvemsm.html

Py:   self.name = "x"
来源：http://hz.aibaodan.cn/gtgcodmjop.html

PHP:  public string $name = "x";
来源：http://hz.guannengcc.top/gtvydmozxe.html

JS:   this.name = "x";
来源：http://hz.yonumen.top/gthcquynor.html

TS:   name: string = "x";
来源：http://hz.sysykeji.top/gtpjnildqn.html

Java: private String name;
来源：http://hz.yonumen.top/gtovqzpinu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yj20258.top/gtnvfimmes.html

Ruby: @name = "x"
来源：http://hz.shuidangran.top/gtvdnljwqf.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.cqqwz.cn/gtdjhjoisk.html

[G04] 定义方法
来源：http://hz.yj20258.top/gthntwhfxl.html

Py:   def greet(self): return self.name
来源：http://hz.chenjidiqi.icu/gtsqkmdxtw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yongpay.top/gtyakqyhqi.html

JS:   greet() { return this.name; }
来源：http://hz.yangfankeji.com/gtgvofncrc.html

TS:   greet(): string { return this.name; }
来源：http://hz.cucudq.cn/gtekmoqouq.html

Java: String greet() { return name; }
来源：http://hz.jianghu66.top/gtfgfxiyyj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.gzhubu.top/gtdttljlwy.html

Ruby: def greet; @name; end
来源：http://hz.nanxuanxn.top/gtoawxwshj.html

C#:   public string Greet() => Name;
来源：http://hz.jianghu66.top/gtcawrkenp.html

[G05] 继承
来源：http://hz.hnxiangtu.top/gtnciibbso.html

Py:   class Admin(User): pass
来源：http://hz.aizwys.cn/gtqvkwirwm.html

PHP:  class Admin extends User {}
来源：http://hz.iojbl.cn/gtwrgdajwp.html

JS:   class Admin extends User {}
来源：http://hz.dianchejie.cn/gtwsneqrtu.html

TS:   class Admin extends User {}
来源：http://hz.wangdashe.top/gtwupmpzcl.html

Java: class Admin extends User {}
来源：http://hz.c1oappe.top/gttezxxyzw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zhoulong.xyz/gtrmqtyfre.html

Ruby: class Admin < User; end
来源：http://hz.wangshuangyany.cn/gtqovopgbv.html

C#:   class Admin : User {}
来源：http://hz.sysykeji.top/gtlwwcwwwe.html

[G06] 重写方法
来源：http://hz.ybcxt.top/gtlwrguqfs.html

Py:   def greet(self): return "admin"
来源：http://hz.sysykeji.top/gtdwtqhoxp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.daria6918.cn/gtmceqhgaz.html

JS:   greet() { return "admin"; }
来源：http://hz.feifeiyinyue.top/gtfkztjjza.html

TS:   greet(): string { return "admin"; }
来源：http://hz.ydzc1.top/gtvkmmivnv.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.shangyingyoupin.top/gtfgmilitw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.xuanzx.com/gtcistbnbd.html

Ruby: def greet; "admin"; end
来源：http://hz.chenlongwang.top/gtyzlalqdq.html

C#:   public override string Greet() => "admin";
来源：http://hz.hywenlv.cn/gttkltecxy.html

[G07] 调用父类方法
来源：http://hz.tanke756.top/gtoiwjkaxt.html

Py:   super().greet()
来源：http://hz.feifeiyinyue.top/gtvszvdjsh.html

PHP:  parent::greet();
来源：http://hz.yvedp.cn/gtcftakgcy.html

JS:   super.greet();
来源：http://hz.nwbrower.top/gtztbgzpvg.html

TS:   super.greet();
来源：http://hz.gotoacloud.top/gtphcvhzmq.html

Java: super.greet();
来源：http://hz.yvedp.cn/gtcdeixdzi.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.316326.xyz/gtlughwioa.html

Ruby: super
来源：http://hz.nanxuanxn.top/gttthmygso.html

C#:   base.Greet();
来源：http://hz.zdqjudy.top/gtgjtylaav.html

[G08] 静态方法与属性
来源：http://hz.cdnleiting.top/gtoxhyvwuc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhaomingkeji.xyz/gtkvwwhhrm.html

PHP:  public static function f() {}
来源：http://hz.0kj1m.cn/gtypciwnff.html

JS:   static f() {}
来源：http://hz.yangfankeji.com/gtxpmwkfcm.html

TS:   static f(): void {}
来源：http://hz.daxiang520.top/gtkvwxijbs.html

Java: static void f() {}
来源：http://hz.52xcode.cn/gtlztasnnn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yj20258.top/gttttuixdf.html

Ruby: def self.f; end
来源：http://hz.quarkkingdee.top/gtkowuvvxp.html

C#:   public static void F() {}
来源：http://hz.smart0.xyz/gttwaycwzu.html

[G09] 接口 / 抽象类
来源：http://hz.9152youxi.cn/gtnhihbccj.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zhongyouzk.top/gtjtoihsvd.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.fengsongda.top/gtusyxxkdy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zycfv.cn/gtxorxbbnj.html

TS:   interface Shape { area(): number; }
来源：http://hz.ydjk.org.cn/gtyaegvhiz.html

Java: interface Shape { double area(); }
来源：http://hz.52xcode.cn/gtyvveuvan.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.shanyushiyangtech.top/gtrxdvtnny.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hysaishi.cn/gtkkonulik.html

C#:   interface IShape { double Area(); }
来源：http://hz.svipenyu.cn/gtmnvlsyff.html

[G10] 访问控制
来源：http://hz.quarkkingdee.top/gtipdtsocw.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yj20258.top/gtcimbsols.html

PHP:  public / protected / private
来源：http://hz.bjfxy.top/gtkriwkjcl.html

JS:   #private 字段；其余公开
来源：http://hz.feifeiyinyue.top/gtidhkkspe.html

TS:   public / protected / private
来源：http://hz.ybcxt.top/gtyzqzveey.html

Java: public / protected / private / 默认包级
来源：http://hz.cheryme.top/gtuumienvu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.smart0.xyz/gtnsbaizgr.html

Ruby: public / protected / private
来源：http://hz.9152youxi.cn/gtlekvvvte.html

C#:   public / protected / private / internal
来源：http://hz.hywenlv.cn/gtjebdctmg.html

[G11] getter / setter
来源：http://hz.316326.xyz/gtgswwpouo.html

Py:   @property 与 @x.setter
来源：http://hz.daxiang520.top/gtdxkvclil.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.hywenlv.cn/gtdjjnizrn.html

JS:   get name() { return this._name; }
来源：http://hz.havefunace.top/gteaznyynh.html

TS:   get name(): string { return this._name; }
来源：http://hz.jinghuilouyu.cn/gtzcwbgket.html

Java: public String getName() { return name; }
来源：http://hz.jinghuilouyu.cn/gtlqtbuios.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.gogol.net.cn/gtvokhwegx.html

Ruby: attr_accessor :name
来源：http://hz.iojbl.cn/gtdzsxfakg.html

C#:   public string Name { get; set; }
来源：http://hz.shanyushiyangkeji.top/gtddglvcte.html

[G12] 对象转字符串
来源：http://hz.zhiwuduotai.top/gtyymnnlgc.html

Py:   def __str__(self): return self.name
来源：http://hz.jlsjyb.cn/gtqbpsmlwb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yuanzhike.top/gttqtupnjz.html

JS:   toString() { return this.name; }
来源：http://hz.ybcxt.top/gtvlwgnvwe.html

TS:   toString(): string { return this.name; }
来源：http://hz.aizwys.cn/gtsmbifqda.html

Java: @Override public String toString() { return name; }
来源：http://hz.316326.xyz/gtmvoeunsy.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yj20258888.top/gtpynchtuy.html

Ruby: def to_s; @name; end
来源：http://hz.feifeiyinyue.top/gtyblfrwdi.html

C#:   public override string ToString() => Name;
来源：http://hz.ywan-chungtsiang.top/gtaosqqwtu.html

[G13] 判断对象类型
来源：http://hz.jianghu66.top/gtetopyfjx.html

Py:   isinstance(u, User)
来源：http://hz.shanyushiyangkeji.top/gtkjnyedyo.html

PHP:  $u instanceof User
来源：http://hz.shanyushiyangkeji.top/gtbmeoipbd.html

JS:   u instanceof User
来源：http://hz.snrcjt.cn/gtdebxceda.html

TS:   u instanceof User
来源：http://hz.hnxiangtu.top/gtznnxsrge.html

Java: u instanceof User
来源：http://hz.yueranfly.top/gtzyrxanpf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.daria6918.cn/gtmicoygjw.html

Ruby: u.is_a?(User)
来源：http://hz.guannengcc.top/gtefdmiobe.html

C#:   u is User
来源：http://hz.chenzaomai.com/gttrvpnqlp.html

[G14] 数据类 / record
来源：http://hz.316326.xyz/gthdedofvo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.tianlin.xyz/gtfnvebfkq.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.gotoacloud.top/gtxvkktars.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.gzhubu.top/gttoenwuja.html

TS:   type User = { name: string; age: number };
来源：http://hz.sufxvd.cn/gtmkympumj.html

Java: record User(String name, int age) {}
来源：http://hz.jqgfzy.top/gtzzaexovi.html

Go:   type User struct { Name string; Age int }
来源：http://hz.xylfe.cn/gtuufmraif.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yj20258888.top/gtvqgwibpf.html

C#:   record User(string Name, int Age);
来源：http://hz.tian-w.cn/gtmyxnndlb.html

[G15] 枚举
来源：http://hz.jlsjyb.cn/gtejlxsggd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.dashuyun.cn/gtzdtrlsje.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yj20258.top/gtipwocpah.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.0kj1m.cn/gtjagmejzl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ydjk.org.cn/gtcprwbvqy.html

Java: enum Color { RED, GREEN }
来源：http://hz.sxryk.cn/gtvxxabqua.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.shanyushiyangtech.top/gtxjvfoxir.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ydjk.org.cn/gtquiysbxo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xuanzx.com/gtyupudrye.html

[G16] 对象转数组 / 字典
来源：http://hz.jinghuilouyu.cn/gtfcgmhdcr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.guannengcc.top/gtebxlvzlb.html

PHP:  get_object_vars($obj);
来源：http://hz.mhx1999.top/gtzlbrhgrj.html

JS:   Object.entries(obj)
来源：http://hz.yj20258.top/gtwiomntlc.html

TS:   Object.entries(obj)
来源：http://hz.yongpay.top/gtagbwtrpu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jianghu66.top/gtzfldnalo.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.zhengqikj.top/gtkkeshxwb.html

Ruby: obj.instance_variables
来源：http://hz.mhx1999.top/gtywftbvac.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yj202588.top/gtoqwqocmc.html

================================================================================
来源：http://hz.zhengqikj.top/gtqnmwhonk.html

H. 异常与错误处理
来源：http://hz.zhaomingkeji.xyz/gthkbjfyrc.html

================================================================================
来源：http://hz.quarkkingdee.top/gtvvamosih.html

[H01] try / catch 基础
来源：http://hz.c1oappe.top/gtpktpqgie.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.cucudq.cn/gtbpjvwzxr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zhijiandao.cn/gtynvyuhki.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yangfankeji.com/gtddyjyyrb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.sysykeji.top/gtoumfjjbv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ybcxt.top/gtmcvykazs.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.gotoacloud.top/gtnicsfvew.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.gogol.net.cn/gtshonwkej.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.hnqzz.top/gtkxjpmjsx.html

[H02] finally / ensure 收尾
来源：http://hz.tianlin.xyz/gtbhxilsbn.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zhaomingkeji.xyz/gtguazuwff.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jqgfzy.top/gtwyisagut.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.havefunace.top/gtvdyqjenu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.tianlin.xyz/gtuafttngi.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.havefunace.top/gtzoxwdfgs.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ydzc1.top/gtlcbbmpba.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.gotoacloud.top/gtzgxgwyse.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yj20258888.top/gtsnkqnbek.html

[H03] 主动抛出异常
来源：http://hz.xziqi.cn/gtntscgebe.html

Py:   raise ValueError("错误信息")
来源：http://hz.hywenlv.cn/gtmytxhuch.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.mhx1999.top/gtowtxptwd.html

JS:   throw new Error("错误信息");
来源：http://hz.yuanzhike.top/gtpewqliji.html

TS:   throw new Error("错误信息");
来源：http://hz.jianghu66.top/gtnnmsifdm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.havefunace.top/gtalhrampg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hammf.cn/gtatopgmks.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.dianchejie.cn/gtqybfnzbk.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.gogol.net.cn/gthlbeuipl.html

[H04] 自定义异常类型
来源：http://hz.zhijiandao.cn/gtizwbfgpi.html

Py:   class MyError(Exception): pass
来源：http://hz.xinyue.icu/gtcfamismk.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yj202588.top/gthvygcqle.html

JS:   class MyError extends Error {}
来源：http://hz.jqgufenzy.top/gtorosqvsk.html

TS:   class MyError extends Error {}
来源：http://hz.zhoulong.xyz/gtbpilpcrv.html

Java: class MyException extends RuntimeException {}
来源：http://hz.chenjidiqi.icu/gtovydixjb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.birdmap.top/gtiyyoevyv.html

Ruby: class MyError < StandardError; end
来源：http://hz.jianghu66.top/gtvetxwokq.html

C#:   class MyException : Exception {}
来源：http://hz.wangdashe.top/gtyjeumoas.html

[H05] 捕获特定类型
来源：http://hz.52xcode.cn/gtlhbrgami.html

Py:   except ValueError as e:
来源：http://hz.jqgufenzy.top/gtduidqynv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yangfankeji.com/gtebwbssry.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zhengqikj.top/gtzoxtogyw.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yj20258.top/gtueezenpt.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.kuanghao11.cn/gtggomodsq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zhaomingkeji.xyz/gtyuhbawum.html

Ruby: rescue ArgumentError => e
来源：http://hz.yonumen.top/gthfcpbnpi.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhixingplan.top/gtrtcqwmip.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yueranfly.top/gthimrxigt.html

Py:   value = d.get("k") or default
来源：http://hz.guannengcc.top/gtreoboyhc.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.daxiang520.top/gtibxoduot.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.cheryme.top/gtyobvqwph.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.birdmap.top/gteweazmae.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yueranfly.top/gthrmchxiu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.gaohongyu789.top/gtgfwhkygz.html

Ruby: d&.dig(:a, :b)
来源：http://hz.wangdashe.top/gtoebtrded.html

C#:   obj?.A?.B ?? default
来源：http://hz.ivvv.top/gtpgrbxjbk.html

[H07] 断言
来源：http://hz.316326.xyz/gteyimzdil.html

Py:   assert x > 0, "必须为正"
来源：http://hz.dashuyun.cn/gtaidoixiw.html

PHP:  assert($x > 0);
来源：http://hz.daria6918.cn/gtkyvlmnbm.html

JS:   console.assert(x > 0);
来源：http://hz.daria6918.cn/gtfrqaujgh.html


<!-- 参考信息 -->