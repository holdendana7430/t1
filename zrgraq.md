代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hongshengwenyu.top/gtyyahzkxk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.ehwqpu.com/gtajdnfhod.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zhiwuduotai.top/gtlgrtffhs.html

[F08] 遍历目录
来源：http://hz.mhx1999.top/gtiebiuvrr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.0kj1m.cn/gtlflautjq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.pengpengdd.cyou/gtlpdvnrvg.html

JS:   fs.readdirSync("dir")
来源：http://hz.nwbrower.top/gtrhmizuwk.html

TS:   fs.readdirSync("dir")
来源：http://hz.haohaochexian.top/gtjvktazen.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yvedp.cn/gtogdoigbq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.52xcode.cn/gtmncmqaag.html

Ruby: Dir.children("dir")
来源：http://hz.jinghuilouyu.cn/gtgwvthkol.html

C#:   Directory.GetFiles("dir")
来源：http://hz.shanyushiyangtech.top/gtkhpkohzc.html

[F09] 获取文件大小
来源：http://hz.jlsjyb.cn/gticglxnxs.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yvedp.cn/gtfxdvpdam.html

PHP:  filesize("a.txt");
来源：http://hz.chenzaomai.com/gtqwganauu.html

JS:   fs.statSync("a.txt").size
来源：http://hz.shzxlz.cn/gtjuodunfm.html

TS:   fs.statSync("a.txt").size
来源：http://hz.sufxvd.cn/gtydcxzxii.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.c1oappe.top/gtwiyryjdb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yuxming.cn/gtbdmqvmtu.html

Ruby: File.size("a.txt")
来源：http://hz.andypj.xyz/gtyqtvmpjw.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.zhiwuduotai.top/gtmkyjywil.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jinghuilouyu.cn/gtgsydnfon.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.birdmap.top/gtfwzokwml.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.ydzc1.top/gtuxltnbmf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zycfv.cn/gtjrdqarcx.html

TS:   path.extname("a.txt")
来源：http://hz.sysykeji.top/gteacefeuw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.chenjidiqi.icu/gtalozasui.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.xziqi.cn/gtoksrazul.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yonumen.top/gtpfkbigil.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.wangdashe.top/gtmnrmqvtf.html

[F11] 复制与移动文件
来源：http://hz.hysaishi.cn/gtjptidsno.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jiagoushi.top/gtdbimlddz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yanxiufei.cn/gtfkcvvrxy.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.nanxuanxn.top/gthvkjlfwr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jinghuilouyu.cn/gtvojeqxxq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jqgufenzy.top/gtjuyjlthq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.fzhhl.top/gtalwytpep.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.nanxuanxn.top/gtkwawdvke.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhaomingkeji.xyz/gtlxnwztma.html

[F12] CSV 读写
来源：http://hz.hfpthk.cn/gtympookht.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xingfuxueyuan.xyz/gttxkamjfx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.0kj1m.cn/gtdnygseiy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jqgfzy.top/gtntbifeho.html

TS:   // 同上
来源：http://hz.dashuyun.cn/gtxblehzyw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.tanke756.top/gtuvpbqjbr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.shuidangran.top/gtocyybjgp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zdqjudy.top/gtxlervkrh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.sufxvd.cn/gtrhamxeer.html

================================================================================
来源：http://hz.wangshuangyany.cn/gthwejxpvd.html

G. 面向对象
来源：http://hz.9152youxi.cn/gtliwwvwuj.html

================================================================================
来源：http://hz.sweek.top/gtnzxryjjo.html

[G01] 定义类
来源：http://hz.hnqzz.top/gtuhffacjv.html

Py:   class User: pass
来源：http://hz.jinqigfzy.top/gtxdoojsqn.html

PHP:  class User {}
来源：http://hz.jinyuanbaomall.cn/gtnpphgptw.html

JS:   class User {}
来源：http://hz.zdqjudy.top/gtxglhdfui.html

TS:   class User { name: string = ""; }
来源：http://hz.jqgufenzy.top/gtdrmwejas.html

Java: class User {}
来源：http://hz.zdqjudy.top/gtlybekkir.html

Go:   type User struct { Name string }
来源：http://hz.andypj.xyz/gtyxxjcfgw.html

Ruby: class User; end
来源：http://hz.meibo888.top/gtardbduhw.html

C#:   class User {}
来源：http://hz.tanke756.top/gtgesivuvs.html

[G02] 构造函数
来源：http://hz.svipenyu.cn/gtvteevluq.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.nwbrower.top/gtssvlyrro.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ybcxt.top/gttobfxczv.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.gzhubu.top/gtifiipwzk.html

TS:   constructor(public name: string) {}
来源：http://hz.sysykeji.top/gtbbmnirpu.html

Java: User(String name) { this.name = name; }
来源：http://hz.cdnleiting.top/gtbsxzrjqh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.52xcode.cn/gtsczrqcrj.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.zhijiandao.cn/gtncbgivzy.html

C#:   public User(string name) { Name = name; }
来源：http://hz.hywenlv.cn/gtkzfcrpwb.html

[G03] 实例属性
来源：http://hz.tian-w.cn/gtduoustjd.html

Py:   self.name = "x"
来源：http://hz.jinqigfzy.top/gtgntjvgjm.html

PHP:  public string $name = "x";
来源：http://hz.nanxinkj.top/gtuuaeyfoy.html

JS:   this.name = "x";
来源：http://hz.yuanzhike.top/gtgndsctfr.html

TS:   name: string = "x";
来源：http://hz.cheryme.top/gtacohglau.html

Java: private String name;
来源：http://hz.ywan-chungtsiang.top/gtbqwmdyrg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.0kj1m.cn/gtoxgjeepu.html

Ruby: @name = "x"
来源：http://hz.yj20258888.top/gtkmnxygqw.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yj202588.top/gthvooghzk.html

[G04] 定义方法
来源：http://hz.0kj1m.cn/gtlootdqyg.html

Py:   def greet(self): return self.name
来源：http://hz.fengsongda.top/gtnyhxrbdr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jinqigfzy.top/gtakjycoxz.html

JS:   greet() { return this.name; }
来源：http://hz.shuidangran.top/gtwdcksdpw.html

TS:   greet(): string { return this.name; }
来源：http://hz.fzhhl.top/gtferkdkke.html

Java: String greet() { return name; }
来源：http://hz.cheryme.top/gtxpdgkzdf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yangfankeji.com/gtnmvbjbyu.html

Ruby: def greet; @name; end
来源：http://hz.cdnleiting.top/gtatvdwtyt.html

C#:   public string Greet() => Name;
来源：http://hz.yj20258.top/gtexgbnmlc.html

[G05] 继承
来源：http://hz.birdmap.top/gtfrdbsbci.html

Py:   class Admin(User): pass
来源：http://hz.zhengqikj.top/gtmxzdptjp.html

PHP:  class Admin extends User {}
来源：http://hz.zhoulong.xyz/gtcupguphu.html

JS:   class Admin extends User {}
来源：http://hz.hywenlv.cn/gtvkqxyusr.html

TS:   class Admin extends User {}
来源：http://hz.zycfv.cn/gtezulpcbw.html

Java: class Admin extends User {}
来源：http://hz.jyoumei.cn/gtppfzmyzj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.sweek.top/gtxxsmfufj.html

Ruby: class Admin < User; end
来源：http://hz.cucudq.cn/gtjdwlilyi.html

C#:   class Admin : User {}
来源：http://hz.c1oappe.top/gtgtagyhkw.html

[G06] 重写方法
来源：http://hz.yonumen.top/gtkvhfejwy.html

Py:   def greet(self): return "admin"
来源：http://hz.smart0.xyz/gtvjbhumly.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ppjwa.cn/gtbtswvrpj.html

JS:   greet() { return "admin"; }
来源：http://hz.chenzaomai.com/gtxgkpmogh.html

TS:   greet(): string { return "admin"; }
来源：http://hz.cheryme.top/gtjsiodxtl.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hfpthk.cn/gtqmwszzay.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.vqdsnc.cn/gtwktuuchl.html

Ruby: def greet; "admin"; end
来源：http://hz.shuidangran.top/gtgkqudtnt.html

C#:   public override string Greet() => "admin";
来源：http://hz.sufxvd.cn/gtjdziplkk.html

[G07] 调用父类方法
来源：http://hz.aizwys.cn/gtarkgzraa.html

Py:   super().greet()
来源：http://hz.yuxming.cn/gtawzqernf.html

PHP:  parent::greet();
来源：http://hz.fengsongda.top/gtvegsryls.html

JS:   super.greet();
来源：http://hz.yueranfly.top/gtvhvaspug.html

TS:   super.greet();
来源：http://hz.shanyushiyangkeji.top/gtgvxyvrod.html

Java: super.greet();
来源：http://hz.zycfv.cn/gtxwnowtoi.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zhixingplan.top/gtpdyrekcm.html

Ruby: super
来源：http://hz.yj202588.top/gtdrqmhlnc.html

C#:   base.Greet();
来源：http://hz.ywan-chungtsiang.top/gtirstmein.html

[G08] 静态方法与属性
来源：http://hz.daxiang520.top/gtvhhsvras.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zycfv.cn/gtwjrosdxv.html

PHP:  public static function f() {}
来源：http://hz.jinyuanbaomall.cn/gtaohdqrpq.html

JS:   static f() {}
来源：http://hz.c1oappe.top/gthsjnmnhh.html

TS:   static f(): void {}
来源：http://hz.316326.xyz/gtfvmgvkjj.html

Java: static void f() {}
来源：http://hz.yonumen.top/gtscivsgva.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.0kj1m.cn/gtuysnkaeq.html

Ruby: def self.f; end
来源：http://hz.gaohongyu789.top/gtjprfzlwl.html

C#:   public static void F() {}
来源：http://hz.jinyuanbaomall.cn/gtowxehndz.html

[G09] 接口 / 抽象类
来源：http://hz.cucudq.cn/gtuikmgaya.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jiagoushi.top/gtyqupusut.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.chenjidiqi.icu/gtdkfcpucm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.xylfe.cn/gteqbuzbfc.html

TS:   interface Shape { area(): number; }
来源：http://hz.gogol.net.cn/gtfhuutjlm.html

Java: interface Shape { double area(); }
来源：http://hz.zhixingplan.top/gtdtkowlng.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.mhx1999.top/gtuicdqbrm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhixingplan.top/gtbzsrspfz.html

C#:   interface IShape { double Area(); }
来源：http://hz.xingfuxueyuan.xyz/gtkdjktnqn.html

[G10] 访问控制
来源：http://hz.pycfn.com/gtonqsugti.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jqgfzy.top/gtcpifkdjl.html

PHP:  public / protected / private
来源：http://hz.pengpengdd.cyou/gtwkilfzdi.html

JS:   #private 字段；其余公开
来源：http://hz.guannengcc.top/gtdmqjdbdp.html

TS:   public / protected / private
来源：http://hz.kuanghao11.cn/gtnflyzswi.html

Java: public / protected / private / 默认包级
来源：http://hz.snrcjt.cn/gtrceckmyh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.xziqi.cn/gtxvhyctto.html

Ruby: public / protected / private
来源：http://hz.jianghu66.top/gtioafwksj.html

C#:   public / protected / private / internal
来源：http://hz.sufxvd.cn/gtsfkqywgi.html

[G11] getter / setter
来源：http://hz.yj20258.top/gtdzwihgon.html

Py:   @property 与 @x.setter
来源：http://hz.yongpay.top/gtqihuudvb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.ppjwa.cn/gtnnabnbcw.html

JS:   get name() { return this._name; }
来源：http://hz.cucudq.cn/gtxxmsrave.html

TS:   get name(): string { return this._name; }
来源：http://hz.svipenyu.cn/gtywtgjifb.html

Java: public String getName() { return name; }
来源：http://hz.chenlongwang.top/gtpvtqfswu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.fzhhl.top/gtafeggnab.html

Ruby: attr_accessor :name
来源：http://hz.yangfankeji.com/gtemlsgztw.html

C#:   public string Name { get; set; }
来源：http://hz.jqgfzy.top/gtyiwxfuie.html

[G12] 对象转字符串
来源：http://hz.nanxinkj.top/gtwbtjunxl.html

Py:   def __str__(self): return self.name
来源：http://hz.zhoulong.xyz/gtemezsisx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.svipenyu.cn/gtswiawwsa.html

JS:   toString() { return this.name; }
来源：http://hz.tianlin.xyz/gtfbxiwclf.html

TS:   toString(): string { return this.name; }
来源：http://hz.yongpay.top/gtqhsqyfqo.html

Java: @Override public String toString() { return name; }
来源：http://hz.feifeiyinyue.top/gtmuismtcp.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.9152youxi.cn/gtwniexuch.html

Ruby: def to_s; @name; end
来源：http://hz.hammf.cn/gttmaiqisk.html

C#:   public override string ToString() => Name;
来源：http://hz.sufxvd.cn/gtcmlxsbvo.html

[G13] 判断对象类型
来源：http://hz.smart0.xyz/gtshqcoejj.html

Py:   isinstance(u, User)
来源：http://hz.guannengcc.top/gtvmcavowa.html

PHP:  $u instanceof User
来源：http://hz.hywenlv.cn/gtelpsnukk.html

JS:   u instanceof User
来源：http://hz.zhijiandao.cn/gtddwblrsi.html

TS:   u instanceof User
来源：http://hz.hywenlv.cn/gtazowzgwn.html

Java: u instanceof User
来源：http://hz.hnxiangtu.top/gtiaapzrcd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.bjfxy.top/gtdmltrqqr.html

Ruby: u.is_a?(User)
来源：http://hz.zhixingplan.top/gtxakiykgd.html

C#:   u is User
来源：http://hz.yueranfly.top/gtzvnxvwyk.html

[G14] 数据类 / record
来源：http://hz.shanyushiyangkeji.top/gtcajrbkfj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zdqjudy.top/gtjlahyxsp.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jyoumei.cn/gtytkrpyaf.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.nwbrower.top/gtkwmkihct.html

TS:   type User = { name: string; age: number };
来源：http://hz.kuanghao11.cn/gthcjpyvjx.html

Java: record User(String name, int age) {}
来源：http://hz.9152youxi.cn/gtqsvzgnzw.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yj202588.top/gtzqkdcqge.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.xylfe.cn/gtnxuxfxvr.html

C#:   record User(string Name, int Age);
来源：http://hz.snrcjt.cn/gtjzwancdh.html

[G15] 枚举
来源：http://hz.cheryme.top/gtmflpsrwo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.chenlongwang.top/gtmngmyrkw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.meibo888.top/gtbsjdsjej.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.xuetiantiany.cn/gtxnhuamex.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yj20258888.top/gtcsmhbnqw.html

Java: enum Color { RED, GREEN }
来源：http://hz.yj20258.top/gtmxxyiakd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ehwqpu.com/gtnwsnzdso.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ydzc1.top/gtdtqgtpfa.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ppjwa.cn/gtewhjftxa.html

[G16] 对象转数组 / 字典
来源：http://hz.nwbrower.top/gtbylvbriq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.xinyue.icu/gtpaiggewo.html

PHP:  get_object_vars($obj);
来源：http://hz.yj20258888.top/gtqpwpnecm.html

JS:   Object.entries(obj)
来源：http://hz.sxryk.cn/gtqalocrmc.html

TS:   Object.entries(obj)
来源：http://hz.fzhhl.top/gtlglbenjm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hnxiangtu.top/gtgybfwdew.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.aizwys.cn/gtkqcznneh.html

Ruby: obj.instance_variables
来源：http://hz.hnqzz.top/gtlmkixzgl.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yj202588.top/gtbbvchwzw.html

================================================================================
来源：http://hz.gotoacloud.top/gtnkvwwjri.html

H. 异常与错误处理
来源：http://hz.0kj1m.cn/gtmfzldkvo.html

================================================================================
来源：http://hz.gaohongyu789.top/gtepkmhbar.html

[H01] try / catch 基础
来源：http://hz.sufxvd.cn/gtmcrjredg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.gotoacloud.top/gtcnwslqfy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.52xcode.cn/gteybvsqbd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.sysykeji.top/gttjwwfdrs.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.aibaodan.cn/gtpvqruumg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.bjfxy.top/gthpvizvqt.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.xingfuxueyuan.xyz/gtwsdkomba.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.cashguo.top/gtkkdxerwv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zdqjudy.top/gtubqypzvp.html

[H02] finally / ensure 收尾
来源：http://hz.shuidangran.top/gtotpzasfx.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.xuanzx.com/gtpfmyyoqj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.cheryme.top/gtznvlwcxq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jinqigfzy.top/gtcpmusnoh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.shangyingyoupin.top/gtzsbyziaq.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.xingfuxueyuan.xyz/gteyrxumer.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.snrcjt.cn/gtyxtydygh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.wangdashe.top/gtknvwgzmx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.gotoacloud.top/gtagivfovm.html

[H03] 主动抛出异常
来源：http://hz.0kj1m.cn/gtrftvwzdq.html

Py:   raise ValueError("错误信息")
来源：http://hz.cqqwz.cn/gtpfycenxp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.smart0.xyz/gtbqtlmvon.html

JS:   throw new Error("错误信息");
来源：http://hz.jinyuanbaomall.cn/gtupcxcbyu.html

TS:   throw new Error("错误信息");
来源：http://hz.gotoacloud.top/gtbwzqvdxi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.tianlin.xyz/gthhwfoflq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.ywan-chungtsiang.top/gtvoacmljx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.tianlin.xyz/gtxtvoezdb.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.dashuyun.cn/gtcchetygh.html

[H04] 自定义异常类型
来源：http://hz.cucudq.cn/gtskqutfrc.html

Py:   class MyError(Exception): pass
来源：http://hz.316326.xyz/gtvvbpeuar.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yvedp.cn/gtibzwqdyn.html

JS:   class MyError extends Error {}
来源：http://hz.xuetiantiany.cn/gtqjjdbqny.html

TS:   class MyError extends Error {}
来源：http://hz.xziqi.cn/gtiablvzkq.html

Java: class MyException extends RuntimeException {}
来源：http://hz.meibo888.top/gtfmgxoydo.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yj202588.top/gtqsbfjybt.html

Ruby: class MyError < StandardError; end
来源：http://hz.sxryk.cn/gttvjkjpwz.html

C#:   class MyException : Exception {}
来源：http://hz.shuidangran.top/gtcqeghfhu.html

[H05] 捕获特定类型
来源：http://hz.gzhubu.top/gtjcwihtzm.html

Py:   except ValueError as e:
来源：http://hz.hywenlv.cn/gtsplemdsi.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.fengsongda.top/gtuultgvhq.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.snrcjt.cn/gtgisqadxg.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhaomingkeji.xyz/gtrhitfzmy.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yj20258.top/gtyvhibgml.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.smart0.xyz/gtoakjrsmu.html

Ruby: rescue ArgumentError => e
来源：http://hz.xziqi.cn/gtanqqeooh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhijiandao.cn/gtgxmurgtz.html

[H06] 可选值 / 空值安全访问
来源：http://hz.xinyue.icu/gtwjyuneyn.html

Py:   value = d.get("k") or default
来源：http://hz.xinyue.icu/gtzjeyglcc.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.nwbrower.top/gtrcxqkzyh.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.dashuyun.cn/gtfczadkad.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jianghu66.top/gtgkblwgzh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jiagoushi.top/gtvjpxjccq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.nwbrower.top/gtskqbwmvc.html

Ruby: d&.dig(:a, :b)
来源：http://hz.hnqzz.top/gtwtbymqud.html

C#:   obj?.A?.B ?? default
来源：http://hz.zhixingplan.top/gtjbdgvrsb.html

[H07] 断言
来源：http://hz.sufxvd.cn/gtosiqemes.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yongpay.top/gtmhmlcqee.html

PHP:  assert($x > 0);
来源：http://hz.ydjk.org.cn/gtuvkxpwmr.html

JS:   console.assert(x > 0);
来源：http://hz.haohaochexian.top/gtiajllpqb.html

TS:   console.assert(x > 0);
来源：http://hz.xuetiantiany.cn/gtddjpwgfb.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jianghu66.top/gtdvmfbkhp.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.tianlin.xyz/gtstygdshc.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hnxiangtu.top/gtlsskwrsv.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zhixingplan.top/gtognkzdfu.html

[H08] 获取错误信息与堆栈
来源：http://hz.yuanzhike.top/gtneykmckq.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zhixingplan.top/gtprtrcxhu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.bjfxy.top/gtylrxdxbb.html

JS:   e.message;  e.stack
来源：http://hz.zhixingplan.top/gtvdqqtams.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.cashguo.top/gtngoaowen.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hnqzz.top/gtxajkemzf.html

Go:   err.Error()
来源：http://hz.ivvv.top/gtpcqjfvrv.html

Ruby: e.message;  e.backtrace
来源：http://hz.mhx1999.top/gtpwggfgsq.html

C#:   e.Message;  e.StackTrace
来源：http://hz.kuanghao11.cn/gtbjxciplm.html

[H09] 带错误码的异常
来源：http://hz.shanyushiyangtech.top/gtybiclwtp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hysaishi.cn/gtilfbklec.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zhiwuduotai.top/gttdouckhh.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yuxming.cn/gtsyxwsopj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yj202588.top/gtxhlnenwr.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.aibaodan.cn/gtftrmlqrr.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yonumen.top/gtybloptyr.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.hfpthk.cn/gtwtvdmrdt.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.gogol.net.cn/gtncxelgcg.html

[H10] 资源自动释放
来源：http://hz.fzhhl.top/gtfkhfivpl.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yongpay.top/gtxdvirdrf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yj202588.top/gtxibcxxfz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cdnleiting.top/gtfjdxiaai.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yj20258.top/gtmqtxdohz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.pengpengdd.cyou/gtipthopdt.html

Go:   defer f.Close()
来源：http://hz.hywenlv.cn/gtwenxfqca.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.fengsongda.top/gtvvgirgcg.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.dianchejie.cn/gtapmjcvaw.html

================================================================================
来源：http://hz.yj20258.top/gtiodvqltj.html

I. 正则表达式
来源：http://hz.0kj1m.cn/gtkmtpldox.html

================================================================================
来源：http://hz.xinyue.icu/gtqmrunqlh.html

[I01] 判断是否匹配
来源：http://hz.9152youxi.cn/gtaznzumow.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.snrcjt.cn/gturvqyepu.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.hysaishi.cn/gtkaoodhdl.html

JS:   /\d+/.test(s)
来源：http://hz.jinqigufen.top/gtfartpjvl.html

TS:   /\d+/.test(s)
来源：http://hz.cqqwz.cn/gtotiphjma.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.tianlin.xyz/gtljiltdnm.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.sxryk.cn/gtjmgvsbst.html

Ruby: s.match?(/\d+/)
来源：http://hz.yanxiufei.cn/gtznzktoay.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zhixingplan.top/gtaymntptp.html


<!-- 参考信息 -->