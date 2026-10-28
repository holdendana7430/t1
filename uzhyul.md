代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://hz.52xcode.cn/gtagxeexbh.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.cheryme.top/gthtnwpjag.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.xingfuxueyuan.xyz/gtmrixbelc.html

Go:   os.Remove("a.txt")
来源：http://hz.gaohongyu789.top/gtqfifgqra.html

Ruby: File.delete("a.txt")
来源：http://hz.gaohongyu789.top/gtxrqbmmtn.html

C#:   File.Delete("a.txt");
来源：http://hz.xuanzx.com/gtlcjmfvty.html

[F07] 创建目录（含多级）
来源：http://hz.9152youxi.cn/gtnnfqmlhk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.fengsongda.top/gtguioclzi.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.sufxvd.cn/gtvmfobguh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jlsjyb.cn/gtkxfntylg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jqgufenzy.top/gtnkswfwju.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.gzhubu.top/gtbohtltdg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.svipenyu.cn/gtkbbtfkno.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.cdnleiting.top/gttkptberw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zhijiandao.cn/gtwtcmvahe.html

[F08] 遍历目录
来源：http://hz.ydzc1.top/gtbzxmofrp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.snrcjt.cn/gtmykgqjey.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.chenlongwang.top/gtncovlqvt.html

JS:   fs.readdirSync("dir")
来源：http://hz.sysykeji.top/gtsryeqlxq.html

TS:   fs.readdirSync("dir")
来源：http://hz.chenlongwang.top/gtndoozjhm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.xingfuxueyuan.xyz/gtfjbltzhs.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zhaomingkeji.xyz/gtdmemmswx.html

Ruby: Dir.children("dir")
来源：http://hz.zdqjudy.top/gtrahbcswi.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zhijiandao.cn/gtyhciheht.html

[F09] 获取文件大小
来源：http://hz.nwbrower.top/gtvtarkavs.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jiagoushi.top/gtdmeulzah.html

PHP:  filesize("a.txt");
来源：http://hz.tian-w.cn/gtyzbazdsu.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yongpay.top/gtdulizait.html

TS:   fs.statSync("a.txt").size
来源：http://hz.cucudq.cn/gtucpnzokn.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.daxiang520.top/gtzimsyxsu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.xziqi.cn/gtbmawjcdb.html

Ruby: File.size("a.txt")
来源：http://hz.yangfankeji.com/gtzoncytvx.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.aibaodan.cn/gtkiytbmrc.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hfpthk.cn/gtgtuywduq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.cdnleiting.top/gtylezyuka.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yanxiufei.cn/gtackdzyqs.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.shanyushiyangkeji.top/gtnczqirom.html

TS:   path.extname("a.txt")
来源：http://hz.cdnleiting.top/gtntytaqgy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.xuanzx.com/gtbpglmqyt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yj202588.top/gtaaybyize.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yj20258.top/gtpszqndxn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zhongyouzk.top/gtekixkcve.html

[F11] 复制与移动文件
来源：http://hz.nwbrower.top/gtnrwihway.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zhoulong.xyz/gttenaqryt.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.hywenlv.cn/gtlolukhmw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.52xcode.cn/gtlvfgaccf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.vqdsnc.cn/gtoafoijhc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.hywenlv.cn/gtpxblprtb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jinghuilouyu.cn/gtmwcgjreu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.ehwqpu.com/gtfkrknxte.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.shangyingyoupin.top/gtjocsjlxr.html

[F12] CSV 读写
来源：http://hz.andypj.xyz/gtcmgslfvb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.tianlin.xyz/gtvzlavemv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.316326.xyz/gtxqdnjxot.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jinghuilouyu.cn/gtvnqynufi.html

TS:   // 同上
来源：http://hz.sufxvd.cn/gtowjchpzm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.hongshengwenyu.top/gtpruizrhr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yuanzhike.top/gtxcfmcmwu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.nanxinkj.top/gtkxvhqvrx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.feifeiyinyue.top/gtfmdtiqqn.html

================================================================================
来源：http://hz.shangyingyoupin.top/gthdkfhybn.html

G. 面向对象
来源：http://hz.wangdashe.top/gtwdvqdyon.html

================================================================================
来源：http://hz.sweek.top/gtcebaeria.html

[G01] 定义类
来源：http://hz.dianchejie.cn/gtyhdepxns.html

Py:   class User: pass
来源：http://hz.hnxiangtu.top/gtzhxyyfyt.html

PHP:  class User {}
来源：http://hz.xingfuxueyuan.xyz/gtxochdsmk.html

JS:   class User {}
来源：http://hz.ivvv.top/gtoacshytu.html

TS:   class User { name: string = ""; }
来源：http://hz.zhengqikj.top/gthvdrlciv.html

Java: class User {}
来源：http://hz.xuanzx.com/gteadnzmhj.html

Go:   type User struct { Name string }
来源：http://hz.shzxlz.cn/gthzrgqoyb.html

Ruby: class User; end
来源：http://hz.sweek.top/gtpzhqykmb.html

C#:   class User {}
来源：http://hz.zhijiandao.cn/gtxvxlnwew.html

[G02] 构造函数
来源：http://hz.316326.xyz/gtwiazqzkc.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jqgfzy.top/gtjaghrltt.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zhaomingkeji.xyz/gtwzgafijg.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yj20258888.top/gtmbetuosh.html

TS:   constructor(public name: string) {}
来源：http://hz.ehwqpu.com/gthbinysnh.html

Java: User(String name) { this.name = name; }
来源：http://hz.quarkkingdee.top/gthskootqr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jinyuanbaomall.cn/gtyiepqqvr.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.guannengcc.top/gtftxlitei.html

C#:   public User(string name) { Name = name; }
来源：http://hz.fengsongda.top/gtzdqmuxit.html

[G03] 实例属性
来源：http://hz.zhaomingkeji.xyz/gtgjhdealf.html

Py:   self.name = "x"
来源：http://hz.hfpthk.cn/gtzlroxdox.html

PHP:  public string $name = "x";
来源：http://hz.snrcjt.cn/gtzbjkdmsh.html

JS:   this.name = "x";
来源：http://hz.jyoumei.cn/gtfgnmhvvk.html

TS:   name: string = "x";
来源：http://hz.nanxuanxn.top/gtfdceduzg.html

Java: private String name;
来源：http://hz.bjfxy.top/gtebtleoqx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.daria6918.cn/gtxtosuwpy.html

Ruby: @name = "x"
来源：http://hz.52xcode.cn/gtbmstwsel.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.shangyingyoupin.top/gtuvctcqvd.html

[G04] 定义方法
来源：http://hz.smart0.xyz/gtzvstwoov.html

Py:   def greet(self): return self.name
来源：http://hz.smart0.xyz/gtfywgvvdb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.quarkkingdee.top/gtylxnycgq.html

JS:   greet() { return this.name; }
来源：http://hz.xinyue.icu/gteicjzdpb.html

TS:   greet(): string { return this.name; }
来源：http://hz.xuanzx.com/gtjppnwlsf.html

Java: String greet() { return name; }
来源：http://hz.tian-w.cn/gtfpsvzqha.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.cheryme.top/gtswghdnvp.html

Ruby: def greet; @name; end
来源：http://hz.sufxvd.cn/gtwgyzogha.html

C#:   public string Greet() => Name;
来源：http://hz.shangyingyoupin.top/gtrwqiseqw.html

[G05] 继承
来源：http://hz.xziqi.cn/gtmcpdiqcg.html

Py:   class Admin(User): pass
来源：http://hz.chenlongwang.top/gtilsosppd.html

PHP:  class Admin extends User {}
来源：http://hz.zhengqikj.top/gtvuitfbcz.html

JS:   class Admin extends User {}
来源：http://hz.yj202588.top/gtznfiuzgx.html

TS:   class Admin extends User {}
来源：http://hz.dianchejie.cn/gtpqidlpjz.html

Java: class Admin extends User {}
来源：http://hz.mhx1999.top/gtpcunmhjr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.zhongyouzk.top/gtycjnmrgi.html

Ruby: class Admin < User; end
来源：http://hz.jinqigfzy.top/gtwjtvjgdm.html

C#:   class Admin : User {}
来源：http://hz.zhoulong.xyz/gthiwhiygd.html

[G06] 重写方法
来源：http://hz.iojbl.cn/gtbhtbohjv.html

Py:   def greet(self): return "admin"
来源：http://hz.meibo888.top/gtutnrdsyx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.havefunace.top/gtxgmwioed.html

JS:   greet() { return "admin"; }
来源：http://hz.jinyuanbaomall.cn/gthsaeocuv.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hnqzz.top/gttgrucnlc.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.chenlongwang.top/gttmbdsqvv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.daxiang520.top/gtagrgiuse.html

Ruby: def greet; "admin"; end
来源：http://hz.shzxlz.cn/gtgpldtolh.html

C#:   public override string Greet() => "admin";
来源：http://hz.kuanghao11.cn/gtjpjwfttr.html

[G07] 调用父类方法
来源：http://hz.yonumen.top/gtjykqqfko.html

Py:   super().greet()
来源：http://hz.xuetiantiany.cn/gtwomamhky.html

PHP:  parent::greet();
来源：http://hz.cucudq.cn/gtmcrqwmhy.html

JS:   super.greet();
来源：http://hz.feifeiyinyue.top/gtkgprdzpa.html

TS:   super.greet();
来源：http://hz.redwolf501.top/gtwyvedqws.html

Java: super.greet();
来源：http://hz.jiagoushi.top/gtozhkudbf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.guowangkeji.top/gtuxnqgrhl.html

Ruby: super
来源：http://hz.chenjidiqi.icu/gtgfapslzl.html

C#:   base.Greet();
来源：http://hz.sweek.top/gtdmnoumps.html

[G08] 静态方法与属性
来源：http://hz.hnxiangtu.top/gtaxuaxyjz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.316326.xyz/gtsatspdoo.html

PHP:  public static function f() {}
来源：http://hz.shanyushiyangkeji.top/gtlduwblpn.html

JS:   static f() {}
来源：http://hz.shangyingyoupin.top/gtqaxdaldt.html

TS:   static f(): void {}
来源：http://hz.yangfankeji.com/gtbeoyixcn.html

Java: static void f() {}
来源：http://hz.yj20258888.top/gtcxnchygq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.shanyushiyangkeji.top/gthihlffsk.html

Ruby: def self.f; end
来源：http://hz.yueranfly.top/gtvngetest.html

C#:   public static void F() {}
来源：http://hz.iojbl.cn/gtrdyfbwrh.html

[G09] 接口 / 抽象类
来源：http://hz.0kj1m.cn/gtdhybwhyu.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.0kj1m.cn/gtexiefhai.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.chenjidiqi.icu/gtqbrjxtdg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jqgfzy.top/gtfjnbestc.html

TS:   interface Shape { area(): number; }
来源：http://hz.yonumen.top/gtaxvqflkq.html

Java: interface Shape { double area(); }
来源：http://hz.sweek.top/gtjsehvymz.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zhongyouzk.top/gttvpagvxq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.meibo888.top/gtogvebtjj.html

C#:   interface IShape { double Area(); }
来源：http://hz.guannengcc.top/gtqhlnpsqi.html

[G10] 访问控制
来源：http://hz.cashguo.top/gtraadbkwg.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.andypj.xyz/gtymepvgoq.html

PHP:  public / protected / private
来源：http://hz.ppjwa.cn/gtinwizuko.html

JS:   #private 字段；其余公开
来源：http://hz.cucudq.cn/gtkcbafnsd.html

TS:   public / protected / private
来源：http://hz.jiagoushi.top/gtyopkfapa.html

Java: public / protected / private / 默认包级
来源：http://hz.shzxlz.cn/gtvmoobjki.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.fzhhl.top/gtztyldsta.html

Ruby: public / protected / private
来源：http://hz.daxiang520.top/gtcxqpnkko.html

C#:   public / protected / private / internal
来源：http://hz.daria6918.cn/gtuvntfghf.html

[G11] getter / setter
来源：http://hz.jianghu66.top/gtvoonyffr.html

Py:   @property 与 @x.setter
来源：http://hz.jinghuilouyu.cn/gtdyegoaiu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.hnxiangtu.top/gtzazsxpvr.html

JS:   get name() { return this._name; }
来源：http://hz.zdqjudy.top/gtrjjbgctx.html

TS:   get name(): string { return this._name; }
来源：http://hz.yuxming.cn/gtthjgvkhm.html

Java: public String getName() { return name; }
来源：http://hz.nanxuanxn.top/gtdroxptal.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.svipenyu.cn/gtrlvzvskz.html

Ruby: attr_accessor :name
来源：http://hz.svipenyu.cn/gthzcytdmx.html

C#:   public string Name { get; set; }
来源：http://hz.vqdsnc.cn/gtmldrndcb.html

[G12] 对象转字符串
来源：http://hz.hammf.cn/gtvwjnmebb.html

Py:   def __str__(self): return self.name
来源：http://hz.ehwqpu.com/gthjucuqhn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.birdmap.top/gtfozoeyfs.html

JS:   toString() { return this.name; }
来源：http://hz.yangfankeji.com/gtnvsojkzg.html

TS:   toString(): string { return this.name; }
来源：http://hz.cheryme.top/gtaqbbzabd.html

Java: @Override public String toString() { return name; }
来源：http://hz.mhx1999.top/gtvfxdazou.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.guowangkeji.top/gthuoquhxa.html

Ruby: def to_s; @name; end
来源：http://hz.ppjwa.cn/gtpumwclpu.html

C#:   public override string ToString() => Name;
来源：http://hz.pycfn.com/gtbadasbba.html

[G13] 判断对象类型
来源：http://hz.52xcode.cn/gtagbcxsdt.html

Py:   isinstance(u, User)
来源：http://hz.bjfxy.top/gthrafmcsj.html

PHP:  $u instanceof User
来源：http://hz.ydjk.org.cn/gtdhxfzwob.html

JS:   u instanceof User
来源：http://hz.svipenyu.cn/gtbjokgxfe.html

TS:   u instanceof User
来源：http://hz.zycfv.cn/gtwrmygrkj.html

Java: u instanceof User
来源：http://hz.shanyushiyangkeji.top/gtrnztuczi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.nanxinkj.top/gtyvqnnnwo.html

Ruby: u.is_a?(User)
来源：http://hz.redwolf501.top/gtaqjuaafn.html

C#:   u is User
来源：http://hz.zdqjudy.top/gtpwlaespn.html

[G14] 数据类 / record
来源：http://hz.yonumen.top/gtwqfrnixw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.nanxuanxn.top/gtcyqfpjcg.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.dianchejie.cn/gtqrwcuoed.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jinyuanbaomall.cn/gteaqidopc.html

TS:   type User = { name: string; age: number };
来源：http://hz.yj20258888.top/gtkpqlpold.html

Java: record User(String name, int age) {}
来源：http://hz.shanyushiyangkeji.top/gtpgsmsymx.html

Go:   type User struct { Name string; Age int }
来源：http://hz.chenjidiqi.icu/gtrqqtrnkb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zhiwuduotai.top/gtvzmgszot.html

C#:   record User(string Name, int Age);
来源：http://hz.yj202588.top/gtclgjafqa.html

[G15] 枚举
来源：http://hz.chenzaomai.com/gtwlydgegw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yueranfly.top/gtasgoirou.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.kuanghao11.cn/gtptjqxair.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zhiwuduotai.top/gtveibicdi.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.guowangkeji.top/gtnnyninlr.html

Java: enum Color { RED, GREEN }
来源：http://hz.jiagoushi.top/gtxlpalxzw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zhixingplan.top/gtzadasvvf.html

Ruby: Color = %i[red green].freeze
来源：http://hz.shanyushiyangtech.top/gtrfxtjhul.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.nanxinkj.top/gtjljynpkl.html

[G16] 对象转数组 / 字典
来源：http://hz.hywenlv.cn/gttrwklpuj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.hywenlv.cn/gtkucsouga.html

PHP:  get_object_vars($obj);
来源：http://hz.nanxinkj.top/gtouphulim.html

JS:   Object.entries(obj)
来源：http://hz.redwolf501.top/gtssavvexg.html

TS:   Object.entries(obj)
来源：http://hz.xziqi.cn/gtpkyqsgij.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.xuetiantiany.cn/gtyjlbiitc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.pycfn.com/gtjvgqqsrq.html

Ruby: obj.instance_variables
来源：http://hz.feifeiyinyue.top/gtsywdwhrc.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.aizwys.cn/gtlmcfppmq.html

================================================================================
来源：http://hz.yanxiufei.cn/gtzzgxeihi.html

H. 异常与错误处理
来源：http://hz.birdmap.top/gtrztxhnvk.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtjcfdwlil.html

[H01] try / catch 基础
来源：http://hz.c1oappe.top/gthmgxdrbx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yuanzhike.top/gtfpajeaoe.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ivvv.top/gtiywfqgkq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.tian-w.cn/gtkicjocul.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jinqigfzy.top/gtaqluklid.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ydjk.org.cn/gtovhkcpso.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.c1oappe.top/gtrxnvgzgf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.svipenyu.cn/gtxfsxchqe.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.pycfn.com/gtxpdpyegm.html

[H02] finally / ensure 收尾
来源：http://hz.dashuyun.cn/gtvxnlwkso.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.ybcxt.top/gtrbgmvwod.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.shuidangran.top/gttulpdxnt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.kuanghao11.cn/gtnzhtmpbe.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.chenjidiqi.icu/gtatmpejjd.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.daria6918.cn/gtlkwizhqo.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.0kj1m.cn/gtitostosb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jinqigufen.top/gtlmvxvifh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jyoumei.cn/gtiqgbgaty.html

[H03] 主动抛出异常
来源：http://hz.yueranfly.top/gtzrnfesbj.html

Py:   raise ValueError("错误信息")
来源：http://hz.jianghu66.top/gtltheuzfs.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.shzxlz.cn/gtuhjpdukd.html

JS:   throw new Error("错误信息");
来源：http://hz.52xcode.cn/gteoljmmht.html

TS:   throw new Error("错误信息");
来源：http://hz.yuxming.cn/gtqvrymeii.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.pycfn.com/gtiawvjvri.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.svipenyu.cn/gtqxvlbfif.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.mhx1999.top/gtwlowbseh.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.tianlin.xyz/gtatfwwvlu.html

[H04] 自定义异常类型
来源：http://hz.jinqigufen.top/gtudgaopzs.html

Py:   class MyError(Exception): pass
来源：http://hz.shzxlz.cn/gtploqqhhl.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.guannengcc.top/gtmxizgosv.html

JS:   class MyError extends Error {}
来源：http://hz.jinghuilouyu.cn/gtlgijhsur.html

TS:   class MyError extends Error {}
来源：http://hz.0kj1m.cn/gtnaoxtfrx.html

Java: class MyException extends RuntimeException {}
来源：http://hz.ydjk.org.cn/gtztpqbozb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yuanzhike.top/gtqxpicetr.html

Ruby: class MyError < StandardError; end
来源：http://hz.jyoumei.cn/gtdvhzfvjb.html

C#:   class MyException : Exception {}
来源：http://hz.jiagoushi.top/gtmsjfvgdd.html

[H05] 捕获特定类型
来源：http://hz.guannengcc.top/gthmgdwjah.html

Py:   except ValueError as e:
来源：http://hz.9152youxi.cn/gtcvfsgtit.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.hfpthk.cn/gtmbbrdlga.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.smart0.xyz/gtjklufrqa.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yueranfly.top/gtufwrxhzq.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.hysaishi.cn/gtvdwtdfqb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.fengsongda.top/gtxagifaaq.html

Ruby: rescue ArgumentError => e
来源：http://hz.birdmap.top/gtyplxydck.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.fzhhl.top/gtoclilrzk.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zhengqikj.top/gtvgwadlrs.html

Py:   value = d.get("k") or default
来源：http://hz.ivvv.top/gtvpgusxqu.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.guowangkeji.top/gthjthnibd.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.havefunace.top/gtljcaefar.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jiagoushi.top/gtsthxeavd.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.pengpengdd.cyou/gtapbfsgij.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.andypj.xyz/gtsztvvmes.html

Ruby: d&.dig(:a, :b)
来源：http://hz.shangyingyoupin.top/gtwgixiqvg.html

C#:   obj?.A?.B ?? default
来源：http://hz.yuxming.cn/gtzdbrjevl.html

[H07] 断言
来源：http://hz.dashuyun.cn/gtwdhvyqan.html

Py:   assert x > 0, "必须为正"
来源：http://hz.mhx1999.top/gtpwizgvio.html

PHP:  assert($x > 0);
来源：http://hz.xingfuxueyuan.xyz/gtljnzdavu.html

JS:   console.assert(x > 0);
来源：http://hz.cqqwz.cn/gtfsgxhbkc.html

TS:   console.assert(x > 0);
来源：http://hz.shuidangran.top/gtklhzmqxb.html

Java: assert x > 0 : "必须为正";
来源：http://hz.gogol.net.cn/gthgscpjkv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.pengpengdd.cyou/gtqidjpprq.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.quarkkingdee.top/gtvyghypid.html

C#:   Debug.Assert(x > 0);
来源：http://hz.316326.xyz/gtwsnzaxiz.html

[H08] 获取错误信息与堆栈
来源：http://hz.zycfv.cn/gteexyibdn.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jlsjyb.cn/gtncamglmn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.shuidangran.top/gtorpgdtuh.html

JS:   e.message;  e.stack
来源：http://hz.pycfn.com/gtbdpichbp.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hywenlv.cn/gttubhjwjl.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.fzhhl.top/gthygrohgs.html

Go:   err.Error()
来源：http://hz.yongpay.top/gtrpcoyvyp.html

Ruby: e.message;  e.backtrace
来源：http://hz.yueranfly.top/gtlqaxlqtl.html

C#:   e.Message;  e.StackTrace
来源：http://hz.cashguo.top/gtvgdzzckl.html

[H09] 带错误码的异常
来源：http://hz.xylfe.cn/gtlpakgsjc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.bjfxy.top/gtqdtvqnmd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jiagoushi.top/gtamegckfc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.wangshuangyany.cn/gtrnoiwapb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.nwbrower.top/gtjxhbftpj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.guannengcc.top/gtrakoutmh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ehwqpu.com/gtupwhgbph.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.ywan-chungtsiang.top/gtiedscezv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.bjfxy.top/gttpmlnkhm.html

[H10] 资源自动释放
来源：http://hz.sxryk.cn/gtzhttcknf.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.redwolf501.top/gtptfszipr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.hnxiangtu.top/gtrfuumafq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.dashuyun.cn/gttadfuxln.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.dianchejie.cn/gtpzlusqri.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.cheryme.top/gttchcscfz.html

Go:   defer f.Close()
来源：http://hz.ppjwa.cn/gtakjxnozu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.xziqi.cn/gtrwjrgpqh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.havefunace.top/gtlkjviaid.html


<!-- 参考信息 -->