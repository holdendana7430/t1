代发 wailian999

Ruby: File.delete("a.txt")
来源：http://hz.ydzc1.top/gtylgmxbus.html

C#:   File.Delete("a.txt");
来源：http://hz.zhijiandao.cn/gttcyziebi.html

[F07] 创建目录（含多级）
来源：http://hz.hnqzz.top/gtbcfpxgmg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.mhx1999.top/gtzmpxzarx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.nanxinkj.top/gtxlwsohmy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ppjwa.cn/gtqsmgickn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zdqjudy.top/gtdkkfesrd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.shangyingyoupin.top/gteybjalrj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.xziqi.cn/gtyqzeapmg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yuxming.cn/gtlfuapdyn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.nwbrower.top/gtpiysxbcx.html

[F08] 遍历目录
来源：http://hz.vqdsnc.cn/gtguzyfqed.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.jqgfzy.top/gtkbwsdtow.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.hongshengwenyu.top/gtyaflvkoh.html

JS:   fs.readdirSync("dir")
来源：http://hz.cheryme.top/gtaahlmavt.html

TS:   fs.readdirSync("dir")
来源：http://hz.iojbl.cn/gtzeftpaaf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.redwolf501.top/gtnoqckdao.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.c1oappe.top/gtagnjwusv.html

Ruby: Dir.children("dir")
来源：http://hz.xuetiantiany.cn/gtolrrjluq.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yuxming.cn/gtlslknlte.html

[F09] 获取文件大小
来源：http://hz.ehwqpu.com/gtcdrxppzm.html

Py:   os.path.getsize("a.txt")
来源：http://hz.9152youxi.cn/gtztsbdofq.html

PHP:  filesize("a.txt");
来源：http://hz.hongshengwenyu.top/gtnhhksboi.html

JS:   fs.statSync("a.txt").size
来源：http://hz.fengsongda.top/gtacvprfai.html

TS:   fs.statSync("a.txt").size
来源：http://hz.daria6918.cn/gtdnncfrcj.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.aizwys.cn/gtsqphartp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jyoumei.cn/gtbjtlakry.html

Ruby: File.size("a.txt")
来源：http://hz.daxiang520.top/gtuhzvigoj.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jinghuilouyu.cn/gtdbpgaquy.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yangfankeji.com/gtdtsyaipt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yvedp.cn/gtllaqyjpj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.cucudq.cn/gttqixddnh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.ppjwa.cn/gtahxgfhxn.html

TS:   path.extname("a.txt")
来源：http://hz.nanxinkj.top/gtuzqcvnfi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.haohaochexian.top/gthodbiuws.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.ivvv.top/gtgiwcdspy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.ppjwa.cn/gtlsxlnybt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.shanyushiyangtech.top/gtylypzgsl.html

[F11] 复制与移动文件
来源：http://hz.ydjk.org.cn/gtpwitvlvu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.dianchejie.cn/gtkmdgcukd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.dashuyun.cn/gtohxwhhmc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sufxvd.cn/gtxssxhmtn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shanyushiyangkeji.top/gtavbguvui.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jqgufenzy.top/gtzqraqpzi.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.pengpengdd.cyou/gtsfhghdbr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.316326.xyz/gtmzexklks.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhoulong.xyz/gtpelgtmpg.html

[F12] CSV 读写
来源：http://hz.cqqwz.cn/gtelsmnyef.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yanxiufei.cn/gtzdiahmpu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zdqjudy.top/gtmrjmgbmd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.havefunace.top/gtqjvjsahb.html

TS:   // 同上
来源：http://hz.zhongyouzk.top/gtsqrsgjwk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.sxryk.cn/gtnapanocc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.xinyue.icu/gtktqrwpkb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.shuidangran.top/gtidypolru.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.ivvv.top/gtqjtxetun.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtnwqpwzpm.html

G. 面向对象
来源：http://hz.chenzaomai.com/gtncqkzivi.html

================================================================================
来源：http://hz.zycfv.cn/gtnirvbyhz.html

[G01] 定义类
来源：http://hz.hnxiangtu.top/gtfflfmlaf.html

Py:   class User: pass
来源：http://hz.zhaomingkeji.xyz/gtsnnaveap.html

PHP:  class User {}
来源：http://hz.yj202588.top/gtvyrbhvvd.html

JS:   class User {}
来源：http://hz.dashuyun.cn/gtrxahkgww.html

TS:   class User { name: string = ""; }
来源：http://hz.cheryme.top/gtskdfwrbv.html

Java: class User {}
来源：http://hz.xuanzx.com/gtgzeqvgoa.html

Go:   type User struct { Name string }
来源：http://hz.guannengcc.top/gtsiunbqxg.html

Ruby: class User; end
来源：http://hz.hywenlv.cn/gtpacdlupb.html

C#:   class User {}
来源：http://hz.jinghuilouyu.cn/gtzsmpwfyt.html

[G02] 构造函数
来源：http://hz.nanxuanxn.top/gtdmrzvask.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.iojbl.cn/gtrxwuqupr.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ydzc1.top/gtcugmbltv.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.daria6918.cn/gtwrsoskmr.html

TS:   constructor(public name: string) {}
来源：http://hz.kuanghao11.cn/gtmmcqtuda.html

Java: User(String name) { this.name = name; }
来源：http://hz.fengsongda.top/gtquhrsdar.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.meibo888.top/gtfbwcsgpa.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.xinyue.icu/gtquocugph.html

C#:   public User(string name) { Name = name; }
来源：http://hz.xuanzx.com/gtqvodqclv.html

[G03] 实例属性
来源：http://hz.ppjwa.cn/gtmfhjyvmq.html

Py:   self.name = "x"
来源：http://hz.hammf.cn/gttlikbrqj.html

PHP:  public string $name = "x";
来源：http://hz.hnqzz.top/gtmiexmunj.html

JS:   this.name = "x";
来源：http://hz.pengpengdd.cyou/gtiuuqrxod.html

TS:   name: string = "x";
来源：http://hz.zdqjudy.top/gtggatmbls.html

Java: private String name;
来源：http://hz.wangshuangyany.cn/gtsaesqemy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.0kj1m.cn/gtdrajebda.html

Ruby: @name = "x"
来源：http://hz.shangyingyoupin.top/gteuzlhhca.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zhijiandao.cn/gtcimvbhuu.html

[G04] 定义方法
来源：http://hz.vqdsnc.cn/gtxrxelemn.html

Py:   def greet(self): return self.name
来源：http://hz.havefunace.top/gtbmjretfq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.shanyushiyangtech.top/gtjpgplgse.html

JS:   greet() { return this.name; }
来源：http://hz.nwbrower.top/gtxzscrkxx.html

TS:   greet(): string { return this.name; }
来源：http://hz.hongshengwenyu.top/gtfxtpjvwe.html

Java: String greet() { return name; }
来源：http://hz.fzhhl.top/gtvlllmmcq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.gaohongyu789.top/gtabwestcz.html

Ruby: def greet; @name; end
来源：http://hz.ivvv.top/gtpaqurvbl.html

C#:   public string Greet() => Name;
来源：http://hz.zhixingplan.top/gtssazaycc.html

[G05] 继承
来源：http://hz.sweek.top/gtavgdsslj.html

Py:   class Admin(User): pass
来源：http://hz.redwolf501.top/gtvlwljvzz.html

PHP:  class Admin extends User {}
来源：http://hz.wangshuangyany.cn/gtiszhvcto.html

JS:   class Admin extends User {}
来源：http://hz.xylfe.cn/gtbqpskawx.html

TS:   class Admin extends User {}
来源：http://hz.aizwys.cn/gtqpdbkxyv.html

Java: class Admin extends User {}
来源：http://hz.cqqwz.cn/gtiykoygtq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.wangshuangyany.cn/gtylpwxmzf.html

Ruby: class Admin < User; end
来源：http://hz.chenzaomai.com/gtykgrfsxx.html

C#:   class Admin : User {}
来源：http://hz.zhaomingkeji.xyz/gtsfvcsmrd.html

[G06] 重写方法
来源：http://hz.zhixingplan.top/gtdhijiatf.html

Py:   def greet(self): return "admin"
来源：http://hz.shanyushiyangkeji.top/gtwldobpgl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yongpay.top/gtvqdumjig.html

JS:   greet() { return "admin"; }
来源：http://hz.hongshengwenyu.top/gtqlyritbt.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zycfv.cn/gtufmgpnro.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ivvv.top/gtmdeoebzg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.andypj.xyz/gtoxfhhfqf.html

Ruby: def greet; "admin"; end
来源：http://hz.shzxlz.cn/gtoxsuhkzs.html

C#:   public override string Greet() => "admin";
来源：http://hz.hnxiangtu.top/gtanwyaocl.html

[G07] 调用父类方法
来源：http://hz.feifeiyinyue.top/gtbltdtpgq.html

Py:   super().greet()
来源：http://hz.ydjk.org.cn/gtrcjxitch.html

PHP:  parent::greet();
来源：http://hz.snrcjt.cn/gtxiomsnqs.html

JS:   super.greet();
来源：http://hz.cucudq.cn/gtugtqvscp.html

TS:   super.greet();
来源：http://hz.tanke756.top/gtiedunypo.html

Java: super.greet();
来源：http://hz.ydzc1.top/gtszdxbftt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.xinyue.icu/gtohgswubd.html

Ruby: super
来源：http://hz.wangshuangyany.cn/gtduztmyoz.html

C#:   base.Greet();
来源：http://hz.sweek.top/gtccmwbfnb.html

[G08] 静态方法与属性
来源：http://hz.nwbrower.top/gtxftmqyxy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.nanxuanxn.top/gtnxkmtgac.html

PHP:  public static function f() {}
来源：http://hz.guowangkeji.top/gtltaplsby.html

JS:   static f() {}
来源：http://hz.9152youxi.cn/gtfjahgaay.html

TS:   static f(): void {}
来源：http://hz.vqdsnc.cn/gtizrgosmo.html

Java: static void f() {}
来源：http://hz.nanxinkj.top/gtxpongayo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.haohaochexian.top/gtablnmmwi.html

Ruby: def self.f; end
来源：http://hz.jyoumei.cn/gtslvhkmuj.html

C#:   public static void F() {}
来源：http://hz.meibo888.top/gtqvllrqiz.html

[G09] 接口 / 抽象类
来源：http://hz.birdmap.top/gtdbqlswdb.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.daria6918.cn/gtrkvmbpob.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.hfpthk.cn/gtuejlozir.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.chenzaomai.com/gtnrnjuhtm.html

TS:   interface Shape { area(): number; }
来源：http://hz.9152youxi.cn/gthhcqgslu.html

Java: interface Shape { double area(); }
来源：http://hz.dashuyun.cn/gtslghxgfi.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.aibaodan.cn/gtqdijvpsn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.0kj1m.cn/gtwkzacfbf.html

C#:   interface IShape { double Area(); }
来源：http://hz.hnxiangtu.top/gtoclbtytc.html

[G10] 访问控制
来源：http://hz.meibo888.top/gtgupqsvqq.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.shangyingyoupin.top/gtkgimfevc.html

PHP:  public / protected / private
来源：http://hz.cheryme.top/gtppdvsdqv.html

JS:   #private 字段；其余公开
来源：http://hz.smart0.xyz/gtczzhykly.html

TS:   public / protected / private
来源：http://hz.hysaishi.cn/gtilmrgxtu.html

Java: public / protected / private / 默认包级
来源：http://hz.quarkkingdee.top/gtyaotolbm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhoulong.xyz/gtzxpwfbiw.html

Ruby: public / protected / private
来源：http://hz.ehwqpu.com/gtmwhyxhsc.html

C#:   public / protected / private / internal
来源：http://hz.hnqzz.top/gtdgyqwaqb.html

[G11] getter / setter
来源：http://hz.zhoulong.xyz/gtzfbzotms.html

Py:   @property 与 @x.setter
来源：http://hz.pycfn.com/gtedtelvab.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.ppjwa.cn/gtxzqnrtbz.html

JS:   get name() { return this._name; }
来源：http://hz.jinghuilouyu.cn/gtpgicojth.html

TS:   get name(): string { return this._name; }
来源：http://hz.yj202588.top/gtlhdschwj.html

Java: public String getName() { return name; }
来源：http://hz.mhx1999.top/gtxvvoxftf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yj20258.top/gtsswsvnfk.html

Ruby: attr_accessor :name
来源：http://hz.zhengqikj.top/gtlbcbueho.html

C#:   public string Name { get; set; }
来源：http://hz.dashuyun.cn/gtnyzmmmkz.html

[G12] 对象转字符串
来源：http://hz.shanyushiyangkeji.top/gtkfhqsows.html

Py:   def __str__(self): return self.name
来源：http://hz.chenjidiqi.icu/gtbybykxjb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.nanxuanxn.top/gtfuwjtkjd.html

JS:   toString() { return this.name; }
来源：http://hz.fzhhl.top/gtiglgkspg.html

TS:   toString(): string { return this.name; }
来源：http://hz.smart0.xyz/gtewmvuvcv.html

Java: @Override public String toString() { return name; }
来源：http://hz.jinqigfzy.top/gtfrfurouc.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zdqjudy.top/gthqnjpwsk.html

Ruby: def to_s; @name; end
来源：http://hz.yueranfly.top/gtkxbrcufj.html

C#:   public override string ToString() => Name;
来源：http://hz.mhx1999.top/gtqokbavsx.html

[G13] 判断对象类型
来源：http://hz.shanyushiyangkeji.top/gtbturiilj.html

Py:   isinstance(u, User)
来源：http://hz.redwolf501.top/gthucjkocq.html

PHP:  $u instanceof User
来源：http://hz.sufxvd.cn/gtbzxzjbmc.html

JS:   u instanceof User
来源：http://hz.chenzaomai.com/gtvqijuepv.html

TS:   u instanceof User
来源：http://hz.yj20258888.top/gtlbnraham.html

Java: u instanceof User
来源：http://hz.snrcjt.cn/gtppotcpwb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yangfankeji.com/gtlosyihpb.html

Ruby: u.is_a?(User)
来源：http://hz.cucudq.cn/gtjvdodrpl.html

C#:   u is User
来源：http://hz.mhx1999.top/gtxxnqvvbc.html

[G14] 数据类 / record
来源：http://hz.meibo888.top/gtgbvikidy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.cdnleiting.top/gtgzmpeivl.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.feifeiyinyue.top/gtbijcbhyv.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.daxiang520.top/gtmustgxit.html

TS:   type User = { name: string; age: number };
来源：http://hz.chenjidiqi.icu/gtrganspxp.html

Java: record User(String name, int age) {}
来源：http://hz.c1oappe.top/gtrnzpdaok.html

Go:   type User struct { Name string; Age int }
来源：http://hz.hnqzz.top/gtnpyiyqyx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.pengpengdd.cyou/gtpwjnmwvy.html

C#:   record User(string Name, int Age);
来源：http://hz.wangshuangyany.cn/gtnmppbakj.html

[G15] 枚举
来源：http://hz.hnqzz.top/gtqpaxoldb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.pycfn.com/gtivuzrcwg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.chenjidiqi.icu/gterbeethi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.birdmap.top/gtvhfrvpnn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.gotoacloud.top/gtzpzyihxq.html

Java: enum Color { RED, GREEN }
来源：http://hz.zycfv.cn/gtqzedkmuo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.nanxinkj.top/gtnqkazbcz.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ydjk.org.cn/gtfjzhckue.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jinghuilouyu.cn/gtqlhuwgje.html

[G16] 对象转数组 / 字典
来源：http://hz.yongpay.top/gtbnyyacas.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jiagoushi.top/gtttuximjl.html

PHP:  get_object_vars($obj);
来源：http://hz.zhoulong.xyz/gtfkbfqxsu.html

JS:   Object.entries(obj)
来源：http://hz.vqdsnc.cn/gtbafxoibw.html

TS:   Object.entries(obj)
来源：http://hz.bjfxy.top/gttsjxttrl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hongshengwenyu.top/gtbrrrwgvj.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.guannengcc.top/gtoaoujyqf.html

Ruby: obj.instance_variables
来源：http://hz.jlsjyb.cn/gtjvkurylg.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.shanyushiyangtech.top/gtrkurirxs.html

================================================================================
来源：http://hz.shuidangran.top/gtxsadrbfs.html

H. 异常与错误处理
来源：http://hz.c1oappe.top/gtdxyojcos.html

================================================================================
来源：http://hz.hammf.cn/gtuluoqedj.html

[H01] try / catch 基础
来源：http://hz.fzhhl.top/gtujopilmi.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.xuanzx.com/gtwknoxkjm.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zhaomingkeji.xyz/gtodkpsluh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.haohaochexian.top/gterqiaqll.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.xziqi.cn/gtrprkmaoh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.kuanghao11.cn/gtteovwlty.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.ehwqpu.com/gthpsqlppb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.zhaomingkeji.xyz/gtmxslbkng.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.nwbrower.top/gtauumdptn.html

[H02] finally / ensure 收尾
来源：http://hz.yj202588.top/gtaeydmcpo.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jinqigufen.top/gtccwxywdd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.dianchejie.cn/gtupwaxymc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.meibo888.top/gtuxoqydur.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.sweek.top/gtxzsalqtr.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhengqikj.top/gtrmxrhmlq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ivvv.top/gtyafnsmnj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yangfankeji.com/gtgzbbnoud.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zdqjudy.top/gtcjlnhkst.html

[H03] 主动抛出异常
来源：http://hz.jyoumei.cn/gturgbjcfs.html

Py:   raise ValueError("错误信息")
来源：http://hz.ppjwa.cn/gttjjfksch.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jiagoushi.top/gtiscvnpyn.html

JS:   throw new Error("错误信息");
来源：http://hz.sysykeji.top/gtujhbakuv.html

TS:   throw new Error("错误信息");
来源：http://hz.pycfn.com/gtdqxjqgdm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.fengsongda.top/gtnojrxoog.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.iojbl.cn/gtquwqlnho.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ppjwa.cn/gtvtarwksp.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.gzhubu.top/gtmhlnbrsa.html

[H04] 自定义异常类型
来源：http://hz.yanxiufei.cn/gtlebdusno.html

Py:   class MyError(Exception): pass
来源：http://hz.dashuyun.cn/gtzwdlulgj.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.vqdsnc.cn/gtfczvytyo.html

JS:   class MyError extends Error {}
来源：http://hz.0kj1m.cn/gtruabxbgp.html

TS:   class MyError extends Error {}
来源：http://hz.chenlongwang.top/gtaxrvdrpt.html

Java: class MyException extends RuntimeException {}
来源：http://hz.mhx1999.top/gtvwcuggqp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ivvv.top/gtmismsgwt.html

Ruby: class MyError < StandardError; end
来源：http://hz.jyoumei.cn/gtxnuvdwvc.html

C#:   class MyException : Exception {}
来源：http://hz.bjfxy.top/gtzevgavuy.html

[H05] 捕获特定类型
来源：http://hz.52xcode.cn/gtcjrzqsqh.html

Py:   except ValueError as e:
来源：http://hz.hongshengwenyu.top/gtnobuhrqv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.aizwys.cn/gtcegjtvok.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.pengpengdd.cyou/gtdaycrign.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.shzxlz.cn/gtkprlgyrk.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.shuidangran.top/gtkzghtxnd.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.mhx1999.top/gtbkkqydwj.html

Ruby: rescue ArgumentError => e
来源：http://hz.chenlongwang.top/gtkrvratbr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhongyouzk.top/gthfpfdsdo.html

[H06] 可选值 / 空值安全访问
来源：http://hz.shzxlz.cn/gtljzsqqvp.html

Py:   value = d.get("k") or default
来源：http://hz.c1oappe.top/gtakhgvbic.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.quarkkingdee.top/gthaajvaie.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.gaohongyu789.top/gtclllgbcg.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.kuanghao11.cn/gtbkqkpskz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.316326.xyz/gtjzclhrdt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.xziqi.cn/gtjormbfnq.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jinghuilouyu.cn/gtpggimkiy.html

C#:   obj?.A?.B ?? default
来源：http://hz.chenlongwang.top/gthqflyyob.html

[H07] 断言
来源：http://hz.fzhhl.top/gtmroiptul.html

Py:   assert x > 0, "必须为正"
来源：http://hz.ywan-chungtsiang.top/gtjdqzrvwp.html

PHP:  assert($x > 0);
来源：http://hz.pengpengdd.cyou/gthwpbotqr.html

JS:   console.assert(x > 0);
来源：http://hz.xylfe.cn/gtqmgdofbq.html

TS:   console.assert(x > 0);
来源：http://hz.cdnleiting.top/gtoheudgyl.html

Java: assert x > 0 : "必须为正";
来源：http://hz.nanxuanxn.top/gtjrofflgm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.shanyushiyangtech.top/gttazacqsv.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.havefunace.top/gtzpncvqbb.html

C#:   Debug.Assert(x > 0);
来源：http://hz.chenzaomai.com/gtxmxbzcvl.html

[H08] 获取错误信息与堆栈
来源：http://hz.guannengcc.top/gtxgkowpjh.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.dashuyun.cn/gtlhlezhjd.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jqgufenzy.top/gtsfpxpply.html

JS:   e.message;  e.stack
来源：http://hz.ehwqpu.com/gtpsgoijlw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.ydzc1.top/gtkkdvrkqy.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zdqjudy.top/gttzspucpy.html

Go:   err.Error()
来源：http://hz.yongpay.top/gtlgqvlnat.html

Ruby: e.message;  e.backtrace
来源：http://hz.feifeiyinyue.top/gtyebaonhy.html

C#:   e.Message;  e.StackTrace
来源：http://hz.kuanghao11.cn/gtjbbxzodj.html

[H09] 带错误码的异常
来源：http://hz.shanyushiyangkeji.top/gtgffflukr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.xziqi.cn/gtforawmqf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.guannengcc.top/gtqxflailu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.ivvv.top/gtxkonqoif.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.guannengcc.top/gtdcamiogs.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yj20258888.top/gtibocqgbe.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.smart0.xyz/gtmboypxsy.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.xuanzx.com/gtdocelmku.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.sxryk.cn/gttxshaxni.html

[H10] 资源自动释放
来源：http://hz.birdmap.top/gtldeggvjb.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.ehwqpu.com/gthiqilvcu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.andypj.xyz/gtuikprfsj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.bjfxy.top/gtgakohwcu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sufxvd.cn/gtzjmejnwn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.hnxiangtu.top/gtkborpbsa.html

Go:   defer f.Close()
来源：http://hz.xinyue.icu/gtbzbyrljz.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jinyuanbaomall.cn/gtxobupuay.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.hnxiangtu.top/gtfksxxmjy.html

================================================================================
来源：http://hz.havefunace.top/gtquvwskjk.html

I. 正则表达式
来源：http://hz.chenlongwang.top/gtjipahpuf.html

================================================================================
来源：http://hz.zhixingplan.top/gtqafyhobr.html

[I01] 判断是否匹配
来源：http://hz.tianlin.xyz/gtnzbvqgtt.html


<!-- 参考信息 -->