代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.feifeiyinyue.top/gtfqjjiksa.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.birdmap.top/gtdxejppvs.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yanxiufei.cn/gtxewxkqut.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.dashuyun.cn/gtgystlmzl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zycfv.cn/gtgqfjjldc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.fengsongda.top/gtftrduoex.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.tian-w.cn/gtmfdolavi.html

[F08] 遍历目录
来源：http://hz.wangshuangyany.cn/gtklzyzczn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.9152youxi.cn/gtdroszeeo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yj202588.top/gtnlsxjqzd.html

JS:   fs.readdirSync("dir")
来源：http://hz.iojbl.cn/gtrlvorixz.html

TS:   fs.readdirSync("dir")
来源：http://hz.shanyushiyangtech.top/gtkfvoockm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zhiwuduotai.top/gtofdfotfc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.vqdsnc.cn/gtwyzbcdgb.html

Ruby: Dir.children("dir")
来源：http://hz.zhijiandao.cn/gtvhatdjcz.html

C#:   Directory.GetFiles("dir")
来源：http://hz.xingfuxueyuan.xyz/gtpobdlxrq.html

[F09] 获取文件大小
来源：http://hz.xylfe.cn/gteuqvlnnz.html

Py:   os.path.getsize("a.txt")
来源：http://hz.feifeiyinyue.top/gtpssvpmgn.html

PHP:  filesize("a.txt");
来源：http://hz.gogol.net.cn/gtpuznvmlq.html

JS:   fs.statSync("a.txt").size
来源：http://hz.tianlin.xyz/gtrtemafob.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jinyuanbaomall.cn/gtunnvlrwn.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.fzhhl.top/gtgmukznbw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zhengqikj.top/gthxcqjwgm.html

Ruby: File.size("a.txt")
来源：http://hz.jqgfzy.top/gtoxzmfqap.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.xuetiantiany.cn/gtugtsxuyv.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zhongyouzk.top/gtvdkgdlmx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jlsjyb.cn/gtbrcaxlni.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.cashguo.top/gtarphblel.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.wangdashe.top/gtjtcscjrq.html

TS:   path.extname("a.txt")
来源：http://hz.hongshengwenyu.top/gtpuenhylo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yj20258888.top/gtiidxxnfz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zhijiandao.cn/gttcqcvirp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.feifeiyinyue.top/gthxkrqddp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.wangdashe.top/gtqktwtjlq.html

[F11] 复制与移动文件
来源：http://hz.yangfankeji.com/gtdmtaiong.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.quarkkingdee.top/gtrormuyak.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.andypj.xyz/gtmzqttatf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sweek.top/gtupuvjfrg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.dashuyun.cn/gtinforavj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.9152youxi.cn/gtbbakbsyw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.zdqjudy.top/gtyylnpmdy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.tianlin.xyz/gtwzcmamjt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.feifeiyinyue.top/gtpsmipbcf.html

[F12] CSV 读写
来源：http://hz.jqgfzy.top/gtpmeipmdm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.guannengcc.top/gtuzuwrmed.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.0kj1m.cn/gtigikjzwg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jianghu66.top/gtcimvryfi.html

TS:   // 同上
来源：http://hz.xinyue.icu/gtugvxibet.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yueranfly.top/gtkdibqpnq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.hywenlv.cn/gtprduqktt.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yj202588.top/gtwdaogtly.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.guowangkeji.top/gtooumyuri.html

================================================================================
来源：http://hz.jianghu66.top/gtvrpegggr.html

G. 面向对象
来源：http://hz.jyoumei.cn/gtkkpztqit.html

================================================================================
来源：http://hz.yonumen.top/gtyxbystfm.html

[G01] 定义类
来源：http://hz.jianghu66.top/gthmybknqz.html

Py:   class User: pass
来源：http://hz.snrcjt.cn/gtdebkfohy.html

PHP:  class User {}
来源：http://hz.feifeiyinyue.top/gtcfvxzbde.html

JS:   class User {}
来源：http://hz.jinqigfzy.top/gtmlnmdsey.html

TS:   class User { name: string = ""; }
来源：http://hz.0kj1m.cn/gtfspeydac.html

Java: class User {}
来源：http://hz.jqgfzy.top/gturygjxtb.html

Go:   type User struct { Name string }
来源：http://hz.fengsongda.top/gtedrnvslv.html

Ruby: class User; end
来源：http://hz.yj202588.top/gtlhehfpym.html

C#:   class User {}
来源：http://hz.jinqigfzy.top/gtrtqhtiwf.html

[G02] 构造函数
来源：http://hz.ywan-chungtsiang.top/gtnntuwxmv.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yj20258.top/gtedufkkfm.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hysaishi.cn/gtnxbdlcgf.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhengqikj.top/gtqelunkbv.html

TS:   constructor(public name: string) {}
来源：http://hz.guannengcc.top/gtigtzggob.html

Java: User(String name) { this.name = name; }
来源：http://hz.chenjidiqi.icu/gtozidvcnw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.xuetiantiany.cn/gttziabscs.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.sysykeji.top/gtyxqdcezl.html

C#:   public User(string name) { Name = name; }
来源：http://hz.cheryme.top/gtzpecsvxe.html

[G03] 实例属性
来源：http://hz.daxiang520.top/gtzacmevcp.html

Py:   self.name = "x"
来源：http://hz.mhx1999.top/gtxddkktqc.html

PHP:  public string $name = "x";
来源：http://hz.bjfxy.top/gtutxivurk.html

JS:   this.name = "x";
来源：http://hz.aibaodan.cn/gtdbnhvbzq.html

TS:   name: string = "x";
来源：http://hz.yj20258888.top/gtfiqngctt.html

Java: private String name;
来源：http://hz.zycfv.cn/gtxuszdxtd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.fengsongda.top/gtqegiahji.html

Ruby: @name = "x"
来源：http://hz.zhijiandao.cn/gtztjmpson.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.sweek.top/gtuyfgrref.html

[G04] 定义方法
来源：http://hz.xuetiantiany.cn/gtizgcvkch.html

Py:   def greet(self): return self.name
来源：http://hz.birdmap.top/gtvmltjpwt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.gogol.net.cn/gtgpekauza.html

JS:   greet() { return this.name; }
来源：http://hz.ppjwa.cn/gtdwmzswuy.html

TS:   greet(): string { return this.name; }
来源：http://hz.guannengcc.top/gtohzrgakh.html

Java: String greet() { return name; }
来源：http://hz.ivvv.top/gtciocjunq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ivvv.top/gtficvwxsw.html

Ruby: def greet; @name; end
来源：http://hz.pycfn.com/gtkginhkmg.html

C#:   public string Greet() => Name;
来源：http://hz.hfpthk.cn/gtijifmbdy.html

[G05] 继承
来源：http://hz.gzhubu.top/gtvbkobynh.html

Py:   class Admin(User): pass
来源：http://hz.zhiwuduotai.top/gtnojpdwdq.html

PHP:  class Admin extends User {}
来源：http://hz.xinyue.icu/gtzthllnsy.html

JS:   class Admin extends User {}
来源：http://hz.smart0.xyz/gtlrksatry.html

TS:   class Admin extends User {}
来源：http://hz.chenjidiqi.icu/gtwvxbxcfy.html

Java: class Admin extends User {}
来源：http://hz.chenzaomai.com/gtammdenqs.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hnxiangtu.top/gtbvotitnn.html

Ruby: class Admin < User; end
来源：http://hz.xingfuxueyuan.xyz/gtoorswkqr.html

C#:   class Admin : User {}
来源：http://hz.xinyue.icu/gtyzckwaqh.html

[G06] 重写方法
来源：http://hz.gzhubu.top/gtdplxgmcm.html

Py:   def greet(self): return "admin"
来源：http://hz.haohaochexian.top/gtxpupfnva.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.cheryme.top/gtgmaceeyx.html

JS:   greet() { return "admin"; }
来源：http://hz.ppjwa.cn/gtbgtodzej.html

TS:   greet(): string { return "admin"; }
来源：http://hz.bjfxy.top/gtlxqlixxn.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.pengpengdd.cyou/gtuadmgukt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.nanxinkj.top/gtlvwkworf.html

Ruby: def greet; "admin"; end
来源：http://hz.yj20258.top/gtraikwemy.html

C#:   public override string Greet() => "admin";
来源：http://hz.hammf.cn/gtewbrzsiz.html

[G07] 调用父类方法
来源：http://hz.redwolf501.top/gtdhbgjlxy.html

Py:   super().greet()
来源：http://hz.xziqi.cn/gtpnhqoctd.html

PHP:  parent::greet();
来源：http://hz.hysaishi.cn/gtflcwqlvw.html

JS:   super.greet();
来源：http://hz.sufxvd.cn/gtbkfpgcun.html

TS:   super.greet();
来源：http://hz.gaohongyu789.top/gtkyapgpri.html

Java: super.greet();
来源：http://hz.fzhhl.top/gtgkxltdkg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.wangdashe.top/gtxwgvlotg.html

Ruby: super
来源：http://hz.redwolf501.top/gtpwigqgla.html

C#:   base.Greet();
来源：http://hz.pengpengdd.cyou/gtuqozpnhk.html

[G08] 静态方法与属性
来源：http://hz.daria6918.cn/gtqaoseiin.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.sufxvd.cn/gtnppowowr.html

PHP:  public static function f() {}
来源：http://hz.yuanzhike.top/gtwrmkloxk.html

JS:   static f() {}
来源：http://hz.hfpthk.cn/gtoyyauixt.html

TS:   static f(): void {}
来源：http://hz.jianghu66.top/gtqlasisov.html

Java: static void f() {}
来源：http://hz.zhengqikj.top/gtkpmobiwq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yanxiufei.cn/gtnximdvch.html

Ruby: def self.f; end
来源：http://hz.tianlin.xyz/gtfnphwjid.html

C#:   public static void F() {}
来源：http://hz.aizwys.cn/gtnretevcr.html

[G09] 接口 / 抽象类
来源：http://hz.feifeiyinyue.top/gtweypofwg.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jinghuilouyu.cn/gtrkkihsqk.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yanxiufei.cn/gtdskzefek.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jinghuilouyu.cn/gtionparcl.html

TS:   interface Shape { area(): number; }
来源：http://hz.dashuyun.cn/gtqgzasmiu.html

Java: interface Shape { double area(); }
来源：http://hz.snrcjt.cn/gtvfeadnrp.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.shzxlz.cn/gtzjeizwey.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.smart0.xyz/gtssuswoah.html

C#:   interface IShape { double Area(); }
来源：http://hz.yueranfly.top/gtemwmnkyh.html

[G10] 访问控制
来源：http://hz.yj20258888.top/gtsuaswuzb.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.xuetiantiany.cn/gtgetcsmoj.html

PHP:  public / protected / private
来源：http://hz.aizwys.cn/gtotmxwafu.html

JS:   #private 字段；其余公开
来源：http://hz.hammf.cn/gtbdevnipz.html

TS:   public / protected / private
来源：http://hz.wangdashe.top/gtifzdhwms.html

Java: public / protected / private / 默认包级
来源：http://hz.chenlongwang.top/gtrjyvdbyk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.iojbl.cn/gtwainpuij.html

Ruby: public / protected / private
来源：http://hz.jqgufenzy.top/gthntzntrv.html

C#:   public / protected / private / internal
来源：http://hz.shangyingyoupin.top/gtluwhgqzl.html

[G11] getter / setter
来源：http://hz.zhaomingkeji.xyz/gtctgtmtqi.html

Py:   @property 与 @x.setter
来源：http://hz.zhengqikj.top/gtbcgnqosb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.c1oappe.top/gtuwswkrpk.html

JS:   get name() { return this._name; }
来源：http://hz.sxryk.cn/gtcuswxitm.html

TS:   get name(): string { return this._name; }
来源：http://hz.yj20258.top/gtlwwpvskp.html

Java: public String getName() { return name; }
来源：http://hz.ybcxt.top/gtcdqnareh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.guannengcc.top/gtcudmeols.html

Ruby: attr_accessor :name
来源：http://hz.c1oappe.top/gtgiegyqeh.html

C#:   public string Name { get; set; }
来源：http://hz.52xcode.cn/gtftwmctnw.html

[G12] 对象转字符串
来源：http://hz.zycfv.cn/gtcrbtkdte.html

Py:   def __str__(self): return self.name
来源：http://hz.zhiwuduotai.top/gtgeppxwoj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.xziqi.cn/gtlmajsptr.html

JS:   toString() { return this.name; }
来源：http://hz.daria6918.cn/gtvgkgogdg.html

TS:   toString(): string { return this.name; }
来源：http://hz.daria6918.cn/gtfydrlohm.html

Java: @Override public String toString() { return name; }
来源：http://hz.shzxlz.cn/gtdduftuvp.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.nanxinkj.top/gtsupvdlrd.html

Ruby: def to_s; @name; end
来源：http://hz.cheryme.top/gtmfahfwls.html

C#:   public override string ToString() => Name;
来源：http://hz.haohaochexian.top/gtplgimclv.html

[G13] 判断对象类型
来源：http://hz.tianlin.xyz/gtcuydodhu.html

Py:   isinstance(u, User)
来源：http://hz.shangyingyoupin.top/gtzwzseoop.html

PHP:  $u instanceof User
来源：http://hz.ivvv.top/gtlqpbsxdq.html

JS:   u instanceof User
来源：http://hz.cdnleiting.top/gtmxbiirzx.html

TS:   u instanceof User
来源：http://hz.andypj.xyz/gtdofrghwy.html

Java: u instanceof User
来源：http://hz.jinqigfzy.top/gtmvjqkwvt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yangfankeji.com/gtolljucaw.html

Ruby: u.is_a?(User)
来源：http://hz.wangdashe.top/gtvztvseme.html

C#:   u is User
来源：http://hz.zdqjudy.top/gtopyovdpt.html

[G14] 数据类 / record
来源：http://hz.gzhubu.top/gtdapkfilc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.ywan-chungtsiang.top/gtimqcuswj.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.fengsongda.top/gtjajzrvbc.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.ivvv.top/gtidejwtho.html

TS:   type User = { name: string; age: number };
来源：http://hz.shuidangran.top/gtbnpwxyrb.html

Java: record User(String name, int age) {}
来源：http://hz.316326.xyz/gtdxrzdxzg.html

Go:   type User struct { Name string; Age int }
来源：http://hz.guannengcc.top/gtzaguzdto.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zhengqikj.top/gtadhudqmz.html

C#:   record User(string Name, int Age);
来源：http://hz.yvedp.cn/gtjzukvxlb.html

[G15] 枚举
来源：http://hz.shuidangran.top/gtibdfuviy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zhoulong.xyz/gtuvbgeumr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yj202588.top/gtigjnbcwb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yuanzhike.top/gtbdnomrur.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.tanke756.top/gtowjaogry.html

Java: enum Color { RED, GREEN }
来源：http://hz.9152youxi.cn/gtmqndbfvk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zhengqikj.top/gtvsefubks.html

Ruby: Color = %i[red green].freeze
来源：http://hz.feifeiyinyue.top/gtvkczqdho.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.316326.xyz/gtfojzqbxa.html

[G16] 对象转数组 / 字典
来源：http://hz.xinyue.icu/gtmkvxbufk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.andypj.xyz/gtytikpous.html

PHP:  get_object_vars($obj);
来源：http://hz.smart0.xyz/gtztlpocfp.html

JS:   Object.entries(obj)
来源：http://hz.jiagoushi.top/gthunetunv.html

TS:   Object.entries(obj)
来源：http://hz.kuanghao11.cn/gtwuvexgle.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.fzhhl.top/gtqrqfyvms.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.sysykeji.top/gtyiqevzsw.html

Ruby: obj.instance_variables
来源：http://hz.dashuyun.cn/gtfamcsvxn.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.hywenlv.cn/gtshbftidq.html

================================================================================
来源：http://hz.haohaochexian.top/gtgkgyhmqh.html

H. 异常与错误处理
来源：http://hz.xuetiantiany.cn/gtodkgxgfw.html

================================================================================
来源：http://hz.9152youxi.cn/gtfadbafot.html

[H01] try / catch 基础
来源：http://hz.andypj.xyz/gtqrxborjh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jinqigufen.top/gtvtkuzkof.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hammf.cn/gtgteygavl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.birdmap.top/gtliutvpuj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hfpthk.cn/gttkjssqvb.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.shanyushiyangkeji.top/gthxqhrlfz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.shanyushiyangtech.top/gtejaevhle.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.xylfe.cn/gtngufwbry.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.tianlin.xyz/gtlpjyyoyp.html

[H02] finally / ensure 收尾
来源：http://hz.ybcxt.top/gtdguiymra.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.gzhubu.top/gtrieownvy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yanxiufei.cn/gtoxhnqdly.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.shangyingyoupin.top/gtbjxmwgve.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.xinyue.icu/gtqwrtzcnj.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.nanxuanxn.top/gtsrnwhmhu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hammf.cn/gtifbxddwu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jyoumei.cn/gteazghpww.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.redwolf501.top/gtbdttqies.html

[H03] 主动抛出异常
来源：http://hz.haohaochexian.top/gtqwwupecz.html

Py:   raise ValueError("错误信息")
来源：http://hz.dashuyun.cn/gthvkrhimp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.guannengcc.top/gtvvhxmzej.html

JS:   throw new Error("错误信息");
来源：http://hz.9152youxi.cn/gtvayvgosx.html

TS:   throw new Error("错误信息");
来源：http://hz.zycfv.cn/gtulpufqol.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.chenzaomai.com/gtpdmxjtpc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.shangyingyoupin.top/gtynybngku.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.snrcjt.cn/gtgalqfdfl.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.cashguo.top/gtihpgwidy.html

[H04] 自定义异常类型
来源：http://hz.dianchejie.cn/gtkboiublt.html

Py:   class MyError(Exception): pass
来源：http://hz.aibaodan.cn/gtnxgahitv.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.ivvv.top/gtecevttja.html

JS:   class MyError extends Error {}
来源：http://hz.xylfe.cn/gtwedhuggc.html

TS:   class MyError extends Error {}
来源：http://hz.yvedp.cn/gtcjlzjgru.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yj202588.top/gtfznyoyxg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.chenjidiqi.icu/gtnjcouaox.html

Ruby: class MyError < StandardError; end
来源：http://hz.ydjk.org.cn/gtulgnumud.html

C#:   class MyException : Exception {}
来源：http://hz.wangdashe.top/gtnlaiucyu.html

[H05] 捕获特定类型
来源：http://hz.jiagoushi.top/gturjjtkrd.html

Py:   except ValueError as e:
来源：http://hz.andypj.xyz/gtnrhzvcty.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yj20258.top/gtgbdjuiyh.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.haohaochexian.top/gtqevwrysl.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.xinyue.icu/gtydcslsjq.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.aibaodan.cn/gtkywnilyu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.9152youxi.cn/gtyfyaksqr.html

Ruby: rescue ArgumentError => e
来源：http://hz.zhiwuduotai.top/gtadcxllry.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hammf.cn/gtimkunnxw.html

[H06] 可选值 / 空值安全访问
来源：http://hz.cheryme.top/gtlxnsxsrz.html

Py:   value = d.get("k") or default
来源：http://hz.cqqwz.cn/gtgicssmaq.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yvedp.cn/gtgunlluio.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.hongshengwenyu.top/gtxtftlccy.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.ppjwa.cn/gtsmhzgeoz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.redwolf501.top/gtikmuyfov.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.nanxinkj.top/gtjsoixwrt.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhijiandao.cn/gtfmmfwrpc.html

C#:   obj?.A?.B ?? default
来源：http://hz.9152youxi.cn/gtymdxymcz.html

[H07] 断言
来源：http://hz.pycfn.com/gtsicnhifw.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zhoulong.xyz/gthlhedbxt.html

PHP:  assert($x > 0);
来源：http://hz.nwbrower.top/gttjuyuhtu.html

JS:   console.assert(x > 0);
来源：http://hz.nwbrower.top/gtqebkpmxx.html

TS:   console.assert(x > 0);
来源：http://hz.nanxinkj.top/gthmbpjwxj.html

Java: assert x > 0 : "必须为正";
来源：http://hz.shzxlz.cn/gtkogxwiuf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yuanzhike.top/gtdctiaxtv.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yueranfly.top/gtzjwehpvn.html

C#:   Debug.Assert(x > 0);
来源：http://hz.ydjk.org.cn/gterucahgs.html

[H08] 获取错误信息与堆栈
来源：http://hz.xingfuxueyuan.xyz/gtutqbdyfu.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.sxryk.cn/gttgrfuord.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zhoulong.xyz/gttlttptdo.html

JS:   e.message;  e.stack
来源：http://hz.sweek.top/gttqklkceb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.xingfuxueyuan.xyz/gtkrpahflk.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhiwuduotai.top/gtjsogrowk.html

Go:   err.Error()
来源：http://hz.shangyingyoupin.top/gtblrirday.html

Ruby: e.message;  e.backtrace
来源：http://hz.yuanzhike.top/gtzjnzaxcr.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhongyouzk.top/gtmwyzfuot.html

[H09] 带错误码的异常
来源：http://hz.hnqzz.top/gtzaqhvajg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.chenzaomai.com/gtpleykzhm.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.tianlin.xyz/gtsswwcnec.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.guannengcc.top/gtsowekfvn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jqgfzy.top/gthfgnyifd.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jinyuanbaomall.cn/gtyfcagkly.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.0kj1m.cn/gtjtycaiug.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jinqigfzy.top/gthtlsfbbd.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.ivvv.top/gtvdohqkgf.html

[H10] 资源自动释放
来源：http://hz.chenzaomai.com/gtczqyausl.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.haohaochexian.top/gthoofyqsr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.nanxinkj.top/gtnjoaxhnd.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xingfuxueyuan.xyz/gtntfgcjhn.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.vqdsnc.cn/gtrhiwebqk.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.pycfn.com/gtloyzbhnx.html

Go:   defer f.Close()
来源：http://hz.pycfn.com/gtvrblhlal.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.feifeiyinyue.top/gtvirjwfcr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.daria6918.cn/gtpvrepcms.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtrpvycakl.html

I. 正则表达式
来源：http://hz.dianchejie.cn/gtcjxtbzaz.html

================================================================================
来源：http://hz.316326.xyz/gtkghgcsvg.html

[I01] 判断是否匹配
来源：http://hz.xziqi.cn/gtkimnccjy.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jqgfzy.top/gtkrvdvcku.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.ydzc1.top/gtjpfgnxav.html

JS:   /\d+/.test(s)
来源：http://hz.quarkkingdee.top/gtaprnikof.html

TS:   /\d+/.test(s)
来源：http://hz.nanxuanxn.top/gtvpsioafb.html


<!-- 参考信息 -->