代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.sxryk.cn/gthdpdtedw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.shangyingyoupin.top/gtxlavdrja.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.sweek.top/gtfabufiwx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.meibo888.top/gtbgwbnpwx.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtwjbaklxy.html

G. 面向对象
来源：http://hz.jianghu66.top/gtnehafdjw.html

================================================================================
来源：http://hz.hammf.cn/gthbdjttpb.html

[G01] 定义类
来源：http://hz.aibaodan.cn/gtlevkzvoo.html

Py:   class User: pass
来源：http://hz.c1oappe.top/gtrlfisykk.html

PHP:  class User {}
来源：http://hz.yj20258888.top/gtddntjmse.html

JS:   class User {}
来源：http://hz.aibaodan.cn/gtgytlzmxj.html

TS:   class User { name: string = ""; }
来源：http://hz.tian-w.cn/gtranqmgzv.html

Java: class User {}
来源：http://hz.yuxming.cn/gtjqjswiur.html

Go:   type User struct { Name string }
来源：http://hz.yangfankeji.com/gtjqmwazrf.html

Ruby: class User; end
来源：http://hz.yj202588.top/gtdhtxwljk.html

C#:   class User {}
来源：http://hz.meibo888.top/gtuvrpgxtd.html

[G02] 构造函数
来源：http://hz.svipenyu.cn/gtsobnkdgg.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yanxiufei.cn/gtgxaqpsae.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.chenlongwang.top/gtrfhbklxf.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.shuidangran.top/gtqhoqpgtw.html

TS:   constructor(public name: string) {}
来源：http://hz.jlsjyb.cn/gtpubfakpg.html

Java: User(String name) { this.name = name; }
来源：http://hz.chenlongwang.top/gtdlnrrwbc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zhaomingkeji.xyz/gtdohggsur.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.c1oappe.top/gtyiakqhop.html

C#:   public User(string name) { Name = name; }
来源：http://hz.cheryme.top/gtsxvarkwe.html

[G03] 实例属性
来源：http://hz.ehwqpu.com/gtlujyygxc.html

Py:   self.name = "x"
来源：http://hz.fengsongda.top/gtzthlhebf.html

PHP:  public string $name = "x";
来源：http://hz.yvedp.cn/gtizscacyv.html

JS:   this.name = "x";
来源：http://hz.gzhubu.top/gtvwvnfzfo.html

TS:   name: string = "x";
来源：http://hz.zdqjudy.top/gtmttidccb.html

Java: private String name;
来源：http://hz.jyoumei.cn/gtcaiokavt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.ivvv.top/gtlizmiqzq.html

Ruby: @name = "x"
来源：http://hz.sxryk.cn/gtszdtczpg.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.ppjwa.cn/gtzrsqoqwk.html

[G04] 定义方法
来源：http://hz.shzxlz.cn/gtjhvhkjcg.html

Py:   def greet(self): return self.name
来源：http://hz.tanke756.top/gtedppcmkd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jqgufenzy.top/gtdlxfyqbg.html

JS:   greet() { return this.name; }
来源：http://hz.yj20258.top/gtydrepeqb.html

TS:   greet(): string { return this.name; }
来源：http://hz.fzhhl.top/gtsiehyrnj.html

Java: String greet() { return name; }
来源：http://hz.52xcode.cn/gtytucuvii.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.guowangkeji.top/gtnpnjwhxo.html

Ruby: def greet; @name; end
来源：http://hz.jianghu66.top/gtfezmyehi.html

C#:   public string Greet() => Name;
来源：http://hz.gotoacloud.top/gtbmspbzof.html

[G05] 继承
来源：http://hz.yj20258888.top/gtsjsvufkm.html

Py:   class Admin(User): pass
来源：http://hz.zhoulong.xyz/gtdozadtue.html

PHP:  class Admin extends User {}
来源：http://hz.wangshuangyany.cn/gtxcldcflf.html

JS:   class Admin extends User {}
来源：http://hz.yanxiufei.cn/gtblpkmjct.html

TS:   class Admin extends User {}
来源：http://hz.aizwys.cn/gtfsixxbwh.html

Java: class Admin extends User {}
来源：http://hz.haohaochexian.top/gtdiidbodh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jlsjyb.cn/gtsoxhbygq.html

Ruby: class Admin < User; end
来源：http://hz.9152youxi.cn/gtqpkjescl.html

C#:   class Admin : User {}
来源：http://hz.hysaishi.cn/gthoamkaql.html

[G06] 重写方法
来源：http://hz.zdqjudy.top/gtewiwrhog.html

Py:   def greet(self): return "admin"
来源：http://hz.tanke756.top/gtktiwdfwg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zhixingplan.top/gtvjpnoyfm.html

JS:   greet() { return "admin"; }
来源：http://hz.hnqzz.top/gtigzopouv.html

TS:   greet(): string { return "admin"; }
来源：http://hz.shuidangran.top/gtbykagwiq.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhoulong.xyz/gtmeuyjslz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yueranfly.top/gtdmjqhlwt.html

Ruby: def greet; "admin"; end
来源：http://hz.zhoulong.xyz/gtvlolotph.html

C#:   public override string Greet() => "admin";
来源：http://hz.havefunace.top/gttbasevla.html

[G07] 调用父类方法
来源：http://hz.yvedp.cn/gtdkmxitgu.html

Py:   super().greet()
来源：http://hz.yvedp.cn/gtrqobzglu.html

PHP:  parent::greet();
来源：http://hz.zhixingplan.top/gtimmktukr.html

JS:   super.greet();
来源：http://hz.kuanghao11.cn/gtgxqnwrkx.html

TS:   super.greet();
来源：http://hz.kuanghao11.cn/gtqnhimwke.html

Java: super.greet();
来源：http://hz.gaohongyu789.top/gthsjginmw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.sxryk.cn/gtyrzbvsxm.html

Ruby: super
来源：http://hz.hfpthk.cn/gtnljzwpix.html

C#:   base.Greet();
来源：http://hz.sxryk.cn/gtsmqchaaw.html

[G08] 静态方法与属性
来源：http://hz.ivvv.top/gtfshjyzpx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.gaohongyu789.top/gtxoizuebg.html

PHP:  public static function f() {}
来源：http://hz.ivvv.top/gtozndnnis.html

JS:   static f() {}
来源：http://hz.jqgfzy.top/gtalxttmmw.html

TS:   static f(): void {}
来源：http://hz.wangshuangyany.cn/gtnmmmjaei.html

Java: static void f() {}
来源：http://hz.haohaochexian.top/gtrecuzdha.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yvedp.cn/gtzcqvobhh.html

Ruby: def self.f; end
来源：http://hz.hysaishi.cn/gtdevbftex.html

C#:   public static void F() {}
来源：http://hz.jinyuanbaomall.cn/gtorliorio.html

[G09] 接口 / 抽象类
来源：http://hz.c1oappe.top/gtqxktiuco.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.316326.xyz/gtqtwkmafr.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.dianchejie.cn/gtniezneny.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zhixingplan.top/gtdislemhw.html

TS:   interface Shape { area(): number; }
来源：http://hz.cdnleiting.top/gtpsblslgy.html

Java: interface Shape { double area(); }
来源：http://hz.cashguo.top/gteevdznme.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.hnqzz.top/gtpohgvcly.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.gaohongyu789.top/gtnwbdftzo.html

C#:   interface IShape { double Area(); }
来源：http://hz.zdqjudy.top/gtchlhrucu.html

[G10] 访问控制
来源：http://hz.wangshuangyany.cn/gthuegsbss.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yanxiufei.cn/gtjtympgha.html

PHP:  public / protected / private
来源：http://hz.ywan-chungtsiang.top/gtlannnodu.html

JS:   #private 字段；其余公开
来源：http://hz.jyoumei.cn/gtgfqopbca.html

TS:   public / protected / private
来源：http://hz.c1oappe.top/gtsgltmgwt.html

Java: public / protected / private / 默认包级
来源：http://hz.jiagoushi.top/gtuqttzhyh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.shanyushiyangtech.top/gtipwbwsyh.html

Ruby: public / protected / private
来源：http://hz.9152youxi.cn/gtbryjpuhc.html

C#:   public / protected / private / internal
来源：http://hz.hysaishi.cn/gtiavduykt.html

[G11] getter / setter
来源：http://hz.xylfe.cn/gthtqwqzmg.html

Py:   @property 与 @x.setter
来源：http://hz.52xcode.cn/gtjmrtmujo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yuanzhike.top/gtiqdoknrt.html

JS:   get name() { return this._name; }
来源：http://hz.0kj1m.cn/gtxweqfjll.html

TS:   get name(): string { return this._name; }
来源：http://hz.xylfe.cn/gtquderpct.html

Java: public String getName() { return name; }
来源：http://hz.bjfxy.top/gtwtntgchw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.tian-w.cn/gtswsbbkcw.html

Ruby: attr_accessor :name
来源：http://hz.fzhhl.top/gtsrmpgquw.html

C#:   public string Name { get; set; }
来源：http://hz.ppjwa.cn/gtnaeutnht.html

[G12] 对象转字符串
来源：http://hz.dashuyun.cn/gtbhcmbgbf.html

Py:   def __str__(self): return self.name
来源：http://hz.jinghuilouyu.cn/gtgfdllgeu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.haohaochexian.top/gtknfdboqg.html

JS:   toString() { return this.name; }
来源：http://hz.cheryme.top/gtnfakymeo.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhaomingkeji.xyz/gtyuremcon.html

Java: @Override public String toString() { return name; }
来源：http://hz.meibo888.top/gtznbjzyfj.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yangfankeji.com/gtusuzixsh.html

Ruby: def to_s; @name; end
来源：http://hz.zhongyouzk.top/gtiwwxwmjo.html

C#:   public override string ToString() => Name;
来源：http://hz.ydzc1.top/gtosvljnjm.html

[G13] 判断对象类型
来源：http://hz.jiagoushi.top/gtdmwwckua.html

Py:   isinstance(u, User)
来源：http://hz.zhiwuduotai.top/gtosjxepco.html

PHP:  $u instanceof User
来源：http://hz.birdmap.top/gtpljmvjdr.html

JS:   u instanceof User
来源：http://hz.bjfxy.top/gtivifzmsh.html

TS:   u instanceof User
来源：http://hz.tianlin.xyz/gtfxszdjyo.html

Java: u instanceof User
来源：http://hz.nwbrower.top/gtucqsubfm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.cheryme.top/gteorxrltn.html

Ruby: u.is_a?(User)
来源：http://hz.hnxiangtu.top/gtgslfmibb.html

C#:   u is User
来源：http://hz.jinghuilouyu.cn/gtofhcrxlu.html

[G14] 数据类 / record
来源：http://hz.shzxlz.cn/gtxicljqqt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yonumen.top/gtsrrxauwv.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.ivvv.top/gtthasvbdp.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.aizwys.cn/gttjjlwfpl.html

TS:   type User = { name: string; age: number };
来源：http://hz.kuanghao11.cn/gtvrmstccp.html

Java: record User(String name, int age) {}
来源：http://hz.aizwys.cn/gtcouykdse.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jinghuilouyu.cn/gtfqoyjlfv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.feifeiyinyue.top/gthdaxajty.html

C#:   record User(string Name, int Age);
来源：http://hz.hysaishi.cn/gthlnikxcm.html

[G15] 枚举
来源：http://hz.haohaochexian.top/gthgggskah.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zhongyouzk.top/gttnclzwsf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.shanyushiyangkeji.top/gtciotbwsx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hnxiangtu.top/gtzzycewrm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhixingplan.top/gtupcsakyp.html

Java: enum Color { RED, GREEN }
来源：http://hz.zhoulong.xyz/gtommzxsjg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.shangyingyoupin.top/gtreugfzcs.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yanxiufei.cn/gtdgmdkaga.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shanyushiyangkeji.top/gtjrlfbblw.html

[G16] 对象转数组 / 字典
来源：http://hz.wangdashe.top/gtmgoparrw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhiwuduotai.top/gtznwfvbrr.html

PHP:  get_object_vars($obj);
来源：http://hz.tianlin.xyz/gtulqnawez.html

JS:   Object.entries(obj)
来源：http://hz.havefunace.top/gtlhxwonkn.html

TS:   Object.entries(obj)
来源：http://hz.gogol.net.cn/gtsjmilqmq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.feifeiyinyue.top/gttfddkdpa.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.ywan-chungtsiang.top/gtztocxqzw.html

Ruby: obj.instance_variables
来源：http://hz.hongshengwenyu.top/gtzvayteyq.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yj20258888.top/gtgqwlrfkd.html

================================================================================
来源：http://hz.redwolf501.top/gtcigdmhnt.html

H. 异常与错误处理
来源：http://hz.jqgufenzy.top/gtxqownqie.html

================================================================================
来源：http://hz.aibaodan.cn/gtssiqqimb.html

[H01] try / catch 基础
来源：http://hz.yonumen.top/gtfprwmaee.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.dashuyun.cn/gtetqofbdb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.cdnleiting.top/gtpkoxrzva.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zycfv.cn/gtuvjsikqx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.chenzaomai.com/gtzobmdtuq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.hysaishi.cn/gtcjickhcr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.svipenyu.cn/gtvkbsuhws.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.wangdashe.top/gtwrfdtvxn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.redwolf501.top/gtxqpkekyx.html

[H02] finally / ensure 收尾
来源：http://hz.yueranfly.top/gtfjlwzibu.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.ppjwa.cn/gthyqqdoqh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.316326.xyz/gtjralnbtl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.ydjk.org.cn/gthnrxqwgq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.chenlongwang.top/gtxybumxys.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.nwbrower.top/gtzuxqxzqq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jlsjyb.cn/gtbsmgklkd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.sxryk.cn/gtflnumxee.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.wangshuangyany.cn/gtcjocewro.html

[H03] 主动抛出异常
来源：http://hz.ydzc1.top/gtmodnvjbm.html

Py:   raise ValueError("错误信息")
来源：http://hz.yj20258.top/gtztdmnael.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.vqdsnc.cn/gtnbwwdvyi.html

JS:   throw new Error("错误信息");
来源：http://hz.ehwqpu.com/gtuxfvrphj.html

TS:   throw new Error("错误信息");
来源：http://hz.yj20258.top/gtpicsutma.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yueranfly.top/gthuxbbpgw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jinqigfzy.top/gtdhlwdscd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.shzxlz.cn/gtebuvqzkq.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.chenjidiqi.icu/gtufnwydly.html

[H04] 自定义异常类型
来源：http://hz.fzhhl.top/gtdhgvowpn.html

Py:   class MyError(Exception): pass
来源：http://hz.yj20258888.top/gtuypugixa.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.xuetiantiany.cn/gtmdrcuneb.html

JS:   class MyError extends Error {}
来源：http://hz.wangshuangyany.cn/gtcmgcgwqt.html

TS:   class MyError extends Error {}
来源：http://hz.yanxiufei.cn/gtfrxngkcc.html

Java: class MyException extends RuntimeException {}
来源：http://hz.ydzc1.top/gtmisqlmvw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.vqdsnc.cn/gtpnoebrwf.html

Ruby: class MyError < StandardError; end
来源：http://hz.sweek.top/gtilvmihow.html

C#:   class MyException : Exception {}
来源：http://hz.jinghuilouyu.cn/gtzujbbmvd.html

[H05] 捕获特定类型
来源：http://hz.hnqzz.top/gtitpvdgis.html

Py:   except ValueError as e:
来源：http://hz.yangfankeji.com/gtlmvzuzsu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.0kj1m.cn/gtskkotybt.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.tanke756.top/gtbvdwsfpb.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yongpay.top/gtswyadklo.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.ybcxt.top/gtdbavztxl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.aibaodan.cn/gtrudgwvao.html

Ruby: rescue ArgumentError => e
来源：http://hz.haohaochexian.top/gtdpxepxov.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yonumen.top/gttmmehxcb.html

[H06] 可选值 / 空值安全访问
来源：http://hz.52xcode.cn/gtlfnpgasf.html

Py:   value = d.get("k") or default
来源：http://hz.zhengqikj.top/gtxxbtzkny.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.smart0.xyz/gtgoxoknmz.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zhoulong.xyz/gtuzfnyzzd.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.chenzaomai.com/gtntqrwcid.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.pycfn.com/gtovnbotwc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.nanxinkj.top/gtnsnxdqbc.html

Ruby: d&.dig(:a, :b)
来源：http://hz.52xcode.cn/gtdhidddmo.html

C#:   obj?.A?.B ?? default
来源：http://hz.ybcxt.top/gtadtverrm.html

[H07] 断言
来源：http://hz.havefunace.top/gtlwnanszg.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jyoumei.cn/gtwjcgdems.html

PHP:  assert($x > 0);
来源：http://hz.nanxinkj.top/gtvymdjqjw.html

JS:   console.assert(x > 0);
来源：http://hz.c1oappe.top/gtqzrluizk.html

TS:   console.assert(x > 0);
来源：http://hz.aibaodan.cn/gtmpwulwtz.html

Java: assert x > 0 : "必须为正";
来源：http://hz.tanke756.top/gttxnoktsr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.sysykeji.top/gttitrxooe.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.redwolf501.top/gtjszksrpn.html

C#:   Debug.Assert(x > 0);
来源：http://hz.haohaochexian.top/gterrbqois.html

[H08] 获取错误信息与堆栈
来源：http://hz.dianchejie.cn/gttuiwwgjh.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.birdmap.top/gtjmqeimtt.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.gogol.net.cn/gthryehahs.html

JS:   e.message;  e.stack
来源：http://hz.gogol.net.cn/gtdsabkezb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yj20258.top/gtooynszlb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.mhx1999.top/gthsrusxob.html

Go:   err.Error()
来源：http://hz.shuidangran.top/gthmrwjhco.html

Ruby: e.message;  e.backtrace
来源：http://hz.sweek.top/gtgqszguki.html

C#:   e.Message;  e.StackTrace
来源：http://hz.52xcode.cn/gtiumvvizv.html

[H09] 带错误码的异常
来源：http://hz.zhengqikj.top/gtsaonyjcb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yongpay.top/gtmmjkqqbx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ehwqpu.com/gtcqkgkfco.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yangfankeji.com/gtkqcudtit.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zhixingplan.top/gtvpnwnxcw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.aibaodan.cn/gtiqoqrexz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.tian-w.cn/gtnyyrznis.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yj202588.top/gtwubtluam.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhixingplan.top/gtsmmwkasr.html

[H10] 资源自动释放
来源：http://hz.zhengqikj.top/gtmukeklik.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yueranfly.top/gteagcyffk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yj20258888.top/gtrtlbpjod.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.316326.xyz/gtpjnltute.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.redwolf501.top/gtrymhoebs.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.hysaishi.cn/gtilhxxwtf.html

Go:   defer f.Close()
来源：http://hz.jinqigufen.top/gtgxatrhum.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yj20258888.top/gtwwamrxyi.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.hywenlv.cn/gtbenvoeru.html

================================================================================
来源：http://hz.xylfe.cn/gtzqzpluvm.html

I. 正则表达式
来源：http://hz.tian-w.cn/gtsleusovm.html

================================================================================
来源：http://hz.yj202588.top/gtzpnzgvtn.html

[I01] 判断是否匹配
来源：http://hz.tianlin.xyz/gtuppfbric.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.gogol.net.cn/gtjwupzwst.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.aizwys.cn/gtmvjiktqs.html

JS:   /\d+/.test(s)
来源：http://hz.fengsongda.top/gtnfbcizrr.html

TS:   /\d+/.test(s)
来源：http://hz.tanke756.top/gtpmvgvhkr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hammf.cn/gtkywnzlep.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hywenlv.cn/gtlwvuqqko.html

Ruby: s.match?(/\d+/)
来源：http://hz.ybcxt.top/gtmxqznmlo.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.pycfn.com/gtwdushxaw.html

[I02] 提取所有匹配
来源：http://hz.redwolf501.top/gttihnfoox.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ydjk.org.cn/gtckcnqkhg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zdqjudy.top/gtzyeamnxo.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yuanzhike.top/gtxshzuesz.html

TS:   s.match(/\d+/g)
来源：http://hz.jinqigfzy.top/gtrpasdmdp.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yuxming.cn/gtzeqraqkj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.pengpengdd.cyou/gtdawvvkev.html

Ruby: s.scan(/\d+/)
来源：http://hz.gogol.net.cn/gtwfavdxkn.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.shuidangran.top/gtdfntginv.html

[I03] 提取捕获分组
来源：http://hz.sufxvd.cn/gtjoxqiebw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.sweek.top/gttnwncyqt.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yuxming.cn/gtnytfaisu.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.shangyingyoupin.top/gtdovzixed.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.0kj1m.cn/gtimhttdlj.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.cqqwz.cn/gtcbjkvhup.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.c1oappe.top/gtqrcomluv.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhiwuduotai.top/gtuigcdmdg.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.nanxinkj.top/gtsrejkdrd.html

[I04] 正则替换
来源：http://hz.aizwys.cn/gttsbryqsu.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.quarkkingdee.top/gtbiqsudjh.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.vqdsnc.cn/gtfzyxkujv.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.hnxiangtu.top/gtcistoiic.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.9152youxi.cn/gtkzagsnyl.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.chenjidiqi.icu/gtwonzrbaj.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.tianlin.xyz/gteqevtyob.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhaomingkeji.xyz/gtsgmlucnu.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.kuanghao11.cn/gtyfyrgrpx.html

[I05] 按正则拆分
来源：http://hz.birdmap.top/gturckkryf.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yvedp.cn/gtzscuuima.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.tianlin.xyz/gtgsfjritk.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jinqigufen.top/gtcgnzghbw.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zhiwuduotai.top/gtectqjyko.html

Java: s.split("\\s*,\\s*")
来源：http://hz.andypj.xyz/gtrzqfpvse.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhaomingkeji.xyz/gtucyhlgev.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.pycfn.com/gtgauokowd.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jinqigufen.top/gtehnoynsh.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.gaohongyu789.top/gtjyysayyq.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.daria6918.cn/gtufzgbgsk.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.jyoumei.cn/gtcgobhuvl.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhongyouzk.top/gtfghaavxp.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.daria6918.cn/gtxdyzhnwb.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.daxiang520.top/gtkgsrntbu.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.havefunace.top/gttqjmkast.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.quarkkingdee.top/gtzbriokhm.html


<!-- 参考信息 -->