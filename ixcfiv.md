代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yueranfly.top/gtrkrqymnl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.chenlongwang.top/gtvgjqrztr.html

[F03] 写入文件（覆盖）
来源：http://hz.xziqi.cn/gtqhnppkuh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jlsjyb.cn/gtbjninufa.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.ppjwa.cn/gtynyibavn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.haohaochexian.top/gtxggpodpl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.nwbrower.top/gttyjlkvrb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.c1oappe.top/gtcmvrotul.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yangfankeji.com/gtanuuhxux.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.guannengcc.top/gtnrrgrgaa.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.wangshuangyany.cn/gtcnttftcv.html

[F04] 追加写入文件
来源：http://hz.chenjidiqi.icu/gtjqjzlvxw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jqgufenzy.top/gthyggxeen.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.mhx1999.top/gtywntbibr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.dianchejie.cn/gtgtscutou.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.andypj.xyz/gtwqaveoxw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.gzhubu.top/gtbfjazanu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.nwbrower.top/gthjzpmrym.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.tian-w.cn/gtemheulkr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yongpay.top/gttirjylby.html

[F05] 判断文件或目录是否存在
来源：http://hz.xingfuxueyuan.xyz/gtzzxyxhxo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.fzhhl.top/gtucysuqah.html

PHP:  file_exists("a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtmdtefycb.html

JS:   fs.existsSync("a.txt")
来源：http://hz.zhoulong.xyz/gtvzlrmgkq.html

TS:   fs.existsSync("a.txt")
来源：http://hz.wangdashe.top/gtyvvqoxwk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jinqigufen.top/gttwwklnqk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yj20258.top/gtsqmqnohw.html

Ruby: File.exist?("a.txt")
来源：http://hz.wangdashe.top/gtyseyiaiw.html

C#:   File.Exists("a.txt")
来源：http://hz.nanxinkj.top/gtfgtbviuw.html

[F06] 删除文件
来源：http://hz.aibaodan.cn/gtefeoecnb.html

Py:   os.remove("a.txt")
来源：http://hz.gaohongyu789.top/gtgwuxutsv.html

PHP:  unlink("a.txt");
来源：http://hz.xuetiantiany.cn/gtrxplseqr.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.316326.xyz/gtfuxzfawg.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.ivvv.top/gthkfisqfm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.dashuyun.cn/gtzoddgxap.html

Go:   os.Remove("a.txt")
来源：http://hz.cheryme.top/gtapmchfik.html

Ruby: File.delete("a.txt")
来源：http://hz.yj20258888.top/gtaidkmpvi.html

C#:   File.Delete("a.txt");
来源：http://hz.feifeiyinyue.top/gtucjmnoyz.html

[F07] 创建目录（含多级）
来源：http://hz.zdqjudy.top/gtjmipvpbh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yj202588.top/gtjgjqctuq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.mhx1999.top/gtjqmsprrn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yanxiufei.cn/gtyktkddrf.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yj202588.top/gtcmvhkhoj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.aibaodan.cn/gtsnfunxqs.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.shuidangran.top/gtwlkitroi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.chenjidiqi.icu/gtuyrxnnlz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.tanke756.top/gtabxjziuh.html

[F08] 遍历目录
来源：http://hz.svipenyu.cn/gtpwkonnff.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.guannengcc.top/gtjjcegjxi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.wangdashe.top/gtadllgndx.html

JS:   fs.readdirSync("dir")
来源：http://hz.xuanzx.com/gtvvphsygp.html

TS:   fs.readdirSync("dir")
来源：http://hz.xylfe.cn/gttywtqbwe.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.smart0.xyz/gtyzhwmief.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.cheryme.top/gtohswlhjj.html

Ruby: Dir.children("dir")
来源：http://hz.nanxuanxn.top/gtqdqxxasp.html

C#:   Directory.GetFiles("dir")
来源：http://hz.gaohongyu789.top/gtntqqgdfw.html

[F09] 获取文件大小
来源：http://hz.sweek.top/gtdyicagjq.html

Py:   os.path.getsize("a.txt")
来源：http://hz.cashguo.top/gtfhqrlkub.html

PHP:  filesize("a.txt");
来源：http://hz.daria6918.cn/gtswbbkmdq.html

JS:   fs.statSync("a.txt").size
来源：http://hz.haohaochexian.top/gtrpgfwkof.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jinyuanbaomall.cn/gtmklmowll.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zhiwuduotai.top/gtoskmsitt.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.shangyingyoupin.top/gtzadineaj.html

Ruby: File.size("a.txt")
来源：http://hz.yj20258.top/gtunjsxdor.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.sxryk.cn/gtpjtgxang.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.xylfe.cn/gtzooldtvd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yj202588.top/gtbymhwdno.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.hysaishi.cn/gtcghytjki.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.ybcxt.top/gtnvsgqfqb.html

TS:   path.extname("a.txt")
来源：http://hz.smart0.xyz/gtsmoostqx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yueranfly.top/gtyfqknaeg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.shangyingyoupin.top/gtkewkefvi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.hywenlv.cn/gtgafgtpla.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.9152youxi.cn/gtfrggmvdw.html

[F11] 复制与移动文件
来源：http://hz.fzhhl.top/gtryfmpvsv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.gaohongyu789.top/gtqekulcme.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.daria6918.cn/gtujwpmbbb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhengqikj.top/gtwaeozdja.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.gzhubu.top/gtraykmnmu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.xylfe.cn/gtbdyzqhmc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yuxming.cn/gttnoyiepx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.cheryme.top/gtkshrksip.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.shuidangran.top/gtpdcetwzq.html

[F12] CSV 读写
来源：http://hz.guannengcc.top/gtwvmqlbsn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jinqigfzy.top/gtowihdftm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.haohaochexian.top/gtfnpvmqmt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yangfankeji.com/gtqwcyoizd.html

TS:   // 同上
来源：http://hz.9152youxi.cn/gtdddypxsu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.tanke756.top/gteraelsxq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zycfv.cn/gtistkmlhk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ivvv.top/gtdhxdizld.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yuanzhike.top/gtmagnfcsq.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtoprhvvzi.html

G. 面向对象
来源：http://hz.cqqwz.cn/gtgbyvqdac.html

================================================================================
来源：http://hz.0kj1m.cn/gtbimehjym.html

[G01] 定义类
来源：http://hz.daria6918.cn/gtxjqxdtwt.html

Py:   class User: pass
来源：http://hz.yongpay.top/gtpwiixhav.html

PHP:  class User {}
来源：http://hz.yongpay.top/gtjqreufbd.html

JS:   class User {}
来源：http://hz.shuidangran.top/gtqbskteua.html

TS:   class User { name: string = ""; }
来源：http://hz.daxiang520.top/gtiurwyjef.html

Java: class User {}
来源：http://hz.dianchejie.cn/gtmowniktc.html

Go:   type User struct { Name string }
来源：http://hz.guowangkeji.top/gtrtxpbbjy.html

Ruby: class User; end
来源：http://hz.pycfn.com/gtyehkoqlk.html

C#:   class User {}
来源：http://hz.jyoumei.cn/gthtozheqx.html

[G02] 构造函数
来源：http://hz.9152youxi.cn/gtnxumdfrv.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.hammf.cn/gtcqcgfrko.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.gaohongyu789.top/gtbryccjri.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yvedp.cn/gtvwggqsyq.html

TS:   constructor(public name: string) {}
来源：http://hz.wangdashe.top/gtqjhsuphb.html

Java: User(String name) { this.name = name; }
来源：http://hz.jlsjyb.cn/gtgvwigtqd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hfpthk.cn/gtztgfuwru.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.aibaodan.cn/gtkhmwrzfd.html

C#:   public User(string name) { Name = name; }
来源：http://hz.sweek.top/gtoqvajjvi.html

[G03] 实例属性
来源：http://hz.daria6918.cn/gtqiyiuzcz.html

Py:   self.name = "x"
来源：http://hz.jinyuanbaomall.cn/gtxwlffxzk.html

PHP:  public string $name = "x";
来源：http://hz.yanxiufei.cn/gtxpxwwsqh.html

JS:   this.name = "x";
来源：http://hz.jlsjyb.cn/gtyxyhoytv.html

TS:   name: string = "x";
来源：http://hz.redwolf501.top/gtxxounksn.html

Java: private String name;
来源：http://hz.redwolf501.top/gtlgvzrost.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yvedp.cn/gtvhtrnizb.html

Ruby: @name = "x"
来源：http://hz.fengsongda.top/gtnmppmrmq.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.mhx1999.top/gtottwamrg.html

[G04] 定义方法
来源：http://hz.bjfxy.top/gtqyheqdgl.html

Py:   def greet(self): return self.name
来源：http://hz.zdqjudy.top/gtcsnwzvpf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.redwolf501.top/gtxyetavet.html

JS:   greet() { return this.name; }
来源：http://hz.nanxinkj.top/gtzauwinmk.html

TS:   greet(): string { return this.name; }
来源：http://hz.aizwys.cn/gtjhmuruqk.html

Java: String greet() { return name; }
来源：http://hz.gzhubu.top/gtdverqmov.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.shanyushiyangtech.top/gtpnqnrzvw.html

Ruby: def greet; @name; end
来源：http://hz.sweek.top/gtfidrqbji.html

C#:   public string Greet() => Name;
来源：http://hz.tianlin.xyz/gtumvnecvz.html

[G05] 继承
来源：http://hz.jlsjyb.cn/gtdafvtlzt.html

Py:   class Admin(User): pass
来源：http://hz.daxiang520.top/gtibebcraq.html

PHP:  class Admin extends User {}
来源：http://hz.smart0.xyz/gtgafsgcxk.html

JS:   class Admin extends User {}
来源：http://hz.jyoumei.cn/gtoycdloae.html

TS:   class Admin extends User {}
来源：http://hz.zhongyouzk.top/gthgnmykrv.html

Java: class Admin extends User {}
来源：http://hz.nwbrower.top/gtqcckymth.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zhaomingkeji.xyz/gtghdossme.html

Ruby: class Admin < User; end
来源：http://hz.9152youxi.cn/gtmjzzfaqu.html

C#:   class Admin : User {}
来源：http://hz.zhengqikj.top/gtbmmyomhu.html

[G06] 重写方法
来源：http://hz.hysaishi.cn/gtwvhvfnpr.html

Py:   def greet(self): return "admin"
来源：http://hz.guannengcc.top/gtboyoutjh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.xuetiantiany.cn/gtwhkoujaj.html

JS:   greet() { return "admin"; }
来源：http://hz.ivvv.top/gtmoknjpui.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jlsjyb.cn/gtmncfutvx.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yonumen.top/gtoqmufjse.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.feifeiyinyue.top/gttjriincm.html

Ruby: def greet; "admin"; end
来源：http://hz.wangdashe.top/gtukyltdhi.html

C#:   public override string Greet() => "admin";
来源：http://hz.hfpthk.cn/gtpiwqgtri.html

[G07] 调用父类方法
来源：http://hz.gotoacloud.top/gtfcaoxwym.html

Py:   super().greet()
来源：http://hz.jyoumei.cn/gtaqjwlrrc.html

PHP:  parent::greet();
来源：http://hz.gogol.net.cn/gtepmdvgwh.html

JS:   super.greet();
来源：http://hz.yonumen.top/gtevetkivk.html

TS:   super.greet();
来源：http://hz.hongshengwenyu.top/gtrdnhzofy.html

Java: super.greet();
来源：http://hz.dianchejie.cn/gtpcnhnaru.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.xziqi.cn/gtysjfsynq.html

Ruby: super
来源：http://hz.jqgfzy.top/gtbywcsppl.html

C#:   base.Greet();
来源：http://hz.zhixingplan.top/gtwbxvfews.html

[G08] 静态方法与属性
来源：http://hz.zhengqikj.top/gtglorqvif.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.andypj.xyz/gtvyxwbiey.html

PHP:  public static function f() {}
来源：http://hz.snrcjt.cn/gtyvxamuyr.html

JS:   static f() {}
来源：http://hz.ybcxt.top/gtynzesqod.html

TS:   static f(): void {}
来源：http://hz.0kj1m.cn/gtfsncxzvb.html

Java: static void f() {}
来源：http://hz.cqqwz.cn/gtwodsrcrb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.guannengcc.top/gtdjahshwr.html

Ruby: def self.f; end
来源：http://hz.yj20258888.top/gtajmqxpzy.html

C#:   public static void F() {}
来源：http://hz.zhiwuduotai.top/gtmnryhvls.html

[G09] 接口 / 抽象类
来源：http://hz.nanxinkj.top/gtqphrfgzi.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.chenjidiqi.icu/gtdfjkaaaw.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.tian-w.cn/gtsnanbjqu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.feifeiyinyue.top/gtxdurprpu.html

TS:   interface Shape { area(): number; }
来源：http://hz.ywan-chungtsiang.top/gtjwiiptrf.html

Java: interface Shape { double area(); }
来源：http://hz.jinqigfzy.top/gtynsvjkko.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zhixingplan.top/gtbxujyycv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yj20258888.top/gtffuvsxsl.html

C#:   interface IShape { double Area(); }
来源：http://hz.chenzaomai.com/gtpqgtfglr.html

[G10] 访问控制
来源：http://hz.wangdashe.top/gtodjdfsja.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hnxiangtu.top/gteaxhncpi.html

PHP:  public / protected / private
来源：http://hz.iojbl.cn/gtlgjxbukz.html

JS:   #private 字段；其余公开
来源：http://hz.birdmap.top/gtwsykszch.html

TS:   public / protected / private
来源：http://hz.guannengcc.top/gtuwipymbt.html

Java: public / protected / private / 默认包级
来源：http://hz.hfpthk.cn/gtxonacfom.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.c1oappe.top/gtzemkdlbv.html

Ruby: public / protected / private
来源：http://hz.jinyuanbaomall.cn/gteoqpgrxd.html

C#:   public / protected / private / internal
来源：http://hz.52xcode.cn/gtgwfqvaec.html

[G11] getter / setter
来源：http://hz.aizwys.cn/gtdugexyuv.html

Py:   @property 与 @x.setter
来源：http://hz.chenjidiqi.icu/gtexrxlbmp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jianghu66.top/gtrriarfgh.html

JS:   get name() { return this._name; }
来源：http://hz.xinyue.icu/gtnddrxzzl.html

TS:   get name(): string { return this._name; }
来源：http://hz.nwbrower.top/gttoghpzyu.html

Java: public String getName() { return name; }
来源：http://hz.zhaomingkeji.xyz/gttxlhydja.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.gaohongyu789.top/gtphaozyha.html

Ruby: attr_accessor :name
来源：http://hz.aizwys.cn/gtgmdrqpgp.html

C#:   public string Name { get; set; }
来源：http://hz.andypj.xyz/gtcwnltrws.html

[G12] 对象转字符串
来源：http://hz.xinyue.icu/gtmnqmkmlc.html

Py:   def __str__(self): return self.name
来源：http://hz.zhijiandao.cn/gthortbiub.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.feifeiyinyue.top/gtpkpdxkhb.html

JS:   toString() { return this.name; }
来源：http://hz.yj202588.top/gtxdrianej.html

TS:   toString(): string { return this.name; }
来源：http://hz.feifeiyinyue.top/gtjdbzjmia.html

Java: @Override public String toString() { return name; }
来源：http://hz.yuxming.cn/gtxuiinwrw.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.nanxinkj.top/gtnexndtdi.html

Ruby: def to_s; @name; end
来源：http://hz.cdnleiting.top/gtdsfjbddk.html

C#:   public override string ToString() => Name;
来源：http://hz.cashguo.top/gtoezmabpd.html

[G13] 判断对象类型
来源：http://hz.zhaomingkeji.xyz/gtkgjxiycx.html

Py:   isinstance(u, User)
来源：http://hz.yvedp.cn/gtoqygemxg.html

PHP:  $u instanceof User
来源：http://hz.zhoulong.xyz/gtsavqwzwc.html

JS:   u instanceof User
来源：http://hz.jqgufenzy.top/gtrhrwtdrw.html

TS:   u instanceof User
来源：http://hz.c1oappe.top/gtjiyatwsk.html

Java: u instanceof User
来源：http://hz.iojbl.cn/gtgthxeynf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.feifeiyinyue.top/gtorvvhfod.html

Ruby: u.is_a?(User)
来源：http://hz.dashuyun.cn/gtoxtwulns.html

C#:   u is User
来源：http://hz.zhixingplan.top/gtfgnyfkbt.html

[G14] 数据类 / record
来源：http://hz.zhaomingkeji.xyz/gtfwwukzfx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.pengpengdd.cyou/gtazrihnza.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.daria6918.cn/gtpxarrbqw.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.bjfxy.top/gtgoofgbcb.html

TS:   type User = { name: string; age: number };
来源：http://hz.ydzc1.top/gtgcyskgaw.html

Java: record User(String name, int age) {}
来源：http://hz.nwbrower.top/gtemswlupo.html

Go:   type User struct { Name string; Age int }
来源：http://hz.fzhhl.top/gtvzvpmwhq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jqgfzy.top/gtcrkxdcqa.html

C#:   record User(string Name, int Age);
来源：http://hz.chenlongwang.top/gtgcfusrsx.html

[G15] 枚举
来源：http://hz.yj202588.top/gtjomlknob.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.guowangkeji.top/gtrviprdki.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jinqigfzy.top/gtgfxnwtvu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.iojbl.cn/gteyekevth.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.c1oappe.top/gthidctfae.html

Java: enum Color { RED, GREEN }
来源：http://hz.wangdashe.top/gtixvqgrub.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ppjwa.cn/gttcdehzbb.html

Ruby: Color = %i[red green].freeze
来源：http://hz.shuidangran.top/gtvjkzuthm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.fzhhl.top/gtoiqnkllb.html

[G16] 对象转数组 / 字典
来源：http://hz.hnxiangtu.top/gtqxmlbiel.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.daria6918.cn/gtpmmmvrjm.html

PHP:  get_object_vars($obj);
来源：http://hz.shanyushiyangtech.top/gtfjzrwbsi.html

JS:   Object.entries(obj)
来源：http://hz.yvedp.cn/gtrsynigkr.html

TS:   Object.entries(obj)
来源：http://hz.shzxlz.cn/gtxstmpqon.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jiagoushi.top/gtlbczejum.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.daria6918.cn/gtsdrxaooc.html

Ruby: obj.instance_variables
来源：http://hz.cdnleiting.top/gtmfrdjswd.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.shzxlz.cn/gtfznfgxfg.html

================================================================================
来源：http://hz.ppjwa.cn/gtglsxtnfd.html

H. 异常与错误处理
来源：http://hz.jinyuanbaomall.cn/gtisgrgbls.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtrikzhmqi.html

[H01] try / catch 基础
来源：http://hz.sufxvd.cn/gtidflzatf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhengqikj.top/gtgoxsujnq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.cashguo.top/gtfwdrdqfd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.feifeiyinyue.top/gtmirvyyqj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hnqzz.top/gtaviljdkw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ywan-chungtsiang.top/gtqfkmkvnd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yj202588.top/gtigrgkbff.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.zycfv.cn/gthcgzsatr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.c1oappe.top/gtexnfyoun.html

[H02] finally / ensure 收尾
来源：http://hz.haohaochexian.top/gtivkzpkwi.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.nanxinkj.top/gtkfyhlgyq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.ydjk.org.cn/gtupanpbcm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.aibaodan.cn/gtfwndxbdm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jianghu66.top/gtaykhoipm.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hnqzz.top/gtlvyiiiux.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jiagoushi.top/gtgnrhwmhg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.guannengcc.top/gtcrsfxvet.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.feifeiyinyue.top/gtkbcbvqhu.html

[H03] 主动抛出异常
来源：http://hz.yonumen.top/gthihdfskg.html

Py:   raise ValueError("错误信息")
来源：http://hz.snrcjt.cn/gtwrpttytf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.smart0.xyz/gtmqfzzewc.html

JS:   throw new Error("错误信息");
来源：http://hz.jqgufenzy.top/gtpqxizjwt.html

TS:   throw new Error("错误信息");
来源：http://hz.daria6918.cn/gtcitascor.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.9152youxi.cn/gtrdmzrzdp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yuanzhike.top/gtjqytgasw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.sufxvd.cn/gtffnpmlyq.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.tian-w.cn/gtkhbinkrb.html

[H04] 自定义异常类型
来源：http://hz.ppjwa.cn/gtvdbtaunf.html

Py:   class MyError(Exception): pass
来源：http://hz.svipenyu.cn/gtmsjdsrpl.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.cucudq.cn/gtgovifrdt.html

JS:   class MyError extends Error {}
来源：http://hz.ydzc1.top/gtlhrypxvz.html

TS:   class MyError extends Error {}
来源：http://hz.tanke756.top/gtqkrhyfbr.html

Java: class MyException extends RuntimeException {}
来源：http://hz.tian-w.cn/gtrapcrlbu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.cheryme.top/gtuaxqlwcc.html

Ruby: class MyError < StandardError; end
来源：http://hz.shanyushiyangtech.top/gtiuohbpaq.html

C#:   class MyException : Exception {}
来源：http://hz.ydjk.org.cn/gtzbiajvwh.html

[H05] 捕获特定类型
来源：http://hz.zhongyouzk.top/gtjrmlbbhh.html

Py:   except ValueError as e:
来源：http://hz.chenlongwang.top/gtdwjdndix.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.dashuyun.cn/gtuekcmigx.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jlsjyb.cn/gtfesontlh.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.xziqi.cn/gtrmdtouiu.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.ywan-chungtsiang.top/gtofprsdqy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.tanke756.top/gtghpckbxg.html

Ruby: rescue ArgumentError => e
来源：http://hz.nwbrower.top/gthykkygjr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhiwuduotai.top/gtgzytuqrv.html

[H06] 可选值 / 空值安全访问
来源：http://hz.shuidangran.top/gthsxzbjnf.html

Py:   value = d.get("k") or default
来源：http://hz.cqqwz.cn/gtpbhhpned.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yj20258.top/gtttlbzobg.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jinqigufen.top/gtyyhvnoif.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yonumen.top/gtdyzttpbt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.xingfuxueyuan.xyz/gtoczftxeu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.tanke756.top/gttncavrwj.html

Ruby: d&.dig(:a, :b)
来源：http://hz.fengsongda.top/gtcjtxjmci.html

C#:   obj?.A?.B ?? default
来源：http://hz.smart0.xyz/gtoyxeqcpd.html

[H07] 断言
来源：http://hz.shzxlz.cn/gtzdiryvvp.html

Py:   assert x > 0, "必须为正"
来源：http://hz.9152youxi.cn/gtrgaqbarp.html

PHP:  assert($x > 0);
来源：http://hz.shanyushiyangkeji.top/gtxszeqnbo.html

JS:   console.assert(x > 0);
来源：http://hz.jinghuilouyu.cn/gtpqbnbscg.html


<!-- 参考信息 -->