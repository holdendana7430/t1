代发 wailian999

Ruby: File.delete("a.txt")
来源：http://hz.xuetiantiany.cn/gtikhcplby.html

C#:   File.Delete("a.txt");
来源：http://hz.xylfe.cn/gtjyzarwtj.html

[F07] 创建目录（含多级）
来源：http://hz.hnqzz.top/gtgqxgazhs.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jinyuanbaomall.cn/gttkeiwcso.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.mhx1999.top/gtijrfkhpz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.nanxuanxn.top/gtrsdyycbp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xylfe.cn/gtjshiapnd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jinghuilouyu.cn/gtybdlobbo.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yvedp.cn/gtdfkmvfik.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.havefunace.top/gtxnoubxsn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.cheryme.top/gtlfrvngqb.html

[F08] 遍历目录
来源：http://hz.yj202588.top/gtqnhbdpen.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.0kj1m.cn/gtwxstrpsv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.hnxiangtu.top/gtwclzbzcl.html

JS:   fs.readdirSync("dir")
来源：http://hz.zhengqikj.top/gtdmzxjioh.html

TS:   fs.readdirSync("dir")
来源：http://hz.yuanzhike.top/gtodjgavxy.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.feifeiyinyue.top/gtvcuvxavv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yj20258.top/gtayrogbob.html

Ruby: Dir.children("dir")
来源：http://hz.fzhhl.top/gttcpkyrcf.html

C#:   Directory.GetFiles("dir")
来源：http://hz.dianchejie.cn/gtmiypsjua.html

[F09] 获取文件大小
来源：http://hz.zhiwuduotai.top/gtmshputcy.html

Py:   os.path.getsize("a.txt")
来源：http://hz.aizwys.cn/gtldixxcbe.html

PHP:  filesize("a.txt");
来源：http://hz.fzhhl.top/gtompxlhjt.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jiagoushi.top/gthycosuck.html

TS:   fs.statSync("a.txt").size
来源：http://hz.haohaochexian.top/gtjelaaapc.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.ehwqpu.com/gtrecnrhem.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.ehwqpu.com/gteuvydxez.html

Ruby: File.size("a.txt")
来源：http://hz.pycfn.com/gtiannxgko.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jlsjyb.cn/gtowobgteb.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.gogol.net.cn/gtemolsocc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.dianchejie.cn/gtbjqryswu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.svipenyu.cn/gtybvleiwn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.chenzaomai.com/gtjojslwyp.html

TS:   path.extname("a.txt")
来源：http://hz.chenlongwang.top/gtuxgjomju.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.hywenlv.cn/gtpehckomx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.shangyingyoupin.top/gtqqsqjcbj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jqgufenzy.top/gtslsazcoi.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.nanxinkj.top/gtztcdovmo.html

[F11] 复制与移动文件
来源：http://hz.shanyushiyangtech.top/gtimcguddl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yj20258.top/gtflnmwdpy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.bjfxy.top/gtqpclacvd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yj20258888.top/gtaatgmotm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.meibo888.top/gtevxvjisa.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.xinyue.icu/gthbmygbca.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.xuanzx.com/gtlwqsiein.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.nanxuanxn.top/gtagpmxiod.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yangfankeji.com/gtscbrjdax.html

[F12] CSV 读写
来源：http://hz.ppjwa.cn/gtvlmuldae.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.daxiang520.top/gteggnqvsp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yvedp.cn/gtjjfwpmcs.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jinghuilouyu.cn/gtkipdwwyu.html

TS:   // 同上
来源：http://hz.jqgufenzy.top/gtebckmilk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ywan-chungtsiang.top/gtfgjfschq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.iojbl.cn/gtevajalhp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.hfpthk.cn/gtcotcflet.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.sufxvd.cn/gtwlpsbamv.html

================================================================================
来源：http://hz.iojbl.cn/gtdvhmkmwv.html

G. 面向对象
来源：http://hz.ydzc1.top/gtagfbzgyo.html

================================================================================
来源：http://hz.fzhhl.top/gtdlsddwhz.html

[G01] 定义类
来源：http://hz.hongshengwenyu.top/gtdqqwvpwl.html

Py:   class User: pass
来源：http://hz.xingfuxueyuan.xyz/gtjvyfqbeo.html

PHP:  class User {}
来源：http://hz.nwbrower.top/gtvbebalve.html

JS:   class User {}
来源：http://hz.vqdsnc.cn/gtcawszuhc.html

TS:   class User { name: string = ""; }
来源：http://hz.zhixingplan.top/gtjkzpxoob.html

Java: class User {}
来源：http://hz.zhiwuduotai.top/gtvuyyyuag.html

Go:   type User struct { Name string }
来源：http://hz.daria6918.cn/gtkyhlqhel.html

Ruby: class User; end
来源：http://hz.hywenlv.cn/gtaqyybknf.html

C#:   class User {}
来源：http://hz.vqdsnc.cn/gtloynvmso.html

[G02] 构造函数
来源：http://hz.hnxiangtu.top/gtfuvvivkk.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zycfv.cn/gtpsfpqzrk.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.feifeiyinyue.top/gtvmjifiju.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.hongshengwenyu.top/gtwbltkaxj.html

TS:   constructor(public name: string) {}
来源：http://hz.havefunace.top/gtwfihooiz.html

Java: User(String name) { this.name = name; }
来源：http://hz.cashguo.top/gtelfwvmtf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.iojbl.cn/gtwqgbpgki.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.ehwqpu.com/gtlzuctkij.html

C#:   public User(string name) { Name = name; }
来源：http://hz.hongshengwenyu.top/gtjdvpduux.html

[G03] 实例属性
来源：http://hz.zhiwuduotai.top/gtzaceypda.html

Py:   self.name = "x"
来源：http://hz.wangdashe.top/gtxezygrfv.html

PHP:  public string $name = "x";
来源：http://hz.cashguo.top/gtlxpyagvo.html

JS:   this.name = "x";
来源：http://hz.iojbl.cn/gttfvcwmjt.html

TS:   name: string = "x";
来源：http://hz.zhixingplan.top/gtczbkxfou.html

Java: private String name;
来源：http://hz.wangdashe.top/gtdrbtiqsj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.sweek.top/gtjmqkdofr.html

Ruby: @name = "x"
来源：http://hz.yuxming.cn/gtphlardta.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.sxryk.cn/gtpgjvdizm.html

[G04] 定义方法
来源：http://hz.ppjwa.cn/gtuyytrsya.html

Py:   def greet(self): return self.name
来源：http://hz.hnxiangtu.top/gtavngkxhk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.tanke756.top/gtdxjhahhc.html

JS:   greet() { return this.name; }
来源：http://hz.sxryk.cn/gtgsxgiuts.html

TS:   greet(): string { return this.name; }
来源：http://hz.gotoacloud.top/gtaxqopaxx.html

Java: String greet() { return name; }
来源：http://hz.sweek.top/gtmhhtqnjs.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.chenzaomai.com/gtlgomzgpx.html

Ruby: def greet; @name; end
来源：http://hz.nanxuanxn.top/gtnwmlecbe.html

C#:   public string Greet() => Name;
来源：http://hz.aizwys.cn/gtoherxrhp.html

[G05] 继承
来源：http://hz.jyoumei.cn/gtunlbhcbg.html

Py:   class Admin(User): pass
来源：http://hz.ywan-chungtsiang.top/gtuyudztwv.html

PHP:  class Admin extends User {}
来源：http://hz.hysaishi.cn/gtscygdhnc.html

JS:   class Admin extends User {}
来源：http://hz.shangyingyoupin.top/gtkjfkylkj.html

TS:   class Admin extends User {}
来源：http://hz.redwolf501.top/gtfasmowee.html

Java: class Admin extends User {}
来源：http://hz.ivvv.top/gtdkqvhwgm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.shuidangran.top/gtmepqugme.html

Ruby: class Admin < User; end
来源：http://hz.pengpengdd.cyou/gtxwdwaurg.html

C#:   class Admin : User {}
来源：http://hz.daria6918.cn/gtjheqdxsj.html

[G06] 重写方法
来源：http://hz.aizwys.cn/gtpsfwjcmr.html

Py:   def greet(self): return "admin"
来源：http://hz.nwbrower.top/gtntehtjgo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zhoulong.xyz/gtdagebcwn.html

JS:   greet() { return "admin"; }
来源：http://hz.jqgfzy.top/gtwvswkvyb.html

TS:   greet(): string { return "admin"; }
来源：http://hz.aibaodan.cn/gtsjdbfglg.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.daxiang520.top/gtgqhrepev.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.xingfuxueyuan.xyz/gtrhypdegz.html

Ruby: def greet; "admin"; end
来源：http://hz.wangdashe.top/gtrassezau.html

C#:   public override string Greet() => "admin";
来源：http://hz.jqgfzy.top/gtliyfbacf.html

[G07] 调用父类方法
来源：http://hz.shangyingyoupin.top/gtrasjblgl.html

Py:   super().greet()
来源：http://hz.ivvv.top/gtdcqmcnwd.html

PHP:  parent::greet();
来源：http://hz.fengsongda.top/gtxgjdnatk.html

JS:   super.greet();
来源：http://hz.haohaochexian.top/gtmmfgzrpz.html

TS:   super.greet();
来源：http://hz.hywenlv.cn/gtdfgmlftc.html

Java: super.greet();
来源：http://hz.yanxiufei.cn/gtuphrcflc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.sxryk.cn/gtyfkztjqc.html

Ruby: super
来源：http://hz.shuidangran.top/gtfdjvgutv.html

C#:   base.Greet();
来源：http://hz.shzxlz.cn/gtftollmzm.html

[G08] 静态方法与属性
来源：http://hz.hammf.cn/gtwrbilerg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.gotoacloud.top/gtdhkxujnp.html

PHP:  public static function f() {}
来源：http://hz.shanyushiyangtech.top/gtqckbvhbd.html

JS:   static f() {}
来源：http://hz.jinghuilouyu.cn/gtfuordxzw.html

TS:   static f(): void {}
来源：http://hz.gaohongyu789.top/gtkcqrgjma.html

Java: static void f() {}
来源：http://hz.svipenyu.cn/gtkqwgzizs.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yuxming.cn/gtpvxdbvhg.html

Ruby: def self.f; end
来源：http://hz.cheryme.top/gtoquuxduv.html

C#:   public static void F() {}
来源：http://hz.bjfxy.top/gthmgaruug.html

[G09] 接口 / 抽象类
来源：http://hz.guowangkeji.top/gtllblvnfw.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yuxming.cn/gtoibkkgnv.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.pycfn.com/gtfkexllbe.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.gotoacloud.top/gtcsnbfjxy.html

TS:   interface Shape { area(): number; }
来源：http://hz.52xcode.cn/gtikciuquk.html

Java: interface Shape { double area(); }
来源：http://hz.daxiang520.top/gtporxbwqb.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.shzxlz.cn/gtkwndpjmm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.redwolf501.top/gtocgnetcx.html

C#:   interface IShape { double Area(); }
来源：http://hz.hysaishi.cn/gtfdqcrddm.html

[G10] 访问控制
来源：http://hz.aizwys.cn/gtprcbosje.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhongyouzk.top/gtmqptdujf.html

PHP:  public / protected / private
来源：http://hz.pycfn.com/gthfmmbgwg.html

JS:   #private 字段；其余公开
来源：http://hz.jianghu66.top/gtlfkeqnrt.html

TS:   public / protected / private
来源：http://hz.0kj1m.cn/gtxqhfzxdw.html

Java: public / protected / private / 默认包级
来源：http://hz.jianghu66.top/gtwaqqzrdm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ehwqpu.com/gtfiprmaqy.html

Ruby: public / protected / private
来源：http://hz.jyoumei.cn/gtcplbetxd.html

C#:   public / protected / private / internal
来源：http://hz.yj202588.top/gtyvadabgk.html

[G11] getter / setter
来源：http://hz.yvedp.cn/gtckhklfvy.html

Py:   @property 与 @x.setter
来源：http://hz.guowangkeji.top/gtblywdvwb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.gzhubu.top/gtdmmlasaf.html

JS:   get name() { return this._name; }
来源：http://hz.hammf.cn/gtsjxdtegt.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhoulong.xyz/gtkncsbhua.html

Java: public String getName() { return name; }
来源：http://hz.tianlin.xyz/gtjgdjamel.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.mhx1999.top/gtjlgzqfam.html

Ruby: attr_accessor :name
来源：http://hz.9152youxi.cn/gtjvtrttuy.html

C#:   public string Name { get; set; }
来源：http://hz.xziqi.cn/gtueialnjk.html

[G12] 对象转字符串
来源：http://hz.xingfuxueyuan.xyz/gtpugjocbc.html

Py:   def __str__(self): return self.name
来源：http://hz.zhixingplan.top/gttvjtesro.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jyoumei.cn/gthbgbxzvw.html

JS:   toString() { return this.name; }
来源：http://hz.ppjwa.cn/gtgyetegqs.html

TS:   toString(): string { return this.name; }
来源：http://hz.hfpthk.cn/gtwlzsaujs.html

Java: @Override public String toString() { return name; }
来源：http://hz.jiagoushi.top/gtpqujflmo.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.aizwys.cn/gttkxwtfyd.html

Ruby: def to_s; @name; end
来源：http://hz.zhongyouzk.top/gtvapiywyu.html

C#:   public override string ToString() => Name;
来源：http://hz.fzhhl.top/gtttmxwhvr.html

[G13] 判断对象类型
来源：http://hz.aizwys.cn/gtjuqainnk.html

Py:   isinstance(u, User)
来源：http://hz.zdqjudy.top/gtmevynlxa.html

PHP:  $u instanceof User
来源：http://hz.wangshuangyany.cn/gtcnsjspiy.html

JS:   u instanceof User
来源：http://hz.meibo888.top/gtggbogwnv.html

TS:   u instanceof User
来源：http://hz.yuxming.cn/gtojaxrygn.html

Java: u instanceof User
来源：http://hz.tian-w.cn/gttqtayxyr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.guowangkeji.top/gtsttmyhsg.html

Ruby: u.is_a?(User)
来源：http://hz.cqqwz.cn/gtonuvctll.html

C#:   u is User
来源：http://hz.zhongyouzk.top/gtppgzsqcy.html

[G14] 数据类 / record
来源：http://hz.svipenyu.cn/gthtlfuwod.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jinqigufen.top/gtkhwxbwmq.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.fengsongda.top/gtwgbshgua.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.tanke756.top/gtqyfaipqd.html

TS:   type User = { name: string; age: number };
来源：http://hz.yvedp.cn/gtwylyygpd.html

Java: record User(String name, int age) {}
来源：http://hz.xinyue.icu/gtccpkgjqw.html

Go:   type User struct { Name string; Age int }
来源：http://hz.chenjidiqi.icu/gtgiyxzlqv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zhoulong.xyz/gtobslmcth.html

C#:   record User(string Name, int Age);
来源：http://hz.nwbrower.top/gtgycohbno.html

[G15] 枚举
来源：http://hz.iojbl.cn/gtfxzkqdky.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.xingfuxueyuan.xyz/gtvwbgxuwn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ywan-chungtsiang.top/gtqyxivclv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.guowangkeji.top/gtzbtcwlfb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xinyue.icu/gtdfuxfwxl.html

Java: enum Color { RED, GREEN }
来源：http://hz.cheryme.top/gtolwffekl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.dashuyun.cn/gtwvjmovib.html

Ruby: Color = %i[red green].freeze
来源：http://hz.52xcode.cn/gtzvkpoerl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhiwuduotai.top/gteonmvhgl.html

[G16] 对象转数组 / 字典
来源：http://hz.zycfv.cn/gtjzxmysia.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.ehwqpu.com/gtduzijtls.html

PHP:  get_object_vars($obj);
来源：http://hz.yonumen.top/gtnylneryv.html

JS:   Object.entries(obj)
来源：http://hz.haohaochexian.top/gtyildgqjw.html

TS:   Object.entries(obj)
来源：http://hz.jinqigufen.top/gtthsaijof.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.316326.xyz/gtbptniumj.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.sxryk.cn/gthgetaatn.html

Ruby: obj.instance_variables
来源：http://hz.xziqi.cn/gtgctcrxoa.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.hongshengwenyu.top/gtcebzlgsc.html

================================================================================
来源：http://hz.hnqzz.top/gtdwdnypkc.html

H. 异常与错误处理
来源：http://hz.gotoacloud.top/gtoapgrbnh.html

================================================================================
来源：http://hz.tian-w.cn/gtpnesgkmi.html

[H01] try / catch 基础
来源：http://hz.jinqigfzy.top/gtxujzavlg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.dashuyun.cn/gtqowavwrx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ehwqpu.com/gtctpbrnbh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yongpay.top/gtbxhdvfxf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.gogol.net.cn/gtguiappob.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.daxiang520.top/gtiwbygmur.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.316326.xyz/gtnsqztvat.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jinghuilouyu.cn/gtclanwqqn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yuxming.cn/gtmettdgyr.html

[H02] finally / ensure 收尾
来源：http://hz.kuanghao11.cn/gtfflafduq.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.dianchejie.cn/gthiwfjyvx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.sweek.top/gtzqjnegwp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.ydzc1.top/gtfgqlddog.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.svipenyu.cn/gtekqbzflc.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhiwuduotai.top/gtbanqmhhz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.smart0.xyz/gtisgtwihq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.0kj1m.cn/gtsaktpmdp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.cucudq.cn/gtuxeiuxxo.html

[H03] 主动抛出异常
来源：http://hz.ehwqpu.com/gtvdubovwz.html

Py:   raise ValueError("错误信息")
来源：http://hz.chenjidiqi.icu/gtrxplbxav.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jyoumei.cn/gtfqodakkn.html

JS:   throw new Error("错误信息");
来源：http://hz.ppjwa.cn/gtpcnbqvjt.html

TS:   throw new Error("错误信息");
来源：http://hz.yuxming.cn/gtwmsznexx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.tianlin.xyz/gtfpweirct.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.ivvv.top/gtzkiiyqnj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.pycfn.com/gtiisqnxhi.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.hongshengwenyu.top/gtlquwikyb.html

[H04] 自定义异常类型
来源：http://hz.ywan-chungtsiang.top/gttogvyqua.html

Py:   class MyError(Exception): pass
来源：http://hz.ivvv.top/gtgnuosniv.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.52xcode.cn/gtjgigocrp.html

JS:   class MyError extends Error {}
来源：http://hz.wangdashe.top/gtjvmjnbmk.html

TS:   class MyError extends Error {}
来源：http://hz.xylfe.cn/gtfnumgpzl.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zhaomingkeji.xyz/gtazlijvfn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.sufxvd.cn/gtmmxwawkq.html

Ruby: class MyError < StandardError; end
来源：http://hz.yj20258888.top/gtwgizdpmy.html

C#:   class MyException : Exception {}
来源：http://hz.tanke756.top/gtktepwayj.html

[H05] 捕获特定类型
来源：http://hz.shzxlz.cn/gtsmrzkrwl.html

Py:   except ValueError as e:
来源：http://hz.hongshengwenyu.top/gtvoplkgtx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.ivvv.top/gtpboenslm.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.andypj.xyz/gtjonzebgr.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yj20258.top/gthlcbreec.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.cdnleiting.top/gtnkmbnyou.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.nanxuanxn.top/gttjcgyaut.html

Ruby: rescue ArgumentError => e
来源：http://hz.hywenlv.cn/gtwzoxkhec.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.birdmap.top/gtyjfmbkxr.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jianghu66.top/gtzuplbkez.html

Py:   value = d.get("k") or default
来源：http://hz.9152youxi.cn/gtunbfnzhg.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hnxiangtu.top/gtcjbrtkfg.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.hysaishi.cn/gtqwnvylqe.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.ivvv.top/gtidwflrqg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.chenzaomai.com/gtrpfovmcp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.sufxvd.cn/gtcnmktmpq.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhiwuduotai.top/gtzfgqftla.html

C#:   obj?.A?.B ?? default
来源：http://hz.0kj1m.cn/gtlwytmrga.html

[H07] 断言
来源：http://hz.kuanghao11.cn/gtkujprwfg.html

Py:   assert x > 0, "必须为正"
来源：http://hz.hammf.cn/gtkqqbpuqj.html

PHP:  assert($x > 0);
来源：http://hz.jlsjyb.cn/gtloxszbfd.html

JS:   console.assert(x > 0);
来源：http://hz.feifeiyinyue.top/gtqmfcahje.html

TS:   console.assert(x > 0);
来源：http://hz.zhiwuduotai.top/gtvmaveduu.html

Java: assert x > 0 : "必须为正";
来源：http://hz.dashuyun.cn/gtfpzytagx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.xuanzx.com/gtliyaeqta.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.feifeiyinyue.top/gtpuukxotv.html

C#:   Debug.Assert(x > 0);
来源：http://hz.cucudq.cn/gtvvgjqirf.html

[H08] 获取错误信息与堆栈
来源：http://hz.jqgfzy.top/gtkvvzxhcp.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yuanzhike.top/gtoxszzryp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.xuanzx.com/gtonpxgwht.html

JS:   e.message;  e.stack
来源：http://hz.ppjwa.cn/gteqdiykgf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.ehwqpu.com/gtullnexas.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yuanzhike.top/gtvntedktu.html

Go:   err.Error()
来源：http://hz.fengsongda.top/gthglpjyfm.html

Ruby: e.message;  e.backtrace
来源：http://hz.daria6918.cn/gtuinvgavo.html

C#:   e.Message;  e.StackTrace
来源：http://hz.chenjidiqi.icu/gtokxeoues.html

[H09] 带错误码的异常
来源：http://hz.shanyushiyangkeji.top/gtyqmaxjyh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hnxiangtu.top/gtqnvybjwf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yonumen.top/gtplmqrseu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.ehwqpu.com/gtgkjrumld.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jinyuanbaomall.cn/gtezzfukjc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.xuetiantiany.cn/gtxlwxwabu.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.xuanzx.com/gtzszayglf.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.feifeiyinyue.top/gtjyzsqeia.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhaomingkeji.xyz/gtbovskksp.html

[H10] 资源自动释放
来源：http://hz.tian-w.cn/gtqpjrskcu.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.nanxinkj.top/gtqzewsgoe.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.c1oappe.top/gtftobrmas.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.tian-w.cn/gtkrlffnci.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xziqi.cn/gtskwjdtyw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.xziqi.cn/gtgtvfelxd.html

Go:   defer f.Close()
来源：http://hz.52xcode.cn/gtnfosfnwo.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.ybcxt.top/gtcdwoggbh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jqgufenzy.top/gtvbephyea.html

================================================================================
来源：http://hz.meibo888.top/gtcelivmgc.html

I. 正则表达式
来源：http://hz.yj20258.top/gtimrmgvhr.html

================================================================================
来源：http://hz.ydzc1.top/gtnpwrkokq.html

[I01] 判断是否匹配
来源：http://hz.zhiwuduotai.top/gtuqauotae.html


<!-- 参考信息 -->