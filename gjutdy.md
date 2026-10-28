代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.ydjk.org.cn/gtodgobygl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yuxming.cn/gtanjwvufo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.sufxvd.cn/gtvingjlvk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.chenzaomai.com/gttvbarczj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.pengpengdd.cyou/gtzzrddtmk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.cucudq.cn/gtgqyqsmnx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yj20258.top/gtchegltua.html

[F08] 遍历目录
来源：http://hz.ywan-chungtsiang.top/gtgbhdskgz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.hammf.cn/gttsjxmyrm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.9152youxi.cn/gtizymvxgk.html

JS:   fs.readdirSync("dir")
来源：http://hz.jinyuanbaomall.cn/gtcjqvycdq.html

TS:   fs.readdirSync("dir")
来源：http://hz.hammf.cn/gtsuieitxo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.sysykeji.top/gtedbtfpam.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.havefunace.top/gtqyxwmwpw.html

Ruby: Dir.children("dir")
来源：http://hz.gogol.net.cn/gtmekkjoms.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yuanzhike.top/gtdcpdstdw.html

[F09] 获取文件大小
来源：http://hz.wangdashe.top/gtqexfdsjg.html

Py:   os.path.getsize("a.txt")
来源：http://hz.cheryme.top/gtwjkthklh.html

PHP:  filesize("a.txt");
来源：http://hz.birdmap.top/gtfshxouoz.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yj20258888.top/gtowekseac.html

TS:   fs.statSync("a.txt").size
来源：http://hz.cdnleiting.top/gtsuktdvyg.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.ehwqpu.com/gticxvntyo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.ppjwa.cn/gtmvrlbnll.html

Ruby: File.size("a.txt")
来源：http://hz.guannengcc.top/gtvrsbviqs.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.svipenyu.cn/gtxwrdcyos.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.wangshuangyany.cn/gtqkgehfba.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.gogol.net.cn/gthqaygmfc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.fengsongda.top/gtffpjqctu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.xylfe.cn/gtypfipygu.html

TS:   path.extname("a.txt")
来源：http://hz.nanxinkj.top/gtlbbbhocn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.52xcode.cn/gtxtdogfoz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.tanke756.top/gtaxttvkvu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zdqjudy.top/gtxdrdcosf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.daxiang520.top/gtkjbehscr.html

[F11] 复制与移动文件
来源：http://hz.jqgfzy.top/gtkscxummb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zhongyouzk.top/gtawwrqvqx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.svipenyu.cn/gtgwjsjgsu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.wangdashe.top/gtjispzdsd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shzxlz.cn/gtzqhbcqjo.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.xuanzx.com/gtiunlsvgx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jyoumei.cn/gtaoabcvyx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yj202588.top/gtsirrjgrg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yuanzhike.top/gtzoguofzg.html

[F12] CSV 读写
来源：http://hz.nwbrower.top/gtluaisugu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jlsjyb.cn/gtnvkcqule.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.0kj1m.cn/gtrmwodxiv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.shzxlz.cn/gtcsqxgyag.html

TS:   // 同上
来源：http://hz.c1oappe.top/gtcmmayqpm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.guannengcc.top/gtcutoxycc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.xuanzx.com/gtnujewlwv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.sufxvd.cn/gtkkdadpqd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.redwolf501.top/gtbrtzuugh.html

================================================================================
来源：http://hz.ydjk.org.cn/gtphbzvbiy.html

G. 面向对象
来源：http://hz.shangyingyoupin.top/gtywekmzph.html

================================================================================
来源：http://hz.xylfe.cn/gtmbylswbw.html

[G01] 定义类
来源：http://hz.gaohongyu789.top/gtiwmlifac.html

Py:   class User: pass
来源：http://hz.jinqigfzy.top/gtimyfbrlp.html

PHP:  class User {}
来源：http://hz.c1oappe.top/gtodljzaxs.html

JS:   class User {}
来源：http://hz.sweek.top/gtlijyaujb.html

TS:   class User { name: string = ""; }
来源：http://hz.kuanghao11.cn/gttkhovhjj.html

Java: class User {}
来源：http://hz.cqqwz.cn/gtdustjvrx.html

Go:   type User struct { Name string }
来源：http://hz.hnxiangtu.top/gtktpfzpiw.html

Ruby: class User; end
来源：http://hz.nanxinkj.top/gtgqbssepa.html

C#:   class User {}
来源：http://hz.gaohongyu789.top/gtvwomiwvl.html

[G02] 构造函数
来源：http://hz.hongshengwenyu.top/gttzpdafps.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.cdnleiting.top/gtxieeqgpv.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.havefunace.top/gtgoxxieoc.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.shuidangran.top/gtrdnwigcj.html

TS:   constructor(public name: string) {}
来源：http://hz.andypj.xyz/gtesjudocc.html

Java: User(String name) { this.name = name; }
来源：http://hz.hysaishi.cn/gtgzgyakjo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jinyuanbaomall.cn/gtgzoedtfd.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jqgfzy.top/gtplkhjzpk.html

C#:   public User(string name) { Name = name; }
来源：http://hz.cdnleiting.top/gthjunrrvq.html

[G03] 实例属性
来源：http://hz.jqgfzy.top/gtspnwaaja.html

Py:   self.name = "x"
来源：http://hz.aizwys.cn/gtdxinyvek.html

PHP:  public string $name = "x";
来源：http://hz.tianlin.xyz/gtxtbmbphh.html

JS:   this.name = "x";
来源：http://hz.vqdsnc.cn/gtvuqhltol.html

TS:   name: string = "x";
来源：http://hz.ppjwa.cn/gtvfdjeuge.html

Java: private String name;
来源：http://hz.gaohongyu789.top/gtvrsujkso.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.feifeiyinyue.top/gtrlgghxbj.html

Ruby: @name = "x"
来源：http://hz.haohaochexian.top/gtsybibhie.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.nanxuanxn.top/gtwbxmtexc.html

[G04] 定义方法
来源：http://hz.xinyue.icu/gtrsmvvsal.html

Py:   def greet(self): return self.name
来源：http://hz.tianlin.xyz/gtaknqzbwy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.xylfe.cn/gtkyitsfrn.html

JS:   greet() { return this.name; }
来源：http://hz.cheryme.top/gteywtrkpp.html

TS:   greet(): string { return this.name; }
来源：http://hz.wangdashe.top/gtgbilswlp.html

Java: String greet() { return name; }
来源：http://hz.xuanzx.com/gtnmgunmuj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jlsjyb.cn/gtzqpdjhma.html

Ruby: def greet; @name; end
来源：http://hz.xylfe.cn/gtyustdowf.html

C#:   public string Greet() => Name;
来源：http://hz.jinyuanbaomall.cn/gtxlbqdqnj.html

[G05] 继承
来源：http://hz.yangfankeji.com/gtcrcpwrzd.html

Py:   class Admin(User): pass
来源：http://hz.jinghuilouyu.cn/gtcsbqozzw.html

PHP:  class Admin extends User {}
来源：http://hz.kuanghao11.cn/gtwrpgtoyo.html

JS:   class Admin extends User {}
来源：http://hz.9152youxi.cn/gtglumcmvr.html

TS:   class Admin extends User {}
来源：http://hz.quarkkingdee.top/gtomhzqewy.html

Java: class Admin extends User {}
来源：http://hz.feifeiyinyue.top/gtvwaezbam.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yonumen.top/gtunaqhswj.html

Ruby: class Admin < User; end
来源：http://hz.smart0.xyz/gteqgkuudm.html

C#:   class Admin : User {}
来源：http://hz.gogol.net.cn/gtbaslhxge.html

[G06] 重写方法
来源：http://hz.sufxvd.cn/gtjmpvtysr.html

Py:   def greet(self): return "admin"
来源：http://hz.chenzaomai.com/gtpijeeacj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.daria6918.cn/gtqsduhzhc.html

JS:   greet() { return "admin"; }
来源：http://hz.bjfxy.top/gteixgelbf.html

TS:   greet(): string { return "admin"; }
来源：http://hz.ydjk.org.cn/gtnfbfykns.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.birdmap.top/gtlggexkwv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhixingplan.top/gtydwklfli.html

Ruby: def greet; "admin"; end
来源：http://hz.andypj.xyz/gtppujdbre.html

C#:   public override string Greet() => "admin";
来源：http://hz.jinqigufen.top/gtokigvxvf.html

[G07] 调用父类方法
来源：http://hz.jqgufenzy.top/gtvjvkzlvl.html

Py:   super().greet()
来源：http://hz.cqqwz.cn/gthfhifeyd.html

PHP:  parent::greet();
来源：http://hz.shanyushiyangkeji.top/gtumyjafac.html

JS:   super.greet();
来源：http://hz.havefunace.top/gtunnhktlp.html

TS:   super.greet();
来源：http://hz.redwolf501.top/gtxdjhfyrv.html

Java: super.greet();
来源：http://hz.vqdsnc.cn/gtxxarelef.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.xuanzx.com/gtteoejykn.html

Ruby: super
来源：http://hz.shanyushiyangkeji.top/gthpborgto.html

C#:   base.Greet();
来源：http://hz.zhoulong.xyz/gtavywrcgs.html

[G08] 静态方法与属性
来源：http://hz.chenjidiqi.icu/gtjskywcbw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.dashuyun.cn/gtfixksfgl.html

PHP:  public static function f() {}
来源：http://hz.ppjwa.cn/gtkedgfrvp.html

JS:   static f() {}
来源：http://hz.dianchejie.cn/gtzvzqmxff.html

TS:   static f(): void {}
来源：http://hz.hfpthk.cn/gtyssjcaol.html

Java: static void f() {}
来源：http://hz.yj20258888.top/gtlxsjgfff.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.feifeiyinyue.top/gtkxuoqqda.html

Ruby: def self.f; end
来源：http://hz.pengpengdd.cyou/gtjmzdsuib.html

C#:   public static void F() {}
来源：http://hz.dashuyun.cn/gtavmusceb.html

[G09] 接口 / 抽象类
来源：http://hz.fzhhl.top/gtufpymply.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jlsjyb.cn/gtgdqphnsq.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.hnqzz.top/gtlyihueuz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.pycfn.com/gthocrmpqt.html

TS:   interface Shape { area(): number; }
来源：http://hz.ppjwa.cn/gtecygzpvh.html

Java: interface Shape { double area(); }
来源：http://hz.nanxuanxn.top/gtbkrngoem.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.chenjidiqi.icu/gtrxmzvhen.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhengqikj.top/gtrgyeasan.html

C#:   interface IShape { double Area(); }
来源：http://hz.iojbl.cn/gtvswpuzbk.html

[G10] 访问控制
来源：http://hz.vqdsnc.cn/gtohgoluqo.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yueranfly.top/gtinbbkbcz.html

PHP:  public / protected / private
来源：http://hz.xinyue.icu/gtsggkjrja.html

JS:   #private 字段；其余公开
来源：http://hz.feifeiyinyue.top/gtxyfcfaxj.html

TS:   public / protected / private
来源：http://hz.haohaochexian.top/gtcupgabdp.html

Java: public / protected / private / 默认包级
来源：http://hz.chenzaomai.com/gtxrfqwqex.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.fzhhl.top/gtbseuavwk.html

Ruby: public / protected / private
来源：http://hz.sxryk.cn/gtylwetzts.html

C#:   public / protected / private / internal
来源：http://hz.zhengqikj.top/gtavyltjrq.html

[G11] getter / setter
来源：http://hz.wangdashe.top/gthzxribmj.html

Py:   @property 与 @x.setter
来源：http://hz.guannengcc.top/gtowpwsqky.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.cucudq.cn/gtntolemfg.html

JS:   get name() { return this._name; }
来源：http://hz.xingfuxueyuan.xyz/gtbebsiwii.html

TS:   get name(): string { return this._name; }
来源：http://hz.xingfuxueyuan.xyz/gtcqjkcuyj.html

Java: public String getName() { return name; }
来源：http://hz.kuanghao11.cn/gthltvjmxb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.ydzc1.top/gtdcphfigh.html

Ruby: attr_accessor :name
来源：http://hz.daxiang520.top/gtztkchvhi.html

C#:   public string Name { get; set; }
来源：http://hz.c1oappe.top/gtoouriiap.html

[G12] 对象转字符串
来源：http://hz.fzhhl.top/gtvrrcerdq.html

Py:   def __str__(self): return self.name
来源：http://hz.quarkkingdee.top/gtrxbnocgl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yonumen.top/gtbmblfmsp.html

JS:   toString() { return this.name; }
来源：http://hz.shanyushiyangtech.top/gtcfyqgmlm.html

TS:   toString(): string { return this.name; }
来源：http://hz.gzhubu.top/gtkaibaxvz.html

Java: @Override public String toString() { return name; }
来源：http://hz.zdqjudy.top/gtblhplgga.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.tanke756.top/gtwhzyzqap.html

Ruby: def to_s; @name; end
来源：http://hz.sysykeji.top/gtidapekfb.html

C#:   public override string ToString() => Name;
来源：http://hz.haohaochexian.top/gtceyegyiu.html

[G13] 判断对象类型
来源：http://hz.jlsjyb.cn/gthogoytcx.html

Py:   isinstance(u, User)
来源：http://hz.ywan-chungtsiang.top/gttmcjityt.html

PHP:  $u instanceof User
来源：http://hz.shanyushiyangtech.top/gtylgxajti.html

JS:   u instanceof User
来源：http://hz.9152youxi.cn/gtqtaphaqk.html

TS:   u instanceof User
来源：http://hz.hongshengwenyu.top/gtabjndpkh.html

Java: u instanceof User
来源：http://hz.zhengqikj.top/gtmqzewlcr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.gotoacloud.top/gtexbgkdhk.html

Ruby: u.is_a?(User)
来源：http://hz.yj20258.top/gtyrmtfxbx.html

C#:   u is User
来源：http://hz.andypj.xyz/gtxwkcldfb.html

[G14] 数据类 / record
来源：http://hz.yvedp.cn/gtsngdkome.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.hnxiangtu.top/gtqjbjbfss.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zhongyouzk.top/gtxsdpgfch.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.gaohongyu789.top/gtluurgapy.html

TS:   type User = { name: string; age: number };
来源：http://hz.yanxiufei.cn/gtpuvqloni.html

Java: record User(String name, int age) {}
来源：http://hz.jlsjyb.cn/gtgzwdcemm.html

Go:   type User struct { Name string; Age int }
来源：http://hz.9152youxi.cn/gtpuejjpyb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.ppjwa.cn/gtxuerucrv.html

C#:   record User(string Name, int Age);
来源：http://hz.c1oappe.top/gtxwmxjpqp.html

[G15] 枚举
来源：http://hz.wangdashe.top/gtbqzwezmm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yj202588.top/gtpxkolxot.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.gogol.net.cn/gtbsnajueu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.ydjk.org.cn/gtjlqepyya.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.fengsongda.top/gtvcupvyxy.html

Java: enum Color { RED, GREEN }
来源：http://hz.yj20258888.top/gtxsdquqfc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jinyuanbaomall.cn/gtdqorpqmf.html

Ruby: Color = %i[red green].freeze
来源：http://hz.xinyue.icu/gtqeopezki.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xziqi.cn/gtftezrewf.html

[G16] 对象转数组 / 字典
来源：http://hz.daxiang520.top/gtwjnaunrc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.hnqzz.top/gttwwihltc.html

PHP:  get_object_vars($obj);
来源：http://hz.jinghuilouyu.cn/gttiggpplv.html

JS:   Object.entries(obj)
来源：http://hz.aibaodan.cn/gttuvjzwtv.html

TS:   Object.entries(obj)
来源：http://hz.zhaomingkeji.xyz/gtourhtjqx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.chenlongwang.top/gtztaesfkh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.cucudq.cn/gtjrpoobgo.html

Ruby: obj.instance_variables
来源：http://hz.sweek.top/gtfyfmklhb.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.fzhhl.top/gtgsgldbmo.html

================================================================================
来源：http://hz.mhx1999.top/gtoskynggx.html

H. 异常与错误处理
来源：http://hz.ehwqpu.com/gtckyamerb.html

================================================================================
来源：http://hz.hnxiangtu.top/gtjcmynvei.html

[H01] try / catch 基础
来源：http://hz.sysykeji.top/gtmoxrugqf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.guannengcc.top/gtqepawzwn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hywenlv.cn/gtntkdrctk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.0kj1m.cn/gtpboxfneq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zhengqikj.top/gttwoawzqc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jqgufenzy.top/gtkvhnpncf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.hfpthk.cn/gtajpcdjvj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.sufxvd.cn/gtdoxuiyhd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yj20258.top/gtlgjxtzzk.html

[H02] finally / ensure 收尾
来源：http://hz.snrcjt.cn/gtytfxswlf.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.cheryme.top/gtxbfyeizw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jqgfzy.top/gtqnpbvkgp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.daxiang520.top/gteeaypzra.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.xingfuxueyuan.xyz/gtqagvosqk.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.vqdsnc.cn/gtwsulwcsu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ppjwa.cn/gtwpbmfgmm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yueranfly.top/gtjupdaieq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.meibo888.top/gtciykjsmn.html

[H03] 主动抛出异常
来源：http://hz.hongshengwenyu.top/gtmqfuuehk.html

Py:   raise ValueError("错误信息")
来源：http://hz.hammf.cn/gtzlomyqik.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.pycfn.com/gtegeepksb.html

JS:   throw new Error("错误信息");
来源：http://hz.yvedp.cn/gtklpogdcr.html

TS:   throw new Error("错误信息");
来源：http://hz.tian-w.cn/gtdsthabrc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhaomingkeji.xyz/gtktemnyby.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhengqikj.top/gtfkoslocq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.tianlin.xyz/gtrudmrqzx.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.hfpthk.cn/gtxscnqono.html

[H04] 自定义异常类型
来源：http://hz.hnxiangtu.top/gtrgennmdw.html

Py:   class MyError(Exception): pass
来源：http://hz.zycfv.cn/gtqekboypp.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jinghuilouyu.cn/gtbbpdxrgq.html

JS:   class MyError extends Error {}
来源：http://hz.ydzc1.top/gtafmsbqxr.html

TS:   class MyError extends Error {}
来源：http://hz.ehwqpu.com/gtzwjhjgdr.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zhiwuduotai.top/gticejmjez.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.hnxiangtu.top/gtlnjzbzzf.html

Ruby: class MyError < StandardError; end
来源：http://hz.xylfe.cn/gtovnjmwwh.html

C#:   class MyException : Exception {}
来源：http://hz.pengpengdd.cyou/gtbijufkqv.html

[H05] 捕获特定类型
来源：http://hz.yj20258888.top/gtqnyddiln.html

Py:   except ValueError as e:
来源：http://hz.zhaomingkeji.xyz/gtcjyqhxql.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yongpay.top/gtjdluxkgx.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jqgufenzy.top/gtbcvncqox.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yanxiufei.cn/gtuigxvfic.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.bjfxy.top/gtwkhhrzip.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jinqigufen.top/gtuskzewej.html

Ruby: rescue ArgumentError => e
来源：http://hz.zdqjudy.top/gtvzpaymqm.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hnxiangtu.top/gtgvyiotnr.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zycfv.cn/gtfphjesbi.html

Py:   value = d.get("k") or default
来源：http://hz.hnqzz.top/gtmraffwni.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.haohaochexian.top/gtbjvcwadl.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yj202588.top/gtvkqmblhy.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jiagoushi.top/gtjpfqrllh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ywan-chungtsiang.top/gtseqkosnq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zhixingplan.top/gtvqwpxwyb.html

Ruby: d&.dig(:a, :b)
来源：http://hz.xziqi.cn/gtfqeyydyh.html

C#:   obj?.A?.B ?? default
来源：http://hz.tianlin.xyz/gtlbtybhde.html

[H07] 断言
来源：http://hz.gotoacloud.top/gtarsztzym.html

Py:   assert x > 0, "必须为正"
来源：http://hz.xziqi.cn/gtbdjpgiac.html

PHP:  assert($x > 0);
来源：http://hz.ywan-chungtsiang.top/gtbutiyuyt.html

JS:   console.assert(x > 0);
来源：http://hz.yueranfly.top/gtvxbupddd.html

TS:   console.assert(x > 0);
来源：http://hz.wangshuangyany.cn/gtiuzkvmpe.html

Java: assert x > 0 : "必须为正";
来源：http://hz.havefunace.top/gtyxmcfjhu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.bjfxy.top/gtxtufwnno.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.kuanghao11.cn/gtzpkdlzmu.html

C#:   Debug.Assert(x > 0);
来源：http://hz.smart0.xyz/gthtttriph.html

[H08] 获取错误信息与堆栈
来源：http://hz.cashguo.top/gthjxtjrsp.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jinghuilouyu.cn/gtjxmwslzb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.nanxinkj.top/gtcdkoicqn.html

JS:   e.message;  e.stack
来源：http://hz.guannengcc.top/gtuoryugly.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.cqqwz.cn/gtupjxwjlr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.wangdashe.top/gtcbecvmjj.html

Go:   err.Error()
来源：http://hz.yangfankeji.com/gtizusouzz.html

Ruby: e.message;  e.backtrace
来源：http://hz.9152youxi.cn/gtqhdjmlkm.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ybcxt.top/gteucvnfsl.html

[H09] 带错误码的异常
来源：http://hz.meibo888.top/gtpsfehsyf.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.tanke756.top/gteartbejy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.daxiang520.top/gtjeajopla.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.pengpengdd.cyou/gtuztafstw.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.fengsongda.top/gtqmbalanh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.hongshengwenyu.top/gtdqmiapbt.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ybcxt.top/gtjmtdbtmc.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.svipenyu.cn/gtudptsqmv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.tianlin.xyz/gtmytcxjqa.html

[H10] 资源自动释放
来源：http://hz.nwbrower.top/gtzruxxfke.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zdqjudy.top/gtkwqrruqs.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.cheryme.top/gtxinbyqrh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.tanke756.top/gtwydcorvn.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jqgfzy.top/gtznjgpata.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yanxiufei.cn/gtnmvsunfl.html

Go:   defer f.Close()
来源：http://hz.wangshuangyany.cn/gtxmamyrqb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yj20258.top/gtjcqtshjn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.redwolf501.top/gtciicojzf.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtroxejtjp.html

I. 正则表达式
来源：http://hz.jianghu66.top/gtntsivjcu.html

================================================================================
来源：http://hz.shzxlz.cn/gthlnuxkrs.html

[I01] 判断是否匹配
来源：http://hz.ppjwa.cn/gtaxcqlkxg.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhixingplan.top/gtarzxgeis.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.quarkkingdee.top/gtcgnkszwc.html

JS:   /\d+/.test(s)
来源：http://hz.chenlongwang.top/gtdgvnqxjx.html

TS:   /\d+/.test(s)
来源：http://hz.yangfankeji.com/gtyaxumikl.html


<!-- 参考信息 -->