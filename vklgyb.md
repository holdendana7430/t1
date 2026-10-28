代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.shuidangran.top/gtuwugciaj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.xziqi.cn/gtwpeftfqp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jinyuanbaomall.cn/gtpskjuusi.html

[F12] CSV 读写
来源：http://hz.yuanzhike.top/gttkimoovm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.chenjidiqi.icu/gtefntztfy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.xuanzx.com/gtvadduntg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zhiwuduotai.top/gtdewcgrhq.html

TS:   // 同上
来源：http://hz.yongpay.top/gttixxsjiv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jinqigfzy.top/gtgiwwwsny.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yongpay.top/gtowvdkzug.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.meibo888.top/gtginjixdz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.fzhhl.top/gtdcnjhuat.html

================================================================================
来源：http://hz.guowangkeji.top/gtycngkkpo.html

G. 面向对象
来源：http://hz.nanxuanxn.top/gtxbuvbfea.html

================================================================================
来源：http://hz.pycfn.com/gtivjtmktn.html

[G01] 定义类
来源：http://hz.dianchejie.cn/gtpkfxswrv.html

Py:   class User: pass
来源：http://hz.snrcjt.cn/gtpiuriorm.html

PHP:  class User {}
来源：http://hz.shzxlz.cn/gtleontsns.html

JS:   class User {}
来源：http://hz.ehwqpu.com/gtqeavzmvs.html

TS:   class User { name: string = ""; }
来源：http://hz.yvedp.cn/gtrwgmgjce.html

Java: class User {}
来源：http://hz.zhijiandao.cn/gtxqbbyrww.html

Go:   type User struct { Name string }
来源：http://hz.xylfe.cn/gtolrjrvaw.html

Ruby: class User; end
来源：http://hz.smart0.xyz/gtdnuhtofr.html

C#:   class User {}
来源：http://hz.xylfe.cn/gtmyqsltbp.html

[G02] 构造函数
来源：http://hz.ydjk.org.cn/gtyfwsllyw.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhengqikj.top/gtcglrkcdx.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.xziqi.cn/gtzfbrztfr.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.cashguo.top/gtqwbtrjmn.html

TS:   constructor(public name: string) {}
来源：http://hz.gaohongyu789.top/gtsudrvdkt.html

Java: User(String name) { this.name = name; }
来源：http://hz.0kj1m.cn/gtqdsppvyt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jinyuanbaomall.cn/gtczpllrij.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.xuetiantiany.cn/gtsmmjamya.html

C#:   public User(string name) { Name = name; }
来源：http://hz.xuetiantiany.cn/gtjkhvonhr.html

[G03] 实例属性
来源：http://hz.zhengqikj.top/gtqumoiyvw.html

Py:   self.name = "x"
来源：http://hz.wangshuangyany.cn/gtresejdfv.html

PHP:  public string $name = "x";
来源：http://hz.jianghu66.top/gtfpaqyyhs.html

JS:   this.name = "x";
来源：http://hz.jinghuilouyu.cn/gthfihvbts.html

TS:   name: string = "x";
来源：http://hz.wangshuangyany.cn/gtvwrmmono.html

Java: private String name;
来源：http://hz.tianlin.xyz/gtfzuwevnh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.nanxuanxn.top/gtcusafzza.html

Ruby: @name = "x"
来源：http://hz.ywan-chungtsiang.top/gtarazhafy.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.smart0.xyz/gtpclcbeau.html

[G04] 定义方法
来源：http://hz.9152youxi.cn/gtmdxlptae.html

Py:   def greet(self): return self.name
来源：http://hz.yj202588.top/gtrjjossck.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.shzxlz.cn/gtfkrqeeii.html

JS:   greet() { return this.name; }
来源：http://hz.fzhhl.top/gtbicutide.html

TS:   greet(): string { return this.name; }
来源：http://hz.nwbrower.top/gtunpazzas.html

Java: String greet() { return name; }
来源：http://hz.cashguo.top/gtpywctxrb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.chenzaomai.com/gtmvbgvryr.html

Ruby: def greet; @name; end
来源：http://hz.ywan-chungtsiang.top/gtaytsfczs.html

C#:   public string Greet() => Name;
来源：http://hz.shangyingyoupin.top/gtyyixzxen.html

[G05] 继承
来源：http://hz.zdqjudy.top/gthgdlxfjz.html

Py:   class Admin(User): pass
来源：http://hz.tanke756.top/gtbkmdzhqt.html

PHP:  class Admin extends User {}
来源：http://hz.kuanghao11.cn/gttrimweaq.html

JS:   class Admin extends User {}
来源：http://hz.jinghuilouyu.cn/gtncgjqqrm.html

TS:   class Admin extends User {}
来源：http://hz.316326.xyz/gtidlrmkpq.html

Java: class Admin extends User {}
来源：http://hz.hongshengwenyu.top/gthqjxazsp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yangfankeji.com/gtuakeqjju.html

Ruby: class Admin < User; end
来源：http://hz.cashguo.top/gthkzwdhrw.html

C#:   class Admin : User {}
来源：http://hz.bjfxy.top/gtnsntjvvv.html

[G06] 重写方法
来源：http://hz.yueranfly.top/gttbbfymqp.html

Py:   def greet(self): return "admin"
来源：http://hz.52xcode.cn/gtyjhcezxc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jqgfzy.top/gtfclvapvo.html

JS:   greet() { return "admin"; }
来源：http://hz.0kj1m.cn/gtgxxqmviz.html

TS:   greet(): string { return "admin"; }
来源：http://hz.shanyushiyangtech.top/gtrfdnzpey.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.cdnleiting.top/gtzhpixgte.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhengqikj.top/gtfnuqzlow.html

Ruby: def greet; "admin"; end
来源：http://hz.nanxuanxn.top/gtcrtlxhvx.html

C#:   public override string Greet() => "admin";
来源：http://hz.gaohongyu789.top/gtqlwciavl.html

[G07] 调用父类方法
来源：http://hz.zdqjudy.top/gtsmltjlml.html

Py:   super().greet()
来源：http://hz.xingfuxueyuan.xyz/gtavncutsg.html

PHP:  parent::greet();
来源：http://hz.zhixingplan.top/gtbteehhbn.html

JS:   super.greet();
来源：http://hz.pengpengdd.cyou/gtvsyshkqs.html

TS:   super.greet();
来源：http://hz.pengpengdd.cyou/gtajyyiffj.html

Java: super.greet();
来源：http://hz.ehwqpu.com/gttfubmehm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yj20258.top/gtuzhxpcgx.html

Ruby: super
来源：http://hz.chenlongwang.top/gtumstcxmk.html

C#:   base.Greet();
来源：http://hz.shanyushiyangtech.top/gtzjfymlif.html

[G08] 静态方法与属性
来源：http://hz.daria6918.cn/gtvizwfgxp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.smart0.xyz/gtubwthqbj.html

PHP:  public static function f() {}
来源：http://hz.nwbrower.top/gtpvnydtrn.html

JS:   static f() {}
来源：http://hz.yj20258.top/gtwfaknehn.html

TS:   static f(): void {}
来源：http://hz.daria6918.cn/gtafrooeiy.html

Java: static void f() {}
来源：http://hz.tian-w.cn/gtxdoignxk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yuanzhike.top/gtonimxbyr.html

Ruby: def self.f; end
来源：http://hz.guannengcc.top/gtfasflsmx.html

C#:   public static void F() {}
来源：http://hz.chenzaomai.com/gtgkgdqodw.html

[G09] 接口 / 抽象类
来源：http://hz.quarkkingdee.top/gtsfrvfnty.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.bjfxy.top/gtcadnbbcm.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yuanzhike.top/gtyomdxptl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yj20258.top/gtbxfunjjr.html

TS:   interface Shape { area(): number; }
来源：http://hz.zycfv.cn/gtvrhcgvus.html

Java: interface Shape { double area(); }
来源：http://hz.c1oappe.top/gtzrmgwjph.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.xziqi.cn/gtzfochsml.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.bjfxy.top/gtpnmtpefx.html

C#:   interface IShape { double Area(); }
来源：http://hz.aibaodan.cn/gtwzlgkhnq.html

[G10] 访问控制
来源：http://hz.cdnleiting.top/gtrdwrzrrk.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.cdnleiting.top/gtfbpnniqi.html

PHP:  public / protected / private
来源：http://hz.ydjk.org.cn/gtbukwgsmo.html

JS:   #private 字段；其余公开
来源：http://hz.ivvv.top/gtzjsgyply.html

TS:   public / protected / private
来源：http://hz.tian-w.cn/gtihijqbbw.html

Java: public / protected / private / 默认包级
来源：http://hz.hongshengwenyu.top/gteadcpraj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.pycfn.com/gtkqjcdyjp.html

Ruby: public / protected / private
来源：http://hz.pengpengdd.cyou/gtilzoslrc.html

C#:   public / protected / private / internal
来源：http://hz.yj202588.top/gtwilgbgef.html

[G11] getter / setter
来源：http://hz.iojbl.cn/gtrkyfyozn.html

Py:   @property 与 @x.setter
来源：http://hz.jqgufenzy.top/gtrhzmldrr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.dashuyun.cn/gteqaeeczj.html

JS:   get name() { return this._name; }
来源：http://hz.yuxming.cn/gtrxnesgfa.html

TS:   get name(): string { return this._name; }
来源：http://hz.gaohongyu789.top/gtzjtauyzw.html

Java: public String getName() { return name; }
来源：http://hz.316326.xyz/gtdvcctnyf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.chenlongwang.top/gtyhqdnuxr.html

Ruby: attr_accessor :name
来源：http://hz.svipenyu.cn/gtvfhdhagx.html

C#:   public string Name { get; set; }
来源：http://hz.yongpay.top/gtdrxxhnln.html

[G12] 对象转字符串
来源：http://hz.yonumen.top/gtsklsmptv.html

Py:   def __str__(self): return self.name
来源：http://hz.zdqjudy.top/gtwfhjbjrp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.0kj1m.cn/gtqkihhhls.html

JS:   toString() { return this.name; }
来源：http://hz.shanyushiyangtech.top/gtujqpgwkb.html

TS:   toString(): string { return this.name; }
来源：http://hz.dianchejie.cn/gtqqttqxfj.html

Java: @Override public String toString() { return name; }
来源：http://hz.yvedp.cn/gtacrstgyd.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.bjfxy.top/gtveneicxd.html

Ruby: def to_s; @name; end
来源：http://hz.svipenyu.cn/gtxrdkftrs.html

C#:   public override string ToString() => Name;
来源：http://hz.iojbl.cn/gtfdqanjpf.html

[G13] 判断对象类型
来源：http://hz.ehwqpu.com/gtmcdsxhdd.html

Py:   isinstance(u, User)
来源：http://hz.yuanzhike.top/gtvbajaoma.html

PHP:  $u instanceof User
来源：http://hz.haohaochexian.top/gtdcveooyk.html

JS:   u instanceof User
来源：http://hz.nanxuanxn.top/gtqsgdythg.html

TS:   u instanceof User
来源：http://hz.fengsongda.top/gtrojczhrn.html

Java: u instanceof User
来源：http://hz.haohaochexian.top/gtdzvgtalw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.sxryk.cn/gtgipjwmet.html

Ruby: u.is_a?(User)
来源：http://hz.wangdashe.top/gtdwzzpobz.html

C#:   u is User
来源：http://hz.jqgfzy.top/gtdtaneyee.html

[G14] 数据类 / record
来源：http://hz.gogol.net.cn/gtsiujjajn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.tian-w.cn/gttlkcfcka.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.sweek.top/gtujspuzcn.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.pycfn.com/gtfktyblix.html

TS:   type User = { name: string; age: number };
来源：http://hz.yj202588.top/gtopdwodyw.html

Java: record User(String name, int age) {}
来源：http://hz.jinqigufen.top/gtraeprtso.html

Go:   type User struct { Name string; Age int }
来源：http://hz.guannengcc.top/gtenvqnkde.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.9152youxi.cn/gtsjwxdhuc.html

C#:   record User(string Name, int Age);
来源：http://hz.chenlongwang.top/gtqimpdclw.html

[G15] 枚举
来源：http://hz.cucudq.cn/gtlbnrbeel.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.meibo888.top/gtvxurdlcs.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jqgufenzy.top/gtteykvnzd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yj202588.top/gtgjpjomqu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jinghuilouyu.cn/gtaovlyqmf.html

Java: enum Color { RED, GREEN }
来源：http://hz.cashguo.top/gtckjchqbv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.aizwys.cn/gtdulatsmr.html

Ruby: Color = %i[red green].freeze
来源：http://hz.vqdsnc.cn/gtfnxoyjmp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ehwqpu.com/gtryzpfuxo.html

[G16] 对象转数组 / 字典
来源：http://hz.ydzc1.top/gtuonquasq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yongpay.top/gtxzoyfswz.html

PHP:  get_object_vars($obj);
来源：http://hz.ywan-chungtsiang.top/gtyxstuixx.html

JS:   Object.entries(obj)
来源：http://hz.bjfxy.top/gtaeuukimx.html

TS:   Object.entries(obj)
来源：http://hz.ydzc1.top/gtascoeros.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hywenlv.cn/gtparmahjp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yangfankeji.com/gttxalaeml.html

Ruby: obj.instance_variables
来源：http://hz.daria6918.cn/gtiwxqvtux.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.xingfuxueyuan.xyz/gtspafruad.html

================================================================================
来源：http://hz.ehwqpu.com/gtukejsszi.html

H. 异常与错误处理
来源：http://hz.zycfv.cn/gtwgwrfblh.html

================================================================================
来源：http://hz.yj20258.top/gttxmudhkp.html

[H01] try / catch 基础
来源：http://hz.zhengqikj.top/gtshelubee.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.redwolf501.top/gtvarhjcnb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.redwolf501.top/gtcdejbvqo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.dashuyun.cn/gtuvpgjbrp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.0kj1m.cn/gtspcibrwy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.xylfe.cn/gtwvmvoauk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zhiwuduotai.top/gtsmjzqvca.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.chenlongwang.top/gtroemakwc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.cucudq.cn/gtzlshxwtu.html

[H02] finally / ensure 收尾
来源：http://hz.gaohongyu789.top/gtsojgsyte.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.xylfe.cn/gtwfjeuhni.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.smart0.xyz/gtolyenriw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.52xcode.cn/gtukulhqxj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhengqikj.top/gtufcyyexe.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.9152youxi.cn/gtpievqgqm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jinyuanbaomall.cn/gtseagmoiu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.gotoacloud.top/gtalnhutgq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.316326.xyz/gtzpdutlqy.html

[H03] 主动抛出异常
来源：http://hz.zhixingplan.top/gtoarcvljm.html

Py:   raise ValueError("错误信息")
来源：http://hz.52xcode.cn/gtwiexovzl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yangfankeji.com/gtxowfqhbj.html

JS:   throw new Error("错误信息");
来源：http://hz.yvedp.cn/gtjsrirxvo.html

TS:   throw new Error("错误信息");
来源：http://hz.xingfuxueyuan.xyz/gtxbemjhze.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.c1oappe.top/gtlbvjoucb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.iojbl.cn/gtffqosyjd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.daxiang520.top/gtvbfxsmtf.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.pengpengdd.cyou/gtftqtyqzm.html

[H04] 自定义异常类型
来源：http://hz.ybcxt.top/gtqevkwwsi.html

Py:   class MyError(Exception): pass
来源：http://hz.zdqjudy.top/gttoknjimd.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jlsjyb.cn/gtipjjrwai.html

JS:   class MyError extends Error {}
来源：http://hz.hammf.cn/gtvkvmrsie.html

TS:   class MyError extends Error {}
来源：http://hz.nanxinkj.top/gtusrkziqz.html

Java: class MyException extends RuntimeException {}
来源：http://hz.pengpengdd.cyou/gtahgymbgo.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.shangyingyoupin.top/gtbhpxurgn.html

Ruby: class MyError < StandardError; end
来源：http://hz.ehwqpu.com/gtrtqnlqvw.html

C#:   class MyException : Exception {}
来源：http://hz.feifeiyinyue.top/gtwidezcli.html

[H05] 捕获特定类型
来源：http://hz.cqqwz.cn/gtdufnqfng.html

Py:   except ValueError as e:
来源：http://hz.yueranfly.top/gtxhdwvlya.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jinqigufen.top/gtpvzcfxwv.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yonumen.top/gtxkjodhtm.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.sxryk.cn/gtraymmbso.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yangfankeji.com/gtsffevaid.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jinqigfzy.top/gtgqkuhvdm.html

Ruby: rescue ArgumentError => e
来源：http://hz.gogol.net.cn/gtfkmmzzuy.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.316326.xyz/gtbtmqjxpy.html

[H06] 可选值 / 空值安全访问
来源：http://hz.tian-w.cn/gtbwdstopa.html

Py:   value = d.get("k") or default
来源：http://hz.zhijiandao.cn/gtiwcaxbjs.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.xuetiantiany.cn/gtehgoifab.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.hnqzz.top/gttrbtnhfx.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zhijiandao.cn/gtgcfofumz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.fengsongda.top/gtdugcqycu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jinqigfzy.top/gtonaaodkn.html

Ruby: d&.dig(:a, :b)
来源：http://hz.mhx1999.top/gtcylubqta.html

C#:   obj?.A?.B ?? default
来源：http://hz.zhengqikj.top/gtfdisbslv.html

[H07] 断言
来源：http://hz.chenlongwang.top/gtjqdevdel.html

Py:   assert x > 0, "必须为正"
来源：http://hz.shuidangran.top/gtjsspxtkg.html

PHP:  assert($x > 0);
来源：http://hz.meibo888.top/gtmislbhri.html

JS:   console.assert(x > 0);
来源：http://hz.chenjidiqi.icu/gtkbikntvs.html

TS:   console.assert(x > 0);
来源：http://hz.yvedp.cn/gttsussygz.html

Java: assert x > 0 : "必须为正";
来源：http://hz.bjfxy.top/gtrfyyisaw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.tian-w.cn/gtokxmckyx.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hywenlv.cn/gtnlexgwfm.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jiagoushi.top/gtmpoyngst.html

[H08] 获取错误信息与堆栈
来源：http://hz.nwbrower.top/gtnnlkoelf.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zycfv.cn/gtdhttbvvv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.gaohongyu789.top/gtspatgdee.html

JS:   e.message;  e.stack
来源：http://hz.nanxinkj.top/gtctpehlbi.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.aizwys.cn/gtmkvtiuuk.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.ywan-chungtsiang.top/gtrpeddbup.html

Go:   err.Error()
来源：http://hz.wangdashe.top/gtudsxselk.html

Ruby: e.message;  e.backtrace
来源：http://hz.jinghuilouyu.cn/gtjzvhmzgw.html

C#:   e.Message;  e.StackTrace
来源：http://hz.dianchejie.cn/gtupndubhu.html

[H09] 带错误码的异常
来源：http://hz.cucudq.cn/gtaugvzxvl.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.mhx1999.top/gtwdtixvam.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.daria6918.cn/gtahtuoidt.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.ydjk.org.cn/gtjdevalhc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.aizwys.cn/gtvchgcrff.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.dashuyun.cn/gtsfwiupof.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hammf.cn/gtfkozpktv.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.nanxinkj.top/gtdoeltzuf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.ivvv.top/gtcetbhkmu.html

[H10] 资源自动释放
来源：http://hz.xuetiantiany.cn/gtjwvqfisd.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zdqjudy.top/gtcsingclq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yj202588.top/gtewturbza.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zycfv.cn/gtpffbomwj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sysykeji.top/gtayucjdny.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.0kj1m.cn/gtnvlnerkh.html

Go:   defer f.Close()
来源：http://hz.yuxming.cn/gtspvmcwdq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.aizwys.cn/gtgmkcghhq.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.feifeiyinyue.top/gtimfedhgz.html

================================================================================
来源：http://hz.zhoulong.xyz/gtyhwzfdtm.html

I. 正则表达式
来源：http://hz.guannengcc.top/gtgpuonytu.html

================================================================================
来源：http://hz.zhixingplan.top/gtgqfucapx.html

[I01] 判断是否匹配
来源：http://hz.jinqigfzy.top/gtutjwdxhr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jianghu66.top/gtgmgdnqyu.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.ppjwa.cn/gthbypgfat.html

JS:   /\d+/.test(s)
来源：http://hz.cdnleiting.top/gtgqijfusb.html

TS:   /\d+/.test(s)
来源：http://hz.jqgufenzy.top/gtqyekobwd.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.nanxinkj.top/gtxkobzxii.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.feifeiyinyue.top/gtbtankvkg.html

Ruby: s.match?(/\d+/)
来源：http://hz.ydjk.org.cn/gtrvbpiubb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.fzhhl.top/gtbnhegart.html

[I02] 提取所有匹配
来源：http://hz.ydzc1.top/gtwvyywxav.html

Py:   re.findall(r"\d+", s)
来源：http://hz.cdnleiting.top/gtguyadcrd.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jqgfzy.top/gtlzokadey.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.bjfxy.top/gtdrjnsvlf.html

TS:   s.match(/\d+/g)
来源：http://hz.sxryk.cn/gtrcydyrvn.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.cdnleiting.top/gtsilvvgpr.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.ybcxt.top/gtytwrsdyf.html

Ruby: s.scan(/\d+/)
来源：http://hz.jinqigufen.top/gtszcnzvpe.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.xuanzx.com/gtwfbruuhq.html

[I03] 提取捕获分组
来源：http://hz.feifeiyinyue.top/gtymdsedqx.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.sufxvd.cn/gtoscdigbk.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.xingfuxueyuan.xyz/gtkijfddec.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yuanzhike.top/gtzctzgqmm.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.tanke756.top/gtidbxddfn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zdqjudy.top/gtztpyayhc.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.xuetiantiany.cn/gtxwgkjeef.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhengqikj.top/gtuvuvjulh.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.fengsongda.top/gtbsdymcfb.html

[I04] 正则替换
来源：http://hz.xuetiantiany.cn/gtbbozysie.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.fzhhl.top/gtrurfpinj.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.xingfuxueyuan.xyz/gtlflggrzo.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.sweek.top/gtzroacboo.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yvedp.cn/gtikdyanng.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.gotoacloud.top/gtwdnuckra.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.tanke756.top/gtxeobshws.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.tanke756.top/gtubrzxxgl.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.cdnleiting.top/gtrgirrrnl.html

[I05] 按正则拆分
来源：http://hz.ehwqpu.com/gtzcokakdb.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zhijiandao.cn/gtoeeysejc.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hongshengwenyu.top/gtajjwbjnw.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.vqdsnc.cn/gtrmqoginb.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.pycfn.com/gtebtfenzw.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jianghu66.top/gtyubaswbb.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.xingfuxueyuan.xyz/gtxbextjao.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yj20258.top/gttaryfrdb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.fzhhl.top/gterbwoqrs.html


<!-- 参考信息 -->