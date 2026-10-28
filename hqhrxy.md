代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jinghuilouyu.cn/gtpoelgeyk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.shangyingyoupin.top/gtpgodhkri.html

[F11] 复制与移动文件
来源：http://hz.cheryme.top/gtscuhgmar.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.shzxlz.cn/gtxzyxinnh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.shanyushiyangkeji.top/gtyfwbuqxm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.guowangkeji.top/gtbozqfxwh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hysaishi.cn/gtfyuasafb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.tian-w.cn/gthvrecwvl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.feifeiyinyue.top/gtuiveucnz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jqgfzy.top/gtasstuyqo.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.iojbl.cn/gtwaiiqrjf.html

[F12] CSV 读写
来源：http://hz.9152youxi.cn/gtjsteufku.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yj20258888.top/gtlpykmpdh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.sxryk.cn/gtmtmpifro.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.havefunace.top/gtsftlcxml.html

TS:   // 同上
来源：http://hz.zhixingplan.top/gtncstwojj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.pengpengdd.cyou/gtorvdrkgx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.pycfn.com/gtmgwmqxtw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jianghu66.top/gtocbrtruc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.snrcjt.cn/gtkeiiyuzh.html

================================================================================
来源：http://hz.yj20258.top/gtnoudlgaj.html

G. 面向对象
来源：http://hz.chenlongwang.top/gtzcitcbyi.html

================================================================================
来源：http://hz.fengsongda.top/gtatuoudxb.html

[G01] 定义类
来源：http://hz.bjfxy.top/gtmkrhvdac.html

Py:   class User: pass
来源：http://hz.guowangkeji.top/gtcjzyivqr.html

PHP:  class User {}
来源：http://hz.yuanzhike.top/gtlqinfclp.html

JS:   class User {}
来源：http://hz.feifeiyinyue.top/gtddtjalmu.html

TS:   class User { name: string = ""; }
来源：http://hz.cqqwz.cn/gtnbstrgde.html

Java: class User {}
来源：http://hz.cdnleiting.top/gtsodvhbsk.html

Go:   type User struct { Name string }
来源：http://hz.vqdsnc.cn/gtdwwldodb.html

Ruby: class User; end
来源：http://hz.cheryme.top/gttncyiswf.html

C#:   class User {}
来源：http://hz.0kj1m.cn/gtyeaxecdc.html

[G02] 构造函数
来源：http://hz.gaohongyu789.top/gtwvkwkvsq.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.gotoacloud.top/gtzlfexdxj.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.nanxuanxn.top/gtfquakcll.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.cucudq.cn/gtlanadjnx.html

TS:   constructor(public name: string) {}
来源：http://hz.hysaishi.cn/gtpuskrgud.html

Java: User(String name) { this.name = name; }
来源：http://hz.sufxvd.cn/gtfsqufnwj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.wangdashe.top/gtxrmqakjr.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.gaohongyu789.top/gtzoswpdhl.html

C#:   public User(string name) { Name = name; }
来源：http://hz.hywenlv.cn/gthuczzolb.html

[G03] 实例属性
来源：http://hz.guowangkeji.top/gtrhwktwrx.html

Py:   self.name = "x"
来源：http://hz.snrcjt.cn/gtixtmddzo.html

PHP:  public string $name = "x";
来源：http://hz.gotoacloud.top/gterekytiw.html

JS:   this.name = "x";
来源：http://hz.fengsongda.top/gtgazikkse.html

TS:   name: string = "x";
来源：http://hz.gzhubu.top/gtgibbbznt.html

Java: private String name;
来源：http://hz.mhx1999.top/gtdnugrzbl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.9152youxi.cn/gtshobsmea.html

Ruby: @name = "x"
来源：http://hz.hysaishi.cn/gtsosobcys.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.ydjk.org.cn/gtbiraelqo.html

[G04] 定义方法
来源：http://hz.gogol.net.cn/gtrzyrugkm.html

Py:   def greet(self): return self.name
来源：http://hz.birdmap.top/gtplpotfnp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.sweek.top/gtuksdhkbx.html

JS:   greet() { return this.name; }
来源：http://hz.mhx1999.top/gtzcxzznpy.html

TS:   greet(): string { return this.name; }
来源：http://hz.ywan-chungtsiang.top/gtbzfwzzzz.html

Java: String greet() { return name; }
来源：http://hz.hfpthk.cn/gtdugtbwgw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.birdmap.top/gtbkfccdlf.html

Ruby: def greet; @name; end
来源：http://hz.snrcjt.cn/gtztakplva.html

C#:   public string Greet() => Name;
来源：http://hz.yongpay.top/gtqkyypzzq.html

[G05] 继承
来源：http://hz.gotoacloud.top/gtmqtbuehp.html

Py:   class Admin(User): pass
来源：http://hz.hnqzz.top/gtmxbealwc.html

PHP:  class Admin extends User {}
来源：http://hz.guowangkeji.top/gtqhnijzup.html

JS:   class Admin extends User {}
来源：http://hz.yuxming.cn/gtrnhlcenr.html

TS:   class Admin extends User {}
来源：http://hz.0kj1m.cn/gtwnxaktzs.html

Java: class Admin extends User {}
来源：http://hz.chenjidiqi.icu/gtrfkypbwo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.redwolf501.top/gtoquzxmmn.html

Ruby: class Admin < User; end
来源：http://hz.wangshuangyany.cn/gtqibgzcxu.html

C#:   class Admin : User {}
来源：http://hz.yj20258888.top/gtiezqhxnd.html

[G06] 重写方法
来源：http://hz.wangshuangyany.cn/gtqkdqjhel.html

Py:   def greet(self): return "admin"
来源：http://hz.daxiang520.top/gtcbxwhwxg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yj20258888.top/gtxtzbmwhu.html

JS:   greet() { return "admin"; }
来源：http://hz.chenzaomai.com/gtepkttsub.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jinyuanbaomall.cn/gtrublibdx.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yueranfly.top/gtvpypuxzp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.316326.xyz/gtfcwglfdm.html

Ruby: def greet; "admin"; end
来源：http://hz.wangdashe.top/gttvzsrkwl.html

C#:   public override string Greet() => "admin";
来源：http://hz.sufxvd.cn/gtccuqvijp.html

[G07] 调用父类方法
来源：http://hz.cashguo.top/gtfiydbkdl.html

Py:   super().greet()
来源：http://hz.zhengqikj.top/gtkctevufk.html

PHP:  parent::greet();
来源：http://hz.pengpengdd.cyou/gtbcocybjz.html

JS:   super.greet();
来源：http://hz.svipenyu.cn/gtkuyynjum.html

TS:   super.greet();
来源：http://hz.sxryk.cn/gtlxczjqyi.html

Java: super.greet();
来源：http://hz.9152youxi.cn/gtfbsgcetq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.hnxiangtu.top/gtkzdxlcxa.html

Ruby: super
来源：http://hz.sysykeji.top/gtcgovpfrm.html

C#:   base.Greet();
来源：http://hz.jlsjyb.cn/gtzlwknpcs.html

[G08] 静态方法与属性
来源：http://hz.vqdsnc.cn/gtgpegcsxx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.c1oappe.top/gtyhnyvhza.html

PHP:  public static function f() {}
来源：http://hz.havefunace.top/gtzzcwsozm.html

JS:   static f() {}
来源：http://hz.ppjwa.cn/gtqmmtofdd.html

TS:   static f(): void {}
来源：http://hz.nwbrower.top/gttvganvcd.html

Java: static void f() {}
来源：http://hz.haohaochexian.top/gtplsqbbzr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yangfankeji.com/gtnyyhqqzw.html

Ruby: def self.f; end
来源：http://hz.aibaodan.cn/gttgfwbtjv.html

C#:   public static void F() {}
来源：http://hz.shanyushiyangkeji.top/gtduamtmut.html

[G09] 接口 / 抽象类
来源：http://hz.hywenlv.cn/gtdfziwhxg.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.hfpthk.cn/gtlfnvrshy.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jinghuilouyu.cn/gtosvrcges.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yongpay.top/gthxdsmwmz.html

TS:   interface Shape { area(): number; }
来源：http://hz.yonumen.top/gtrudurdck.html

Java: interface Shape { double area(); }
来源：http://hz.hnqzz.top/gtesenhste.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.dianchejie.cn/gtmwmxbofc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.smart0.xyz/gtdefsygnh.html

C#:   interface IShape { double Area(); }
来源：http://hz.svipenyu.cn/gtvcqgprfk.html

[G10] 访问控制
来源：http://hz.shuidangran.top/gtovlmoqop.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.tian-w.cn/gtfozevilw.html

PHP:  public / protected / private
来源：http://hz.fzhhl.top/gthjgveobu.html

JS:   #private 字段；其余公开
来源：http://hz.ybcxt.top/gtngglxodv.html

TS:   public / protected / private
来源：http://hz.pycfn.com/gtqdwobzwq.html

Java: public / protected / private / 默认包级
来源：http://hz.xylfe.cn/gtermlrwdl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yonumen.top/gtmveejben.html

Ruby: public / protected / private
来源：http://hz.yj20258.top/gthekzdzke.html

C#:   public / protected / private / internal
来源：http://hz.jianghu66.top/gtpndyojls.html

[G11] getter / setter
来源：http://hz.cdnleiting.top/gtuzuvbooz.html

Py:   @property 与 @x.setter
来源：http://hz.smart0.xyz/gtdceuxdwv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jqgufenzy.top/gtbuwpmmza.html

JS:   get name() { return this._name; }
来源：http://hz.9152youxi.cn/gtrthzfhtl.html

TS:   get name(): string { return this._name; }
来源：http://hz.sweek.top/gtbeydkwtv.html

Java: public String getName() { return name; }
来源：http://hz.zdqjudy.top/gtxcjdzozm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zhiwuduotai.top/gtoseouzri.html

Ruby: attr_accessor :name
来源：http://hz.yuxming.cn/gtzqwzktxk.html

C#:   public string Name { get; set; }
来源：http://hz.yangfankeji.com/gtdsfpiqba.html

[G12] 对象转字符串
来源：http://hz.yj202588.top/gtsqdxcgds.html

Py:   def __str__(self): return self.name
来源：http://hz.chenjidiqi.icu/gtrredykgt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yvedp.cn/gtzsvxmbhl.html

JS:   toString() { return this.name; }
来源：http://hz.zycfv.cn/gtnpkjrttm.html

TS:   toString(): string { return this.name; }
来源：http://hz.9152youxi.cn/gtbolweycr.html

Java: @Override public String toString() { return name; }
来源：http://hz.jianghu66.top/gtiqdebokb.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yj202588.top/gtdtkfcowd.html

Ruby: def to_s; @name; end
来源：http://hz.aibaodan.cn/gteagbblgq.html

C#:   public override string ToString() => Name;
来源：http://hz.wangshuangyany.cn/gtberwxxiz.html

[G13] 判断对象类型
来源：http://hz.fzhhl.top/gtgmavyhjx.html

Py:   isinstance(u, User)
来源：http://hz.xuanzx.com/gtfszsufln.html

PHP:  $u instanceof User
来源：http://hz.52xcode.cn/gtqqqlrjhj.html

JS:   u instanceof User
来源：http://hz.dianchejie.cn/gtwgmiqmos.html

TS:   u instanceof User
来源：http://hz.jinyuanbaomall.cn/gtycuhmipk.html

Java: u instanceof User
来源：http://hz.vqdsnc.cn/gtaxmgybcp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.aibaodan.cn/gtwyhhvxgs.html

Ruby: u.is_a?(User)
来源：http://hz.nanxinkj.top/gtpwkkhutc.html

C#:   u is User
来源：http://hz.hammf.cn/gtoiihelje.html

[G14] 数据类 / record
来源：http://hz.9152youxi.cn/gtcalfrvqi.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.hysaishi.cn/gtrjcfosmb.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.meibo888.top/gtpxmdltzm.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jqgufenzy.top/gtlkdemfxx.html

TS:   type User = { name: string; age: number };
来源：http://hz.havefunace.top/gtcfcgzqsg.html

Java: record User(String name, int age) {}
来源：http://hz.jqgfzy.top/gtlaswxmjc.html

Go:   type User struct { Name string; Age int }
来源：http://hz.hnxiangtu.top/gtnouqheyf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.pengpengdd.cyou/gtzryixzfw.html

C#:   record User(string Name, int Age);
来源：http://hz.hywenlv.cn/gtuaapaouc.html

[G15] 枚举
来源：http://hz.hfpthk.cn/gtpviakwlv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.cucudq.cn/gtaibfkocb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ivvv.top/gtvqcjqtwh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yj20258888.top/gttdrkdpac.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hnxiangtu.top/gtibeehoqc.html

Java: enum Color { RED, GREEN }
来源：http://hz.yvedp.cn/gtyczbuhiw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ivvv.top/gtvuwmcjrn.html

Ruby: Color = %i[red green].freeze
来源：http://hz.52xcode.cn/gtmswmoydh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ppjwa.cn/gtcfrpmwdu.html

[G16] 对象转数组 / 字典
来源：http://hz.c1oappe.top/gtxppownmr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.iojbl.cn/gtfnbomhec.html

PHP:  get_object_vars($obj);
来源：http://hz.yj202588.top/gtzjgsocwe.html

JS:   Object.entries(obj)
来源：http://hz.jqgufenzy.top/gtewbnapjb.html

TS:   Object.entries(obj)
来源：http://hz.smart0.xyz/gtnjtlwefs.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.redwolf501.top/gtadtrvhhp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.chenzaomai.com/gtjeepyguj.html

Ruby: obj.instance_variables
来源：http://hz.smart0.xyz/gtojshtjwv.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.gotoacloud.top/gtftlyjflg.html

================================================================================
来源：http://hz.jlsjyb.cn/gtvfbzvaum.html

H. 异常与错误处理
来源：http://hz.hywenlv.cn/gtqsivzvsx.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtqwluvgqy.html

[H01] try / catch 基础
来源：http://hz.zdqjudy.top/gttnaxbtag.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.gotoacloud.top/gtywbthibo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.cqqwz.cn/gtokxhspwq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.birdmap.top/gtfcdnbhvl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.nwbrower.top/gtwifymlmx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.cdnleiting.top/gtqaiiucfc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.ivvv.top/gtwedwpoim.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.zhongyouzk.top/gtnxiartif.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.aizwys.cn/gtxjvxmmly.html

[H02] finally / ensure 收尾
来源：http://hz.aibaodan.cn/gtudnbdfci.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.birdmap.top/gtjsazygvc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.gzhubu.top/gtwcqqyxuk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.nwbrower.top/gthsnhkpok.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.cdnleiting.top/gtaylgfwxy.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hnxiangtu.top/gtagpqqshx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.guowangkeji.top/gtqbdkypxu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.aizwys.cn/gtrejeirtr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yj20258.top/gtweopdpuq.html

[H03] 主动抛出异常
来源：http://hz.shangyingyoupin.top/gtahupdvnz.html

Py:   raise ValueError("错误信息")
来源：http://hz.nanxinkj.top/gtnuicplqm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jqgufenzy.top/gtbxlvbkpt.html

JS:   throw new Error("错误信息");
来源：http://hz.wangshuangyany.cn/gtlrpuzfeq.html

TS:   throw new Error("错误信息");
来源：http://hz.aizwys.cn/gtesjdbvyd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.tian-w.cn/gtusifzuat.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yangfankeji.com/gtfanyvxkw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.wangshuangyany.cn/gtnuhgvwdd.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.nanxuanxn.top/gtfnjheqml.html

[H04] 自定义异常类型
来源：http://hz.svipenyu.cn/gtmzberpxk.html

Py:   class MyError(Exception): pass
来源：http://hz.dianchejie.cn/gtcfkqwqvo.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zhixingplan.top/gthqefqyez.html

JS:   class MyError extends Error {}
来源：http://hz.andypj.xyz/gtqsigxfqb.html

TS:   class MyError extends Error {}
来源：http://hz.ehwqpu.com/gtsrjwpkyo.html

Java: class MyException extends RuntimeException {}
来源：http://hz.316326.xyz/gtaicmvkak.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.xuetiantiany.cn/gtagqliutr.html

Ruby: class MyError < StandardError; end
来源：http://hz.bjfxy.top/gtybzrduez.html

C#:   class MyException : Exception {}
来源：http://hz.pycfn.com/gtugjcpaar.html

[H05] 捕获特定类型
来源：http://hz.birdmap.top/gttpzikuzc.html

Py:   except ValueError as e:
来源：http://hz.xuanzx.com/gtppiexnar.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.cashguo.top/gtmhdipswp.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.shuidangran.top/gtkshcxztf.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.hywenlv.cn/gtnokliysh.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.gaohongyu789.top/gtighulawy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jqgufenzy.top/gtcguuwjlq.html

Ruby: rescue ArgumentError => e
来源：http://hz.tanke756.top/gtqtfunnse.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.sufxvd.cn/gtekjqtrab.html

[H06] 可选值 / 空值安全访问
来源：http://hz.dianchejie.cn/gtpnhfsknj.html

Py:   value = d.get("k") or default
来源：http://hz.ehwqpu.com/gttznentjf.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hfpthk.cn/gtzrflpxsk.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yvedp.cn/gtqpgsxxth.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.birdmap.top/gtgdyyezyz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ppjwa.cn/gtejyepjdg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.cdnleiting.top/gtqajieqhr.html

Ruby: d&.dig(:a, :b)
来源：http://hz.aizwys.cn/gtyhqkbtvh.html

C#:   obj?.A?.B ?? default
来源：http://hz.dianchejie.cn/gtyfvpgffx.html

[H07] 断言
来源：http://hz.cashguo.top/gtrariuqpx.html

Py:   assert x > 0, "必须为正"
来源：http://hz.52xcode.cn/gtmtwnppmw.html

PHP:  assert($x > 0);
来源：http://hz.316326.xyz/gtpbxcicoe.html

JS:   console.assert(x > 0);
来源：http://hz.gzhubu.top/gtmigcsuxs.html

TS:   console.assert(x > 0);
来源：http://hz.chenjidiqi.icu/gtpytzyltj.html

Java: assert x > 0 : "必须为正";
来源：http://hz.xingfuxueyuan.xyz/gtiaodkpwe.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.hysaishi.cn/gtsdwoawtf.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.c1oappe.top/gtplsghzpd.html

C#:   Debug.Assert(x > 0);
来源：http://hz.gzhubu.top/gtbhzclqcg.html

[H08] 获取错误信息与堆栈
来源：http://hz.aibaodan.cn/gtjjzfsgql.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.kuanghao11.cn/gtuthmyzjd.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.aizwys.cn/gthvedsgin.html

JS:   e.message;  e.stack
来源：http://hz.yj20258888.top/gtpphcfspm.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jqgfzy.top/gtkjytusmn.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhiwuduotai.top/gtiwnvidpk.html

Go:   err.Error()
来源：http://hz.xylfe.cn/gtxilulzqq.html

Ruby: e.message;  e.backtrace
来源：http://hz.zycfv.cn/gtoliglkqx.html

C#:   e.Message;  e.StackTrace
来源：http://hz.mhx1999.top/gtkthscrow.html

[H09] 带错误码的异常
来源：http://hz.gaohongyu789.top/gtrjpovgwm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.xuetiantiany.cn/gtlvsmvtto.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yj20258.top/gtiqsxkmyx.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.mhx1999.top/gtcgfgovqu.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.hywenlv.cn/gtekaqsehy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zhijiandao.cn/gtlwauxmey.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zhixingplan.top/gtrcepnrbn.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jinqigufen.top/gtsklbqaec.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.kuanghao11.cn/gtzzzdsypu.html

[H10] 资源自动释放
来源：http://hz.sufxvd.cn/gtfpbyviht.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yj20258888.top/gtiyqgfmjc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jianghu66.top/gtkpvdnzdm.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yj20258888.top/gtkrzcfpwp.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hammf.cn/gtrntvjori.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.daria6918.cn/gtwtovjnlf.html

Go:   defer f.Close()
来源：http://hz.sweek.top/gtbkcntjoc.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jqgufenzy.top/gtjgvpnrav.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.shanyushiyangkeji.top/gtkoesljvu.html

================================================================================
来源：http://hz.nanxuanxn.top/gtgrwqibdr.html

I. 正则表达式
来源：http://hz.c1oappe.top/gthaurfpme.html

================================================================================
来源：http://hz.zhixingplan.top/gtjldbcelk.html

[I01] 判断是否匹配
来源：http://hz.xuetiantiany.cn/gtelcthreu.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.cdnleiting.top/gtjwhirmqu.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zhoulong.xyz/gttupxgmaa.html

JS:   /\d+/.test(s)
来源：http://hz.hammf.cn/gtpfnhfsmm.html

TS:   /\d+/.test(s)
来源：http://hz.zhijiandao.cn/gtinanfgbt.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.dashuyun.cn/gttmklvyxh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.gogol.net.cn/gtdufyztyc.html

Ruby: s.match?(/\d+/)
来源：http://hz.dianchejie.cn/gtnborllrk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.quarkkingdee.top/gtzeflhmqf.html

[I02] 提取所有匹配
来源：http://hz.yvedp.cn/gtqhjunaed.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ywan-chungtsiang.top/gtoghdxiov.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.guowangkeji.top/gtjubzawxj.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yangfankeji.com/gtvofusqrl.html

TS:   s.match(/\d+/g)
来源：http://hz.jinyuanbaomall.cn/gtomymgbqq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hammf.cn/gttljiicrf.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.xuetiantiany.cn/gtdxpzsjeu.html

Ruby: s.scan(/\d+/)
来源：http://hz.jqgufenzy.top/gtcqbjvide.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yj20258.top/gtnyuddalj.html

[I03] 提取捕获分组
来源：http://hz.ehwqpu.com/gtwqvjjhfu.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.wangdashe.top/gtclekycku.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yuxming.cn/gtovsihryn.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.iojbl.cn/gtsumrvbmc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jianghu66.top/gtxexdxmgf.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.gotoacloud.top/gtkyiucylc.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.cqqwz.cn/gtigsaltun.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.nanxinkj.top/gtyhkdpehc.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.sweek.top/gtidozrrqa.html

[I04] 正则替换
来源：http://hz.zycfv.cn/gtvbikisbu.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.tanke756.top/gtprmbjoyo.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.gzhubu.top/gtkzukmnks.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.snrcjt.cn/gtjrmwrvtv.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.aizwys.cn/gtytpuzvvs.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.shanyushiyangtech.top/gtnnrlcviy.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zhoulong.xyz/gtwasyiasn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.daxiang520.top/gtopjcgibl.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.sysykeji.top/gtaowqopmx.html

[I05] 按正则拆分
来源：http://hz.xuetiantiany.cn/gtpehyndjp.html


<!-- 参考信息 -->