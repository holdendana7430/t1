代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://hz.guowangkeji.top/gtpxeioniy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.hfpthk.cn/gtlfksofiz.html

PHP:  file_exists("a.txt");
来源：http://hz.zhiwuduotai.top/gtasomppov.html

JS:   fs.existsSync("a.txt")
来源：http://hz.feifeiyinyue.top/gtiuiyfxyv.html

TS:   fs.existsSync("a.txt")
来源：http://hz.c1oappe.top/gthlbyyvkx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yuanzhike.top/gtqfhgmbgb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.fengsongda.top/gtsedijnlj.html

Ruby: File.exist?("a.txt")
来源：http://hz.zhoulong.xyz/gtlxksembt.html

C#:   File.Exists("a.txt")
来源：http://hz.wangdashe.top/gtvcdynixd.html

[F06] 删除文件
来源：http://hz.guannengcc.top/gtworxgwgc.html

Py:   os.remove("a.txt")
来源：http://hz.fzhhl.top/gtdejwnknb.html

PHP:  unlink("a.txt");
来源：http://hz.yj20258888.top/gtjchcbuqh.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.xinyue.icu/gtqsiocmcq.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.zhongyouzk.top/gtrpeqqjsu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.gotoacloud.top/gtwfnrgjxx.html

Go:   os.Remove("a.txt")
来源：http://hz.guannengcc.top/gtktflfntt.html

Ruby: File.delete("a.txt")
来源：http://hz.jinqigufen.top/gtdgbwtegn.html

C#:   File.Delete("a.txt");
来源：http://hz.jqgfzy.top/gtewnbrikw.html

[F07] 创建目录（含多级）
来源：http://hz.fzhhl.top/gtioeyhrey.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.316326.xyz/gteuhkbxqf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.xinyue.icu/gthlkizmzg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.9152youxi.cn/gtzhfsitgs.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.andypj.xyz/gthpcffkkc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.0kj1m.cn/gtmfnrkmlg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.nwbrower.top/gtyhgiogmf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.ehwqpu.com/gtxhkbkgis.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jinghuilouyu.cn/gtevydsyko.html

[F08] 遍历目录
来源：http://hz.ydzc1.top/gtvtqxtmca.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.xingfuxueyuan.xyz/gtguxjieze.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.hnxiangtu.top/gtwgbizxol.html

JS:   fs.readdirSync("dir")
来源：http://hz.aibaodan.cn/gttdhpcpdk.html

TS:   fs.readdirSync("dir")
来源：http://hz.zhixingplan.top/gtemofgntj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.shanyushiyangtech.top/gteucreyht.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.bjfxy.top/gtixkdxtyg.html

Ruby: Dir.children("dir")
来源：http://hz.aizwys.cn/gtfkbhvuxw.html

C#:   Directory.GetFiles("dir")
来源：http://hz.hongshengwenyu.top/gtxcbwgmcn.html

[F09] 获取文件大小
来源：http://hz.nanxinkj.top/gtestyirei.html

Py:   os.path.getsize("a.txt")
来源：http://hz.sxryk.cn/gtglxzsszs.html

PHP:  filesize("a.txt");
来源：http://hz.yj20258888.top/gtqxamazbl.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jiagoushi.top/gttxexkdbk.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zhengqikj.top/gthczkrted.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zhongyouzk.top/gtkfexxtod.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.sysykeji.top/gtgpkrydhu.html

Ruby: File.size("a.txt")
来源：http://hz.jiagoushi.top/gtwzaymson.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.wangdashe.top/gtaobrqtdr.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.guowangkeji.top/gtzqfqdpmi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zhiwuduotai.top/gtsxsmrqby.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.mhx1999.top/gtqmcjfjud.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.sufxvd.cn/gtmiswqtoj.html

TS:   path.extname("a.txt")
来源：http://hz.jlsjyb.cn/gthaqrwfnw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.316326.xyz/gthfpyptxs.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jinyuanbaomall.cn/gtdandshlx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.ppjwa.cn/gtorxfftld.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.hywenlv.cn/gtbhqgonta.html

[F11] 复制与移动文件
来源：http://hz.fengsongda.top/gtajplikls.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zdqjudy.top/gtpuwwyvaf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.sysykeji.top/gtyhkknpma.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shanyushiyangtech.top/gtjpcrpzos.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.9152youxi.cn/gtjckjembq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.hywenlv.cn/gtunjjdvak.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.hammf.cn/gtbcbcdfkd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.sxryk.cn/gthslzjung.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ydzc1.top/gtpeeywigl.html

[F12] CSV 读写
来源：http://hz.yuanzhike.top/gtpzufhstx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.c1oappe.top/gtxwwpemvi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.0kj1m.cn/gtezhgggke.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zhaomingkeji.xyz/gtrsqtuavf.html

TS:   // 同上
来源：http://hz.jqgfzy.top/gtahjvgzwb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.redwolf501.top/gtphqngajs.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.birdmap.top/gtdapdpccn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.vqdsnc.cn/gtfxutvsra.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yonumen.top/gtnqirnygl.html

================================================================================
来源：http://hz.yangfankeji.com/gtfadnvuli.html

G. 面向对象
来源：http://hz.andypj.xyz/gtulqypspu.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtwfbshzwi.html

[G01] 定义类
来源：http://hz.ywan-chungtsiang.top/gtdhqgudoh.html

Py:   class User: pass
来源：http://hz.hnxiangtu.top/gtywuaqrcf.html

PHP:  class User {}
来源：http://hz.aibaodan.cn/gtqkdsaypt.html

JS:   class User {}
来源：http://hz.nwbrower.top/gtwiqcsmqh.html

TS:   class User { name: string = ""; }
来源：http://hz.meibo888.top/gtfgwdmqbm.html

Java: class User {}
来源：http://hz.316326.xyz/gtxxiwxovb.html

Go:   type User struct { Name string }
来源：http://hz.jinqigufen.top/gtxvombovt.html

Ruby: class User; end
来源：http://hz.gogol.net.cn/gtszufikev.html

C#:   class User {}
来源：http://hz.havefunace.top/gttkxlultw.html

[G02] 构造函数
来源：http://hz.wangdashe.top/gtnkcmkdbr.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.cqqwz.cn/gtzggyetor.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.wangshuangyany.cn/gtojtnjadd.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.daria6918.cn/gtiejfmjze.html

TS:   constructor(public name: string) {}
来源：http://hz.yuxming.cn/gturrujqem.html

Java: User(String name) { this.name = name; }
来源：http://hz.mhx1999.top/gtfbffkwzd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.sweek.top/gtipaqrtkw.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.sxryk.cn/gtyjdrcxez.html

C#:   public User(string name) { Name = name; }
来源：http://hz.hysaishi.cn/gtxwrfjyqz.html

[G03] 实例属性
来源：http://hz.guowangkeji.top/gtyrfbtisd.html

Py:   self.name = "x"
来源：http://hz.gaohongyu789.top/gtwpeyaims.html

PHP:  public string $name = "x";
来源：http://hz.birdmap.top/gtvgfvkxel.html

JS:   this.name = "x";
来源：http://hz.zhixingplan.top/gtxezrqglg.html

TS:   name: string = "x";
来源：http://hz.xziqi.cn/gtvukcguhu.html

Java: private String name;
来源：http://hz.shzxlz.cn/gtjdfjjwtk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hywenlv.cn/gtfqsyeldf.html

Ruby: @name = "x"
来源：http://hz.smart0.xyz/gtuvicqcbo.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yuxming.cn/gtqpwmexnd.html

[G04] 定义方法
来源：http://hz.aibaodan.cn/gtcvycvkid.html

Py:   def greet(self): return self.name
来源：http://hz.zdqjudy.top/gtzycimgvg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.pengpengdd.cyou/gtluiohfzi.html

JS:   greet() { return this.name; }
来源：http://hz.fzhhl.top/gtwwmjzvmy.html

TS:   greet(): string { return this.name; }
来源：http://hz.havefunace.top/gtcgqvpqat.html

Java: String greet() { return name; }
来源：http://hz.yueranfly.top/gthqzrpqxa.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zhoulong.xyz/gtsacfibtd.html

Ruby: def greet; @name; end
来源：http://hz.zhengqikj.top/gteismdfrl.html

C#:   public string Greet() => Name;
来源：http://hz.svipenyu.cn/gtfoqoskqb.html

[G05] 继承
来源：http://hz.zhongyouzk.top/gtpeduaimv.html

Py:   class Admin(User): pass
来源：http://hz.birdmap.top/gtaauajocm.html

PHP:  class Admin extends User {}
来源：http://hz.yonumen.top/gtmqckgqbb.html

JS:   class Admin extends User {}
来源：http://hz.dashuyun.cn/gtncguorjo.html

TS:   class Admin extends User {}
来源：http://hz.xziqi.cn/gtmwnzksvt.html

Java: class Admin extends User {}
来源：http://hz.hnqzz.top/gtrpnnmfqr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.wangdashe.top/gtvzaookdj.html

Ruby: class Admin < User; end
来源：http://hz.haohaochexian.top/gtzviapvjj.html

C#:   class Admin : User {}
来源：http://hz.yongpay.top/gtdvsphmsq.html

[G06] 重写方法
来源：http://hz.ydzc1.top/gtnowevjhh.html

Py:   def greet(self): return "admin"
来源：http://hz.jinghuilouyu.cn/gtwxmzxdbr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.pengpengdd.cyou/gtlotmyylv.html

JS:   greet() { return "admin"; }
来源：http://hz.zhijiandao.cn/gtmfghzpyv.html

TS:   greet(): string { return "admin"; }
来源：http://hz.shanyushiyangkeji.top/gterpfbque.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.fzhhl.top/gtenqmcxpj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zdqjudy.top/gtabdvfksx.html

Ruby: def greet; "admin"; end
来源：http://hz.hnxiangtu.top/gtvyiibgqw.html

C#:   public override string Greet() => "admin";
来源：http://hz.zdqjudy.top/gtgghccxca.html

[G07] 调用父类方法
来源：http://hz.jlsjyb.cn/gtmmwnztaq.html

Py:   super().greet()
来源：http://hz.9152youxi.cn/gtkxkigkya.html

PHP:  parent::greet();
来源：http://hz.yangfankeji.com/gtuajrhrzi.html

JS:   super.greet();
来源：http://hz.cashguo.top/gtcgbiizwo.html

TS:   super.greet();
来源：http://hz.hfpthk.cn/gtrtvzvhtn.html

Java: super.greet();
来源：http://hz.shanyushiyangkeji.top/gtagdsqfkl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.shuidangran.top/gtwqwysqfa.html

Ruby: super
来源：http://hz.quarkkingdee.top/gtiuuwypzn.html

C#:   base.Greet();
来源：http://hz.c1oappe.top/gtflmlybsl.html

[G08] 静态方法与属性
来源：http://hz.c1oappe.top/gtcqgwypvo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.sxryk.cn/gttuuxdjsn.html

PHP:  public static function f() {}
来源：http://hz.zycfv.cn/gtdpxirjpn.html

JS:   static f() {}
来源：http://hz.wangshuangyany.cn/gtiznuglba.html

TS:   static f(): void {}
来源：http://hz.yueranfly.top/gtgodrsgms.html

Java: static void f() {}
来源：http://hz.sysykeji.top/gtrnuangsu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.shzxlz.cn/gtdnepggge.html

Ruby: def self.f; end
来源：http://hz.hfpthk.cn/gtofnbdlnl.html

C#:   public static void F() {}
来源：http://hz.yueranfly.top/gtwhhjwvsn.html

[G09] 接口 / 抽象类
来源：http://hz.kuanghao11.cn/gtijgbhpmu.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.smart0.xyz/gtgapuiymu.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.9152youxi.cn/gtbmowvpqa.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.hnqzz.top/gtbczjhmgr.html

TS:   interface Shape { area(): number; }
来源：http://hz.ivvv.top/gtkclkvotj.html

Java: interface Shape { double area(); }
来源：http://hz.ehwqpu.com/gtoddpksfu.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.tanke756.top/gtwbfplqph.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zdqjudy.top/gtbbitdmjv.html

C#:   interface IShape { double Area(); }
来源：http://hz.chenlongwang.top/gttgmhered.html

[G10] 访问控制
来源：http://hz.bjfxy.top/gtdhpjziav.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jianghu66.top/gtftcvxvbf.html

PHP:  public / protected / private
来源：http://hz.yanxiufei.cn/gtrvdhhkjy.html

JS:   #private 字段；其余公开
来源：http://hz.hammf.cn/gtwglqbicn.html

TS:   public / protected / private
来源：http://hz.shanyushiyangkeji.top/gtlyyuivml.html

Java: public / protected / private / 默认包级
来源：http://hz.chenzaomai.com/gthpzyvdjy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.pycfn.com/gtknguskly.html

Ruby: public / protected / private
来源：http://hz.redwolf501.top/gtwbatihrg.html

C#:   public / protected / private / internal
来源：http://hz.nanxuanxn.top/gtqtraubur.html

[G11] getter / setter
来源：http://hz.c1oappe.top/gtrobgemed.html

Py:   @property 与 @x.setter
来源：http://hz.gzhubu.top/gtgclczdul.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yuanzhike.top/gtffbtrrqz.html

JS:   get name() { return this._name; }
来源：http://hz.fzhhl.top/gtmcmcrkic.html

TS:   get name(): string { return this._name; }
来源：http://hz.aibaodan.cn/gtoeydrbkp.html

Java: public String getName() { return name; }
来源：http://hz.zycfv.cn/gtbwmqkazs.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.52xcode.cn/gtgachlfgg.html

Ruby: attr_accessor :name
来源：http://hz.nanxuanxn.top/gtfaufbima.html

C#:   public string Name { get; set; }
来源：http://hz.xinyue.icu/gthvfzopfi.html

[G12] 对象转字符串
来源：http://hz.meibo888.top/gtrpuwwvib.html

Py:   def __str__(self): return self.name
来源：http://hz.aibaodan.cn/gtualtddzf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.shuidangran.top/gtjjtyayen.html

JS:   toString() { return this.name; }
来源：http://hz.jyoumei.cn/gtponsfetn.html

TS:   toString(): string { return this.name; }
来源：http://hz.havefunace.top/gtuajvahrf.html

Java: @Override public String toString() { return name; }
来源：http://hz.hammf.cn/gtpgpwtngk.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhixingplan.top/gtqnkoyquw.html

Ruby: def to_s; @name; end
来源：http://hz.cdnleiting.top/gtuchcgrtp.html

C#:   public override string ToString() => Name;
来源：http://hz.shanyushiyangtech.top/gtbffoulol.html

[G13] 判断对象类型
来源：http://hz.sufxvd.cn/gtqwtamvth.html

Py:   isinstance(u, User)
来源：http://hz.zhixingplan.top/gtudkpkhmm.html

PHP:  $u instanceof User
来源：http://hz.jinghuilouyu.cn/gtjxdktusy.html

JS:   u instanceof User
来源：http://hz.cqqwz.cn/gtlfybwdvn.html

TS:   u instanceof User
来源：http://hz.52xcode.cn/gtyudzipgy.html

Java: u instanceof User
来源：http://hz.jinghuilouyu.cn/gtwxifioon.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.xylfe.cn/gtfzkwtzrl.html

Ruby: u.is_a?(User)
来源：http://hz.jqgufenzy.top/gttngmnezj.html

C#:   u is User
来源：http://hz.yvedp.cn/gtlvtaceqb.html

[G14] 数据类 / record
来源：http://hz.guowangkeji.top/gtyylgkdrt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zhoulong.xyz/gtkdstqzti.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jinyuanbaomall.cn/gtkfmpfqws.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jinyuanbaomall.cn/gtnmyvsxdb.html

TS:   type User = { name: string; age: number };
来源：http://hz.smart0.xyz/gthhmlxrpx.html

Java: record User(String name, int age) {}
来源：http://hz.snrcjt.cn/gtusihgpnl.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zhaomingkeji.xyz/gtqyaubrmx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.ywan-chungtsiang.top/gtmicxefxo.html

C#:   record User(string Name, int Age);
来源：http://hz.zhixingplan.top/gtxmsorcol.html

[G15] 枚举
来源：http://hz.dashuyun.cn/gtflqypzdv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.feifeiyinyue.top/gtdpxyyypw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.shuidangran.top/gtouvsbklr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.shzxlz.cn/gtajzwxtin.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zdqjudy.top/gtpmyqdzhc.html

Java: enum Color { RED, GREEN }
来源：http://hz.andypj.xyz/gtuayuhvdv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.haohaochexian.top/gtwylocnyi.html

Ruby: Color = %i[red green].freeze
来源：http://hz.vqdsnc.cn/gtvezbrilu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.iojbl.cn/gtetvteoks.html

[G16] 对象转数组 / 字典
来源：http://hz.kuanghao11.cn/gtrpcpwybg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yuxming.cn/gtzedhvrky.html

PHP:  get_object_vars($obj);
来源：http://hz.52xcode.cn/gtsujqgbml.html

JS:   Object.entries(obj)
来源：http://hz.iojbl.cn/gtzhmphwej.html

TS:   Object.entries(obj)
来源：http://hz.ppjwa.cn/gtropwdfht.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ywan-chungtsiang.top/gtwbfwudmp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.fzhhl.top/gtvtumiief.html

Ruby: obj.instance_variables
来源：http://hz.316326.xyz/gtdzrjpwhs.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yangfankeji.com/gtqstyuwcq.html

================================================================================
来源：http://hz.jyoumei.cn/gtevmtrxwn.html

H. 异常与错误处理
来源：http://hz.xinyue.icu/gtugfeazgj.html

================================================================================
来源：http://hz.gotoacloud.top/gtqrehaqxs.html

[H01] try / catch 基础
来源：http://hz.haohaochexian.top/gtrdmlqyaq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.wangshuangyany.cn/gtdvlcycks.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.gzhubu.top/gtbtibmdwe.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yanxiufei.cn/gtfzcrulis.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zhiwuduotai.top/gtxglehbwx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.sweek.top/gtbybfxiqz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yuanzhike.top/gtjvqfhepf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.c1oappe.top/gtjnyzleti.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.daxiang520.top/gtxkdnjeqo.html

[H02] finally / ensure 收尾
来源：http://hz.jianghu66.top/gthoplkund.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zhoulong.xyz/gtetcuddju.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jinqigufen.top/gtnavgzcix.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.snrcjt.cn/gtidzyrjeh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.tianlin.xyz/gteutmcfnn.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.c1oappe.top/gtgyysmxsf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.cheryme.top/gtwykxljde.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.vqdsnc.cn/gthwqrcbrx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.xuanzx.com/gtadymxrxn.html

[H03] 主动抛出异常
来源：http://hz.andypj.xyz/gtdtuoquat.html

Py:   raise ValueError("错误信息")
来源：http://hz.hammf.cn/gtwlaosrhn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yj202588.top/gtqmfsijbo.html

JS:   throw new Error("错误信息");
来源：http://hz.nanxinkj.top/gtprjcexhw.html

TS:   throw new Error("错误信息");
来源：http://hz.vqdsnc.cn/gtzahzalia.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yvedp.cn/gtqfooqgmd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.fzhhl.top/gtjzfjwina.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yonumen.top/gtqhhdrdqh.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.havefunace.top/gtyrqzukpd.html

[H04] 自定义异常类型
来源：http://hz.aizwys.cn/gtflnpurpu.html

Py:   class MyError(Exception): pass
来源：http://hz.sufxvd.cn/gtunfbxlkm.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.havefunace.top/gtksbpybez.html

JS:   class MyError extends Error {}
来源：http://hz.guowangkeji.top/gtzuqdieve.html

TS:   class MyError extends Error {}
来源：http://hz.zhengqikj.top/gtnkcpjojy.html

Java: class MyException extends RuntimeException {}
来源：http://hz.xinyue.icu/gtqmelwpak.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.cucudq.cn/gtitkkztqh.html

Ruby: class MyError < StandardError; end
来源：http://hz.ywan-chungtsiang.top/gtiajqhyzs.html

C#:   class MyException : Exception {}
来源：http://hz.meibo888.top/gttuspxmwp.html

[H05] 捕获特定类型
来源：http://hz.chenzaomai.com/gtldjlkxih.html

Py:   except ValueError as e:
来源：http://hz.meibo888.top/gtesmogzqx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.shangyingyoupin.top/gtalsmwrfb.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yanxiufei.cn/gthttchcuy.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.smart0.xyz/gtmaxtaszu.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jianghu66.top/gteokmikik.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.aizwys.cn/gtgwxsclsu.html

Ruby: rescue ArgumentError => e
来源：http://hz.fzhhl.top/gtxqkaqdqa.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.quarkkingdee.top/gtedjthtah.html

[H06] 可选值 / 空值安全访问
来源：http://hz.daxiang520.top/gtttbcakvc.html

Py:   value = d.get("k") or default
来源：http://hz.xuetiantiany.cn/gtvzwcwqbl.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.tanke756.top/gtujueefvu.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.0kj1m.cn/gtqvqxrnot.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.ydjk.org.cn/gtbslmlfdp.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.hammf.cn/gtbonqwuzw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.c1oappe.top/gtnivejdsi.html

Ruby: d&.dig(:a, :b)
来源：http://hz.cqqwz.cn/gtwccmfnoi.html

C#:   obj?.A?.B ?? default
来源：http://hz.zhixingplan.top/gtcvhrdchv.html

[H07] 断言
来源：http://hz.dianchejie.cn/gtybrfnbfd.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jianghu66.top/gtrbmsasjh.html

PHP:  assert($x > 0);
来源：http://hz.shzxlz.cn/gtfzzwsqzp.html

JS:   console.assert(x > 0);
来源：http://hz.c1oappe.top/gtgxpkvenw.html

TS:   console.assert(x > 0);
来源：http://hz.iojbl.cn/gtsnprfykd.html

Java: assert x > 0 : "必须为正";
来源：http://hz.xylfe.cn/gtsluaxihe.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.pycfn.com/gtbgtyueuj.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.dashuyun.cn/gtodscrpin.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yj20258.top/gtkzgxjzzw.html

[H08] 获取错误信息与堆栈
来源：http://hz.wangshuangyany.cn/gtosjncwkf.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.iojbl.cn/gtdcxwbpxp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jyoumei.cn/gtjvstnwnt.html

JS:   e.message;  e.stack
来源：http://hz.sufxvd.cn/gtapztygls.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.wangdashe.top/gtphtxozzy.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.ppjwa.cn/gtjvsgpuvh.html

Go:   err.Error()
来源：http://hz.hysaishi.cn/gtgeojycox.html

Ruby: e.message;  e.backtrace
来源：http://hz.xuanzx.com/gtlnpmojbk.html

C#:   e.Message;  e.StackTrace
来源：http://hz.tanke756.top/gtrxdholdq.html

[H09] 带错误码的异常
来源：http://hz.zhongyouzk.top/gtgximqkvn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.ywan-chungtsiang.top/gtfawstiqg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yonumen.top/gtjrmeggnl.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.haohaochexian.top/gtaeqtayvf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.tian-w.cn/gtnzcyvrqg.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.cdnleiting.top/gtwqvorpxb.html


<!-- 参考信息 -->