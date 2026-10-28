代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zhaomingkeji.xyz/gtzfabskhg.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.aibaodan.cn/gtbuycufof.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.daria6918.cn/gtvzjwssiw.html

[F04] 追加写入文件
来源：http://hz.jianghu66.top/gtdwbaejng.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.hnqzz.top/gtmcckcuns.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.quarkkingdee.top/gtkalrznbx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.andypj.xyz/gtjnsbcofa.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.svipenyu.cn/gtoraobhxv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jlsjyb.cn/gtslwwzwoj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.xylfe.cn/gtfnkymbun.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zycfv.cn/gtkohexoro.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.zhijiandao.cn/gtsgncrzmt.html

[F05] 判断文件或目录是否存在
来源：http://hz.ydzc1.top/gtyjvulcee.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.shanyushiyangkeji.top/gtiuhrydat.html

PHP:  file_exists("a.txt");
来源：http://hz.sweek.top/gtecnmiwqy.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yangfankeji.com/gthcqbgknt.html

TS:   fs.existsSync("a.txt")
来源：http://hz.hammf.cn/gtbiutbroj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.xuetiantiany.cn/gtlxyxoyad.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.9152youxi.cn/gtoewswehl.html

Ruby: File.exist?("a.txt")
来源：http://hz.daria6918.cn/gttvsqpnbu.html

C#:   File.Exists("a.txt")
来源：http://hz.sufxvd.cn/gtvljvkiyy.html

[F06] 删除文件
来源：http://hz.sxryk.cn/gtnvqenqtz.html

Py:   os.remove("a.txt")
来源：http://hz.ivvv.top/gtqzubdvpl.html

PHP:  unlink("a.txt");
来源：http://hz.zhiwuduotai.top/gtxuulidyg.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.tian-w.cn/gtciagnyak.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.zhijiandao.cn/gtercxvmik.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.sysykeji.top/gtoxhtfvaq.html

Go:   os.Remove("a.txt")
来源：http://hz.gaohongyu789.top/gtwzyfopfn.html

Ruby: File.delete("a.txt")
来源：http://hz.cdnleiting.top/gthrjdgtkp.html

C#:   File.Delete("a.txt");
来源：http://hz.zdqjudy.top/gtnmwnyyln.html

[F07] 创建目录（含多级）
来源：http://hz.zhaomingkeji.xyz/gtsaupiupm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.kuanghao11.cn/gtcjnnbnut.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jianghu66.top/gtmspjorud.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.0kj1m.cn/gtiqxhfigr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hongshengwenyu.top/gtibgtkeua.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.c1oappe.top/gtlnszsqfg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.chenzaomai.com/gtujevzdix.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.vqdsnc.cn/gtjehvedqy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.nwbrower.top/gtlasvfszm.html

[F08] 遍历目录
来源：http://hz.xylfe.cn/gtrdcghfdm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.iojbl.cn/gtkjajibmu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.xziqi.cn/gtjuirdsqh.html

JS:   fs.readdirSync("dir")
来源：http://hz.gogol.net.cn/gtidpnbdmb.html

TS:   fs.readdirSync("dir")
来源：http://hz.yonumen.top/gtwpxibtpp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.chenlongwang.top/gtcpinsars.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.shanyushiyangkeji.top/gtfrodcynw.html

Ruby: Dir.children("dir")
来源：http://hz.hnxiangtu.top/gtvccaunqk.html

C#:   Directory.GetFiles("dir")
来源：http://hz.mhx1999.top/gtbsvkrdbe.html

[F09] 获取文件大小
来源：http://hz.ehwqpu.com/gtpxjscokr.html

Py:   os.path.getsize("a.txt")
来源：http://hz.sufxvd.cn/gtnltlwgum.html

PHP:  filesize("a.txt");
来源：http://hz.yvedp.cn/gtgfvcmylo.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jinqigfzy.top/gtjdhiofrp.html

TS:   fs.statSync("a.txt").size
来源：http://hz.birdmap.top/gtyjvyeisn.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.sufxvd.cn/gtnuyhpzma.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.xylfe.cn/gtgdwerren.html

Ruby: File.size("a.txt")
来源：http://hz.yuxming.cn/gtzxkvmkzz.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.xinyue.icu/gtguvlfmev.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zhiwuduotai.top/gtvesxjmcc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.svipenyu.cn/gtvrnkfthu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.cqqwz.cn/gtthbdnzrd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.c1oappe.top/gtbrghijqq.html

TS:   path.extname("a.txt")
来源：http://hz.jinqigfzy.top/gtsxpqrozs.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhengqikj.top/gtytdcmqsy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.hysaishi.cn/gtspmfmajc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zdqjudy.top/gtidqiowge.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.chenlongwang.top/gtdfdeaesy.html

[F11] 复制与移动文件
来源：http://hz.zhiwuduotai.top/gtpgwkojcg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.sweek.top/gtublukyrm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jinqigfzy.top/gtfcsnepem.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hammf.cn/gtjntbbphm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shanyushiyangtech.top/gtmxqefxxs.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.hnqzz.top/gthjvkvgzr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.nanxuanxn.top/gtnvxqoicm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.aibaodan.cn/gtducutcxk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhengqikj.top/gtkoorijts.html

[F12] CSV 读写
来源：http://hz.yvedp.cn/gtuquxafdb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.pengpengdd.cyou/gtjfzejhkl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jqgfzy.top/gtveigeilz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.ybcxt.top/gtnpzurlof.html

TS:   // 同上
来源：http://hz.kuanghao11.cn/gtssmmljbc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yvedp.cn/gtqrdpghsy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.havefunace.top/gtgfruskgj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.guannengcc.top/gttmcrqbxp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.guowangkeji.top/gttqhmwrtw.html

================================================================================
来源：http://hz.hammf.cn/gtlolaylhg.html

G. 面向对象
来源：http://hz.hongshengwenyu.top/gtmubzraxw.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtvthkafun.html

[G01] 定义类
来源：http://hz.havefunace.top/gtqbcszkox.html

Py:   class User: pass
来源：http://hz.jiagoushi.top/gtcakhcpsg.html

PHP:  class User {}
来源：http://hz.pycfn.com/gtluixiwhu.html

JS:   class User {}
来源：http://hz.cashguo.top/gtaxitgkkj.html

TS:   class User { name: string = ""; }
来源：http://hz.cucudq.cn/gtnravxoeq.html

Java: class User {}
来源：http://hz.shanyushiyangtech.top/gtohohrfic.html

Go:   type User struct { Name string }
来源：http://hz.shuidangran.top/gtpcmwffhv.html

Ruby: class User; end
来源：http://hz.gaohongyu789.top/gtjyjnkqdp.html

C#:   class User {}
来源：http://hz.aizwys.cn/gtobsikmip.html

[G02] 构造函数
来源：http://hz.nwbrower.top/gtwfztbmwu.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.nanxinkj.top/gtmyydgxvc.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.meibo888.top/gtysslmjrf.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.ydzc1.top/gtosynwenm.html

TS:   constructor(public name: string) {}
来源：http://hz.yuxming.cn/gtuikjqnwz.html

Java: User(String name) { this.name = name; }
来源：http://hz.andypj.xyz/gtcewxebwi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.gotoacloud.top/gtxsaqcjef.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jqgufenzy.top/gtshdmshhj.html

C#:   public User(string name) { Name = name; }
来源：http://hz.birdmap.top/gtioefsdkx.html

[G03] 实例属性
来源：http://hz.yj20258888.top/gtscpcohip.html

Py:   self.name = "x"
来源：http://hz.chenzaomai.com/gtqruyhvvr.html

PHP:  public string $name = "x";
来源：http://hz.zycfv.cn/gtngbyqlfh.html

JS:   this.name = "x";
来源：http://hz.nwbrower.top/gtdlfncerx.html

TS:   name: string = "x";
来源：http://hz.gzhubu.top/gtehlnnnxf.html

Java: private String name;
来源：http://hz.jiagoushi.top/gtrbbeevox.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.gaohongyu789.top/gttwrqgobq.html

Ruby: @name = "x"
来源：http://hz.jinqigufen.top/gtkivgkjmg.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.daria6918.cn/gtzfkginbu.html

[G04] 定义方法
来源：http://hz.quarkkingdee.top/gthtlcbprd.html

Py:   def greet(self): return self.name
来源：http://hz.yongpay.top/gtucgxgnfv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.pycfn.com/gtpmrlkmtg.html

JS:   greet() { return this.name; }
来源：http://hz.ydzc1.top/gtztajzksu.html

TS:   greet(): string { return this.name; }
来源：http://hz.yangfankeji.com/gteducipuu.html

Java: String greet() { return name; }
来源：http://hz.dianchejie.cn/gtnbnqdnue.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yj20258.top/gtxcwohgxq.html

Ruby: def greet; @name; end
来源：http://hz.yuxming.cn/gtwnwplbee.html

C#:   public string Greet() => Name;
来源：http://hz.yueranfly.top/gtnnwhtxuj.html

[G05] 继承
来源：http://hz.daria6918.cn/gtaryeuvgj.html

Py:   class Admin(User): pass
来源：http://hz.ydjk.org.cn/gtdodgljaa.html

PHP:  class Admin extends User {}
来源：http://hz.hnqzz.top/gtrsxxbqei.html

JS:   class Admin extends User {}
来源：http://hz.aibaodan.cn/gthkdurqmm.html

TS:   class Admin extends User {}
来源：http://hz.yuxming.cn/gtpsfwdpaa.html

Java: class Admin extends User {}
来源：http://hz.sufxvd.cn/gtzydjibdj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ppjwa.cn/gtkzulsioq.html

Ruby: class Admin < User; end
来源：http://hz.iojbl.cn/gtuwkncojt.html

C#:   class Admin : User {}
来源：http://hz.guowangkeji.top/gtkvddvelg.html

[G06] 重写方法
来源：http://hz.snrcjt.cn/gtwzjmwgun.html

Py:   def greet(self): return "admin"
来源：http://hz.aibaodan.cn/gtlncjxbwo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.cqqwz.cn/gtixdapwmn.html

JS:   greet() { return "admin"; }
来源：http://hz.sweek.top/gtxrlibrml.html

TS:   greet(): string { return "admin"; }
来源：http://hz.guowangkeji.top/gtqtenvrcb.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.sysykeji.top/gtgmlttpzw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zycfv.cn/gtextbmpgn.html

Ruby: def greet; "admin"; end
来源：http://hz.jinqigufen.top/gtidkvytbj.html

C#:   public override string Greet() => "admin";
来源：http://hz.jianghu66.top/gtxoyvfuaf.html

[G07] 调用父类方法
来源：http://hz.wangshuangyany.cn/gtpozmunqf.html

Py:   super().greet()
来源：http://hz.aibaodan.cn/gtaqmtmtiw.html

PHP:  parent::greet();
来源：http://hz.wangshuangyany.cn/gtlhksmbol.html

JS:   super.greet();
来源：http://hz.mhx1999.top/gtjxwtabrv.html

TS:   super.greet();
来源：http://hz.gzhubu.top/gttxmkqppn.html

Java: super.greet();
来源：http://hz.hnqzz.top/gtptptmeem.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.ehwqpu.com/gtjkkztqqq.html

Ruby: super
来源：http://hz.yvedp.cn/gtpzpyrgts.html

C#:   base.Greet();
来源：http://hz.xuetiantiany.cn/gtfzisowrj.html

[G08] 静态方法与属性
来源：http://hz.yuxming.cn/gtzckxmukp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yongpay.top/gtbszoroni.html

PHP:  public static function f() {}
来源：http://hz.cdnleiting.top/gtjcwbdyzm.html

JS:   static f() {}
来源：http://hz.dianchejie.cn/gtrxapklbm.html

TS:   static f(): void {}
来源：http://hz.xuetiantiany.cn/gtdhxvrlpr.html

Java: static void f() {}
来源：http://hz.zhijiandao.cn/gtudswodum.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jinghuilouyu.cn/gtfutjawmx.html

Ruby: def self.f; end
来源：http://hz.xziqi.cn/gtudyeceqb.html

C#:   public static void F() {}
来源：http://hz.yueranfly.top/gtszxzfkdd.html

[G09] 接口 / 抽象类
来源：http://hz.tian-w.cn/gtyoznwaqz.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.chenjidiqi.icu/gtogrkkvrc.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jinqigfzy.top/gtqdkzcnye.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.haohaochexian.top/gtgjbzwufw.html

TS:   interface Shape { area(): number; }
来源：http://hz.yuanzhike.top/gtsarkvsmb.html

Java: interface Shape { double area(); }
来源：http://hz.gogol.net.cn/gtlehqlaof.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.dashuyun.cn/gtvwjuhogw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yangfankeji.com/gteebzwmvm.html

C#:   interface IShape { double Area(); }
来源：http://hz.ivvv.top/gtpydqkwho.html

[G10] 访问控制
来源：http://hz.yj202588.top/gtccdwxmgq.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yangfankeji.com/gtbgiphlpb.html

PHP:  public / protected / private
来源：http://hz.guannengcc.top/gtqlfpraux.html

JS:   #private 字段；其余公开
来源：http://hz.bjfxy.top/gtzkendpcq.html

TS:   public / protected / private
来源：http://hz.hammf.cn/gtwlqehuio.html

Java: public / protected / private / 默认包级
来源：http://hz.meibo888.top/gtzdlmzozq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.snrcjt.cn/gtssdrzvxf.html

Ruby: public / protected / private
来源：http://hz.sysykeji.top/gtzbvqccrt.html

C#:   public / protected / private / internal
来源：http://hz.sufxvd.cn/gtxpsieidn.html

[G11] getter / setter
来源：http://hz.jqgfzy.top/gtguajqzju.html

Py:   @property 与 @x.setter
来源：http://hz.ywan-chungtsiang.top/gtypyogjlw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.haohaochexian.top/gtxxzadyxt.html

JS:   get name() { return this._name; }
来源：http://hz.redwolf501.top/gtzbaizmgt.html

TS:   get name(): string { return this._name; }
来源：http://hz.smart0.xyz/gtyxinxpql.html

Java: public String getName() { return name; }
来源：http://hz.hfpthk.cn/gtuwmfxlba.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.shanyushiyangtech.top/gtyhvkuoco.html

Ruby: attr_accessor :name
来源：http://hz.hongshengwenyu.top/gtpmgkqoro.html

C#:   public string Name { get; set; }
来源：http://hz.hnxiangtu.top/gtiqvaspwv.html

[G12] 对象转字符串
来源：http://hz.zhongyouzk.top/gtzksjtblh.html

Py:   def __str__(self): return self.name
来源：http://hz.wangshuangyany.cn/gtaqdypqrx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yj20258888.top/gtltttilwz.html

JS:   toString() { return this.name; }
来源：http://hz.mhx1999.top/gtwsuradyf.html

TS:   toString(): string { return this.name; }
来源：http://hz.pengpengdd.cyou/gtioydrotp.html

Java: @Override public String toString() { return name; }
来源：http://hz.fengsongda.top/gtlmlhqbcv.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.hammf.cn/gtitvmvtbc.html

Ruby: def to_s; @name; end
来源：http://hz.shanyushiyangkeji.top/gtzacodlob.html

C#:   public override string ToString() => Name;
来源：http://hz.shzxlz.cn/gtnebkklfp.html

[G13] 判断对象类型
来源：http://hz.cdnleiting.top/gtozughvhw.html

Py:   isinstance(u, User)
来源：http://hz.meibo888.top/gtxnlsivta.html

PHP:  $u instanceof User
来源：http://hz.yvedp.cn/gtlmhrvlqi.html

JS:   u instanceof User
来源：http://hz.hongshengwenyu.top/gtvdkcwdkv.html

TS:   u instanceof User
来源：http://hz.wangdashe.top/gtmhqupawk.html

Java: u instanceof User
来源：http://hz.pengpengdd.cyou/gtzvnuekpm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.dashuyun.cn/gtnanyefsf.html

Ruby: u.is_a?(User)
来源：http://hz.zhoulong.xyz/gtfbcqzvhq.html

C#:   u is User
来源：http://hz.sxryk.cn/gtnfugsgax.html

[G14] 数据类 / record
来源：http://hz.bjfxy.top/gtqvhsapaf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zhaomingkeji.xyz/gtmlvyokae.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zhijiandao.cn/gtdaplakbl.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.ivvv.top/gtgehuhvik.html

TS:   type User = { name: string; age: number };
来源：http://hz.yuxming.cn/gtwyvaqlrd.html

Java: record User(String name, int age) {}
来源：http://hz.jinqigufen.top/gtyvpjcjez.html

Go:   type User struct { Name string; Age int }
来源：http://hz.pengpengdd.cyou/gtoecrvlyn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.andypj.xyz/gtqbyaerno.html

C#:   record User(string Name, int Age);
来源：http://hz.zhongyouzk.top/gtgbrrmoom.html

[G15] 枚举
来源：http://hz.sxryk.cn/gtiqllwbir.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zhengqikj.top/gthvgcldly.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yj202588.top/gtsikjktgn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.ydzc1.top/gthnmnqcna.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhengqikj.top/gtoxbccrrf.html

Java: enum Color { RED, GREEN }
来源：http://hz.shanyushiyangtech.top/gtacvjizpd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.cheryme.top/gtbsitlwmo.html

Ruby: Color = %i[red green].freeze
来源：http://hz.shangyingyoupin.top/gtqscqufpk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cheryme.top/gtgyjhtnok.html

[G16] 对象转数组 / 字典
来源：http://hz.daxiang520.top/gtwhclybjz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.cucudq.cn/gthjujivad.html

PHP:  get_object_vars($obj);
来源：http://hz.zycfv.cn/gtenvtvrqj.html

JS:   Object.entries(obj)
来源：http://hz.aizwys.cn/gtqebbcypf.html

TS:   Object.entries(obj)
来源：http://hz.jinyuanbaomall.cn/gtzrhfkuec.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jiagoushi.top/gturkztwot.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hnqzz.top/gtzjlcrymw.html

Ruby: obj.instance_variables
来源：http://hz.hongshengwenyu.top/gtljzgoxyt.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.aizwys.cn/gtqfiunpje.html

================================================================================
来源：http://hz.zhoulong.xyz/gtdabxueoa.html

H. 异常与错误处理
来源：http://hz.kuanghao11.cn/gtkwqpxvpa.html

================================================================================
来源：http://hz.guannengcc.top/gtnpjplikv.html

[H01] try / catch 基础
来源：http://hz.52xcode.cn/gtfcgpfetk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.birdmap.top/gtyodyexod.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.c1oappe.top/gtlsfxlabs.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yongpay.top/gtuyxrnboh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hammf.cn/gtjzzluecx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.quarkkingdee.top/gthikfaptj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.9152youxi.cn/gtsgcdqnqa.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jinyuanbaomall.cn/gtyulhilft.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yueranfly.top/gtfmkhvudl.html

[H02] finally / ensure 收尾
来源：http://hz.nanxuanxn.top/gtaqdkwrsl.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.chenjidiqi.icu/gteirifukd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.nanxinkj.top/gtstvdadtq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.bjfxy.top/gtmrjkussy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.hnxiangtu.top/gtcvanocob.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.quarkkingdee.top/gtyvharyjj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hfpthk.cn/gtkdnvhhwf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.hongshengwenyu.top/gtekxvdkpd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.xylfe.cn/gtfycjxhgb.html

[H03] 主动抛出异常
来源：http://hz.cqqwz.cn/gtzodtgypd.html

Py:   raise ValueError("错误信息")
来源：http://hz.ywan-chungtsiang.top/gtnibizqcg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yj202588.top/gtayncfxou.html

JS:   throw new Error("错误信息");
来源：http://hz.tian-w.cn/gtvfpuzqwd.html

TS:   throw new Error("错误信息");
来源：http://hz.xuetiantiany.cn/gtspsngdxf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yvedp.cn/gtyamdyfqa.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jinqigfzy.top/gthrfztmxq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.xziqi.cn/gtgcpmknni.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.cucudq.cn/gtzvdnxchq.html

[H04] 自定义异常类型
来源：http://hz.feifeiyinyue.top/gtrjczszza.html

Py:   class MyError(Exception): pass
来源：http://hz.iojbl.cn/gtmqadharm.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jinyuanbaomall.cn/gtrlhtjdqe.html

JS:   class MyError extends Error {}
来源：http://hz.nanxinkj.top/gtfwakqkzl.html

TS:   class MyError extends Error {}
来源：http://hz.hammf.cn/gtgfwhkatd.html

Java: class MyException extends RuntimeException {}
来源：http://hz.iojbl.cn/gtrautugck.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.tianlin.xyz/gtgwrdfpdc.html

Ruby: class MyError < StandardError; end
来源：http://hz.feifeiyinyue.top/gtfhhasmqw.html

C#:   class MyException : Exception {}
来源：http://hz.zdqjudy.top/gtiziechft.html

[H05] 捕获特定类型
来源：http://hz.jianghu66.top/gtktxpnoij.html

Py:   except ValueError as e:
来源：http://hz.9152youxi.cn/gtqkdzvgkv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yj202588.top/gtswjclyuc.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.aizwys.cn/gtadqbcelp.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.xingfuxueyuan.xyz/gtbqmiknkt.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.meibo888.top/gtfwtjnfcd.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.meibo888.top/gtwgzytfkc.html

Ruby: rescue ArgumentError => e
来源：http://hz.zhiwuduotai.top/gtcheyoomd.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.xuanzx.com/gtxfclcuzw.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jinqigufen.top/gtcnltrnri.html

Py:   value = d.get("k") or default
来源：http://hz.pengpengdd.cyou/gtjyhkvfkt.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yonumen.top/gtihgyjuir.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jqgufenzy.top/gtiintjchu.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.ehwqpu.com/gtwxrneqsy.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.guannengcc.top/gtpmeiwovp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.haohaochexian.top/gtfavnfehl.html

Ruby: d&.dig(:a, :b)
来源：http://hz.gogol.net.cn/gtuaitydxp.html

C#:   obj?.A?.B ?? default
来源：http://hz.tianlin.xyz/gtmhaohsfj.html

[H07] 断言
来源：http://hz.daria6918.cn/gtatbahpek.html

Py:   assert x > 0, "必须为正"
来源：http://hz.aizwys.cn/gtcuxkhvlh.html

PHP:  assert($x > 0);
来源：http://hz.nanxinkj.top/gtryvxysrs.html

JS:   console.assert(x > 0);
来源：http://hz.cucudq.cn/gtoxmmqzxh.html

TS:   console.assert(x > 0);
来源：http://hz.bjfxy.top/gtmjlwagfc.html

Java: assert x > 0 : "必须为正";
来源：http://hz.cheryme.top/gtetwumoon.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.snrcjt.cn/gtgbuyrjbj.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.sufxvd.cn/gtrbqhgqzi.html

C#:   Debug.Assert(x > 0);
来源：http://hz.hfpthk.cn/gtwzuklvrl.html

[H08] 获取错误信息与堆栈
来源：http://hz.smart0.xyz/gtevpbvsuw.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yueranfly.top/gtkflllajw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.chenlongwang.top/gtwwgipbwb.html


<!-- 参考信息 -->