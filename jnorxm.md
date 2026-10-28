代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.gotoacloud.top/gtcswinzed.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.shanyushiyangtech.top/gtlsfokguh.html

[F11] 复制与移动文件
来源：http://hz.tianlin.xyz/gtypozuqqk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zhongyouzk.top/gtxyycpdqc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.havefunace.top/gtuqdpudwv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yuxming.cn/gtxhrxwubp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cheryme.top/gtfjbqihwb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zdqjudy.top/gtouzzesef.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.ehwqpu.com/gtbpwolppw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.meibo888.top/gtzeejcldo.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.dianchejie.cn/gtvgemisoh.html

[F12] CSV 读写
来源：http://hz.zdqjudy.top/gtcrogqhet.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.shangyingyoupin.top/gtjiuczjhd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.tianlin.xyz/gtyceubdix.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.316326.xyz/gtwsyhcrhm.html

TS:   // 同上
来源：http://hz.zhiwuduotai.top/gtypezdrvt.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.haohaochexian.top/gtibbyswco.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.xziqi.cn/gtwshoefha.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jqgfzy.top/gtzitzvhcz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yj20258888.top/gtdptbbxsm.html

================================================================================
来源：http://hz.yangfankeji.com/gtfyglupds.html

G. 面向对象
来源：http://hz.zycfv.cn/gtqnhdojai.html

================================================================================
来源：http://hz.cucudq.cn/gtfydcpzta.html

[G01] 定义类
来源：http://hz.dianchejie.cn/gtahoabphu.html

Py:   class User: pass
来源：http://hz.jlsjyb.cn/gtuwrxmfzh.html

PHP:  class User {}
来源：http://hz.yj202588.top/gtfcwffgqn.html

JS:   class User {}
来源：http://hz.hywenlv.cn/gtpzcnxbba.html

TS:   class User { name: string = ""; }
来源：http://hz.guowangkeji.top/gtmuhsgjrc.html

Java: class User {}
来源：http://hz.feifeiyinyue.top/gtlanxsequ.html

Go:   type User struct { Name string }
来源：http://hz.svipenyu.cn/gtvwwjxhsv.html

Ruby: class User; end
来源：http://hz.yonumen.top/gtzjbcejgw.html

C#:   class User {}
来源：http://hz.wangdashe.top/gthvbfdmkz.html

[G02] 构造函数
来源：http://hz.pycfn.com/gtfhwwbzvh.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yj20258888.top/gtaewlkoef.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.aibaodan.cn/gtxhakjzjr.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.sxryk.cn/gtqveiewlq.html

TS:   constructor(public name: string) {}
来源：http://hz.zhongyouzk.top/gtglszqpfh.html

Java: User(String name) { this.name = name; }
来源：http://hz.kuanghao11.cn/gtszofppwi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.sysykeji.top/gtfbkkcepe.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.0kj1m.cn/gtvecywkyx.html

C#:   public User(string name) { Name = name; }
来源：http://hz.guowangkeji.top/gtxvgihqdx.html

[G03] 实例属性
来源：http://hz.shanyushiyangtech.top/gtzpbtvqex.html

Py:   self.name = "x"
来源：http://hz.havefunace.top/gtmihjroqa.html

PHP:  public string $name = "x";
来源：http://hz.vqdsnc.cn/gtdmkwmgry.html

JS:   this.name = "x";
来源：http://hz.cdnleiting.top/gtaqjpjjwj.html

TS:   name: string = "x";
来源：http://hz.pycfn.com/gtmpvyedia.html

Java: private String name;
来源：http://hz.chenlongwang.top/gtwhsekawf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jinyuanbaomall.cn/gtxuyzkioa.html

Ruby: @name = "x"
来源：http://hz.jiagoushi.top/gtkfsjqnqj.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.cashguo.top/gtxmedfukd.html

[G04] 定义方法
来源：http://hz.tianlin.xyz/gttbicsvnx.html

Py:   def greet(self): return self.name
来源：http://hz.hnxiangtu.top/gtrppqrhss.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jqgfzy.top/gtpdkqwuml.html

JS:   greet() { return this.name; }
来源：http://hz.sxryk.cn/gtpazaorga.html

TS:   greet(): string { return this.name; }
来源：http://hz.ybcxt.top/gtzwnjetid.html

Java: String greet() { return name; }
来源：http://hz.smart0.xyz/gtvejbmgkd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hnxiangtu.top/gtsctrmtqr.html

Ruby: def greet; @name; end
来源：http://hz.vqdsnc.cn/gtcjogkunk.html

C#:   public string Greet() => Name;
来源：http://hz.cashguo.top/gtrcusqrtx.html

[G05] 继承
来源：http://hz.zdqjudy.top/gtykmejuyo.html

Py:   class Admin(User): pass
来源：http://hz.shzxlz.cn/gtyzqjkdfn.html

PHP:  class Admin extends User {}
来源：http://hz.hnxiangtu.top/gtifxnjkzj.html

JS:   class Admin extends User {}
来源：http://hz.cheryme.top/gtnawbxxfy.html

TS:   class Admin extends User {}
来源：http://hz.kuanghao11.cn/gtkffkhiyd.html

Java: class Admin extends User {}
来源：http://hz.zhengqikj.top/gttpumpmuu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.cucudq.cn/gtjrfnbdpg.html

Ruby: class Admin < User; end
来源：http://hz.jinqigfzy.top/gtrdbkacif.html

C#:   class Admin : User {}
来源：http://hz.quarkkingdee.top/gttywrqlxn.html

[G06] 重写方法
来源：http://hz.aizwys.cn/gtmzkiwsgm.html

Py:   def greet(self): return "admin"
来源：http://hz.yj20258.top/gtbsbjvgkg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.dashuyun.cn/gtfeoyvddv.html

JS:   greet() { return "admin"; }
来源：http://hz.redwolf501.top/gtxtgtryzi.html

TS:   greet(): string { return "admin"; }
来源：http://hz.kuanghao11.cn/gtpuhemxyk.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jinghuilouyu.cn/gtutnwalnr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhoulong.xyz/gtlzvakpyh.html

Ruby: def greet; "admin"; end
来源：http://hz.zhijiandao.cn/gtudibhinl.html

C#:   public override string Greet() => "admin";
来源：http://hz.shanyushiyangtech.top/gtjevkiiem.html

[G07] 调用父类方法
来源：http://hz.52xcode.cn/gtwiepxrgb.html

Py:   super().greet()
来源：http://hz.yuxming.cn/gthtpqtjqt.html

PHP:  parent::greet();
来源：http://hz.zhaomingkeji.xyz/gtmxbuejoq.html

JS:   super.greet();
来源：http://hz.yuxming.cn/gtwfwamzem.html

TS:   super.greet();
来源：http://hz.gzhubu.top/gtmepccflw.html

Java: super.greet();
来源：http://hz.shangyingyoupin.top/gthaftuegr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yj20258.top/gtckeesirt.html

Ruby: super
来源：http://hz.xuetiantiany.cn/gtocjpajlc.html

C#:   base.Greet();
来源：http://hz.daria6918.cn/gtbqaskhqq.html

[G08] 静态方法与属性
来源：http://hz.daria6918.cn/gtlfbdptda.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jinqigfzy.top/gtzppsqwio.html

PHP:  public static function f() {}
来源：http://hz.wangdashe.top/gtyxbenpsu.html

JS:   static f() {}
来源：http://hz.0kj1m.cn/gtvhkydlny.html

TS:   static f(): void {}
来源：http://hz.316326.xyz/gtxhcageih.html

Java: static void f() {}
来源：http://hz.fzhhl.top/gtjwnuiwed.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.nanxinkj.top/gtgvhgpimm.html

Ruby: def self.f; end
来源：http://hz.yj20258.top/gtgtaicwrn.html

C#:   public static void F() {}
来源：http://hz.wangdashe.top/gtxebrxwis.html

[G09] 接口 / 抽象类
来源：http://hz.ywan-chungtsiang.top/gtflzgkmdz.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.meibo888.top/gttgqvcfis.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.hysaishi.cn/gtoxztavae.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.nanxinkj.top/gtjryzlbbn.html

TS:   interface Shape { area(): number; }
来源：http://hz.9152youxi.cn/gtufgnigyf.html

Java: interface Shape { double area(); }
来源：http://hz.zycfv.cn/gtzxwnatpy.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.feifeiyinyue.top/gtphidpost.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.ydzc1.top/gtjoxbwmjc.html

C#:   interface IShape { double Area(); }
来源：http://hz.c1oappe.top/gtjsyzztlo.html

[G10] 访问控制
来源：http://hz.quarkkingdee.top/gtusazkgfl.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.xuanzx.com/gtxcqkcffo.html

PHP:  public / protected / private
来源：http://hz.andypj.xyz/gtrsacgjjq.html

JS:   #private 字段；其余公开
来源：http://hz.sxryk.cn/gtdcvzjjhg.html

TS:   public / protected / private
来源：http://hz.daria6918.cn/gtxduafjwo.html

Java: public / protected / private / 默认包级
来源：http://hz.cashguo.top/gtbmkyawac.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.iojbl.cn/gtkshpoatu.html

Ruby: public / protected / private
来源：http://hz.jinqigufen.top/gtvitqjcfx.html

C#:   public / protected / private / internal
来源：http://hz.sysykeji.top/gtfgpzirfq.html

[G11] getter / setter
来源：http://hz.52xcode.cn/gtdpknvhbu.html

Py:   @property 与 @x.setter
来源：http://hz.0kj1m.cn/gtfvrmejda.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.hnqzz.top/gtruckmgfq.html

JS:   get name() { return this._name; }
来源：http://hz.daxiang520.top/gtkbphtqzu.html

TS:   get name(): string { return this._name; }
来源：http://hz.birdmap.top/gtntjrhzyi.html

Java: public String getName() { return name; }
来源：http://hz.zhijiandao.cn/gtpdxtidbl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.xinyue.icu/gtomqntzib.html

Ruby: attr_accessor :name
来源：http://hz.redwolf501.top/gtsuffferx.html

C#:   public string Name { get; set; }
来源：http://hz.yuanzhike.top/gtrscifjwf.html

[G12] 对象转字符串
来源：http://hz.xingfuxueyuan.xyz/gtfgzotizn.html

Py:   def __str__(self): return self.name
来源：http://hz.iojbl.cn/gtknjwscnd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.shanyushiyangkeji.top/gtxqsumkpc.html

JS:   toString() { return this.name; }
来源：http://hz.tanke756.top/gtxjlshgkw.html

TS:   toString(): string { return this.name; }
来源：http://hz.sufxvd.cn/gtucazncvt.html

Java: @Override public String toString() { return name; }
来源：http://hz.chenjidiqi.icu/gtfgajvqni.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.iojbl.cn/gtczcwmctg.html

Ruby: def to_s; @name; end
来源：http://hz.svipenyu.cn/gtnkwnusia.html

C#:   public override string ToString() => Name;
来源：http://hz.chenlongwang.top/gtnenyuqbd.html

[G13] 判断对象类型
来源：http://hz.shangyingyoupin.top/gthibkiyoa.html

Py:   isinstance(u, User)
来源：http://hz.fzhhl.top/gtegtxozny.html

PHP:  $u instanceof User
来源：http://hz.52xcode.cn/gtxjvzpcqm.html

JS:   u instanceof User
来源：http://hz.hfpthk.cn/gtgicvjepr.html

TS:   u instanceof User
来源：http://hz.sufxvd.cn/gtpgqowvnm.html

Java: u instanceof User
来源：http://hz.nanxuanxn.top/gtejrwxfgy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.sweek.top/gtiahmziwg.html

Ruby: u.is_a?(User)
来源：http://hz.havefunace.top/gtbwhdkylt.html

C#:   u is User
来源：http://hz.daria6918.cn/gtszlxmpwz.html

[G14] 数据类 / record
来源：http://hz.nanxinkj.top/gtyhzgubov.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.dashuyun.cn/gtrzvdhwce.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.smart0.xyz/gtuzgxlffz.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.ydjk.org.cn/gtxvczssci.html

TS:   type User = { name: string; age: number };
来源：http://hz.pycfn.com/gttusacqbk.html

Java: record User(String name, int age) {}
来源：http://hz.gzhubu.top/gtdtrcozpt.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zycfv.cn/gtghcqrzhj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.meibo888.top/gtoumpjfpa.html

C#:   record User(string Name, int Age);
来源：http://hz.c1oappe.top/gtwpusxcmj.html

[G15] 枚举
来源：http://hz.daria6918.cn/gtzphemdie.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jyoumei.cn/gtpfqxyscu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.sufxvd.cn/gtiqoihasd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.snrcjt.cn/gtnptgrbvl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.haohaochexian.top/gtobnplzui.html

Java: enum Color { RED, GREEN }
来源：http://hz.pengpengdd.cyou/gtpyrtsums.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.9152youxi.cn/gtrpmftzes.html

Ruby: Color = %i[red green].freeze
来源：http://hz.xinyue.icu/gtyfaiuyqj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jiagoushi.top/gtvfrnqyuj.html

[G16] 对象转数组 / 字典
来源：http://hz.andypj.xyz/gtheleaolj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.nanxuanxn.top/gtkkanbzgr.html

PHP:  get_object_vars($obj);
来源：http://hz.cqqwz.cn/gtfgigtdbu.html

JS:   Object.entries(obj)
来源：http://hz.fzhhl.top/gtokxwcfqa.html

TS:   Object.entries(obj)
来源：http://hz.zhijiandao.cn/gtvolntprt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.redwolf501.top/gtsdnvidsi.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.daria6918.cn/gtuteoazxx.html

Ruby: obj.instance_variables
来源：http://hz.hywenlv.cn/gtkpophajk.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.hfpthk.cn/gtkhkoenzw.html

================================================================================
来源：http://hz.yuxming.cn/gtjvnmvazl.html

H. 异常与错误处理
来源：http://hz.tianlin.xyz/gtuuwugxsq.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtifssdfrj.html

[H01] try / catch 基础
来源：http://hz.ivvv.top/gtqognuvjk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.shanyushiyangtech.top/gttwpqquxa.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.gzhubu.top/gttzvthuwm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.nanxinkj.top/gtptplcndy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hongshengwenyu.top/gthavdekzd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.kuanghao11.cn/gtiazjvtrk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.iojbl.cn/gtvivakjxh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.havefunace.top/gthpjyodrs.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.dashuyun.cn/gtxgivzocl.html

[H02] finally / ensure 收尾
来源：http://hz.chenlongwang.top/gtyoevplnm.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.sysykeji.top/gtozwnigho.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.sweek.top/gtylcpjylu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.0kj1m.cn/gtdefvtcxi.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.chenjidiqi.icu/gtayeervxe.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.dashuyun.cn/gtbquvibnj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.nanxuanxn.top/gtqvuqkwdw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.zdqjudy.top/gtfuelmecn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.ydzc1.top/gtmmoerrxu.html

[H03] 主动抛出异常
来源：http://hz.zhijiandao.cn/gtbjhvhkcn.html

Py:   raise ValueError("错误信息")
来源：http://hz.jinyuanbaomall.cn/gtesxhnjum.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.guannengcc.top/gtlxeeexzm.html

JS:   throw new Error("错误信息");
来源：http://hz.sufxvd.cn/gtgerbsdke.html

TS:   throw new Error("错误信息");
来源：http://hz.jqgufenzy.top/gtcdloycbw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.hnqzz.top/gtowfcqllm.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yanxiufei.cn/gtiynnfreg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.xylfe.cn/gtpbxkidro.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.havefunace.top/gtjidntzgn.html

[H04] 自定义异常类型
来源：http://hz.meibo888.top/gtstlpjktv.html

Py:   class MyError(Exception): pass
来源：http://hz.jinqigufen.top/gtoszsxzzf.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.ybcxt.top/gtzfeeldge.html

JS:   class MyError extends Error {}
来源：http://hz.redwolf501.top/gtbfymbgkt.html

TS:   class MyError extends Error {}
来源：http://hz.nanxuanxn.top/gtjxptviux.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zhixingplan.top/gttaanzifx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.cheryme.top/gtowdnytja.html

Ruby: class MyError < StandardError; end
来源：http://hz.bjfxy.top/gtzigguhuh.html

C#:   class MyException : Exception {}
来源：http://hz.cheryme.top/gtarozvzxn.html

[H05] 捕获特定类型
来源：http://hz.yangfankeji.com/gtmzwfbxyt.html

Py:   except ValueError as e:
来源：http://hz.xylfe.cn/gtdkimkbgh.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.cashguo.top/gtzvdljlqn.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jyoumei.cn/gttdbtigqi.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.shangyingyoupin.top/gtlvyiiagt.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.shuidangran.top/gtfbpgsbie.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hongshengwenyu.top/gtmhyiyhru.html

Ruby: rescue ArgumentError => e
来源：http://hz.nanxuanxn.top/gtgtcjhzpf.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.gzhubu.top/gtwbqeatmz.html

[H06] 可选值 / 空值安全访问
来源：http://hz.hnqzz.top/gtcjujaioc.html

Py:   value = d.get("k") or default
来源：http://hz.hywenlv.cn/gtceblntbh.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.cucudq.cn/gteuahhxic.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jlsjyb.cn/gtbeinngpz.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yongpay.top/gtwwzzujji.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ybcxt.top/gtezsascfs.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jyoumei.cn/gtfoodmipd.html

Ruby: d&.dig(:a, :b)
来源：http://hz.gzhubu.top/gtkgsbqmzu.html

C#:   obj?.A?.B ?? default
来源：http://hz.hysaishi.cn/gtanzwczhu.html

[H07] 断言
来源：http://hz.guannengcc.top/gtafnkbjni.html

Py:   assert x > 0, "必须为正"
来源：http://hz.sufxvd.cn/gtvgmnizqe.html

PHP:  assert($x > 0);
来源：http://hz.chenjidiqi.icu/gtozqhdcwm.html

JS:   console.assert(x > 0);
来源：http://hz.hnqzz.top/gtfugpagwd.html

TS:   console.assert(x > 0);
来源：http://hz.yanxiufei.cn/gtsdilgunp.html

Java: assert x > 0 : "必须为正";
来源：http://hz.hammf.cn/gtllzfpybs.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.cucudq.cn/gtbskieaom.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhijiandao.cn/gtwhpogkda.html

C#:   Debug.Assert(x > 0);
来源：http://hz.xylfe.cn/gtylydiune.html

[H08] 获取错误信息与堆栈
来源：http://hz.guannengcc.top/gtgwsdmovf.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ybcxt.top/gtpfcrbvff.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.snrcjt.cn/gtbhcniopw.html

JS:   e.message;  e.stack
来源：http://hz.shzxlz.cn/gtfibtbydi.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.mhx1999.top/gtrlkzqchg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.nanxuanxn.top/gtbliyecju.html

Go:   err.Error()
来源：http://hz.sweek.top/gtseuuewbc.html

Ruby: e.message;  e.backtrace
来源：http://hz.xinyue.icu/gtrtbgsefw.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhengqikj.top/gtlkkusshz.html

[H09] 带错误码的异常
来源：http://hz.yongpay.top/gtrssettit.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hammf.cn/gtfxzlcsif.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.tanke756.top/gtiagnjjnl.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.9152youxi.cn/gtrgjshtkf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.fzhhl.top/gtbqdkedbf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.smart0.xyz/gtmkrockoq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.smart0.xyz/gtexgpjvpp.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.shangyingyoupin.top/gtvcmcptnv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhongyouzk.top/gthvoyiuon.html

[H10] 资源自动释放
来源：http://hz.yueranfly.top/gtaeszodds.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yj20258.top/gtsmewhezl.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.zhoulong.xyz/gtzugupgtv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.tian-w.cn/gttlgrxnmt.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yj202588.top/gtbcbsjlva.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.xuanzx.com/gtuyclowhu.html

Go:   defer f.Close()
来源：http://hz.jianghu66.top/gtdjtbkfrg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.smart0.xyz/gtzybywhca.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.316326.xyz/gtawwqfiew.html

================================================================================
来源：http://hz.chenlongwang.top/gtxvwnnidv.html

I. 正则表达式
来源：http://hz.shuidangran.top/gtmvihwjok.html

================================================================================
来源：http://hz.shuidangran.top/gtcsjtilyb.html

[I01] 判断是否匹配
来源：http://hz.xingfuxueyuan.xyz/gtqejrszkd.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hammf.cn/gtveaotguw.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.ydzc1.top/gtrxwkcwdo.html

JS:   /\d+/.test(s)
来源：http://hz.zycfv.cn/gtjdpjrqbz.html

TS:   /\d+/.test(s)
来源：http://hz.wangshuangyany.cn/gtrmuxenwc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hfpthk.cn/gtjncpxjmn.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.fengsongda.top/gtczhcinns.html

Ruby: s.match?(/\d+/)
来源：http://hz.nwbrower.top/gtpldvkuem.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.nwbrower.top/gthsqqkxlo.html

[I02] 提取所有匹配
来源：http://hz.vqdsnc.cn/gtnxejpitn.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jinqigufen.top/gtqbkloegh.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.svipenyu.cn/gtcfmuzfyu.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jinqigfzy.top/gtrwkujayi.html

TS:   s.match(/\d+/g)
来源：http://hz.sysykeji.top/gtjhuvgxqn.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.xingfuxueyuan.xyz/gtefssjnvb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.tanke756.top/gtlcbxosyc.html

Ruby: s.scan(/\d+/)
来源：http://hz.hnxiangtu.top/gtdiopunos.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yangfankeji.com/gtnpviwxcu.html

[I03] 提取捕获分组
来源：http://hz.jinghuilouyu.cn/gtxqxclgpo.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yuanzhike.top/gtucarekyu.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jinghuilouyu.cn/gtrfusutak.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yonumen.top/gtehdeaaof.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zhixingplan.top/gtucwaokux.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jqgufenzy.top/gttaaetavn.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.xuanzx.com/gtukbpmpmc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.c1oappe.top/gticvespcn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jqgfzy.top/gtdigwqerw.html

[I04] 正则替换
来源：http://hz.chenjidiqi.icu/gtecfyfngw.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.cucudq.cn/gtscfrvbxr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.hongshengwenyu.top/gtbrqftkbt.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yuxming.cn/gtevknaczu.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.xziqi.cn/gttfllvnfy.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.gogol.net.cn/gthmmbyige.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.cdnleiting.top/gtkqadyqks.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.kuanghao11.cn/gtpxbkjdzz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.zhengqikj.top/gtzsggtcaz.html

[I05] 按正则拆分
来源：http://hz.zhongyouzk.top/gtnavtszwk.html


<!-- 参考信息 -->