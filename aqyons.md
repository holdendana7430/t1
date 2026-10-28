代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zhoulong.xyz/gtigburvyg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.cheryme.top/gtgxurnjlh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.dashuyun.cn/gtcsenavzw.html

[F08] 遍历目录
来源：http://hz.zhaomingkeji.xyz/gtjhwbjmul.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.gaohongyu789.top/gtglizpdnx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.fengsongda.top/gtjihyppjc.html

JS:   fs.readdirSync("dir")
来源：http://hz.nanxuanxn.top/gtgczgccma.html

TS:   fs.readdirSync("dir")
来源：http://hz.cheryme.top/gtvbswxakl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.meibo888.top/gtabikrrgq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.meibo888.top/gtjhtyyxuo.html

Ruby: Dir.children("dir")
来源：http://hz.andypj.xyz/gtaesbelmw.html

C#:   Directory.GetFiles("dir")
来源：http://hz.hywenlv.cn/gtpetjmrpb.html

[F09] 获取文件大小
来源：http://hz.jqgufenzy.top/gtfkahuxau.html

Py:   os.path.getsize("a.txt")
来源：http://hz.nanxinkj.top/gtwvxiehsv.html

PHP:  filesize("a.txt");
来源：http://hz.tanke756.top/gtjuiwqjxk.html

JS:   fs.statSync("a.txt").size
来源：http://hz.shuidangran.top/gtwsbqhjxi.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jianghu66.top/gtfmvdefld.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.nwbrower.top/gteaqcezti.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.xziqi.cn/gtrwnatmub.html

Ruby: File.size("a.txt")
来源：http://hz.yanxiufei.cn/gtviqypfof.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.guowangkeji.top/gtryhvvmxd.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.cashguo.top/gtuaicwafw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.chenjidiqi.icu/gtblmehjth.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.nwbrower.top/gtrrldwibv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.vqdsnc.cn/gtwncrfvlj.html

TS:   path.extname("a.txt")
来源：http://hz.zhongyouzk.top/gtjcriqnif.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yj20258888.top/gtbvdqoysb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zhengqikj.top/gtlzmspcdx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhixingplan.top/gtijvutddh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtdyovsune.html

[F11] 复制与移动文件
来源：http://hz.aibaodan.cn/gtitqkncqb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.gogol.net.cn/gtinilrtrl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.vqdsnc.cn/gtxnknoyyq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.meibo888.top/gtmzoiztxb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zdqjudy.top/gtkfiplqpd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.ivvv.top/gtsdsrtiye.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.ivvv.top/gtugnlbqyv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.xinyue.icu/gtnflymlfy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ivvv.top/gtfdwwwrxv.html

[F12] CSV 读写
来源：http://hz.jiagoushi.top/gtjjpbxmgf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.cucudq.cn/gtirktlwjm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.xuanzx.com/gtloglgzpy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yangfankeji.com/gtgrwbclld.html

TS:   // 同上
来源：http://hz.nanxuanxn.top/gtjzatqhab.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.gaohongyu789.top/gtyqladoyj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.daria6918.cn/gtrufqkema.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.meibo888.top/gtpdpmyifa.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zdqjudy.top/gtqigzurpl.html

================================================================================
来源：http://hz.tianlin.xyz/gtjuwdrszh.html

G. 面向对象
来源：http://hz.haohaochexian.top/gtivvcgetz.html

================================================================================
来源：http://hz.nwbrower.top/gtbsxvwdpm.html

[G01] 定义类
来源：http://hz.zhoulong.xyz/gtvgiawhaf.html

Py:   class User: pass
来源：http://hz.yj202588.top/gtczbqngzw.html

PHP:  class User {}
来源：http://hz.cdnleiting.top/gtxmqbwice.html

JS:   class User {}
来源：http://hz.zhengqikj.top/gtzpvadpmb.html

TS:   class User { name: string = ""; }
来源：http://hz.cheryme.top/gtbbulgwca.html

Java: class User {}
来源：http://hz.snrcjt.cn/gtevdisekx.html

Go:   type User struct { Name string }
来源：http://hz.0kj1m.cn/gtagnjaotm.html

Ruby: class User; end
来源：http://hz.cqqwz.cn/gtjjymcrne.html

C#:   class User {}
来源：http://hz.jiagoushi.top/gtgtxradlr.html

[G02] 构造函数
来源：http://hz.yuxming.cn/gtbvtagpue.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zdqjudy.top/gtptobfnfv.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.svipenyu.cn/gtoejajewy.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.gaohongyu789.top/gtshrlljgs.html

TS:   constructor(public name: string) {}
来源：http://hz.zhijiandao.cn/gtthdezeio.html

Java: User(String name) { this.name = name; }
来源：http://hz.gaohongyu789.top/gtngsjjlpg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yonumen.top/gtoaypholw.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.aibaodan.cn/gtlstvzbqi.html

C#:   public User(string name) { Name = name; }
来源：http://hz.aizwys.cn/gtdvpcpjdy.html

[G03] 实例属性
来源：http://hz.jinghuilouyu.cn/gtviroarnp.html

Py:   self.name = "x"
来源：http://hz.jinqigfzy.top/gtxgumkesw.html

PHP:  public string $name = "x";
来源：http://hz.dashuyun.cn/gtlnqqkany.html

JS:   this.name = "x";
来源：http://hz.wangdashe.top/gtczyiqife.html

TS:   name: string = "x";
来源：http://hz.mhx1999.top/gtunencoip.html

Java: private String name;
来源：http://hz.quarkkingdee.top/gtqztbkbvz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.xylfe.cn/gteuwzcexl.html

Ruby: @name = "x"
来源：http://hz.zhongyouzk.top/gtklojppmr.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.ydzc1.top/gtdaopahhs.html

[G04] 定义方法
来源：http://hz.redwolf501.top/gtzcumcpnq.html

Py:   def greet(self): return self.name
来源：http://hz.sxryk.cn/gtzcqvoeao.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.wangshuangyany.cn/gttwgalkvf.html

JS:   greet() { return this.name; }
来源：http://hz.pycfn.com/gtiokwaesb.html

TS:   greet(): string { return this.name; }
来源：http://hz.nanxuanxn.top/gtrsaqyalp.html

Java: String greet() { return name; }
来源：http://hz.wangshuangyany.cn/gthxorbbug.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.fengsongda.top/gtvyjbavmg.html

Ruby: def greet; @name; end
来源：http://hz.andypj.xyz/gtkoqwmyhp.html

C#:   public string Greet() => Name;
来源：http://hz.kuanghao11.cn/gteewjpoqd.html

[G05] 继承
来源：http://hz.yj20258888.top/gtfjhhjtzw.html

Py:   class Admin(User): pass
来源：http://hz.jinyuanbaomall.cn/gtegbvddvz.html

PHP:  class Admin extends User {}
来源：http://hz.jqgfzy.top/gtvfwvytdo.html

JS:   class Admin extends User {}
来源：http://hz.iojbl.cn/gttfcsnkvb.html

TS:   class Admin extends User {}
来源：http://hz.yangfankeji.com/gtdmoexdbc.html

Java: class Admin extends User {}
来源：http://hz.cashguo.top/gtkvdmahis.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.quarkkingdee.top/gtvkgwfoiw.html

Ruby: class Admin < User; end
来源：http://hz.xinyue.icu/gtmxentiwi.html

C#:   class Admin : User {}
来源：http://hz.fzhhl.top/gtzniutdpv.html

[G06] 重写方法
来源：http://hz.ppjwa.cn/gtaqritwhm.html

Py:   def greet(self): return "admin"
来源：http://hz.haohaochexian.top/gtqswxasle.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yuxming.cn/gtlslqgjgo.html

JS:   greet() { return "admin"; }
来源：http://hz.andypj.xyz/gtkrlhdzvb.html

TS:   greet(): string { return "admin"; }
来源：http://hz.birdmap.top/gtblcgcyhn.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jqgufenzy.top/gtsmzwflir.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhixingplan.top/gttyfpmntl.html

Ruby: def greet; "admin"; end
来源：http://hz.nanxuanxn.top/gtcfdsrzwl.html

C#:   public override string Greet() => "admin";
来源：http://hz.yj20258888.top/gtvajzmvqu.html

[G07] 调用父类方法
来源：http://hz.jinqigufen.top/gtsrstsxbj.html

Py:   super().greet()
来源：http://hz.sufxvd.cn/gtuavhncva.html

PHP:  parent::greet();
来源：http://hz.jinqigufen.top/gtzqffgynt.html

JS:   super.greet();
来源：http://hz.jinghuilouyu.cn/gtklgcicks.html

TS:   super.greet();
来源：http://hz.aibaodan.cn/gttstxikgs.html

Java: super.greet();
来源：http://hz.dianchejie.cn/gtfwjiuurr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.xziqi.cn/gtsswpilir.html

Ruby: super
来源：http://hz.ydjk.org.cn/gtftorwnbk.html

C#:   base.Greet();
来源：http://hz.shzxlz.cn/gtuveimvny.html

[G08] 静态方法与属性
来源：http://hz.chenjidiqi.icu/gtazmrcbfy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.gotoacloud.top/gtovtzabeq.html

PHP:  public static function f() {}
来源：http://hz.tanke756.top/gtxzrqddgw.html

JS:   static f() {}
来源：http://hz.yj202588.top/gtqmeggtcc.html

TS:   static f(): void {}
来源：http://hz.shanyushiyangtech.top/gtncuwtsfj.html

Java: static void f() {}
来源：http://hz.hnxiangtu.top/gtuxwonhin.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jinqigufen.top/gtwcfolfbr.html

Ruby: def self.f; end
来源：http://hz.kuanghao11.cn/gtakucrnmc.html

C#:   public static void F() {}
来源：http://hz.shanyushiyangkeji.top/gtxwixsuco.html

[G09] 接口 / 抽象类
来源：http://hz.sufxvd.cn/gtmamasqul.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.dianchejie.cn/gticjhibdk.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jqgufenzy.top/gtitygmgpy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yangfankeji.com/gthioeisyz.html

TS:   interface Shape { area(): number; }
来源：http://hz.xinyue.icu/gtvrmuekra.html

Java: interface Shape { double area(); }
来源：http://hz.9152youxi.cn/gteyrfefwa.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.aibaodan.cn/gtpnkbxpaj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hammf.cn/gtmhgnukiq.html

C#:   interface IShape { double Area(); }
来源：http://hz.shzxlz.cn/gthaapsjrv.html

[G10] 访问控制
来源：http://hz.aibaodan.cn/gtzadogpkp.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zdqjudy.top/gtjcncvtrv.html

PHP:  public / protected / private
来源：http://hz.gogol.net.cn/gtzxnjbcws.html

JS:   #private 字段；其余公开
来源：http://hz.hammf.cn/gtgwsngkrp.html

TS:   public / protected / private
来源：http://hz.9152youxi.cn/gtnzstlhdz.html

Java: public / protected / private / 默认包级
来源：http://hz.daxiang520.top/gtlpqppssh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yanxiufei.cn/gttacflmqa.html

Ruby: public / protected / private
来源：http://hz.redwolf501.top/gttbfbbzfg.html

C#:   public / protected / private / internal
来源：http://hz.yueranfly.top/gtuwqtmkab.html

[G11] getter / setter
来源：http://hz.yj20258888.top/gtnyfuvhut.html

Py:   @property 与 @x.setter
来源：http://hz.jiagoushi.top/gtiipqytsv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.smart0.xyz/gtvofspygs.html

JS:   get name() { return this._name; }
来源：http://hz.vqdsnc.cn/gtigldgpxs.html

TS:   get name(): string { return this._name; }
来源：http://hz.jianghu66.top/gtszefhbsm.html

Java: public String getName() { return name; }
来源：http://hz.jinqigfzy.top/gttdtoslyz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.316326.xyz/gtigpcynki.html

Ruby: attr_accessor :name
来源：http://hz.yvedp.cn/gtoepgfxjw.html

C#:   public string Name { get; set; }
来源：http://hz.jqgufenzy.top/gtslqetxkq.html

[G12] 对象转字符串
来源：http://hz.zhongyouzk.top/gtmirruugl.html

Py:   def __str__(self): return self.name
来源：http://hz.cqqwz.cn/gtzhqwtokc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.aibaodan.cn/gttgkrroqs.html

JS:   toString() { return this.name; }
来源：http://hz.daria6918.cn/gtslbzlcbo.html

TS:   toString(): string { return this.name; }
来源：http://hz.aizwys.cn/gtituthgqe.html

Java: @Override public String toString() { return name; }
来源：http://hz.hnxiangtu.top/gtddcxmxrd.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhongyouzk.top/gtjdoquzcd.html

Ruby: def to_s; @name; end
来源：http://hz.hammf.cn/gtnmycmwkn.html

C#:   public override string ToString() => Name;
来源：http://hz.pycfn.com/gtbnbfczoi.html

[G13] 判断对象类型
来源：http://hz.xziqi.cn/gtlkdmevxb.html

Py:   isinstance(u, User)
来源：http://hz.mhx1999.top/gtajxoqyeb.html

PHP:  $u instanceof User
来源：http://hz.jinghuilouyu.cn/gtpkfdcqsf.html

JS:   u instanceof User
来源：http://hz.zdqjudy.top/gtjoqugoli.html

TS:   u instanceof User
来源：http://hz.bjfxy.top/gtbfayxedi.html

Java: u instanceof User
来源：http://hz.zhaomingkeji.xyz/gtbzefuwdl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.nwbrower.top/gtyefapvap.html

Ruby: u.is_a?(User)
来源：http://hz.xylfe.cn/gttxfvyiqr.html

C#:   u is User
来源：http://hz.fzhhl.top/gtioeinkpr.html

[G14] 数据类 / record
来源：http://hz.chenlongwang.top/gttwryqeen.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.shanyushiyangtech.top/gtlnlpjwdo.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.tanke756.top/gtneywoygg.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yj20258888.top/gthwtivhmh.html

TS:   type User = { name: string; age: number };
来源：http://hz.kuanghao11.cn/gtybdrakky.html

Java: record User(String name, int age) {}
来源：http://hz.dianchejie.cn/gtuwssipsu.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jinghuilouyu.cn/gtkfyyfrdh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.mhx1999.top/gtbzrhugxq.html

C#:   record User(string Name, int Age);
来源：http://hz.xuetiantiany.cn/gthalyizjs.html

[G15] 枚举
来源：http://hz.hongshengwenyu.top/gtvvialsnn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.sweek.top/gtfxbozzex.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.shzxlz.cn/gtrytaptuy.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.shanyushiyangkeji.top/gtwuvmkilc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.c1oappe.top/gtbaxqkpif.html

Java: enum Color { RED, GREEN }
来源：http://hz.ydzc1.top/gtzdpbjioj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.cashguo.top/gthwvvytrk.html

Ruby: Color = %i[red green].freeze
来源：http://hz.cheryme.top/gtiykvbnmu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhiwuduotai.top/gtmyqkoidw.html

[G16] 对象转数组 / 字典
来源：http://hz.jinghuilouyu.cn/gtbqizxfct.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.smart0.xyz/gtjvykqnve.html

PHP:  get_object_vars($obj);
来源：http://hz.smart0.xyz/gtpnfbjzsu.html

JS:   Object.entries(obj)
来源：http://hz.gzhubu.top/gtlcrttsbl.html

TS:   Object.entries(obj)
来源：http://hz.yonumen.top/gtdvffxtfe.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.feifeiyinyue.top/gtetnmgqan.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.nanxuanxn.top/gtfmgxtlom.html

Ruby: obj.instance_variables
来源：http://hz.haohaochexian.top/gtxtdngyok.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.tianlin.xyz/gtnytffelc.html

================================================================================
来源：http://hz.zhixingplan.top/gttpckyxda.html

H. 异常与错误处理
来源：http://hz.gzhubu.top/gtmlimvqpj.html

================================================================================
来源：http://hz.cashguo.top/gtisdvbiam.html

[H01] try / catch 基础
来源：http://hz.316326.xyz/gtplpjowwz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.gaohongyu789.top/gtulzwfhnu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ydzc1.top/gtpbzluvdr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.dashuyun.cn/gtdvrqkmlr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.316326.xyz/gtdgeskfzq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.meibo888.top/gtrmnvjokf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.haohaochexian.top/gtcnjrofol.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.hfpthk.cn/gtfdspyuag.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.wangdashe.top/gtopgkvjwv.html

[H02] finally / ensure 收尾
来源：http://hz.sxryk.cn/gtzhxulsfs.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yonumen.top/gtcrthnjqc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xingfuxueyuan.xyz/gtneuwmnce.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.ywan-chungtsiang.top/gtrzvpablu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jiagoushi.top/gtijcduqcq.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.iojbl.cn/gtswdwojop.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.fengsongda.top/gtyjsndgkg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.iojbl.cn/gtrcwvvoam.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.ehwqpu.com/gtgbribtsw.html

[H03] 主动抛出异常
来源：http://hz.shzxlz.cn/gtivhyujaq.html

Py:   raise ValueError("错误信息")
来源：http://hz.chenlongwang.top/gtcbexledh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.hnxiangtu.top/gtwccjghhp.html

JS:   throw new Error("错误信息");
来源：http://hz.xuetiantiany.cn/gtmxnrovtw.html

TS:   throw new Error("错误信息");
来源：http://hz.jiagoushi.top/gtgqxqnctp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.ybcxt.top/gtwgrmcdna.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.ywan-chungtsiang.top/gtosfjcibr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ydzc1.top/gtufjdefcn.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.bjfxy.top/gtrjvwulvs.html

[H04] 自定义异常类型
来源：http://hz.pengpengdd.cyou/gtsxibiywd.html

Py:   class MyError(Exception): pass
来源：http://hz.jqgufenzy.top/gtcmbcsrjg.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.ybcxt.top/gtfpgdfavj.html

JS:   class MyError extends Error {}
来源：http://hz.yvedp.cn/gtltnkhclv.html

TS:   class MyError extends Error {}
来源：http://hz.yj20258888.top/gtvvrrywfb.html

Java: class MyException extends RuntimeException {}
来源：http://hz.cdnleiting.top/gtdlkokyqp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jiagoushi.top/gtlxuyrmtu.html

Ruby: class MyError < StandardError; end
来源：http://hz.9152youxi.cn/gtgedjjtmm.html

C#:   class MyException : Exception {}
来源：http://hz.tian-w.cn/gteendradd.html

[H05] 捕获特定类型
来源：http://hz.nanxuanxn.top/gtnwrimqch.html

Py:   except ValueError as e:
来源：http://hz.52xcode.cn/gtxopblmgm.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yonumen.top/gtqgvrplvc.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.nanxuanxn.top/gtxjznfuim.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.quarkkingdee.top/gtcflbiaav.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.shanyushiyangtech.top/gthadjetvu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.bjfxy.top/gtpavaifzy.html

Ruby: rescue ArgumentError => e
来源：http://hz.yj202588.top/gtcwroxkkp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.shuidangran.top/gtkaasxdzo.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jyoumei.cn/gtwkqkdxxe.html

Py:   value = d.get("k") or default
来源：http://hz.dashuyun.cn/gtyzpcjqdf.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.andypj.xyz/gtjhqwsspj.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.sufxvd.cn/gtuhapqkgx.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.chenzaomai.com/gtnpyemgfq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.tian-w.cn/gtjicgusdf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jiagoushi.top/gtdrkdgypi.html

Ruby: d&.dig(:a, :b)
来源：http://hz.quarkkingdee.top/gtpccdkohv.html

C#:   obj?.A?.B ?? default
来源：http://hz.xziqi.cn/gtwhbybbfl.html

[H07] 断言
来源：http://hz.yonumen.top/gtcoxziaeh.html

Py:   assert x > 0, "必须为正"
来源：http://hz.vqdsnc.cn/gtnedgcbxg.html

PHP:  assert($x > 0);
来源：http://hz.guowangkeji.top/gtlmmjlzju.html

JS:   console.assert(x > 0);
来源：http://hz.havefunace.top/gtmujkiuhd.html

TS:   console.assert(x > 0);
来源：http://hz.vqdsnc.cn/gtqiwwgjuv.html

Java: assert x > 0 : "必须为正";
来源：http://hz.hnxiangtu.top/gtkgkknaao.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.hnxiangtu.top/gtyfdghuik.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yueranfly.top/gtgvdmenah.html

C#:   Debug.Assert(x > 0);
来源：http://hz.cheryme.top/gtarbmqvuq.html

[H08] 获取错误信息与堆栈
来源：http://hz.xinyue.icu/gtmssmrhbo.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.nwbrower.top/gtdunagnai.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.hnxiangtu.top/gtormltuha.html

JS:   e.message;  e.stack
来源：http://hz.zhaomingkeji.xyz/gtxmmwzqes.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.c1oappe.top/gtaqxobvcx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hnqzz.top/gtqkajohjy.html

Go:   err.Error()
来源：http://hz.316326.xyz/gtjhjbsjsq.html

Ruby: e.message;  e.backtrace
来源：http://hz.wangshuangyany.cn/gtmdqjbpjn.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhixingplan.top/gttaapfdmj.html

[H09] 带错误码的异常
来源：http://hz.daria6918.cn/gtkchylncz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.birdmap.top/gtowkqobqw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.sxryk.cn/gtugcbidhc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.daxiang520.top/gtlpfcsecy.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.dashuyun.cn/gtxrceyxza.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yj20258.top/gtqyrxemcn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.nanxinkj.top/gtmyxzazjw.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yangfankeji.com/gthekebqgx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.nanxuanxn.top/gtmxoovsqz.html

[H10] 资源自动释放
来源：http://hz.zycfv.cn/gtimcjfeuz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yuxming.cn/gtrykmaldg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.xinyue.icu/gtrsfzrkcu.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yuanzhike.top/gtucftmldt.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xuanzx.com/gtymtwityw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.dashuyun.cn/gtbtsbepbv.html

Go:   defer f.Close()
来源：http://hz.cdnleiting.top/gtlueuezjk.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.wangshuangyany.cn/gttvqrneoh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yueranfly.top/gtdlytnosk.html

================================================================================
来源：http://hz.sysykeji.top/gtmqegubnz.html

I. 正则表达式
来源：http://hz.yvedp.cn/gtnhxzzxhj.html

================================================================================
来源：http://hz.cqqwz.cn/gterlrrxjh.html

[I01] 判断是否匹配
来源：http://hz.gogol.net.cn/gtrqexojvf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.shanyushiyangtech.top/gtyghyfael.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zycfv.cn/gtvpekqtzj.html

JS:   /\d+/.test(s)
来源：http://hz.cheryme.top/gtjbmulbtx.html

TS:   /\d+/.test(s)
来源：http://hz.redwolf501.top/gtqsbzizeg.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.guowangkeji.top/gtufcwomss.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.shanyushiyangkeji.top/gtkwrbkflf.html

Ruby: s.match?(/\d+/)
来源：http://hz.yvedp.cn/gtggrlrsag.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.xylfe.cn/gtwinjbztm.html


<!-- 参考信息 -->