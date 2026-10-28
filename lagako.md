代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhongyouzk.top/gtrnbnsphm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jyoumei.cn/gtxtaikolj.html

[F11] 复制与移动文件
来源：http://hz.snrcjt.cn/gtfvulehcu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.tianlin.xyz/gtbgzauwny.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.xinyue.icu/gtoqfrasfc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.gaohongyu789.top/gtlhxnmoyn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.gzhubu.top/gtknyrjdyz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.guowangkeji.top/gtlhxymnvt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.hfpthk.cn/gtbbumhlsz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.chenlongwang.top/gtvxltrqix.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhaomingkeji.xyz/gtpckezkhr.html

[F12] CSV 读写
来源：http://hz.jinyuanbaomall.cn/gtjwflnauc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.meibo888.top/gtpzuvobmp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.ybcxt.top/gtdrjbvazz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.aibaodan.cn/gtfyijyqti.html

TS:   // 同上
来源：http://hz.pengpengdd.cyou/gtrtrqhgou.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.guannengcc.top/gthcupvqnz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhoulong.xyz/gtkmuyorkl.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.mhx1999.top/gtddcvpmiy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.hywenlv.cn/gtgohlvipw.html

================================================================================
来源：http://hz.xuetiantiany.cn/gttbowbzcs.html

G. 面向对象
来源：http://hz.ydzc1.top/gtgkhzpqgr.html

================================================================================
来源：http://hz.cucudq.cn/gtrnxgxyrv.html

[G01] 定义类
来源：http://hz.c1oappe.top/gtzuwbwdez.html

Py:   class User: pass
来源：http://hz.yj20258.top/gtxbuyexzq.html

PHP:  class User {}
来源：http://hz.birdmap.top/gtzmrbxkof.html

JS:   class User {}
来源：http://hz.hnqzz.top/gtfixwnidy.html

TS:   class User { name: string = ""; }
来源：http://hz.yj20258.top/gtuwsxajbw.html

Java: class User {}
来源：http://hz.zhiwuduotai.top/gtetiyxksr.html

Go:   type User struct { Name string }
来源：http://hz.wangshuangyany.cn/gtgpuffjqs.html

Ruby: class User; end
来源：http://hz.shuidangran.top/gtcekkmpmp.html

C#:   class User {}
来源：http://hz.gotoacloud.top/gtchgmjdmb.html

[G02] 构造函数
来源：http://hz.xinyue.icu/gtbvhybbhy.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.sufxvd.cn/gtyhxuvkqj.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zycfv.cn/gthfgdgqud.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.xylfe.cn/gtqzdrtohv.html

TS:   constructor(public name: string) {}
来源：http://hz.dianchejie.cn/gtcjpyffqh.html

Java: User(String name) { this.name = name; }
来源：http://hz.mhx1999.top/gtannjwvus.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.wangdashe.top/gtljgswprx.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.tanke756.top/gtatqbosqn.html

C#:   public User(string name) { Name = name; }
来源：http://hz.pengpengdd.cyou/gtoprduzko.html

[G03] 实例属性
来源：http://hz.wangdashe.top/gtvnkosklq.html

Py:   self.name = "x"
来源：http://hz.nanxinkj.top/gtylckqtvi.html

PHP:  public string $name = "x";
来源：http://hz.hnqzz.top/gtirbwyayi.html

JS:   this.name = "x";
来源：http://hz.xinyue.icu/gtiqvbmlii.html

TS:   name: string = "x";
来源：http://hz.hysaishi.cn/gtvsswoalg.html

Java: private String name;
来源：http://hz.ydjk.org.cn/gtrefqmhas.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.nanxinkj.top/gtnekmulek.html

Ruby: @name = "x"
来源：http://hz.svipenyu.cn/gtvwtaovmp.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zhaomingkeji.xyz/gtksljapfu.html

[G04] 定义方法
来源：http://hz.ywan-chungtsiang.top/gtlormwsiw.html

Py:   def greet(self): return self.name
来源：http://hz.yvedp.cn/gtxrykcufo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jqgfzy.top/gtkwicklcn.html

JS:   greet() { return this.name; }
来源：http://hz.cucudq.cn/gtwypmciel.html

TS:   greet(): string { return this.name; }
来源：http://hz.ydzc1.top/gtcmjraowt.html

Java: String greet() { return name; }
来源：http://hz.hnqzz.top/gtbudvyvfq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.smart0.xyz/gtpehgcooy.html

Ruby: def greet; @name; end
来源：http://hz.hongshengwenyu.top/gtyuwhfgie.html

C#:   public string Greet() => Name;
来源：http://hz.pengpengdd.cyou/gtfzxqifjo.html

[G05] 继承
来源：http://hz.zhengqikj.top/gtxnqywzxm.html

Py:   class Admin(User): pass
来源：http://hz.tian-w.cn/gtonshgmyn.html

PHP:  class Admin extends User {}
来源：http://hz.wangdashe.top/gtxgkofqzf.html

JS:   class Admin extends User {}
来源：http://hz.jinghuilouyu.cn/gtifflkrua.html

TS:   class Admin extends User {}
来源：http://hz.zdqjudy.top/gtnsnagrnn.html

Java: class Admin extends User {}
来源：http://hz.zhixingplan.top/gtznqcawwn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hfpthk.cn/gtroeqisgn.html

Ruby: class Admin < User; end
来源：http://hz.jyoumei.cn/gtnwnpmmyk.html

C#:   class Admin : User {}
来源：http://hz.yongpay.top/gtgimbisnc.html

[G06] 重写方法
来源：http://hz.jyoumei.cn/gtyxsirnik.html

Py:   def greet(self): return "admin"
来源：http://hz.jinghuilouyu.cn/gtpecvstfn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.sweek.top/gtxcekowxq.html

JS:   greet() { return "admin"; }
来源：http://hz.ppjwa.cn/gtcukbwjpm.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jianghu66.top/gtqpxccjsp.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.quarkkingdee.top/gtzsuwthqb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yj20258.top/gtgtlstdgu.html

Ruby: def greet; "admin"; end
来源：http://hz.dashuyun.cn/gtchgwjogc.html

C#:   public override string Greet() => "admin";
来源：http://hz.0kj1m.cn/gtzmlvitmp.html

[G07] 调用父类方法
来源：http://hz.ybcxt.top/gtaghgiutk.html

Py:   super().greet()
来源：http://hz.aizwys.cn/gtsbgscjde.html

PHP:  parent::greet();
来源：http://hz.meibo888.top/gtdpkodxxl.html

JS:   super.greet();
来源：http://hz.hammf.cn/gtzonlptyl.html

TS:   super.greet();
来源：http://hz.havefunace.top/gtdvjzknfn.html

Java: super.greet();
来源：http://hz.jinghuilouyu.cn/gttdhkcgtg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.snrcjt.cn/gtylfwwlrp.html

Ruby: super
来源：http://hz.hnqzz.top/gtrwowxovc.html

C#:   base.Greet();
来源：http://hz.shzxlz.cn/gtmpyepohl.html

[G08] 静态方法与属性
来源：http://hz.hfpthk.cn/gtuqhnyxsr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yuxming.cn/gtbyhkmooe.html

PHP:  public static function f() {}
来源：http://hz.dashuyun.cn/gtolvosouo.html

JS:   static f() {}
来源：http://hz.yangfankeji.com/gtkcnrhxkv.html

TS:   static f(): void {}
来源：http://hz.wangshuangyany.cn/gtkcadbwsp.html

Java: static void f() {}
来源：http://hz.gotoacloud.top/gtoqzaqflc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yuxming.cn/gtorbqgmeh.html

Ruby: def self.f; end
来源：http://hz.xuanzx.com/gtqxkdmipz.html

C#:   public static void F() {}
来源：http://hz.zhaomingkeji.xyz/gtzscsvqco.html

[G09] 接口 / 抽象类
来源：http://hz.chenzaomai.com/gtjgsvqpjc.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yuxming.cn/gtqekssqkw.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.0kj1m.cn/gtlivnhjwk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.shzxlz.cn/gtlsqccoxg.html

TS:   interface Shape { area(): number; }
来源：http://hz.ywan-chungtsiang.top/gtkavfqhdi.html

Java: interface Shape { double area(); }
来源：http://hz.chenlongwang.top/gtwortwidh.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.ivvv.top/gtwnjhgagz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.nanxuanxn.top/gtjowcgzve.html

C#:   interface IShape { double Area(); }
来源：http://hz.jinghuilouyu.cn/gtutpkgixd.html

[G10] 访问控制
来源：http://hz.andypj.xyz/gtwyvkubwb.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.tanke756.top/gtrnqdmgjs.html

PHP:  public / protected / private
来源：http://hz.316326.xyz/gtnreimiki.html

JS:   #private 字段；其余公开
来源：http://hz.yonumen.top/gtlhmxrwdi.html

TS:   public / protected / private
来源：http://hz.yuxming.cn/gtydjjexcx.html

Java: public / protected / private / 默认包级
来源：http://hz.zhaomingkeji.xyz/gtfqpokifm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.shanyushiyangtech.top/gtqhjnrqvu.html

Ruby: public / protected / private
来源：http://hz.mhx1999.top/gtxegvywce.html

C#:   public / protected / private / internal
来源：http://hz.kuanghao11.cn/gtlcewklyv.html

[G11] getter / setter
来源：http://hz.jyoumei.cn/gtwderyjxs.html

Py:   @property 与 @x.setter
来源：http://hz.zhiwuduotai.top/gttpqvilyk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.kuanghao11.cn/gtfyccdqwq.html

JS:   get name() { return this._name; }
来源：http://hz.aibaodan.cn/gtcqridsbv.html

TS:   get name(): string { return this._name; }
来源：http://hz.hysaishi.cn/gtfsvzffkb.html

Java: public String getName() { return name; }
来源：http://hz.ppjwa.cn/gtbybafzgs.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.tian-w.cn/gtweiowqap.html

Ruby: attr_accessor :name
来源：http://hz.yongpay.top/gtxkkkywmd.html

C#:   public string Name { get; set; }
来源：http://hz.dianchejie.cn/gtcygbsevi.html

[G12] 对象转字符串
来源：http://hz.shuidangran.top/gthcdfwkcq.html

Py:   def __str__(self): return self.name
来源：http://hz.chenzaomai.com/gtqrsubrao.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zycfv.cn/gtbtahcmlv.html

JS:   toString() { return this.name; }
来源：http://hz.fengsongda.top/gtllmefivc.html

TS:   toString(): string { return this.name; }
来源：http://hz.gotoacloud.top/gtyskjubeq.html

Java: @Override public String toString() { return name; }
来源：http://hz.jqgfzy.top/gtthrznrzn.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.sxryk.cn/gtajnsgbxa.html

Ruby: def to_s; @name; end
来源：http://hz.sweek.top/gtrdsmossk.html

C#:   public override string ToString() => Name;
来源：http://hz.jqgufenzy.top/gtvpnydqvs.html

[G13] 判断对象类型
来源：http://hz.zhiwuduotai.top/gtzeqomcki.html

Py:   isinstance(u, User)
来源：http://hz.gogol.net.cn/gtefxezgmt.html

PHP:  $u instanceof User
来源：http://hz.jinqigfzy.top/gtadmhcagi.html

JS:   u instanceof User
来源：http://hz.nanxuanxn.top/gtfeiuwfer.html

TS:   u instanceof User
来源：http://hz.fengsongda.top/gtnpoolzvz.html

Java: u instanceof User
来源：http://hz.yvedp.cn/gtyjuscxez.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.sufxvd.cn/gtcnlfjojc.html

Ruby: u.is_a?(User)
来源：http://hz.zycfv.cn/gtuzackyxs.html

C#:   u is User
来源：http://hz.jinyuanbaomall.cn/gtscqfdxzv.html

[G14] 数据类 / record
来源：http://hz.snrcjt.cn/gtiqzdeblv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.cucudq.cn/gtoeymarif.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zdqjudy.top/gtawhndrgr.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.vqdsnc.cn/gtwamzsjpu.html

TS:   type User = { name: string; age: number };
来源：http://hz.vqdsnc.cn/gtfgngqwyx.html

Java: record User(String name, int age) {}
来源：http://hz.fzhhl.top/gtpgsadroi.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zhoulong.xyz/gtqdurzzlw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.9152youxi.cn/gtmjkismbi.html

C#:   record User(string Name, int Age);
来源：http://hz.fzhhl.top/gtxickbnct.html

[G15] 枚举
来源：http://hz.mhx1999.top/gtbucpkqev.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.daria6918.cn/gtylvunxzg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ppjwa.cn/gtezdeyrrh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.xuanzx.com/gtzykacnkx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.guannengcc.top/gtjwwzxcno.html

Java: enum Color { RED, GREEN }
来源：http://hz.shanyushiyangtech.top/gtlpiuxsit.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.nwbrower.top/gtsphzpyih.html

Ruby: Color = %i[red green].freeze
来源：http://hz.havefunace.top/gtykhlyfeu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.aizwys.cn/gtzszdrqdn.html

[G16] 对象转数组 / 字典
来源：http://hz.yj20258888.top/gtksstsyhj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.andypj.xyz/gtctdryrqt.html

PHP:  get_object_vars($obj);
来源：http://hz.yuxming.cn/gtvnalsicy.html

JS:   Object.entries(obj)
来源：http://hz.zhijiandao.cn/gtzqbonhsg.html

TS:   Object.entries(obj)
来源：http://hz.daxiang520.top/gtecdavqnu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hnqzz.top/gtsfcyrbke.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hfpthk.cn/gtzqhkxwoc.html

Ruby: obj.instance_variables
来源：http://hz.wangshuangyany.cn/gtyqiygpxu.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.ydzc1.top/gtjrydhybu.html

================================================================================
来源：http://hz.cashguo.top/gtjtamodgd.html

H. 异常与错误处理
来源：http://hz.xziqi.cn/gteknmyazt.html

================================================================================
来源：http://hz.tanke756.top/gtmkhkznbr.html

[H01] try / catch 基础
来源：http://hz.yanxiufei.cn/gtgwyzkicy.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.nwbrower.top/gtmtnpttxu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.dashuyun.cn/gtwciubwuw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zhiwuduotai.top/gtvrogjqlo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.aizwys.cn/gtvvvlexzs.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.hywenlv.cn/gtfsbusjrc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.hnxiangtu.top/gtgtqbgbpq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jinyuanbaomall.cn/gtfnviapbw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.316326.xyz/gtoenjiklt.html

[H02] finally / ensure 收尾
来源：http://hz.pycfn.com/gtilxorzpr.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.shangyingyoupin.top/gtruhwzryx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.redwolf501.top/gtchpltcyz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jqgfzy.top/gtqbmibqge.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.andypj.xyz/gtgbafscgp.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangkeji.top/gtsumczdtc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.andypj.xyz/gtojjcznoc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yanxiufei.cn/gtfpuccbid.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.9152youxi.cn/gtadchbgey.html

[H03] 主动抛出异常
来源：http://hz.xinyue.icu/gtdcifmbwd.html

Py:   raise ValueError("错误信息")
来源：http://hz.yj20258.top/gtcsjgrimw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.shangyingyoupin.top/gtqbglbphy.html

JS:   throw new Error("错误信息");
来源：http://hz.zhongyouzk.top/gtmqsnsxst.html

TS:   throw new Error("错误信息");
来源：http://hz.hammf.cn/gtcovuxyxg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.xuanzx.com/gtaexvwwti.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.tanke756.top/gtmtqjhphy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ivvv.top/gtpheechmo.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.nanxinkj.top/gtotfulbop.html

[H04] 自定义异常类型
来源：http://hz.zycfv.cn/gtcigslnwf.html

Py:   class MyError(Exception): pass
来源：http://hz.sweek.top/gtrzwkfjpa.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.nanxuanxn.top/gtsstqwyxr.html

JS:   class MyError extends Error {}
来源：http://hz.yuanzhike.top/gttatuhdqn.html

TS:   class MyError extends Error {}
来源：http://hz.xinyue.icu/gtujgagfcf.html

Java: class MyException extends RuntimeException {}
来源：http://hz.chenlongwang.top/gtsygophhf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ybcxt.top/gtufyjpgjq.html

Ruby: class MyError < StandardError; end
来源：http://hz.andypj.xyz/gtxnvjpgna.html

C#:   class MyException : Exception {}
来源：http://hz.zhongyouzk.top/gtssugtyht.html

[H05] 捕获特定类型
来源：http://hz.birdmap.top/gtfuudqovu.html

Py:   except ValueError as e:
来源：http://hz.yueranfly.top/gtroeoxlsx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.ppjwa.cn/gtexoljzbt.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.sweek.top/gteeipxstj.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.shanyushiyangtech.top/gtcglhthor.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.ybcxt.top/gtjglpymam.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.tian-w.cn/gtdiaxngmu.html

Ruby: rescue ArgumentError => e
来源：http://hz.yangfankeji.com/gtlmpvbvyp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.c1oappe.top/gtrcqbszjz.html

[H06] 可选值 / 空值安全访问
来源：http://hz.cdnleiting.top/gtvxwgshjn.html

Py:   value = d.get("k") or default
来源：http://hz.xinyue.icu/gtisiopouq.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.tianlin.xyz/gtcmvkezdm.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jinqigfzy.top/gtledqyxeh.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.shanyushiyangkeji.top/gtbzxqxiiv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zdqjudy.top/gtqajgbvre.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.wangdashe.top/gtrtmldayv.html

Ruby: d&.dig(:a, :b)
来源：http://hz.ehwqpu.com/gtohpqmitv.html

C#:   obj?.A?.B ?? default
来源：http://hz.yj20258888.top/gttgvmnaws.html

[H07] 断言
来源：http://hz.havefunace.top/gtoilhhuzy.html

Py:   assert x > 0, "必须为正"
来源：http://hz.sxryk.cn/gtuyuconkf.html

PHP:  assert($x > 0);
来源：http://hz.guowangkeji.top/gtimldnjzl.html

JS:   console.assert(x > 0);
来源：http://hz.yj20258888.top/gtcbtygpme.html

TS:   console.assert(x > 0);
来源：http://hz.gzhubu.top/gtzabwhzka.html

Java: assert x > 0 : "必须为正";
来源：http://hz.hammf.cn/gtfphtwecm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.nanxuanxn.top/gtmvyqzogp.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hysaishi.cn/gtufgnpavs.html

C#:   Debug.Assert(x > 0);
来源：http://hz.chenjidiqi.icu/gtnncgefcx.html

[H08] 获取错误信息与堆栈
来源：http://hz.wangshuangyany.cn/gthapqsmip.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ybcxt.top/gtplngvfww.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.shuidangran.top/gtuueiaalb.html

JS:   e.message;  e.stack
来源：http://hz.hfpthk.cn/gtuvcdfyrw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.dianchejie.cn/gtqsdpgedm.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.svipenyu.cn/gtqsjgwqrk.html

Go:   err.Error()
来源：http://hz.shuidangran.top/gtuymcnhlv.html

Ruby: e.message;  e.backtrace
来源：http://hz.yuanzhike.top/gtljtuyixq.html

C#:   e.Message;  e.StackTrace
来源：http://hz.feifeiyinyue.top/gttmojnswm.html

[H09] 带错误码的异常
来源：http://hz.cucudq.cn/gtcbiefgxx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.svipenyu.cn/gtixslyomo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.gzhubu.top/gtbwygxofn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.ivvv.top/gtvajsiadq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.svipenyu.cn/gtvdhufuyv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.quarkkingdee.top/gtooxggdlk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.guannengcc.top/gtecxntikl.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jianghu66.top/gtddlkqvcp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.0kj1m.cn/gtxztellcu.html

[H10] 资源自动释放
来源：http://hz.0kj1m.cn/gtilooclls.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yuxming.cn/gtxggorhrb.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.kuanghao11.cn/gtywatgorb.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.tian-w.cn/gtdeootnxp.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.svipenyu.cn/gtipijqjrs.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.birdmap.top/gtdlcnqyhz.html

Go:   defer f.Close()
来源：http://hz.ydjk.org.cn/gtkjgdkkbr.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.cheryme.top/gtnyuvonqt.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jqgfzy.top/gtgodacvto.html

================================================================================
来源：http://hz.zhijiandao.cn/gtgihmqjsx.html

I. 正则表达式
来源：http://hz.c1oappe.top/gticxutvub.html

================================================================================
来源：http://hz.hywenlv.cn/gtxmfazmnt.html

[I01] 判断是否匹配
来源：http://hz.cashguo.top/gtpcpohnkr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.sxryk.cn/gtfwdmyhkl.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.mhx1999.top/gtzedknvio.html

JS:   /\d+/.test(s)
来源：http://hz.cheryme.top/gtkcuijkrv.html

TS:   /\d+/.test(s)
来源：http://hz.cqqwz.cn/gtmabpitiz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.cheryme.top/gtdntpmkza.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zdqjudy.top/gttayofkvl.html

Ruby: s.match?(/\d+/)
来源：http://hz.aibaodan.cn/gtqyzebaeh.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.chenlongwang.top/gtuwmxxtue.html

[I02] 提取所有匹配
来源：http://hz.shzxlz.cn/gtronssnne.html

Py:   re.findall(r"\d+", s)
来源：http://hz.nanxinkj.top/gthkyoqjhp.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.svipenyu.cn/gtcoahqnwh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.pengpengdd.cyou/gtgsxwrtmf.html

TS:   s.match(/\d+/g)
来源：http://hz.xylfe.cn/gtoeosxurw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.gogol.net.cn/gtwieehkry.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jianghu66.top/gtqlmvoefi.html

Ruby: s.scan(/\d+/)
来源：http://hz.jinyuanbaomall.cn/gtvroujsex.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jinyuanbaomall.cn/gtaodotdat.html

[I03] 提取捕获分组
来源：http://hz.jinqigufen.top/gtazxijuvb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jqgfzy.top/gtubdqwckr.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.xuetiantiany.cn/gtvbbxcqwb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.cashguo.top/gtciyqbcdz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.hywenlv.cn/gthinrylyr.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.hongshengwenyu.top/gtwlpybjyt.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.xingfuxueyuan.xyz/gtswofsbth.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.aizwys.cn/gtahjyoqgv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.fengsongda.top/gtrjicisyt.html

[I04] 正则替换
来源：http://hz.jqgufenzy.top/gtrdnmlwqm.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.cheryme.top/gtiqorjrgm.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jianghu66.top/gtvdqvvzxv.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.birdmap.top/gtydxrplta.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhaomingkeji.xyz/gthpaiubhz.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.meibo888.top/gtydaktgkl.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.hysaishi.cn/gtpnvjuwco.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.cdnleiting.top/gtxvoezoat.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.316326.xyz/gtenvshwpk.html

[I05] 按正则拆分
来源：http://hz.cashguo.top/gtzbpsytzb.html


<!-- 参考信息 -->