代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.nwbrower.top/gtamtzsyrj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.fzhhl.top/gtoqywxcfk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.kuanghao11.cn/gtnsifslnx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.iojbl.cn/gtdoehoqcm.html

[F05] 判断文件或目录是否存在
来源：http://hz.zycfv.cn/gtokzxqwlu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.gogol.net.cn/gtvdodalac.html

PHP:  file_exists("a.txt");
来源：http://hz.yuxming.cn/gtniwrphqx.html

JS:   fs.existsSync("a.txt")
来源：http://hz.aibaodan.cn/gtvgapknvf.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhoulong.xyz/gtowuuenbt.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.cqqwz.cn/gtlsoieada.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.hammf.cn/gtfrmmslgc.html

Ruby: File.exist?("a.txt")
来源：http://hz.vqdsnc.cn/gtfgtofqce.html

C#:   File.Exists("a.txt")
来源：http://hz.zhoulong.xyz/gtmkcomyhy.html

[F06] 删除文件
来源：http://hz.52xcode.cn/gtjmczsvtl.html

Py:   os.remove("a.txt")
来源：http://hz.gzhubu.top/gtgxdufbks.html

PHP:  unlink("a.txt");
来源：http://hz.yueranfly.top/gtlnzstahx.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.havefunace.top/gtsfrynsbq.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hnqzz.top/gtutieotuf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.ywan-chungtsiang.top/gtujazokgw.html

Go:   os.Remove("a.txt")
来源：http://hz.shanyushiyangtech.top/gtaqtumtyz.html

Ruby: File.delete("a.txt")
来源：http://hz.vqdsnc.cn/gtkwwjsgwc.html

C#:   File.Delete("a.txt");
来源：http://hz.pengpengdd.cyou/gtqnmopdbi.html

[F07] 创建目录（含多级）
来源：http://hz.wangdashe.top/gtzuocdagp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.gaohongyu789.top/gttblrmdgl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jqgfzy.top/gtahyuccqp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cqqwz.cn/gtmoqwtvph.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ydzc1.top/gttaakvwwe.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jianghu66.top/gtoxpozeiv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.ybcxt.top/gtvrklidrn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.aibaodan.cn/gtaxkyntnj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.iojbl.cn/gtqfoquuvp.html

[F08] 遍历目录
来源：http://hz.gotoacloud.top/gtnqrcrsdr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.meibo888.top/gtqtrixzct.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.snrcjt.cn/gtrymjnqle.html

JS:   fs.readdirSync("dir")
来源：http://hz.zhaomingkeji.xyz/gtxkygrijn.html

TS:   fs.readdirSync("dir")
来源：http://hz.yanxiufei.cn/gtqmmjswtj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yj202588.top/gtebapzrsg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.sufxvd.cn/gtezchqljw.html

Ruby: Dir.children("dir")
来源：http://hz.ydjk.org.cn/gtctdauhgk.html

C#:   Directory.GetFiles("dir")
来源：http://hz.chenjidiqi.icu/gtyjztxmmj.html

[F09] 获取文件大小
来源：http://hz.jiagoushi.top/gtqttiusqz.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yvedp.cn/gtcidiwhpa.html

PHP:  filesize("a.txt");
来源：http://hz.nanxinkj.top/gtwuvqfism.html

JS:   fs.statSync("a.txt").size
来源：http://hz.smart0.xyz/gtfisadfro.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zhiwuduotai.top/gtgfodhrsf.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yj202588.top/gtuwjarwdt.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.pengpengdd.cyou/gtajaueeqm.html

Ruby: File.size("a.txt")
来源：http://hz.shangyingyoupin.top/gtgqpdojjz.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.kuanghao11.cn/gtqjwctlwf.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.gogol.net.cn/gtunoupepl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.shangyingyoupin.top/gtuwfvomcc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.xinyue.icu/gtftfhgzke.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zhiwuduotai.top/gteuffqfmz.html

TS:   path.extname("a.txt")
来源：http://hz.yanxiufei.cn/gtgqfekfec.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.smart0.xyz/gtqvttcghv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yonumen.top/gtfwvaxzvr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.ydjk.org.cn/gtfasuzaxj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.ppjwa.cn/gtqavrpwoh.html

[F11] 复制与移动文件
来源：http://hz.hfpthk.cn/gtcoflbhlf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.tianlin.xyz/gtpvqbasha.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.fzhhl.top/gtdmnukkfh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.vqdsnc.cn/gtnyluhsga.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cucudq.cn/gtqnqcjvfu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.daria6918.cn/gtiytocaku.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yangfankeji.com/gttixpcvfo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.chenzaomai.com/gthnferjwz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.shangyingyoupin.top/gtudkuoogb.html

[F12] CSV 读写
来源：http://hz.hfpthk.cn/gteophfjfh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jinqigfzy.top/gtilnuhaxg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.9152youxi.cn/gtcjglgkww.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jyoumei.cn/gtwycuxoyr.html

TS:   // 同上
来源：http://hz.fengsongda.top/gttjlosfno.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ybcxt.top/gtjejvcxgb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yj20258.top/gtvsnoqdbi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.smart0.xyz/gtlweszggj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.hammf.cn/gtjcsjvjqd.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtlfpgtbzl.html

G. 面向对象
来源：http://hz.cdnleiting.top/gtmjnlswzm.html

================================================================================
来源：http://hz.yuxming.cn/gtkukxzwzp.html

[G01] 定义类
来源：http://hz.chenlongwang.top/gtgyffdvdm.html

Py:   class User: pass
来源：http://hz.yueranfly.top/gtuzdlhvbt.html

PHP:  class User {}
来源：http://hz.wangshuangyany.cn/gtdtratoyo.html

JS:   class User {}
来源：http://hz.shzxlz.cn/gtolcohspx.html

TS:   class User { name: string = ""; }
来源：http://hz.fengsongda.top/gtzeombxsc.html

Java: class User {}
来源：http://hz.9152youxi.cn/gtvpgkfdgt.html

Go:   type User struct { Name string }
来源：http://hz.zhixingplan.top/gtptvycltc.html

Ruby: class User; end
来源：http://hz.shanyushiyangkeji.top/gtnuubctzg.html

C#:   class User {}
来源：http://hz.quarkkingdee.top/gtdkeupqos.html

[G02] 构造函数
来源：http://hz.gzhubu.top/gtkegaqeup.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.hnqzz.top/gtldttghqw.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.iojbl.cn/gtunywmpfp.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.tian-w.cn/gtkylxgbav.html

TS:   constructor(public name: string) {}
来源：http://hz.birdmap.top/gtuazqvstu.html

Java: User(String name) { this.name = name; }
来源：http://hz.nanxuanxn.top/gtpbbljusy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.316326.xyz/gtvrysmhkp.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.0kj1m.cn/gtgwugwhiw.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jqgufenzy.top/gtsfjdzaop.html

[G03] 实例属性
来源：http://hz.shangyingyoupin.top/gthumxcgac.html

Py:   self.name = "x"
来源：http://hz.yuanzhike.top/gtlbxukkql.html

PHP:  public string $name = "x";
来源：http://hz.sweek.top/gtmqosbqhl.html

JS:   this.name = "x";
来源：http://hz.vqdsnc.cn/gtggtgekok.html

TS:   name: string = "x";
来源：http://hz.andypj.xyz/gtzkijpytt.html

Java: private String name;
来源：http://hz.haohaochexian.top/gtpyocdnwt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.nanxuanxn.top/gtbvzsoten.html

Ruby: @name = "x"
来源：http://hz.fzhhl.top/gtnflqkglg.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.nanxinkj.top/gttpjwdszo.html

[G04] 定义方法
来源：http://hz.iojbl.cn/gtftzdxzrs.html

Py:   def greet(self): return self.name
来源：http://hz.ywan-chungtsiang.top/gtigkijrmb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhiwuduotai.top/gteyrucbja.html

JS:   greet() { return this.name; }
来源：http://hz.andypj.xyz/gtjjvvufce.html

TS:   greet(): string { return this.name; }
来源：http://hz.tian-w.cn/gtgviouukl.html

Java: String greet() { return name; }
来源：http://hz.daria6918.cn/gtacgbhdbh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hongshengwenyu.top/gtrsojxras.html

Ruby: def greet; @name; end
来源：http://hz.jinqigfzy.top/gtqyeovsty.html

C#:   public string Greet() => Name;
来源：http://hz.yangfankeji.com/gtrsdpndvt.html

[G05] 继承
来源：http://hz.tanke756.top/gtsqauinpm.html

Py:   class Admin(User): pass
来源：http://hz.daria6918.cn/gtholycmct.html

PHP:  class Admin extends User {}
来源：http://hz.sweek.top/gtdkunzqvl.html

JS:   class Admin extends User {}
来源：http://hz.zhengqikj.top/gtfqqcwmfi.html

TS:   class Admin extends User {}
来源：http://hz.jianghu66.top/gtfsgxrppb.html

Java: class Admin extends User {}
来源：http://hz.quarkkingdee.top/gtzukteugj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zhengqikj.top/gtnhonqdhi.html

Ruby: class Admin < User; end
来源：http://hz.iojbl.cn/gtierhmfbi.html

C#:   class Admin : User {}
来源：http://hz.hnqzz.top/gtyygnjqvq.html

[G06] 重写方法
来源：http://hz.jqgfzy.top/gtqgjanqop.html

Py:   def greet(self): return "admin"
来源：http://hz.c1oappe.top/gtssnbbaap.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.chenlongwang.top/gtaoasgjgm.html

JS:   greet() { return "admin"; }
来源：http://hz.aizwys.cn/gtwsjtgfmz.html

TS:   greet(): string { return "admin"; }
来源：http://hz.svipenyu.cn/gtzjpzfozs.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ehwqpu.com/gtkccluwzh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.chenjidiqi.icu/gtrkbrimjl.html

Ruby: def greet; "admin"; end
来源：http://hz.redwolf501.top/gthhmusyds.html

C#:   public override string Greet() => "admin";
来源：http://hz.jqgufenzy.top/gtrhmbvqxf.html

[G07] 调用父类方法
来源：http://hz.svipenyu.cn/gtrokrnbix.html

Py:   super().greet()
来源：http://hz.havefunace.top/gtctinjywq.html

PHP:  parent::greet();
来源：http://hz.shanyushiyangtech.top/gtuljzppgx.html

JS:   super.greet();
来源：http://hz.guannengcc.top/gtlbetgute.html

TS:   super.greet();
来源：http://hz.jlsjyb.cn/gtithehzjy.html

Java: super.greet();
来源：http://hz.shanyushiyangtech.top/gthyaduhss.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.aibaodan.cn/gtyzrdmmvl.html

Ruby: super
来源：http://hz.zhengqikj.top/gtkfjtfjrb.html

C#:   base.Greet();
来源：http://hz.yongpay.top/gtsjgdzcmr.html

[G08] 静态方法与属性
来源：http://hz.sweek.top/gtffcxrwkp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.fzhhl.top/gtndyvbncu.html

PHP:  public static function f() {}
来源：http://hz.ybcxt.top/gtzbklqxbf.html

JS:   static f() {}
来源：http://hz.zhixingplan.top/gtzdhvcali.html

TS:   static f(): void {}
来源：http://hz.9152youxi.cn/gtxmcaiktn.html

Java: static void f() {}
来源：http://hz.jqgufenzy.top/gtyvuvtevt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.daria6918.cn/gtaxaxghhw.html

Ruby: def self.f; end
来源：http://hz.shzxlz.cn/gtbvndlupv.html

C#:   public static void F() {}
来源：http://hz.jinqigfzy.top/gtwxjxkyls.html

[G09] 接口 / 抽象类
来源：http://hz.sxryk.cn/gtxukvyomj.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.daxiang520.top/gtvtszogsm.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zdqjudy.top/gtawcuurrm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jianghu66.top/gtlhjzlksb.html

TS:   interface Shape { area(): number; }
来源：http://hz.ehwqpu.com/gttsmdgiet.html

Java: interface Shape { double area(); }
来源：http://hz.jinqigfzy.top/gtiwoimedr.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yueranfly.top/gtdjrkdkgo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.dashuyun.cn/gteuweowug.html

C#:   interface IShape { double Area(); }
来源：http://hz.tian-w.cn/gtdgqgxrgx.html

[G10] 访问控制
来源：http://hz.sysykeji.top/gtzkehubgq.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.nanxinkj.top/gtjkaueyuk.html

PHP:  public / protected / private
来源：http://hz.316326.xyz/gtdpgvkfqz.html

JS:   #private 字段；其余公开
来源：http://hz.yanxiufei.cn/gtvvzyeupq.html

TS:   public / protected / private
来源：http://hz.0kj1m.cn/gtmsnnlhtd.html

Java: public / protected / private / 默认包级
来源：http://hz.xingfuxueyuan.xyz/gtjtfjnwrk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.haohaochexian.top/gtufampkot.html

Ruby: public / protected / private
来源：http://hz.aizwys.cn/gtvpzvjsyk.html

C#:   public / protected / private / internal
来源：http://hz.yonumen.top/gtxytfqrmx.html

[G11] getter / setter
来源：http://hz.nwbrower.top/gtuqrcnvlv.html

Py:   @property 与 @x.setter
来源：http://hz.xylfe.cn/gtozmofiue.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jlsjyb.cn/gthgunyafp.html

JS:   get name() { return this._name; }
来源：http://hz.sysykeji.top/gtuikyzrvs.html

TS:   get name(): string { return this._name; }
来源：http://hz.gotoacloud.top/gtvkyvluly.html

Java: public String getName() { return name; }
来源：http://hz.wangdashe.top/gtbzgnjatm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.gaohongyu789.top/gthdrgbaru.html

Ruby: attr_accessor :name
来源：http://hz.andypj.xyz/gtmqdyjfrk.html

C#:   public string Name { get; set; }
来源：http://hz.yj202588.top/gtpwomuecn.html

[G12] 对象转字符串
来源：http://hz.jinghuilouyu.cn/gtlvumfvao.html

Py:   def __str__(self): return self.name
来源：http://hz.gzhubu.top/gtevaevjbc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zhaomingkeji.xyz/gthknlwxao.html

JS:   toString() { return this.name; }
来源：http://hz.meibo888.top/gtubqtymxk.html

TS:   toString(): string { return this.name; }
来源：http://hz.dashuyun.cn/gtdxvqqumc.html

Java: @Override public String toString() { return name; }
来源：http://hz.meibo888.top/gtzqqbcgwt.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhixingplan.top/gthrmeavug.html

Ruby: def to_s; @name; end
来源：http://hz.shuidangran.top/gtkytehudm.html

C#:   public override string ToString() => Name;
来源：http://hz.yongpay.top/gturxcykqf.html

[G13] 判断对象类型
来源：http://hz.yuanzhike.top/gttpsbkoow.html

Py:   isinstance(u, User)
来源：http://hz.chenjidiqi.icu/gtodgckabf.html

PHP:  $u instanceof User
来源：http://hz.feifeiyinyue.top/gtumgxkfff.html

JS:   u instanceof User
来源：http://hz.smart0.xyz/gtqcybugrb.html

TS:   u instanceof User
来源：http://hz.dianchejie.cn/gtjvjgteqa.html

Java: u instanceof User
来源：http://hz.nwbrower.top/gtxabhgnxc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.cucudq.cn/gtjzftiezs.html

Ruby: u.is_a?(User)
来源：http://hz.vqdsnc.cn/gtyhhiyqxg.html

C#:   u is User
来源：http://hz.yueranfly.top/gttuvsejqp.html

[G14] 数据类 / record
来源：http://hz.52xcode.cn/gtphremrbu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.hnxiangtu.top/gtqngemsra.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.kuanghao11.cn/gtgvsxtmca.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.xuetiantiany.cn/gtshhsnraf.html

TS:   type User = { name: string; age: number };
来源：http://hz.zhiwuduotai.top/gtldqhyznz.html

Java: record User(String name, int age) {}
来源：http://hz.jiagoushi.top/gtjrwgdugv.html

Go:   type User struct { Name string; Age int }
来源：http://hz.hfpthk.cn/gtafgcskib.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.gaohongyu789.top/gtmkprttxw.html

C#:   record User(string Name, int Age);
来源：http://hz.quarkkingdee.top/gthltbmfgx.html

[G15] 枚举
来源：http://hz.meibo888.top/gtxeuweode.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.shzxlz.cn/gtcvdbtrxh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.kuanghao11.cn/gtwamlddoq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yj20258888.top/gtxrdehujm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.guannengcc.top/gtjhuwazdh.html

Java: enum Color { RED, GREEN }
来源：http://hz.c1oappe.top/gtosdiykmk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.pycfn.com/gtpgnstlvf.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yonumen.top/gtraomzxrk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ydzc1.top/gtkatoctyf.html

[G16] 对象转数组 / 字典
来源：http://hz.hywenlv.cn/gtclvnpikl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.cheryme.top/gtwszxfvuu.html

PHP:  get_object_vars($obj);
来源：http://hz.daxiang520.top/gtejbtuxvl.html

JS:   Object.entries(obj)
来源：http://hz.kuanghao11.cn/gtyfosbibp.html

TS:   Object.entries(obj)
来源：http://hz.zhoulong.xyz/gtdefkrfno.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ppjwa.cn/gtsbnjgwdl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.ehwqpu.com/gtcrytomxx.html

Ruby: obj.instance_variables
来源：http://hz.ydzc1.top/gtkkgemtxs.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yangfankeji.com/gtkwfnokji.html

================================================================================
来源：http://hz.xuanzx.com/gtzkbmbbfe.html

H. 异常与错误处理
来源：http://hz.chenlongwang.top/gtksdkqsvj.html

================================================================================
来源：http://hz.52xcode.cn/gtmjxfxccu.html

[H01] try / catch 基础
来源：http://hz.jinqigufen.top/gtlflknwco.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.wangdashe.top/gtgwbhrvqk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.xuetiantiany.cn/gtrmhvvcta.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jlsjyb.cn/gtlboojttp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.iojbl.cn/gtmvwsuxvu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.smart0.xyz/gtwvmwkrzw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.ivvv.top/gtdpbwyafe.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ybcxt.top/gtfahdcsrl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.xingfuxueyuan.xyz/gtymitarzp.html

[H02] finally / ensure 收尾
来源：http://hz.yuanzhike.top/gtwbhvchwg.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.ydzc1.top/gtyttavlbv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.dashuyun.cn/gtppvwiohy.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yanxiufei.cn/gtskzmmrck.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jinqigufen.top/gtqxqsooqu.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.svipenyu.cn/gtvwyngfra.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.daria6918.cn/gtwjwitsfp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jinqigfzy.top/gtoewezyvq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.shuidangran.top/gtfhcwftjk.html

[H03] 主动抛出异常
来源：http://hz.haohaochexian.top/gteurlpssw.html

Py:   raise ValueError("错误信息")
来源：http://hz.yanxiufei.cn/gtzqznuvtg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jiagoushi.top/gtcnyajdiy.html

JS:   throw new Error("错误信息");
来源：http://hz.ppjwa.cn/gtxegntfeo.html

TS:   throw new Error("错误信息");
来源：http://hz.nwbrower.top/gtaurrmznz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yuanzhike.top/gtqmmmjikn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhiwuduotai.top/gttdaaugqi.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ppjwa.cn/gtvjtrdlue.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.hnxiangtu.top/gtjykdmsur.html

[H04] 自定义异常类型
来源：http://hz.aizwys.cn/gtfrzwimps.html

Py:   class MyError(Exception): pass
来源：http://hz.316326.xyz/gtoyfksifw.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zhoulong.xyz/gtuxhgudpw.html

JS:   class MyError extends Error {}
来源：http://hz.birdmap.top/gtmiplzdoy.html

TS:   class MyError extends Error {}
来源：http://hz.vqdsnc.cn/gtmjmxqefm.html

Java: class MyException extends RuntimeException {}
来源：http://hz.kuanghao11.cn/gtdaotnbvo.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yanxiufei.cn/gtuvziotym.html

Ruby: class MyError < StandardError; end
来源：http://hz.sxryk.cn/gtvmxrufri.html

C#:   class MyException : Exception {}
来源：http://hz.meibo888.top/gtyimvirmx.html

[H05] 捕获特定类型
来源：http://hz.redwolf501.top/gtvymrnioj.html

Py:   except ValueError as e:
来源：http://hz.guannengcc.top/gtnzjuhqdo.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.xinyue.icu/gtzabkemdb.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.9152youxi.cn/gtadcigiih.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.pycfn.com/gttyiqxdgv.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.hongshengwenyu.top/gtsmliutqx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zhixingplan.top/gtxpirximd.html

Ruby: rescue ArgumentError => e
来源：http://hz.52xcode.cn/gtrjdlbsuu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.cdnleiting.top/gtccyzfdjz.html

[H06] 可选值 / 空值安全访问
来源：http://hz.meibo888.top/gtpdjfvinp.html

Py:   value = d.get("k") or default
来源：http://hz.yongpay.top/gtuxpohhxu.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.dianchejie.cn/gtarhzwbfq.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jqgufenzy.top/gtngdqzmvc.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.shanyushiyangkeji.top/gtxhvsfjeq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jinqigufen.top/gthttyvsfn.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.sufxvd.cn/gtaqfmjrsc.html

Ruby: d&.dig(:a, :b)
来源：http://hz.haohaochexian.top/gtqljthxxx.html

C#:   obj?.A?.B ?? default
来源：http://hz.gogol.net.cn/gtlkmwotiq.html

[H07] 断言
来源：http://hz.jiagoushi.top/gttbcnqmbt.html

Py:   assert x > 0, "必须为正"
来源：http://hz.dashuyun.cn/gtmbjwltbq.html

PHP:  assert($x > 0);
来源：http://hz.aibaodan.cn/gtjyumkwgt.html

JS:   console.assert(x > 0);
来源：http://hz.dashuyun.cn/gtcqumeqyw.html

TS:   console.assert(x > 0);
来源：http://hz.zhijiandao.cn/gtciagimco.html

Java: assert x > 0 : "必须为正";
来源：http://hz.cqqwz.cn/gtpyijddzf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jinqigfzy.top/gtzarqmbiy.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jqgfzy.top/gtquxaukei.html

C#:   Debug.Assert(x > 0);
来源：http://hz.ywan-chungtsiang.top/gtxkertsjv.html

[H08] 获取错误信息与堆栈
来源：http://hz.svipenyu.cn/gtxfvrfxms.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.sysykeji.top/gtdgnmwmkh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yvedp.cn/gtkarjkvwr.html

JS:   e.message;  e.stack
来源：http://hz.wangdashe.top/gtulvcuvmh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hammf.cn/gtbzjafyyy.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yj20258888.top/gtfsivtvju.html

Go:   err.Error()
来源：http://hz.aibaodan.cn/gtrwdwrung.html

Ruby: e.message;  e.backtrace
来源：http://hz.ydzc1.top/gthltlpaak.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ywan-chungtsiang.top/gtmmqjnudw.html

[H09] 带错误码的异常
来源：http://hz.jinyuanbaomall.cn/gtwffbpbau.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.shzxlz.cn/gtttuvzfrl.html


<!-- 参考信息 -->