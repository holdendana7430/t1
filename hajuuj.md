代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtgsjtmijy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.pengpengdd.cyou/gtyduexfbh.html

[F11] 复制与移动文件
来源：http://hz.jinghuilouyu.cn/gtwugvrlzo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.sweek.top/gtdqgucjhw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jianghu66.top/gtscoetast.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yuanzhike.top/gtualuurlb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ybcxt.top/gtxpwzeflg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.xingfuxueyuan.xyz/gtsbnyromx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.xuetiantiany.cn/gtuqooisln.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jqgfzy.top/gtroeoxjlh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.guannengcc.top/gtzgccench.html

[F12] CSV 读写
来源：http://hz.hywenlv.cn/gtyygtgrmq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.ydjk.org.cn/gtkamqrtdv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.birdmap.top/gthjjovlrv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yj20258888.top/gtvdpvubzt.html

TS:   // 同上
来源：http://hz.jqgfzy.top/gtdhvgqhsv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.daxiang520.top/gtikzlzerk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.tianlin.xyz/gtedwnnuad.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zhixingplan.top/gtlcpsajqu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.gzhubu.top/gtizcfeglj.html

================================================================================
来源：http://hz.tanke756.top/gtppmohuei.html

G. 面向对象
来源：http://hz.mhx1999.top/gttpegasts.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtwgwmwyss.html

[G01] 定义类
来源：http://hz.chenlongwang.top/gtbtswnmil.html

Py:   class User: pass
来源：http://hz.yonumen.top/gtlnvaxsgv.html

PHP:  class User {}
来源：http://hz.feifeiyinyue.top/gtdknrvham.html

JS:   class User {}
来源：http://hz.cqqwz.cn/gtdroccjxj.html

TS:   class User { name: string = ""; }
来源：http://hz.nanxuanxn.top/gtutzhyvqg.html

Java: class User {}
来源：http://hz.dashuyun.cn/gtpauxqlui.html

Go:   type User struct { Name string }
来源：http://hz.sweek.top/gtlixamsjy.html

Ruby: class User; end
来源：http://hz.aibaodan.cn/gtzijbygjk.html

C#:   class User {}
来源：http://hz.tian-w.cn/gtwrtambag.html

[G02] 构造函数
来源：http://hz.nanxuanxn.top/gtyxozuoqy.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.shanyushiyangtech.top/gtjnbqaqel.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ywan-chungtsiang.top/gtaxzoyccf.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.cucudq.cn/gthjlxukok.html

TS:   constructor(public name: string) {}
来源：http://hz.nwbrower.top/gtehmldzqj.html

Java: User(String name) { this.name = name; }
来源：http://hz.gaohongyu789.top/gtntcrcapa.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.nwbrower.top/gtpgkxbsjd.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.zhoulong.xyz/gtsysqzwrd.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jianghu66.top/gttkfejuev.html

[G03] 实例属性
来源：http://hz.jinyuanbaomall.cn/gtwfxnutyj.html

Py:   self.name = "x"
来源：http://hz.jqgufenzy.top/gtxukhjfgx.html

PHP:  public string $name = "x";
来源：http://hz.zdqjudy.top/gtrirdxrbe.html

JS:   this.name = "x";
来源：http://hz.tanke756.top/gtytcmqson.html

TS:   name: string = "x";
来源：http://hz.jlsjyb.cn/gtdkvslxqy.html

Java: private String name;
来源：http://hz.zycfv.cn/gtafbmjxdp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zdqjudy.top/gtvkzsbivl.html

Ruby: @name = "x"
来源：http://hz.bjfxy.top/gtfbwqjbew.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jyoumei.cn/gtzigoecoe.html

[G04] 定义方法
来源：http://hz.nwbrower.top/gtuddblugi.html

Py:   def greet(self): return self.name
来源：http://hz.zycfv.cn/gtqksfbrfa.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hongshengwenyu.top/gtlruhjdhy.html

JS:   greet() { return this.name; }
来源：http://hz.shuidangran.top/gtgqjmcmyd.html

TS:   greet(): string { return this.name; }
来源：http://hz.zhixingplan.top/gtsqajmlwb.html

Java: String greet() { return name; }
来源：http://hz.feifeiyinyue.top/gtogzggnwy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jiagoushi.top/gtxfpkqivq.html

Ruby: def greet; @name; end
来源：http://hz.shangyingyoupin.top/gtzilhtavb.html

C#:   public string Greet() => Name;
来源：http://hz.zhaomingkeji.xyz/gtizswygqx.html

[G05] 继承
来源：http://hz.xziqi.cn/gtyksvypgd.html

Py:   class Admin(User): pass
来源：http://hz.xuetiantiany.cn/gtmjcxgfam.html

PHP:  class Admin extends User {}
来源：http://hz.zhijiandao.cn/gtckupfxql.html

JS:   class Admin extends User {}
来源：http://hz.aizwys.cn/gtslbfmikr.html

TS:   class Admin extends User {}
来源：http://hz.xuanzx.com/gtpyenseui.html

Java: class Admin extends User {}
来源：http://hz.feifeiyinyue.top/gtjajsjysv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.tanke756.top/gtgiyxhkxd.html

Ruby: class Admin < User; end
来源：http://hz.havefunace.top/gtmxyyrovz.html

C#:   class Admin : User {}
来源：http://hz.jiagoushi.top/gtxxafefza.html

[G06] 重写方法
来源：http://hz.chenjidiqi.icu/gtunrdohvu.html

Py:   def greet(self): return "admin"
来源：http://hz.hfpthk.cn/gtidresubo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.hysaishi.cn/gtaoqlqcwr.html

JS:   greet() { return "admin"; }
来源：http://hz.hnxiangtu.top/gtiyictjqw.html

TS:   greet(): string { return "admin"; }
来源：http://hz.tianlin.xyz/gtvhohrspq.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hysaishi.cn/gtvpnwbjxv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhongyouzk.top/gtibilcyep.html

Ruby: def greet; "admin"; end
来源：http://hz.sufxvd.cn/gtqvydqbsx.html

C#:   public override string Greet() => "admin";
来源：http://hz.hywenlv.cn/gttmxchqdq.html

[G07] 调用父类方法
来源：http://hz.sxryk.cn/gtxcetkdav.html

Py:   super().greet()
来源：http://hz.jianghu66.top/gtfbqomfym.html

PHP:  parent::greet();
来源：http://hz.zdqjudy.top/gtsvmjuvhp.html

JS:   super.greet();
来源：http://hz.guannengcc.top/gtbitoclxd.html

TS:   super.greet();
来源：http://hz.zdqjudy.top/gthyipixhb.html

Java: super.greet();
来源：http://hz.hfpthk.cn/gttwrhgusd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.mhx1999.top/gttdflkipr.html

Ruby: super
来源：http://hz.cheryme.top/gtulzjlvgu.html

C#:   base.Greet();
来源：http://hz.gogol.net.cn/gtbcoiwnea.html

[G08] 静态方法与属性
来源：http://hz.cashguo.top/gtukfvgsce.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jinqigufen.top/gtitywitew.html

PHP:  public static function f() {}
来源：http://hz.gaohongyu789.top/gtmewqkqgs.html

JS:   static f() {}
来源：http://hz.cashguo.top/gtxviksvuu.html

TS:   static f(): void {}
来源：http://hz.yanxiufei.cn/gtatgazemc.html

Java: static void f() {}
来源：http://hz.aizwys.cn/gtwrhccjoh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.xuetiantiany.cn/gtuouxtlsz.html

Ruby: def self.f; end
来源：http://hz.hysaishi.cn/gtaobsjied.html

C#:   public static void F() {}
来源：http://hz.zhixingplan.top/gtalfubhgs.html

[G09] 接口 / 抽象类
来源：http://hz.tian-w.cn/gttssplosa.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yueranfly.top/gtgakyqezg.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.hammf.cn/gtnvyfusgo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.0kj1m.cn/gtluoymajq.html

TS:   interface Shape { area(): number; }
来源：http://hz.jyoumei.cn/gtkhvpsuwm.html

Java: interface Shape { double area(); }
来源：http://hz.zhiwuduotai.top/gtypyqhdwx.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.shuidangran.top/gtrbhiphkj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.pycfn.com/gtpoblfnoy.html

C#:   interface IShape { double Area(); }
来源：http://hz.shuidangran.top/gtjvcysfsv.html

[G10] 访问控制
来源：http://hz.shangyingyoupin.top/gtkohxrdim.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jinghuilouyu.cn/gtrxmqdhhj.html

PHP:  public / protected / private
来源：http://hz.sysykeji.top/gtwhgvgtep.html

JS:   #private 字段；其余公开
来源：http://hz.zhoulong.xyz/gtlgdnxwkd.html

TS:   public / protected / private
来源：http://hz.tian-w.cn/gtorqdjevc.html

Java: public / protected / private / 默认包级
来源：http://hz.zdqjudy.top/gtvhyvrvtq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.xylfe.cn/gtndogexdg.html

Ruby: public / protected / private
来源：http://hz.hammf.cn/gtcxoraubp.html

C#:   public / protected / private / internal
来源：http://hz.dashuyun.cn/gtkmcokozd.html

[G11] getter / setter
来源：http://hz.zhongyouzk.top/gtdrkdxrei.html

Py:   @property 与 @x.setter
来源：http://hz.fzhhl.top/gtozqiqgmt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yanxiufei.cn/gtknbxvjnv.html

JS:   get name() { return this._name; }
来源：http://hz.sxryk.cn/gtnmzomioy.html

TS:   get name(): string { return this._name; }
来源：http://hz.0kj1m.cn/gtbifbeocb.html

Java: public String getName() { return name; }
来源：http://hz.yanxiufei.cn/gtzyycmezf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.shanyushiyangtech.top/gtocbbwery.html

Ruby: attr_accessor :name
来源：http://hz.cucudq.cn/gtewrghqnf.html

C#:   public string Name { get; set; }
来源：http://hz.wangshuangyany.cn/gtvvcnwfxm.html

[G12] 对象转字符串
来源：http://hz.yj202588.top/gtomadyppe.html

Py:   def __str__(self): return self.name
来源：http://hz.feifeiyinyue.top/gtiayqitoc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jinyuanbaomall.cn/gtlzetxwfm.html

JS:   toString() { return this.name; }
来源：http://hz.316326.xyz/gtvrumskpz.html

TS:   toString(): string { return this.name; }
来源：http://hz.shangyingyoupin.top/gtoemcbgla.html

Java: @Override public String toString() { return name; }
来源：http://hz.pengpengdd.cyou/gtyigawebs.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.chenzaomai.com/gtigvbjffa.html

Ruby: def to_s; @name; end
来源：http://hz.xinyue.icu/gtmttndpwu.html

C#:   public override string ToString() => Name;
来源：http://hz.gzhubu.top/gtmggxsbxx.html

[G13] 判断对象类型
来源：http://hz.aizwys.cn/gtwryjtqlp.html

Py:   isinstance(u, User)
来源：http://hz.nwbrower.top/gtdgluvazz.html

PHP:  $u instanceof User
来源：http://hz.xuanzx.com/gtmglfaazw.html

JS:   u instanceof User
来源：http://hz.nanxuanxn.top/gtualzogxy.html

TS:   u instanceof User
来源：http://hz.zhaomingkeji.xyz/gtsqbazwbc.html

Java: u instanceof User
来源：http://hz.jinqigfzy.top/gtspgoqxne.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jqgfzy.top/gtqfpbnmhm.html

Ruby: u.is_a?(User)
来源：http://hz.tian-w.cn/gtmurmaivz.html

C#:   u is User
来源：http://hz.zhiwuduotai.top/gtlcoxjhwj.html

[G14] 数据类 / record
来源：http://hz.wangdashe.top/gtupksbegn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yangfankeji.com/gtwmbudoxo.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.birdmap.top/gtquxpwbst.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.sxryk.cn/gtubejpwdc.html

TS:   type User = { name: string; age: number };
来源：http://hz.zycfv.cn/gtlaxkexzf.html

Java: record User(String name, int age) {}
来源：http://hz.chenzaomai.com/gtkzdyqwli.html

Go:   type User struct { Name string; Age int }
来源：http://hz.haohaochexian.top/gtjcmlubha.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.daria6918.cn/gtfwasarid.html

C#:   record User(string Name, int Age);
来源：http://hz.zhaomingkeji.xyz/gtnyvajfri.html

[G15] 枚举
来源：http://hz.yueranfly.top/gttnjotowg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.daxiang520.top/gtxxwvkkco.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.feifeiyinyue.top/gtglzrcjzd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.guannengcc.top/gtqnmpvggg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ydzc1.top/gthjulvrtx.html

Java: enum Color { RED, GREEN }
来源：http://hz.ydzc1.top/gtujacamss.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.dashuyun.cn/gtxfssjjse.html

Ruby: Color = %i[red green].freeze
来源：http://hz.iojbl.cn/gtiukzwgvs.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sxryk.cn/gtimcoeoqg.html

[G16] 对象转数组 / 字典
来源：http://hz.gogol.net.cn/gthnrpsvlw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.0kj1m.cn/gtbsjfpout.html

PHP:  get_object_vars($obj);
来源：http://hz.daxiang520.top/gtndijazru.html

JS:   Object.entries(obj)
来源：http://hz.meibo888.top/gtqtakibqt.html

TS:   Object.entries(obj)
来源：http://hz.pycfn.com/gtwduirtun.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.svipenyu.cn/gtghuyqtwv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.xinyue.icu/gtewfkmxja.html

Ruby: obj.instance_variables
来源：http://hz.yj20258888.top/gtynhxotyd.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.9152youxi.cn/gtbtfhbaxw.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtlerpruiq.html

H. 异常与错误处理
来源：http://hz.cqqwz.cn/gtwsmvadxy.html

================================================================================
来源：http://hz.xuanzx.com/gtjenbbnbl.html

[H01] try / catch 基础
来源：http://hz.52xcode.cn/gtmckivstz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jinghuilouyu.cn/gtuithousx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hammf.cn/gtvwartnfp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.tanke756.top/gtpgtnjmen.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zhaomingkeji.xyz/gtzciybvlb.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.wangshuangyany.cn/gtxkbpnlfe.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.daxiang520.top/gtpdgmttsm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.xuanzx.com/gtpqypizra.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jqgufenzy.top/gthtpudkjg.html

[H02] finally / ensure 收尾
来源：http://hz.gzhubu.top/gtiwccymym.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.chenlongwang.top/gtmuhmlnpg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.tian-w.cn/gtlgsunbtz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hnxiangtu.top/gtdcciaqxp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.cheryme.top/gtxgrkuyow.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.sweek.top/gthihhwiks.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.sufxvd.cn/gtxdcmfcea.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.c1oappe.top/gtvqqdvujc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yj202588.top/gtfgnyeloh.html

[H03] 主动抛出异常
来源：http://hz.tian-w.cn/gtvbtvrnwo.html

Py:   raise ValueError("错误信息")
来源：http://hz.gzhubu.top/gtasmztdzt.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.cheryme.top/gtsecjtknp.html

JS:   throw new Error("错误信息");
来源：http://hz.shangyingyoupin.top/gtrltpywlx.html

TS:   throw new Error("错误信息");
来源：http://hz.shzxlz.cn/gtdfbjqzve.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.xingfuxueyuan.xyz/gtaswnvnxp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhaomingkeji.xyz/gtbeybgbds.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.xingfuxueyuan.xyz/gtglwbmgbr.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.9152youxi.cn/gtpznvsjwb.html

[H04] 自定义异常类型
来源：http://hz.ybcxt.top/gtaswklcgy.html

Py:   class MyError(Exception): pass
来源：http://hz.ydzc1.top/gteopkmofj.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.xinyue.icu/gtwnurdbkq.html

JS:   class MyError extends Error {}
来源：http://hz.jiagoushi.top/gtjdhyvoni.html

TS:   class MyError extends Error {}
来源：http://hz.ybcxt.top/gtsidscvsw.html

Java: class MyException extends RuntimeException {}
来源：http://hz.52xcode.cn/gtudpyxmmw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.tianlin.xyz/gtuiregiww.html

Ruby: class MyError < StandardError; end
来源：http://hz.0kj1m.cn/gtmabuzipw.html

C#:   class MyException : Exception {}
来源：http://hz.redwolf501.top/gtttlegbse.html

[H05] 捕获特定类型
来源：http://hz.nanxinkj.top/gtewoqsaeh.html

Py:   except ValueError as e:
来源：http://hz.zhaomingkeji.xyz/gtpfseqaqo.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.aibaodan.cn/gtmvdoepjq.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yj202588.top/gtsfrsayan.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jinghuilouyu.cn/gttjeqsmmb.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.guannengcc.top/gtbnlwiswx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.0kj1m.cn/gtezpssglt.html

Ruby: rescue ArgumentError => e
来源：http://hz.hysaishi.cn/gtciuollan.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jinyuanbaomall.cn/gtgadlecez.html

[H06] 可选值 / 空值安全访问
来源：http://hz.bjfxy.top/gtupwakwti.html

Py:   value = d.get("k") or default
来源：http://hz.daria6918.cn/gthwybfftd.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yj20258888.top/gthzonepxn.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.hnxiangtu.top/gtzcmqrydp.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yj202588.top/gtrrkiztqg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.cdnleiting.top/gtjqkchgfw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.wangshuangyany.cn/gtprnnkorm.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhoulong.xyz/gtbepcyblx.html

C#:   obj?.A?.B ?? default
来源：http://hz.ehwqpu.com/gtnfkumukn.html

[H07] 断言
来源：http://hz.ydjk.org.cn/gteqwbbvxi.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yongpay.top/gtnatfsmty.html

PHP:  assert($x > 0);
来源：http://hz.fengsongda.top/gtcbumahfk.html

JS:   console.assert(x > 0);
来源：http://hz.ywan-chungtsiang.top/gtuwruwbpv.html

TS:   console.assert(x > 0);
来源：http://hz.ehwqpu.com/gtyvargtes.html

Java: assert x > 0 : "必须为正";
来源：http://hz.gogol.net.cn/gtagdvyjnp.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.sysykeji.top/gtwofndema.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhongyouzk.top/gtfvvanekt.html

C#:   Debug.Assert(x > 0);
来源：http://hz.shangyingyoupin.top/gtkdngsxxv.html

[H08] 获取错误信息与堆栈
来源：http://hz.cucudq.cn/gtrxwpnxho.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jqgufenzy.top/gtqgstrjdj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yangfankeji.com/gtcdmndzkc.html

JS:   e.message;  e.stack
来源：http://hz.zhengqikj.top/gtjucvgbwu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.aibaodan.cn/gthvrrkjsg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.meibo888.top/gtbzyzzwac.html

Go:   err.Error()
来源：http://hz.nwbrower.top/gtmsfumlut.html

Ruby: e.message;  e.backtrace
来源：http://hz.xinyue.icu/gtlfijpfcr.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jyoumei.cn/gtrptrapbc.html

[H09] 带错误码的异常
来源：http://hz.quarkkingdee.top/gtwnoyyqwp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yj20258.top/gtijodxnpl.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ivvv.top/gtvrscxcjp.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zhiwuduotai.top/gtjaplhnic.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.xuanzx.com/gtfrjhhnsc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.chenjidiqi.icu/gttlbpdglq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yonumen.top/gtxmybtoff.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jinqigufen.top/gtthaqspyl.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.sxryk.cn/gtvnlqlhbt.html

[H10] 资源自动释放
来源：http://hz.redwolf501.top/gtadpzvjue.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.fengsongda.top/gturyyngur.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.cheryme.top/gtxcxrbwje.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xylfe.cn/gtgjhakvzd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hywenlv.cn/gtmtvvgntf.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.tanke756.top/gtlntzpatv.html

Go:   defer f.Close()
来源：http://hz.xuetiantiany.cn/gtprdurpgl.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.c1oappe.top/gtyytfptvd.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.aibaodan.cn/gtzyjdbyhu.html

================================================================================
来源：http://hz.guannengcc.top/gtoticlqxg.html

I. 正则表达式
来源：http://hz.hnqzz.top/gtqnscvqxc.html

================================================================================
来源：http://hz.xinyue.icu/gtpxctrysq.html

[I01] 判断是否匹配
来源：http://hz.quarkkingdee.top/gtueibvxei.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zdqjudy.top/gthfwixsuy.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.gogol.net.cn/gtblfpjhpk.html

JS:   /\d+/.test(s)
来源：http://hz.nanxuanxn.top/gtqtndyldm.html

TS:   /\d+/.test(s)
来源：http://hz.birdmap.top/gthvqtisnk.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.aibaodan.cn/gtbtyxsllw.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.pycfn.com/gtfinsoihe.html

Ruby: s.match?(/\d+/)
来源：http://hz.ywan-chungtsiang.top/gtybhiemlk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.ehwqpu.com/gtarzxeymx.html

[I02] 提取所有匹配
来源：http://hz.yuanzhike.top/gtpeqtjafl.html

Py:   re.findall(r"\d+", s)
来源：http://hz.aibaodan.cn/gtgvmgwsky.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zycfv.cn/gtwvkyllix.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.0kj1m.cn/gtbjzuucxr.html

TS:   s.match(/\d+/g)
来源：http://hz.jlsjyb.cn/gtugjuccrr.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.sxryk.cn/gtvywgnxed.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.cqqwz.cn/gtdaoqsdkr.html

Ruby: s.scan(/\d+/)
来源：http://hz.yonumen.top/gtdxhpkqzv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.snrcjt.cn/gtjxcjgcza.html

[I03] 提取捕获分组
来源：http://hz.ydzc1.top/gtuncpxfxp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.mhx1999.top/gthqhfvyhs.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zhengqikj.top/gtspoxljuo.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.xingfuxueyuan.xyz/gtumwsuyvu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.tian-w.cn/gtorppfecp.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.meibo888.top/gtsiloqdlz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.sweek.top/gtkbcpjrri.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jianghu66.top/gtrfnvjdsc.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jianghu66.top/gtbxhrfvvh.html

[I04] 正则替换
来源：http://hz.52xcode.cn/gtwmxxgjaj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.snrcjt.cn/gthndiuxfx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yvedp.cn/gtocbfiikk.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.aizwys.cn/gttsckuftj.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhoulong.xyz/gtslijhlyc.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.smart0.xyz/gtvfwimscm.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.hywenlv.cn/gtvsfzbjyy.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.9152youxi.cn/gtwmnajvso.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.xuetiantiany.cn/gthojhqrrf.html

[I05] 按正则拆分
来源：http://hz.aibaodan.cn/gtyryxatln.html


<!-- 参考信息 -->