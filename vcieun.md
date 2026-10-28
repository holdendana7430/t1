代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yvedp.cn/gtimvpsxin.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yj20258888.top/gtsnlxrirp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zhixingplan.top/gtrlbgnmxm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.hnqzz.top/gtrwvdneam.html

================================================================================
来源：http://hz.shuidangran.top/gtuuqykkwn.html

G. 面向对象
来源：http://hz.yuxming.cn/gtuqdwocfm.html

================================================================================
来源：http://hz.zhoulong.xyz/gtzksbqhgu.html

[G01] 定义类
来源：http://hz.nanxinkj.top/gtcadeofts.html

Py:   class User: pass
来源：http://hz.ivvv.top/gtcdpukcjh.html

PHP:  class User {}
来源：http://hz.gzhubu.top/gtdgzvdvyl.html

JS:   class User {}
来源：http://hz.ydzc1.top/gtngufonnq.html

TS:   class User { name: string = ""; }
来源：http://hz.xuetiantiany.cn/gtyjlrvqzn.html

Java: class User {}
来源：http://hz.jinghuilouyu.cn/gtjyoanesc.html

Go:   type User struct { Name string }
来源：http://hz.ywan-chungtsiang.top/gttbidvmyx.html

Ruby: class User; end
来源：http://hz.ydzc1.top/gtyfjydovz.html

C#:   class User {}
来源：http://hz.cqqwz.cn/gtdciivihc.html

[G02] 构造函数
来源：http://hz.chenjidiqi.icu/gtppuuxgst.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.shanyushiyangtech.top/gtmofgxylz.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hnxiangtu.top/gtprtvbjib.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zhiwuduotai.top/gtjnfqpyos.html

TS:   constructor(public name: string) {}
来源：http://hz.aibaodan.cn/gtadjgtetu.html

Java: User(String name) { this.name = name; }
来源：http://hz.cashguo.top/gtfyzkqqpg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.cdnleiting.top/gtxyibzfly.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.ywan-chungtsiang.top/gtyeyxqkqi.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zhengqikj.top/gtqevntkhz.html

[G03] 实例属性
来源：http://hz.cqqwz.cn/gtpxqnaguz.html

Py:   self.name = "x"
来源：http://hz.iojbl.cn/gtleqszjxt.html

PHP:  public string $name = "x";
来源：http://hz.chenzaomai.com/gtczbvrjyp.html

JS:   this.name = "x";
来源：http://hz.gotoacloud.top/gtjhqmlwfb.html

TS:   name: string = "x";
来源：http://hz.bjfxy.top/gtacjopzze.html

Java: private String name;
来源：http://hz.sysykeji.top/gtrboyqnad.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jinghuilouyu.cn/gtiyyctemj.html

Ruby: @name = "x"
来源：http://hz.sweek.top/gttkzxzfzb.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zhaomingkeji.xyz/gtvzvrarlr.html

[G04] 定义方法
来源：http://hz.nanxuanxn.top/gtarifswsj.html

Py:   def greet(self): return self.name
来源：http://hz.zhijiandao.cn/gtaqyryghy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.havefunace.top/gtpzedadwv.html

JS:   greet() { return this.name; }
来源：http://hz.zhaomingkeji.xyz/gtbftjpiny.html

TS:   greet(): string { return this.name; }
来源：http://hz.yangfankeji.com/gtdzqygpet.html

Java: String greet() { return name; }
来源：http://hz.yj20258888.top/gtrymdaofe.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zdqjudy.top/gtkavngoen.html

Ruby: def greet; @name; end
来源：http://hz.gaohongyu789.top/gtlwkcwrbe.html

C#:   public string Greet() => Name;
来源：http://hz.meibo888.top/gtrfqixkta.html

[G05] 继承
来源：http://hz.cashguo.top/gtaxyusolp.html

Py:   class Admin(User): pass
来源：http://hz.chenjidiqi.icu/gtjqjulujw.html

PHP:  class Admin extends User {}
来源：http://hz.andypj.xyz/gtzkkqwuca.html

JS:   class Admin extends User {}
来源：http://hz.gogol.net.cn/gtbdlqsgmm.html

TS:   class Admin extends User {}
来源：http://hz.andypj.xyz/gtsnjlxuax.html

Java: class Admin extends User {}
来源：http://hz.pycfn.com/gtqmxvaqmu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.cashguo.top/gtqjsxxgql.html

Ruby: class Admin < User; end
来源：http://hz.pengpengdd.cyou/gtejtssebq.html

C#:   class Admin : User {}
来源：http://hz.ywan-chungtsiang.top/gtsuqboajm.html

[G06] 重写方法
来源：http://hz.smart0.xyz/gtgrzseflg.html

Py:   def greet(self): return "admin"
来源：http://hz.jinyuanbaomall.cn/gtxmplliba.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.sufxvd.cn/gtwjbhqxsd.html

JS:   greet() { return "admin"; }
来源：http://hz.wangdashe.top/gtsvvstbap.html

TS:   greet(): string { return "admin"; }
来源：http://hz.snrcjt.cn/gtzxcsqxzn.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.nwbrower.top/gttlajpfaf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.hnxiangtu.top/gtqcnzvjzm.html

Ruby: def greet; "admin"; end
来源：http://hz.gotoacloud.top/gtydqgyrya.html

C#:   public override string Greet() => "admin";
来源：http://hz.ivvv.top/gtkmvkhxrv.html

[G07] 调用父类方法
来源：http://hz.svipenyu.cn/gtxybjgfit.html

Py:   super().greet()
来源：http://hz.gzhubu.top/gthotwylcq.html

PHP:  parent::greet();
来源：http://hz.gotoacloud.top/gtoxnngzct.html

JS:   super.greet();
来源：http://hz.feifeiyinyue.top/gtgyumdbyt.html

TS:   super.greet();
来源：http://hz.hongshengwenyu.top/gtvwijogey.html

Java: super.greet();
来源：http://hz.gogol.net.cn/gtzdcrjppf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yuanzhike.top/gtkwmejqnd.html

Ruby: super
来源：http://hz.c1oappe.top/gtwryxfbhe.html

C#:   base.Greet();
来源：http://hz.hfpthk.cn/gtivywfjom.html

[G08] 静态方法与属性
来源：http://hz.zhiwuduotai.top/gthgzaojrg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.shangyingyoupin.top/gtrbgvwceg.html

PHP:  public static function f() {}
来源：http://hz.jinghuilouyu.cn/gtebacrxdu.html

JS:   static f() {}
来源：http://hz.daria6918.cn/gtwowqvnzg.html

TS:   static f(): void {}
来源：http://hz.sxryk.cn/gtxxsyfsqw.html

Java: static void f() {}
来源：http://hz.birdmap.top/gtmkkaaszk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.hfpthk.cn/gtygmhfrht.html

Ruby: def self.f; end
来源：http://hz.daxiang520.top/gtonmqxeoh.html

C#:   public static void F() {}
来源：http://hz.chenzaomai.com/gtacqgkfjr.html

[G09] 接口 / 抽象类
来源：http://hz.hnxiangtu.top/gtcqkhdmhc.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.sysykeji.top/gtdsiwxpdi.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.daria6918.cn/gtcuadfzyb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zhaomingkeji.xyz/gtiojorwzw.html

TS:   interface Shape { area(): number; }
来源：http://hz.birdmap.top/gtoxypwbkq.html

Java: interface Shape { double area(); }
来源：http://hz.nanxinkj.top/gttzjjapoh.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.daria6918.cn/gtrbbeaxgv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jianghu66.top/gtcojdvgtz.html

C#:   interface IShape { double Area(); }
来源：http://hz.yvedp.cn/gtghlslbpn.html

[G10] 访问控制
来源：http://hz.zhixingplan.top/gtwhalrrmb.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhongyouzk.top/gtrsyjjnjz.html

PHP:  public / protected / private
来源：http://hz.ywan-chungtsiang.top/gtrcdiufie.html

JS:   #private 字段；其余公开
来源：http://hz.zhoulong.xyz/gtrlbmrzap.html

TS:   public / protected / private
来源：http://hz.shanyushiyangkeji.top/gtawpqsxtn.html

Java: public / protected / private / 默认包级
来源：http://hz.jqgfzy.top/gtevkazkeq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jyoumei.cn/gtzirbfbks.html

Ruby: public / protected / private
来源：http://hz.cqqwz.cn/gtllzwthhd.html

C#:   public / protected / private / internal
来源：http://hz.havefunace.top/gtavktfzeq.html

[G11] getter / setter
来源：http://hz.guannengcc.top/gtyviamqdy.html

Py:   @property 与 @x.setter
来源：http://hz.jqgufenzy.top/gtcqmzouuf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jlsjyb.cn/gtzziuapek.html

JS:   get name() { return this._name; }
来源：http://hz.haohaochexian.top/gtmjzphtco.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhengqikj.top/gtonyqhjzj.html

Java: public String getName() { return name; }
来源：http://hz.nanxuanxn.top/gtzxmxskty.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jinyuanbaomall.cn/gtmlldtcbq.html

Ruby: attr_accessor :name
来源：http://hz.havefunace.top/gtegxbjqqr.html

C#:   public string Name { get; set; }
来源：http://hz.cqqwz.cn/gtidijuobw.html

[G12] 对象转字符串
来源：http://hz.bjfxy.top/gtbdsjnmbu.html

Py:   def __str__(self): return self.name
来源：http://hz.redwolf501.top/gtjacznypd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.sweek.top/gtjjkclxds.html

JS:   toString() { return this.name; }
来源：http://hz.quarkkingdee.top/gtgngymtcy.html

TS:   toString(): string { return this.name; }
来源：http://hz.gaohongyu789.top/gtmxxfufyz.html

Java: @Override public String toString() { return name; }
来源：http://hz.pengpengdd.cyou/gtesljhfou.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.aizwys.cn/gtgjqtlktg.html

Ruby: def to_s; @name; end
来源：http://hz.xinyue.icu/gtcgztlfbc.html

C#:   public override string ToString() => Name;
来源：http://hz.pengpengdd.cyou/gtlixuetmb.html

[G13] 判断对象类型
来源：http://hz.xylfe.cn/gtonlyejff.html

Py:   isinstance(u, User)
来源：http://hz.shanyushiyangkeji.top/gtqlmfzppl.html

PHP:  $u instanceof User
来源：http://hz.c1oappe.top/gtnmsfeepp.html

JS:   u instanceof User
来源：http://hz.zhengqikj.top/gtidwvjbqk.html

TS:   u instanceof User
来源：http://hz.9152youxi.cn/gtntqlswys.html

Java: u instanceof User
来源：http://hz.hnxiangtu.top/gtphxwfnhl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.hysaishi.cn/gtfvpsasxi.html

Ruby: u.is_a?(User)
来源：http://hz.cdnleiting.top/gtmkkiyjqb.html

C#:   u is User
来源：http://hz.pycfn.com/gtdlcrknrj.html

[G14] 数据类 / record
来源：http://hz.mhx1999.top/gtshbxhbvh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.chenlongwang.top/gttiodhcgz.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.vqdsnc.cn/gtxaokaazr.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.0kj1m.cn/gtsiohftbs.html

TS:   type User = { name: string; age: number };
来源：http://hz.52xcode.cn/gtdfvrfobv.html

Java: record User(String name, int age) {}
来源：http://hz.guannengcc.top/gtwxrzbahe.html

Go:   type User struct { Name string; Age int }
来源：http://hz.fengsongda.top/gtqldgyprw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zhoulong.xyz/gtolxfyxxc.html

C#:   record User(string Name, int Age);
来源：http://hz.guannengcc.top/gtdmqssmpw.html

[G15] 枚举
来源：http://hz.nwbrower.top/gtaxmiwwpg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.wangdashe.top/gtuwlbntcp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.wangshuangyany.cn/gtevxoipcp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jinyuanbaomall.cn/gtyjhqrymo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shangyingyoupin.top/gtddnxvlyr.html

Java: enum Color { RED, GREEN }
来源：http://hz.kuanghao11.cn/gtqrmehbyi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.cdnleiting.top/gtfwedkctk.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zhaomingkeji.xyz/gtckqcuipd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yueranfly.top/gtkflgrwra.html

[G16] 对象转数组 / 字典
来源：http://hz.yvedp.cn/gtqkfokqzd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.mhx1999.top/gtismjmvxa.html

PHP:  get_object_vars($obj);
来源：http://hz.jinqigufen.top/gtshmjvfcs.html

JS:   Object.entries(obj)
来源：http://hz.andypj.xyz/gtuoefycrs.html

TS:   Object.entries(obj)
来源：http://hz.sysykeji.top/gtzheqcwpc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.wangdashe.top/gtbaubekys.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.zhaomingkeji.xyz/gtvgzoxsyi.html

Ruby: obj.instance_variables
来源：http://hz.ehwqpu.com/gtqyqwoolq.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.bjfxy.top/gtuiphxmlr.html

================================================================================
来源：http://hz.yj20258.top/gtifsdcpvn.html

H. 异常与错误处理
来源：http://hz.gzhubu.top/gtdunfwrtg.html

================================================================================
来源：http://hz.cheryme.top/gtzmbnvyeb.html

[H01] try / catch 基础
来源：http://hz.snrcjt.cn/gttugoqnpn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.hysaishi.cn/gtkfrwyibi.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.mhx1999.top/gtfnrgzhln.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yj202588.top/gtpxocrwse.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hysaishi.cn/gtnwfwmkah.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.shanyushiyangtech.top/gthdryrhsp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.pycfn.com/gtgfknidrp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.zhiwuduotai.top/gtcygommzk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.wangshuangyany.cn/gtshcpllex.html

[H02] finally / ensure 收尾
来源：http://hz.pycfn.com/gtlybxrtqu.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.cqqwz.cn/gtazmiisey.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hywenlv.cn/gtwbpjzduy.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhongyouzk.top/gtiutvkwsn.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.snrcjt.cn/gthrzxpezd.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.smart0.xyz/gtmzdjuewe.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.cucudq.cn/gtwcqogsgj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.hnxiangtu.top/gtohujutfs.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.xziqi.cn/gtveczclql.html

[H03] 主动抛出异常
来源：http://hz.yonumen.top/gtprtkbnij.html

Py:   raise ValueError("错误信息")
来源：http://hz.bjfxy.top/gtedbgycaw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jinyuanbaomall.cn/gtvjcdtlmu.html

JS:   throw new Error("错误信息");
来源：http://hz.xuanzx.com/gtrbhyppgk.html

TS:   throw new Error("错误信息");
来源：http://hz.mhx1999.top/gteykzzcae.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.shuidangran.top/gtmvdysxmw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yj202588.top/gtbtpwyrph.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zhengqikj.top/gtzuejmjnx.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.nanxuanxn.top/gtzdddmtvu.html

[H04] 自定义异常类型
来源：http://hz.jinyuanbaomall.cn/gtjwgwymuz.html

Py:   class MyError(Exception): pass
来源：http://hz.daria6918.cn/gtdllfplhk.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.shzxlz.cn/gtuyswnyyy.html

JS:   class MyError extends Error {}
来源：http://hz.cheryme.top/gtqpmsdols.html

TS:   class MyError extends Error {}
来源：http://hz.zhiwuduotai.top/gtfnglknfc.html

Java: class MyException extends RuntimeException {}
来源：http://hz.hongshengwenyu.top/gtsouayypl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.hammf.cn/gtobqhynzw.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhijiandao.cn/gtfslcnbla.html

C#:   class MyException : Exception {}
来源：http://hz.tanke756.top/gtelmtaxor.html

[H05] 捕获特定类型
来源：http://hz.gogol.net.cn/gtghwlxugd.html

Py:   except ValueError as e:
来源：http://hz.shangyingyoupin.top/gtwrxubbfn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.tian-w.cn/gtkbfdnbgq.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.ywan-chungtsiang.top/gtujhwqfjf.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.cashguo.top/gtzmbmkpve.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.dianchejie.cn/gtsckomqhu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yj202588.top/gtnxkqfsyl.html

Ruby: rescue ArgumentError => e
来源：http://hz.fengsongda.top/gtsvzurjjh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.cucudq.cn/gtitljxxsj.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zdqjudy.top/gturyawnjl.html

Py:   value = d.get("k") or default
来源：http://hz.hongshengwenyu.top/gtbattpwcc.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.316326.xyz/gtjqzbfyny.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.aizwys.cn/gtbfsmbdvm.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.guannengcc.top/gtvnambwzf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.9152youxi.cn/gthicnmllm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.daria6918.cn/gtxbsmaowl.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhijiandao.cn/gtjxfgdvub.html

C#:   obj?.A?.B ?? default
来源：http://hz.shanyushiyangtech.top/gtkgbfibgf.html

[H07] 断言
来源：http://hz.9152youxi.cn/gtgemlmnnx.html

Py:   assert x > 0, "必须为正"
来源：http://hz.aibaodan.cn/gtgelcrlpl.html

PHP:  assert($x > 0);
来源：http://hz.xinyue.icu/gtvjirnpjr.html

JS:   console.assert(x > 0);
来源：http://hz.shangyingyoupin.top/gtdgvbmduv.html

TS:   console.assert(x > 0);
来源：http://hz.guannengcc.top/gtsurvzshs.html

Java: assert x > 0 : "必须为正";
来源：http://hz.birdmap.top/gtpiugtjkn.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.dashuyun.cn/gtzddemcvf.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jinqigfzy.top/gtqpbtjstq.html

C#:   Debug.Assert(x > 0);
来源：http://hz.shuidangran.top/gtzppvgimy.html

[H08] 获取错误信息与堆栈
来源：http://hz.gogol.net.cn/gtobrukens.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.9152youxi.cn/gtbonegllc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.wangdashe.top/gtituosivw.html

JS:   e.message;  e.stack
来源：http://hz.hfpthk.cn/gtdsgkprqg.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.daria6918.cn/gtypcviwwb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yongpay.top/gtsxrkknan.html

Go:   err.Error()
来源：http://hz.fzhhl.top/gtdtvbfgfn.html

Ruby: e.message;  e.backtrace
来源：http://hz.yanxiufei.cn/gtduiakbjq.html

C#:   e.Message;  e.StackTrace
来源：http://hz.52xcode.cn/gtpbfwraig.html

[H09] 带错误码的异常
来源：http://hz.zhiwuduotai.top/gtvmquiodp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.cashguo.top/gtiducbvmn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.sufxvd.cn/gtmtmdlykn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.vqdsnc.cn/gtgvbmfthi.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.chenlongwang.top/gtycnofchd.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.gzhubu.top/gtmgwyrfvy.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.fzhhl.top/gtzdmhdrpf.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.ywan-chungtsiang.top/gtacqjuaxr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.cdnleiting.top/gtkuwdziyj.html

[H10] 资源自动释放
来源：http://hz.yanxiufei.cn/gtqetkuvym.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.sxryk.cn/gtbviahzma.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.52xcode.cn/gtylrapfsf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hfpthk.cn/gtoomhxypy.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yuanzhike.top/gtgszzssnd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.xingfuxueyuan.xyz/gtwidrqfbr.html

Go:   defer f.Close()
来源：http://hz.havefunace.top/gtdvuwjzhh.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zycfv.cn/gtazyixhwv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yuxming.cn/gtfkqxswwo.html

================================================================================
来源：http://hz.ybcxt.top/gtaidioprh.html

I. 正则表达式
来源：http://hz.feifeiyinyue.top/gttbpvaygg.html

================================================================================
来源：http://hz.0kj1m.cn/gtazyoukss.html

[I01] 判断是否匹配
来源：http://hz.daxiang520.top/gtlifjyywj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.wangshuangyany.cn/gtxhrrbpli.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.fengsongda.top/gtlslcfcjc.html

JS:   /\d+/.test(s)
来源：http://hz.yj202588.top/gtgvnowyra.html

TS:   /\d+/.test(s)
来源：http://hz.chenzaomai.com/gtyemcvmnp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.svipenyu.cn/gtbwbczxnu.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yj20258888.top/gtjouvkylj.html

Ruby: s.match?(/\d+/)
来源：http://hz.hammf.cn/gtidfosmrw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.shanyushiyangtech.top/gtolgigpnd.html

[I02] 提取所有匹配
来源：http://hz.jinghuilouyu.cn/gtjwvyghhv.html

Py:   re.findall(r"\d+", s)
来源：http://hz.bjfxy.top/gteyycofds.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.nanxuanxn.top/gtgdimafis.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhijiandao.cn/gttbiafgxi.html

TS:   s.match(/\d+/g)
来源：http://hz.vqdsnc.cn/gtozoeyxql.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.svipenyu.cn/gtxrdjyjgo.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.cqqwz.cn/gtxyuwvpin.html

Ruby: s.scan(/\d+/)
来源：http://hz.yj202588.top/gtnmroahfe.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hongshengwenyu.top/gtvibcwdse.html

[I03] 提取捕获分组
来源：http://hz.yueranfly.top/gtbilrlcyi.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zhoulong.xyz/gtgspiyblr.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.dashuyun.cn/gtkdbwdxdp.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yanxiufei.cn/gtqqyxjapn.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jqgfzy.top/gthaboylbu.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yanxiufei.cn/gttvpzgujq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yj20258.top/gtfmnwoqhl.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.9152youxi.cn/gtoajyiwbt.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jinghuilouyu.cn/gtgkecmabp.html

[I04] 正则替换
来源：http://hz.0kj1m.cn/gtwwzyptmj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yonumen.top/gtxleoygzn.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yonumen.top/gttnagicwd.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.guannengcc.top/gtofvpaxsw.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.cheryme.top/gtmxyrdbbe.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hfpthk.cn/gtycuutjdy.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.sysykeji.top/gtepyuhclx.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yuanzhike.top/gtlqxravwj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.zdqjudy.top/gtxrghdomx.html

[I05] 按正则拆分
来源：http://hz.cheryme.top/gtecmdjzbz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ydjk.org.cn/gtyshyyjot.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.sufxvd.cn/gtjseqncwt.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.52xcode.cn/gtwfjqondb.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.guannengcc.top/gtnvevzird.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jinqigufen.top/gtjoaspsid.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.hysaishi.cn/gtxosrgrbm.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jqgfzy.top/gtaigeowiu.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yangfankeji.com/gtkpwoqtlt.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yuxming.cn/gtvvsqonlk.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jqgfzy.top/gtestocnfc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.sufxvd.cn/gtixrcrsco.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gaohongyu789.top/gtgwzwdutt.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sweek.top/gthpdjdjqt.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.quarkkingdee.top/gtagldnhnk.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.nanxinkj.top/gtqesazgsj.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.sysykeji.top/gtifdyykib.html


<!-- 参考信息 -->