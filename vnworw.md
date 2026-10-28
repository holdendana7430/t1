代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.daxiang520.top/gtjnpqtusi.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yvedp.cn/gthezzkidn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.gotoacloud.top/gtxkcmzoju.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.sysykeji.top/gtemntcdca.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.guowangkeji.top/gteuppqros.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zhongyouzk.top/gtowzvrhza.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.wangdashe.top/gtfzjwntyx.html

[F04] 追加写入文件
来源：http://hz.shangyingyoupin.top/gtejxftopo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.dashuyun.cn/gtzikhzplb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yangfankeji.com/gtxybywqwk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jinqigufen.top/gtcybwotyq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yangfankeji.com/gtrmbtieke.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jlsjyb.cn/gtgvhuzycy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.gaohongyu789.top/gtlmdxspwo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.gaohongyu789.top/gtomzwjwoc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.snrcjt.cn/gtbovczudy.html

[F05] 判断文件或目录是否存在
来源：http://hz.zhiwuduotai.top/gthvuskbeb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.fengsongda.top/gthacsfqub.html

PHP:  file_exists("a.txt");
来源：http://hz.yongpay.top/gtsrhollxj.html

JS:   fs.existsSync("a.txt")
来源：http://hz.xuetiantiany.cn/gtxceiqibd.html

TS:   fs.existsSync("a.txt")
来源：http://hz.guannengcc.top/gtlnbitxzj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.xuanzx.com/gtaxxxxesz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jyoumei.cn/gtxohpacie.html

Ruby: File.exist?("a.txt")
来源：http://hz.hammf.cn/gtjatucwum.html

C#:   File.Exists("a.txt")
来源：http://hz.jinqigfzy.top/gtqajahvnp.html

[F06] 删除文件
来源：http://hz.pycfn.com/gtnlbrozmd.html

Py:   os.remove("a.txt")
来源：http://hz.cucudq.cn/gtclfrppyx.html

PHP:  unlink("a.txt");
来源：http://hz.hnqzz.top/gtrgrinuvq.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.feifeiyinyue.top/gtyyxgewds.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.iojbl.cn/gtnvtzhuby.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.wangdashe.top/gtdmsjdyss.html

Go:   os.Remove("a.txt")
来源：http://hz.quarkkingdee.top/gtxyouqefq.html

Ruby: File.delete("a.txt")
来源：http://hz.yj202588.top/gtqzfjnhxc.html

C#:   File.Delete("a.txt");
来源：http://hz.yuanzhike.top/gttgqssisj.html

[F07] 创建目录（含多级）
来源：http://hz.jinqigufen.top/gtokrckshi.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jianghu66.top/gtpoyqvwwa.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zhiwuduotai.top/gtfgxncboj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yonumen.top/gtxecumsfn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shanyushiyangtech.top/gtfkmsoaoh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.aizwys.cn/gtljaggvya.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.nanxinkj.top/gtlkxmmgms.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.shanyushiyangtech.top/gtvjfptmgt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.andypj.xyz/gticoeuydl.html

[F08] 遍历目录
来源：http://hz.zhengqikj.top/gtahdjflaq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yj20258.top/gthdzavlyn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jinyuanbaomall.cn/gtpzdqhuep.html

JS:   fs.readdirSync("dir")
来源：http://hz.316326.xyz/gtxfenzsxf.html

TS:   fs.readdirSync("dir")
来源：http://hz.zhiwuduotai.top/gtzcbjauxg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.chenzaomai.com/gthongkirl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zhoulong.xyz/gtjhrpsdhu.html

Ruby: Dir.children("dir")
来源：http://hz.birdmap.top/gtzxwseusl.html

C#:   Directory.GetFiles("dir")
来源：http://hz.meibo888.top/gtzdvgkcpe.html

[F09] 获取文件大小
来源：http://hz.yj20258.top/gtykxxnsrr.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jiagoushi.top/gtngxobojt.html

PHP:  filesize("a.txt");
来源：http://hz.guannengcc.top/gtkseftprn.html

JS:   fs.statSync("a.txt").size
来源：http://hz.havefunace.top/gtevzsyypa.html

TS:   fs.statSync("a.txt").size
来源：http://hz.quarkkingdee.top/gtgnmaonbu.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jlsjyb.cn/gtawzdtwcq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.shzxlz.cn/gtzwxqzuyg.html

Ruby: File.size("a.txt")
来源：http://hz.yangfankeji.com/gtwrrmcczs.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.hammf.cn/gtzybdvipi.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yj20258888.top/gtlrravvyd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.iojbl.cn/gthsukiwnq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.guannengcc.top/gtiohzrpfk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jiagoushi.top/gtzpoeviqs.html

TS:   path.extname("a.txt")
来源：http://hz.gzhubu.top/gthllrhivm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.hfpthk.cn/gtespagodz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.svipenyu.cn/gtmfudfmbi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.sysykeji.top/gtdzcjvfye.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.fengsongda.top/gtjisesjdb.html

[F11] 复制与移动文件
来源：http://hz.jinqigfzy.top/gtgwplogtg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.shuidangran.top/gtugbnrvwi.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.sysykeji.top/gteufaikfb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xziqi.cn/gtsjvbbzez.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.wangshuangyany.cn/gtplsdtvou.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.xylfe.cn/gtdjdmuefa.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jqgufenzy.top/gtdcemysdo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.smart0.xyz/gtynftalmu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.xinyue.icu/gtuqkgjoqa.html

[F12] CSV 读写
来源：http://hz.snrcjt.cn/gtqehxchcp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.havefunace.top/gtztbxhvgb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zycfv.cn/gtobidksqq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.gzhubu.top/gtdbqvhjsl.html

TS:   // 同上
来源：http://hz.ywan-chungtsiang.top/gtewenmeqo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zhaomingkeji.xyz/gtftawmdkz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yueranfly.top/gtiqdocnum.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.feifeiyinyue.top/gtgerohhem.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.haohaochexian.top/gtbermfjkc.html

================================================================================
来源：http://hz.yangfankeji.com/gtvcayznjj.html

G. 面向对象
来源：http://hz.xinyue.icu/gtsajzjhpx.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtljsgcphx.html

[G01] 定义类
来源：http://hz.xylfe.cn/gthldvvljt.html

Py:   class User: pass
来源：http://hz.jqgufenzy.top/gtaxvjrdqd.html

PHP:  class User {}
来源：http://hz.daria6918.cn/gtxnufakyv.html

JS:   class User {}
来源：http://hz.tianlin.xyz/gtamiozkil.html

TS:   class User { name: string = ""; }
来源：http://hz.ydzc1.top/gtlidjdxek.html

Java: class User {}
来源：http://hz.guowangkeji.top/gtdyipblrw.html

Go:   type User struct { Name string }
来源：http://hz.quarkkingdee.top/gttwqdqshp.html

Ruby: class User; end
来源：http://hz.jinqigfzy.top/gtgxbqjrgv.html

C#:   class User {}
来源：http://hz.yanxiufei.cn/gthjfvmaae.html

[G02] 构造函数
来源：http://hz.daxiang520.top/gtmpjzoidp.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.chenzaomai.com/gtojyrritl.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.sweek.top/gtmllovqjg.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.ehwqpu.com/gtiqxwilxp.html

TS:   constructor(public name: string) {}
来源：http://hz.fengsongda.top/gthdbwiwzn.html

Java: User(String name) { this.name = name; }
来源：http://hz.yj20258.top/gtcdycrhzh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.xinyue.icu/gtdnhcufni.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yangfankeji.com/gtxlfgtsud.html

C#:   public User(string name) { Name = name; }
来源：http://hz.ivvv.top/gtuwerulhf.html

[G03] 实例属性
来源：http://hz.haohaochexian.top/gtmtjohkca.html

Py:   self.name = "x"
来源：http://hz.cqqwz.cn/gtuxsdpdxg.html

PHP:  public string $name = "x";
来源：http://hz.hywenlv.cn/gtfubsjegu.html

JS:   this.name = "x";
来源：http://hz.guannengcc.top/gtwgvzobpg.html

TS:   name: string = "x";
来源：http://hz.redwolf501.top/gtoxlnrmcp.html

Java: private String name;
来源：http://hz.jlsjyb.cn/gthmvllswm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.daxiang520.top/gtvoyoygts.html

Ruby: @name = "x"
来源：http://hz.hongshengwenyu.top/gtrvxfczzm.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yuxming.cn/gtzsxwiofo.html

[G04] 定义方法
来源：http://hz.daxiang520.top/gtibonutui.html

Py:   def greet(self): return self.name
来源：http://hz.bjfxy.top/gtcpfbgray.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jqgfzy.top/gthvznsxrc.html

JS:   greet() { return this.name; }
来源：http://hz.yj202588.top/gthuavymiz.html

TS:   greet(): string { return this.name; }
来源：http://hz.cucudq.cn/gtfahpebvb.html

Java: String greet() { return name; }
来源：http://hz.0kj1m.cn/gtywmmbzkq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.nwbrower.top/gtvppdcfgr.html

Ruby: def greet; @name; end
来源：http://hz.shanyushiyangkeji.top/gttgsqqdiz.html

C#:   public string Greet() => Name;
来源：http://hz.wangdashe.top/gtotxrsxqy.html

[G05] 继承
来源：http://hz.zycfv.cn/gthtipuhky.html

Py:   class Admin(User): pass
来源：http://hz.chenlongwang.top/gtmnajzfvv.html

PHP:  class Admin extends User {}
来源：http://hz.jyoumei.cn/gtfqliqrpk.html

JS:   class Admin extends User {}
来源：http://hz.hysaishi.cn/gtnnfyjyng.html

TS:   class Admin extends User {}
来源：http://hz.xylfe.cn/gtyvmwejdq.html

Java: class Admin extends User {}
来源：http://hz.xziqi.cn/gtkdlbjxfz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yuanzhike.top/gtyoqivgpc.html

Ruby: class Admin < User; end
来源：http://hz.316326.xyz/gtjzvswgcn.html

C#:   class Admin : User {}
来源：http://hz.hnqzz.top/gtxmjawiaz.html

[G06] 重写方法
来源：http://hz.ppjwa.cn/gtodjwvilv.html

Py:   def greet(self): return "admin"
来源：http://hz.yangfankeji.com/gtcmlfdeoe.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ydjk.org.cn/gtvrmxoxwd.html

JS:   greet() { return "admin"; }
来源：http://hz.ydjk.org.cn/gtrjmmwsnl.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hywenlv.cn/gtngllhdjg.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zycfv.cn/gtvzztmqnx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.tian-w.cn/gtjtdvxfia.html

Ruby: def greet; "admin"; end
来源：http://hz.cucudq.cn/gtujupuwyt.html

C#:   public override string Greet() => "admin";
来源：http://hz.jlsjyb.cn/gtzwmmxztp.html

[G07] 调用父类方法
来源：http://hz.xuetiantiany.cn/gtfucecefk.html

Py:   super().greet()
来源：http://hz.zhaomingkeji.xyz/gtlpnpmpve.html

PHP:  parent::greet();
来源：http://hz.yvedp.cn/gtzuzlxeai.html

JS:   super.greet();
来源：http://hz.zhoulong.xyz/gtegwtycdx.html

TS:   super.greet();
来源：http://hz.yuanzhike.top/gtqdtuiocd.html

Java: super.greet();
来源：http://hz.ydzc1.top/gtofqhgkgg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.hongshengwenyu.top/gttitlrocy.html

Ruby: super
来源：http://hz.tanke756.top/gtmpovwrsl.html

C#:   base.Greet();
来源：http://hz.sxryk.cn/gtoustawpv.html

[G08] 静态方法与属性
来源：http://hz.ybcxt.top/gtqndxgifl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.ydzc1.top/gtqkxmshge.html

PHP:  public static function f() {}
来源：http://hz.ivvv.top/gtpxjmitug.html

JS:   static f() {}
来源：http://hz.xziqi.cn/gtcxnxgzxt.html

TS:   static f(): void {}
来源：http://hz.jqgfzy.top/gtlzjcrcce.html

Java: static void f() {}
来源：http://hz.sysykeji.top/gtfpzwxsju.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.sweek.top/gtzeabzmeu.html

Ruby: def self.f; end
来源：http://hz.mhx1999.top/gthelymqcy.html

C#:   public static void F() {}
来源：http://hz.hywenlv.cn/gtcrypalgp.html

[G09] 接口 / 抽象类
来源：http://hz.zhiwuduotai.top/gttmohpbmu.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.aibaodan.cn/gtycbbsaqb.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.0kj1m.cn/gtsarlkoqc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.hysaishi.cn/gtemkviqfh.html

TS:   interface Shape { area(): number; }
来源：http://hz.shanyushiyangtech.top/gtukickcgn.html

Java: interface Shape { double area(); }
来源：http://hz.hywenlv.cn/gtwydbgybw.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jinyuanbaomall.cn/gtgbogbxzh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.gotoacloud.top/gtxlbohoqp.html

C#:   interface IShape { double Area(); }
来源：http://hz.zhoulong.xyz/gtjoovijrb.html

[G10] 访问控制
来源：http://hz.guowangkeji.top/gtokqfsfcb.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jianghu66.top/gtpruxmmgc.html

PHP:  public / protected / private
来源：http://hz.ivvv.top/gtlaiswofp.html

JS:   #private 字段；其余公开
来源：http://hz.jqgufenzy.top/gteoigpiyw.html

TS:   public / protected / private
来源：http://hz.shangyingyoupin.top/gtsmbyrowh.html

Java: public / protected / private / 默认包级
来源：http://hz.xziqi.cn/gtmurrqqrc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jinqigufen.top/gtaxgqdcbf.html

Ruby: public / protected / private
来源：http://hz.zycfv.cn/gtwkhcrjzu.html

C#:   public / protected / private / internal
来源：http://hz.zhixingplan.top/gtnzysijoh.html

[G11] getter / setter
来源：http://hz.yj202588.top/gtpagxbwzf.html

Py:   @property 与 @x.setter
来源：http://hz.zdqjudy.top/gtptvsjkso.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.nwbrower.top/gticljocdd.html

JS:   get name() { return this._name; }
来源：http://hz.jinyuanbaomall.cn/gtgtomtvdr.html

TS:   get name(): string { return this._name; }
来源：http://hz.52xcode.cn/gtrbcfxxei.html

Java: public String getName() { return name; }
来源：http://hz.havefunace.top/gtgzctyiye.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.meibo888.top/gtrzpzeviv.html

Ruby: attr_accessor :name
来源：http://hz.redwolf501.top/gtwelunnsj.html

C#:   public string Name { get; set; }
来源：http://hz.gogol.net.cn/gtsyolwoiz.html

[G12] 对象转字符串
来源：http://hz.sufxvd.cn/gtlaqedzmd.html

Py:   def __str__(self): return self.name
来源：http://hz.havefunace.top/gtyujnavqt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zhiwuduotai.top/gtylrkffcv.html

JS:   toString() { return this.name; }
来源：http://hz.jinghuilouyu.cn/gtnpialhyy.html

TS:   toString(): string { return this.name; }
来源：http://hz.yj20258888.top/gtsphxewlf.html

Java: @Override public String toString() { return name; }
来源：http://hz.bjfxy.top/gtmoeqwxhb.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.shuidangran.top/gtceljoyrf.html

Ruby: def to_s; @name; end
来源：http://hz.xuetiantiany.cn/gtcmbzucqx.html

C#:   public override string ToString() => Name;
来源：http://hz.cashguo.top/gtrindpcgn.html

[G13] 判断对象类型
来源：http://hz.jinyuanbaomall.cn/gtjgxceect.html

Py:   isinstance(u, User)
来源：http://hz.zhijiandao.cn/gtgaleeycv.html

PHP:  $u instanceof User
来源：http://hz.shzxlz.cn/gtnodkbzxx.html

JS:   u instanceof User
来源：http://hz.9152youxi.cn/gtpgmpznak.html

TS:   u instanceof User
来源：http://hz.quarkkingdee.top/gtbybaumnf.html

Java: u instanceof User
来源：http://hz.wangshuangyany.cn/gtfofvrznr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ydjk.org.cn/gtucsypofh.html

Ruby: u.is_a?(User)
来源：http://hz.sysykeji.top/gtszwgplzz.html

C#:   u is User
来源：http://hz.yuxming.cn/gtovasnsiv.html

[G14] 数据类 / record
来源：http://hz.yuanzhike.top/gtpkcvwvzw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zhoulong.xyz/gtezvqhpdv.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yuanzhike.top/gtnkxjghdi.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.ehwqpu.com/gtugiogiti.html

TS:   type User = { name: string; age: number };
来源：http://hz.xuanzx.com/gtqpwefalv.html

Java: record User(String name, int age) {}
来源：http://hz.ydzc1.top/gtdqdjqkcz.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zhiwuduotai.top/gthtfrtvfa.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.ivvv.top/gtzzivrmpg.html

C#:   record User(string Name, int Age);
来源：http://hz.zhongyouzk.top/gtshrftgym.html

[G15] 枚举
来源：http://hz.xuetiantiany.cn/gtfojwledt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.wangshuangyany.cn/gtnsqdsadx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.daria6918.cn/gtvnvffjqb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.snrcjt.cn/gthwtdnzdg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zycfv.cn/gtxhrxlmfm.html

Java: enum Color { RED, GREEN }
来源：http://hz.wangdashe.top/gtebzsjmtf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.hnqzz.top/gtggnentoo.html

Ruby: Color = %i[red green].freeze
来源：http://hz.kuanghao11.cn/gtwvjaaxre.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.guannengcc.top/gthpwoayuo.html

[G16] 对象转数组 / 字典
来源：http://hz.meibo888.top/gtxqiocxng.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.guannengcc.top/gtacyiyvcb.html

PHP:  get_object_vars($obj);
来源：http://hz.0kj1m.cn/gtaxoglpfq.html

JS:   Object.entries(obj)
来源：http://hz.dashuyun.cn/gttihehheb.html

TS:   Object.entries(obj)
来源：http://hz.shzxlz.cn/gtmecppqse.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.shanyushiyangtech.top/gtfwzahozo.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yueranfly.top/gtlmykivzy.html

Ruby: obj.instance_variables
来源：http://hz.yj20258.top/gtybckdram.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.hywenlv.cn/gtwlecqvhm.html

================================================================================
来源：http://hz.hysaishi.cn/gtftjzaddd.html

H. 异常与错误处理
来源：http://hz.sweek.top/gtifhqfpdk.html

================================================================================
来源：http://hz.zdqjudy.top/gtrgvvqvao.html

[H01] try / catch 基础
来源：http://hz.yvedp.cn/gtyfedkgvp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.chenlongwang.top/gtlmgoybox.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.9152youxi.cn/gtbggenjzb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.cdnleiting.top/gtucqkwhwf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jqgufenzy.top/gtqojcixxg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jqgfzy.top/gttnwcdhdr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.chenlongwang.top/gtaqxczojk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jinqigfzy.top/gtimlxysbw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.xziqi.cn/gtoohnjkys.html

[H02] finally / ensure 收尾
来源：http://hz.mhx1999.top/gtntvabxhj.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.svipenyu.cn/gttqbiweee.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.ydjk.org.cn/gteukozlux.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.cqqwz.cn/gtjyhstixm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangtech.top/gtjrlpreiw.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.cucudq.cn/gtrsqcouze.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.mhx1999.top/gtdtmqpmwt.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.hammf.cn/gtpfgeepur.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zhiwuduotai.top/gtpxnixfjh.html

[H03] 主动抛出异常
来源：http://hz.9152youxi.cn/gtlmrwmcnm.html

Py:   raise ValueError("错误信息")
来源：http://hz.zycfv.cn/gtocogjjye.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.sufxvd.cn/gtpabsxlbi.html

JS:   throw new Error("错误信息");
来源：http://hz.jinqigufen.top/gtkryvczbb.html

TS:   throw new Error("错误信息");
来源：http://hz.andypj.xyz/gtvdedmqjl.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.guowangkeji.top/gtfszwbwvq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.ppjwa.cn/gtuomvoeav.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yueranfly.top/gthrbktbpu.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yuanzhike.top/gtotgqraai.html

[H04] 自定义异常类型
来源：http://hz.hnxiangtu.top/gtwjwcahzh.html

Py:   class MyError(Exception): pass
来源：http://hz.xinyue.icu/gtwejmmffm.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.smart0.xyz/gtulfpojbg.html

JS:   class MyError extends Error {}
来源：http://hz.shanyushiyangkeji.top/gtvpnitzaw.html

TS:   class MyError extends Error {}
来源：http://hz.sxryk.cn/gtnqndqkqu.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yj20258888.top/gtgfgrgsiq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.tanke756.top/gtamucqnso.html

Ruby: class MyError < StandardError; end
来源：http://hz.cucudq.cn/gtuewpdzoj.html

C#:   class MyException : Exception {}
来源：http://hz.gotoacloud.top/gtorahisre.html

[H05] 捕获特定类型
来源：http://hz.kuanghao11.cn/gtzgsredks.html

Py:   except ValueError as e:
来源：http://hz.haohaochexian.top/gtorwsajzs.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yueranfly.top/gtdkthvaqp.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.birdmap.top/gtrbdihmcp.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.ehwqpu.com/gtojxwlnzg.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.sweek.top/gtdhxntyho.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.mhx1999.top/gtsinsqbla.html

Ruby: rescue ArgumentError => e
来源：http://hz.ivvv.top/gtarozmnuy.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.daxiang520.top/gtqeemsckt.html

[H06] 可选值 / 空值安全访问
来源：http://hz.dashuyun.cn/gtqeykzkus.html

Py:   value = d.get("k") or default
来源：http://hz.ehwqpu.com/gtvarkedpi.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.havefunace.top/gtlyhaheur.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.gaohongyu789.top/gtfmcnubjv.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.ehwqpu.com/gteyjdllzq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.hnqzz.top/gtnxsveytm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zhiwuduotai.top/gtgjckmefd.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yj202588.top/gtdzsphbxr.html

C#:   obj?.A?.B ?? default
来源：http://hz.svipenyu.cn/gtpljrtnms.html

[H07] 断言
来源：http://hz.cqqwz.cn/gtdvyaxmwg.html

Py:   assert x > 0, "必须为正"
来源：http://hz.hfpthk.cn/gtjatgwjjx.html

PHP:  assert($x > 0);
来源：http://hz.daria6918.cn/gtqpbshrag.html

JS:   console.assert(x > 0);
来源：http://hz.feifeiyinyue.top/gtzwbovvtm.html

TS:   console.assert(x > 0);
来源：http://hz.cheryme.top/gtebsbpsvt.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yj20258888.top/gtckbrcsmj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jinqigufen.top/gtylmvqkyz.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.tanke756.top/gtghccrdpl.html


<!-- 参考信息 -->