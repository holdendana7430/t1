代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://hz.fengsongda.top/gtbxkkoeti.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.gogol.net.cn/gtcrfuapyl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.svipenyu.cn/gtjqtxksyt.html

Ruby: File.size("a.txt")
来源：http://hz.zycfv.cn/gtgmbnmqts.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.52xcode.cn/gtaejvkccp.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.tian-w.cn/gtbtzmlqpt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.nanxinkj.top/gtulyyxjhg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.aibaodan.cn/gtqtptrggg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.kuanghao11.cn/gtcxcvswzw.html

TS:   path.extname("a.txt")
来源：http://hz.yangfankeji.com/gtmadnakvt.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yuxming.cn/gtfmbzvvkc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zhixingplan.top/gtboxmbkxv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.tianlin.xyz/gtgaexqzoa.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.tianlin.xyz/gtwdxiuvdn.html

[F11] 复制与移动文件
来源：http://hz.jyoumei.cn/gtqfklcyak.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.shanyushiyangkeji.top/gtazumzfka.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.nanxuanxn.top/gtyjewoijd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jinqigufen.top/gtbtalgwpy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.tanke756.top/gtkgimibcz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.wangdashe.top/gtcdqvtisj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jqgfzy.top/gtvolsrwju.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jqgufenzy.top/gtcvsymour.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yanxiufei.cn/gttajmtunt.html

[F12] CSV 读写
来源：http://hz.ydjk.org.cn/gtrzcobhua.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zdqjudy.top/gtrxyoravo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.xylfe.cn/gthykeuswv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.ydzc1.top/gtjfylehfg.html

TS:   // 同上
来源：http://hz.nanxinkj.top/gtavujrlep.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.hywenlv.cn/gtyrigoqiw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.cheryme.top/gteehxiawy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jqgufenzy.top/gtwepjgedh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.xinyue.icu/gtqgxzomds.html

================================================================================
来源：http://hz.ivvv.top/gtobdciejr.html

G. 面向对象
来源：http://hz.cdnleiting.top/gtjrdjdjea.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtkiagfcnw.html

[G01] 定义类
来源：http://hz.wangdashe.top/gtqwkrdjzb.html

Py:   class User: pass
来源：http://hz.sxryk.cn/gtobbiyhhy.html

PHP:  class User {}
来源：http://hz.cqqwz.cn/gtcplyynpy.html

JS:   class User {}
来源：http://hz.xuetiantiany.cn/gtzpplmizu.html

TS:   class User { name: string = ""; }
来源：http://hz.pycfn.com/gtsuoekruj.html

Java: class User {}
来源：http://hz.jqgfzy.top/gtoocijzpj.html

Go:   type User struct { Name string }
来源：http://hz.aibaodan.cn/gtrxgokzzw.html

Ruby: class User; end
来源：http://hz.chenjidiqi.icu/gthpzlyxvj.html

C#:   class User {}
来源：http://hz.hywenlv.cn/gtfzpfugii.html

[G02] 构造函数
来源：http://hz.meibo888.top/gtiofyzzaj.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.9152youxi.cn/gtwubuphqk.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.dianchejie.cn/gtjigxwnsg.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.guowangkeji.top/gtktyxlrkk.html

TS:   constructor(public name: string) {}
来源：http://hz.yj20258.top/gtdenwsteq.html

Java: User(String name) { this.name = name; }
来源：http://hz.zdqjudy.top/gthoinnayu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.guowangkeji.top/gtclytmpby.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.tian-w.cn/gtfeukseiu.html

C#:   public User(string name) { Name = name; }
来源：http://hz.nanxinkj.top/gtqoqdxrhj.html

[G03] 实例属性
来源：http://hz.bjfxy.top/gtxfybrjom.html

Py:   self.name = "x"
来源：http://hz.guannengcc.top/gtbqtrkhkx.html

PHP:  public string $name = "x";
来源：http://hz.vqdsnc.cn/gthdarbgej.html

JS:   this.name = "x";
来源：http://hz.shangyingyoupin.top/gtyamzttpo.html

TS:   name: string = "x";
来源：http://hz.aibaodan.cn/gtjdpkttkm.html

Java: private String name;
来源：http://hz.yuanzhike.top/gtqksmzzfs.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hysaishi.cn/gtxojkhmao.html

Ruby: @name = "x"
来源：http://hz.yangfankeji.com/gtllqjlilh.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zhoulong.xyz/gtiekeyckg.html

[G04] 定义方法
来源：http://hz.snrcjt.cn/gtvnwzumaq.html

Py:   def greet(self): return self.name
来源：http://hz.yonumen.top/gtevfyqcdv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jlsjyb.cn/gtsmjjgpco.html

JS:   greet() { return this.name; }
来源：http://hz.zycfv.cn/gtyivctihj.html

TS:   greet(): string { return this.name; }
来源：http://hz.chenjidiqi.icu/gtimnpjmfh.html

Java: String greet() { return name; }
来源：http://hz.jiagoushi.top/gtrrxoyogj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.gzhubu.top/gtgrvxzhvk.html

Ruby: def greet; @name; end
来源：http://hz.yueranfly.top/gtlcnswbai.html

C#:   public string Greet() => Name;
来源：http://hz.kuanghao11.cn/gtnwanspoz.html

[G05] 继承
来源：http://hz.fengsongda.top/gtqyzwrhhv.html

Py:   class Admin(User): pass
来源：http://hz.yj20258.top/gtiweqwbqi.html

PHP:  class Admin extends User {}
来源：http://hz.tian-w.cn/gtavytqpmx.html

JS:   class Admin extends User {}
来源：http://hz.ppjwa.cn/gtrciehiai.html

TS:   class Admin extends User {}
来源：http://hz.ppjwa.cn/gthoknslol.html

Java: class Admin extends User {}
来源：http://hz.shanyushiyangkeji.top/gtlbrwjgeb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.gotoacloud.top/gtrdzlvonx.html

Ruby: class Admin < User; end
来源：http://hz.yvedp.cn/gtdcuvbvcn.html

C#:   class Admin : User {}
来源：http://hz.c1oappe.top/gtgyxwoaup.html

[G06] 重写方法
来源：http://hz.sxryk.cn/gtqikwdqnu.html

Py:   def greet(self): return "admin"
来源：http://hz.yangfankeji.com/gtavqmefev.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.nanxuanxn.top/gtrkimgloy.html

JS:   greet() { return "admin"; }
来源：http://hz.jianghu66.top/gttfmkyhkf.html

TS:   greet(): string { return "admin"; }
来源：http://hz.shanyushiyangkeji.top/gtdmcitskl.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.gotoacloud.top/gtiregnhsh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.dianchejie.cn/gtvtqzzxsi.html

Ruby: def greet; "admin"; end
来源：http://hz.ydzc1.top/gtqpguqged.html

C#:   public override string Greet() => "admin";
来源：http://hz.guowangkeji.top/gtehsxtphi.html

[G07] 调用父类方法
来源：http://hz.ppjwa.cn/gtfljzipln.html

Py:   super().greet()
来源：http://hz.hammf.cn/gtedgpzefh.html

PHP:  parent::greet();
来源：http://hz.yuanzhike.top/gtgfuedjwv.html

JS:   super.greet();
来源：http://hz.zhixingplan.top/gtwbdjtjsu.html

TS:   super.greet();
来源：http://hz.svipenyu.cn/gtnizolutl.html

Java: super.greet();
来源：http://hz.cucudq.cn/gtgrvxkkli.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yonumen.top/gtndtqbuue.html

Ruby: super
来源：http://hz.jyoumei.cn/gtkfoaiiqe.html

C#:   base.Greet();
来源：http://hz.gotoacloud.top/gtcpkwiuet.html

[G08] 静态方法与属性
来源：http://hz.yueranfly.top/gtmolcpntq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jianghu66.top/gtcdypsasx.html

PHP:  public static function f() {}
来源：http://hz.vqdsnc.cn/gtfrfsarew.html

JS:   static f() {}
来源：http://hz.jinqigfzy.top/gttbedygsc.html

TS:   static f(): void {}
来源：http://hz.xylfe.cn/gtnvguoggn.html

Java: static void f() {}
来源：http://hz.shanyushiyangkeji.top/gttzhuciap.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yj20258.top/gtjpfwxsjg.html

Ruby: def self.f; end
来源：http://hz.yonumen.top/gtcgrdjwwo.html

C#:   public static void F() {}
来源：http://hz.cucudq.cn/gtboikgskx.html

[G09] 接口 / 抽象类
来源：http://hz.birdmap.top/gtqdpzhosh.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.ivvv.top/gtmocpsjsb.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.xuanzx.com/gtgcgldrzr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.gzhubu.top/gtemonqlgt.html

TS:   interface Shape { area(): number; }
来源：http://hz.cheryme.top/gtukvjgfif.html

Java: interface Shape { double area(); }
来源：http://hz.iojbl.cn/gtwcditotr.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.gogol.net.cn/gtqpcexyiw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.xuanzx.com/gtkqhcicuv.html

C#:   interface IShape { double Area(); }
来源：http://hz.ydjk.org.cn/gtlfevmrqg.html

[G10] 访问控制
来源：http://hz.aibaodan.cn/gttbzlwfmt.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jiagoushi.top/gtoxszszdq.html

PHP:  public / protected / private
来源：http://hz.yueranfly.top/gthuflnraa.html

JS:   #private 字段；其余公开
来源：http://hz.iojbl.cn/gtybkrdyqn.html

TS:   public / protected / private
来源：http://hz.quarkkingdee.top/gtutrwswxd.html

Java: public / protected / private / 默认包级
来源：http://hz.dashuyun.cn/gtxyeqahrg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ybcxt.top/gtqjwsgyap.html

Ruby: public / protected / private
来源：http://hz.cqqwz.cn/gtzfhmlhdv.html

C#:   public / protected / private / internal
来源：http://hz.hnxiangtu.top/gtyxlysyef.html

[G11] getter / setter
来源：http://hz.chenlongwang.top/gtwnsijhyl.html

Py:   @property 与 @x.setter
来源：http://hz.xylfe.cn/gtjeohmyfd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.nwbrower.top/gtfkmvbbcx.html

JS:   get name() { return this._name; }
来源：http://hz.9152youxi.cn/gtdpgbjudc.html

TS:   get name(): string { return this._name; }
来源：http://hz.sufxvd.cn/gtgfwwjkct.html

Java: public String getName() { return name; }
来源：http://hz.dianchejie.cn/gtxddapckf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.havefunace.top/gtuotorckr.html

Ruby: attr_accessor :name
来源：http://hz.chenzaomai.com/gtlznvjdkk.html

C#:   public string Name { get; set; }
来源：http://hz.cheryme.top/gtmmotbisb.html

[G12] 对象转字符串
来源：http://hz.yvedp.cn/gtmtzkbqbv.html

Py:   def __str__(self): return self.name
来源：http://hz.ybcxt.top/gtonuyxxyk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.kuanghao11.cn/gtzcrwdhuy.html

JS:   toString() { return this.name; }
来源：http://hz.fzhhl.top/gteuonpmyn.html

TS:   toString(): string { return this.name; }
来源：http://hz.chenjidiqi.icu/gtqbxvvwzw.html

Java: @Override public String toString() { return name; }
来源：http://hz.zdqjudy.top/gtvqrpjkkl.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.kuanghao11.cn/gtlqqtccwn.html

Ruby: def to_s; @name; end
来源：http://hz.yj20258.top/gtkrrlqbhj.html

C#:   public override string ToString() => Name;
来源：http://hz.havefunace.top/gtcadqbhlw.html

[G13] 判断对象类型
来源：http://hz.svipenyu.cn/gtxfvzjuxj.html

Py:   isinstance(u, User)
来源：http://hz.zhoulong.xyz/gtjbpjjwni.html

PHP:  $u instanceof User
来源：http://hz.tanke756.top/gtixrpttbt.html

JS:   u instanceof User
来源：http://hz.sweek.top/gtzbfvzavb.html

TS:   u instanceof User
来源：http://hz.aizwys.cn/gtakoexluo.html

Java: u instanceof User
来源：http://hz.haohaochexian.top/gtkvtntbhz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.hnqzz.top/gtddkgctap.html

Ruby: u.is_a?(User)
来源：http://hz.birdmap.top/gtyorxmddm.html

C#:   u is User
来源：http://hz.svipenyu.cn/gtngqhjops.html

[G14] 数据类 / record
来源：http://hz.yj20258.top/gtxlevjxdh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jinyuanbaomall.cn/gtamlacebd.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.redwolf501.top/gtjcwedryv.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.c1oappe.top/gtflfnhabw.html

TS:   type User = { name: string; age: number };
来源：http://hz.jlsjyb.cn/gttrsfuwxs.html

Java: record User(String name, int age) {}
来源：http://hz.jqgufenzy.top/gtbyiaghuy.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jyoumei.cn/gtnixkpxph.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.ivvv.top/gtytxakrav.html

C#:   record User(string Name, int Age);
来源：http://hz.tian-w.cn/gtydwjvywb.html

[G15] 枚举
来源：http://hz.aizwys.cn/gtdmvvmujv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.nanxuanxn.top/gtedbvjwdp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.chenjidiqi.icu/gtohzpunwm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.gzhubu.top/gtjapymqpn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yuxming.cn/gtjaseeitb.html

Java: enum Color { RED, GREEN }
来源：http://hz.andypj.xyz/gtbvljpnrj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jinghuilouyu.cn/gtcrqcjvpt.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jyoumei.cn/gtnpbwkxvt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.dianchejie.cn/gtiqioxqxk.html

[G16] 对象转数组 / 字典
来源：http://hz.daxiang520.top/gtfzpukmxp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.tianlin.xyz/gtypxszrpy.html

PHP:  get_object_vars($obj);
来源：http://hz.guannengcc.top/gtojbgqvby.html

JS:   Object.entries(obj)
来源：http://hz.ppjwa.cn/gtkwaouqrg.html

TS:   Object.entries(obj)
来源：http://hz.yonumen.top/gtxelfyltb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.tianlin.xyz/gtaglzdzua.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hysaishi.cn/gtkiivmels.html

Ruby: obj.instance_variables
来源：http://hz.jinqigfzy.top/gttwhcnagm.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.52xcode.cn/gthlrlhzfz.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtttpxingf.html

H. 异常与错误处理
来源：http://hz.yangfankeji.com/gtvmzhbbvr.html

================================================================================
来源：http://hz.haohaochexian.top/gtiopveuel.html

[H01] try / catch 基础
来源：http://hz.hysaishi.cn/gtfvglxqmz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yuanzhike.top/gtvlqktiwk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.smart0.xyz/gtosmjkrai.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.shzxlz.cn/gtutxfqgtb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jlsjyb.cn/gtyobbzyse.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.chenjidiqi.icu/gthufxwrog.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.iojbl.cn/gtqlpommba.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.sufxvd.cn/gtdusovhpd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhiwuduotai.top/gtvjknplmz.html

[H02] finally / ensure 收尾
来源：http://hz.tianlin.xyz/gtgqywsygl.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.redwolf501.top/gtiegyhgwz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xziqi.cn/gthhqlyhgv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.xylfe.cn/gtzmyqpizl.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.tanke756.top/gtlpmlbpzh.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.xinyue.icu/gtxmcotrsg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.nanxuanxn.top/gtsiwamlad.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.guowangkeji.top/gtimlyugvi.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.aibaodan.cn/gtyvnbwibo.html

[H03] 主动抛出异常
来源：http://hz.gzhubu.top/gtnqcvvjzr.html

Py:   raise ValueError("错误信息")
来源：http://hz.52xcode.cn/gtsbojetmy.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.gaohongyu789.top/gtdtztdwtv.html

JS:   throw new Error("错误信息");
来源：http://hz.yj20258888.top/gtqhjbuwhr.html

TS:   throw new Error("错误信息");
来源：http://hz.bjfxy.top/gtwinffbgk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.hammf.cn/gtmxmteyae.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jinqigufen.top/gtaezikuoe.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.sweek.top/gtdiebnlut.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.ivvv.top/gtohakqetz.html

[H04] 自定义异常类型
来源：http://hz.shanyushiyangkeji.top/gtrrchoqhk.html

Py:   class MyError(Exception): pass
来源：http://hz.yanxiufei.cn/gtintwothq.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.xziqi.cn/gtfkjddapb.html

JS:   class MyError extends Error {}
来源：http://hz.shangyingyoupin.top/gtyftwvcrd.html

TS:   class MyError extends Error {}
来源：http://hz.xuanzx.com/gtrrfbnicx.html

Java: class MyException extends RuntimeException {}
来源：http://hz.haohaochexian.top/gtgchoupmk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.nanxinkj.top/gtufyadfge.html

Ruby: class MyError < StandardError; end
来源：http://hz.gaohongyu789.top/gtfctllfvh.html

C#:   class MyException : Exception {}
来源：http://hz.gogol.net.cn/gtdhoptgan.html

[H05] 捕获特定类型
来源：http://hz.jianghu66.top/gtsnfbnvfc.html

Py:   except ValueError as e:
来源：http://hz.zhongyouzk.top/gtrargeoal.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yanxiufei.cn/gtsapnvbsk.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.cucudq.cn/gtrbfwmvsw.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.cheryme.top/gtgouibgqo.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jinqigfzy.top/gteicswszf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.ivvv.top/gtbbtvmidj.html

Ruby: rescue ArgumentError => e
来源：http://hz.yj20258.top/gtikaznejz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.pengpengdd.cyou/gtiowvrqwf.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zycfv.cn/gttatwynuj.html

Py:   value = d.get("k") or default
来源：http://hz.dashuyun.cn/gtspbjenie.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.daria6918.cn/gturxeetke.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.gaohongyu789.top/gtkbiycrjx.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.guowangkeji.top/gthyvokyxa.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.hnxiangtu.top/gtvkxejamo.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.redwolf501.top/gtenrqctpa.html

Ruby: d&.dig(:a, :b)
来源：http://hz.hywenlv.cn/gtfpoicigy.html

C#:   obj?.A?.B ?? default
来源：http://hz.cashguo.top/gttopkidqb.html

[H07] 断言
来源：http://hz.yueranfly.top/gtksexsool.html

Py:   assert x > 0, "必须为正"
来源：http://hz.xuanzx.com/gtxcxufnxv.html

PHP:  assert($x > 0);
来源：http://hz.kuanghao11.cn/gtgkidbbue.html

JS:   console.assert(x > 0);
来源：http://hz.jlsjyb.cn/gtgilzjxcr.html

TS:   console.assert(x > 0);
来源：http://hz.shuidangran.top/gtfvdgkrri.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jinyuanbaomall.cn/gtbniidoqr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jlsjyb.cn/gtxlmvkzrf.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.fengsongda.top/gtnoqmlynv.html

C#:   Debug.Assert(x > 0);
来源：http://hz.chenlongwang.top/gtbccltptj.html

[H08] 获取错误信息与堆栈
来源：http://hz.cqqwz.cn/gtqlesznbo.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.hongshengwenyu.top/gtnxurlwju.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.dashuyun.cn/gtnfwqgkxi.html

JS:   e.message;  e.stack
来源：http://hz.shzxlz.cn/gtgglecasb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yanxiufei.cn/gtbmheqvwp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zycfv.cn/gtogzgutre.html

Go:   err.Error()
来源：http://hz.feifeiyinyue.top/gtetbbirqp.html

Ruby: e.message;  e.backtrace
来源：http://hz.shanyushiyangtech.top/gthydzntqv.html

C#:   e.Message;  e.StackTrace
来源：http://hz.wangdashe.top/gtgrowfpaw.html

[H09] 带错误码的异常
来源：http://hz.dianchejie.cn/gtasknlojz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hnqzz.top/gtjybwnefw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.redwolf501.top/gtypropqcg.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jinghuilouyu.cn/gtuyyzijtb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.ybcxt.top/gtjqwtzuzd.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yuanzhike.top/gtxrkwpxws.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.fzhhl.top/gthotjcuuu.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.svipenyu.cn/gtztgywkje.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yj20258.top/gtjgauzrii.html

[H10] 资源自动释放
来源：http://hz.pengpengdd.cyou/gtjiwwgkth.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.daxiang520.top/gtkdkrbzfm.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jinyuanbaomall.cn/gtaioglfip.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.redwolf501.top/gttxjazhxd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhoulong.xyz/gtkaeyncyl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jlsjyb.cn/gttmmswkiw.html

Go:   defer f.Close()
来源：http://hz.tian-w.cn/gtuostyjyy.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.gotoacloud.top/gthcpsnkim.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.hongshengwenyu.top/gtfdhbrwoa.html

================================================================================
来源：http://hz.zhengqikj.top/gtrkytidax.html

I. 正则表达式
来源：http://hz.yj202588.top/gtbbzcfgrf.html

================================================================================
来源：http://hz.havefunace.top/gtvewbhvgw.html

[I01] 判断是否匹配
来源：http://hz.hnqzz.top/gthkfaxhgz.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jiagoushi.top/gtzhehytsr.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yuanzhike.top/gtvclugaxd.html

JS:   /\d+/.test(s)
来源：http://hz.shzxlz.cn/gtrpnljbdi.html

TS:   /\d+/.test(s)
来源：http://hz.hongshengwenyu.top/gtkidsiqaz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.chenzaomai.com/gtgdbgnymf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.daxiang520.top/gtpxbxznxn.html

Ruby: s.match?(/\d+/)
来源：http://hz.daxiang520.top/gtozizdshz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.xingfuxueyuan.xyz/gtlrvugioi.html

[I02] 提取所有匹配
来源：http://hz.xinyue.icu/gtdxhxneae.html

Py:   re.findall(r"\d+", s)
来源：http://hz.gogol.net.cn/gtnqkzonog.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.ywan-chungtsiang.top/gtjapbrafm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yuxming.cn/gtnisdvdci.html

TS:   s.match(/\d+/g)
来源：http://hz.xuetiantiany.cn/gtzfdkzfpi.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.daria6918.cn/gtomnduonb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.ydjk.org.cn/gtqymkwuhw.html

Ruby: s.scan(/\d+/)
来源：http://hz.iojbl.cn/gtftdbusrh.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.wangdashe.top/gtyvvzcoxp.html

[I03] 提取捕获分组
来源：http://hz.tanke756.top/gtdomyuhyz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yuanzhike.top/gtgbiuegns.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.9152youxi.cn/gthtsogwgi.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.pengpengdd.cyou/gttpelhsxj.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.redwolf501.top/gtdkzgmxwn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhongyouzk.top/gtfmqjsdat.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yongpay.top/gtymgvxfci.html


<!-- 参考信息 -->