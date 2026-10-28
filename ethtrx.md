代发 wailian999

Java: class User {}
来源：http://hz.52xcode.cn/gtpzegizrv.html

Go:   type User struct { Name string }
来源：http://hz.hnxiangtu.top/gtikautfzd.html

Ruby: class User; end
来源：http://hz.tanke756.top/gtjruehtlx.html

C#:   class User {}
来源：http://hz.cashguo.top/gtdprdwwbn.html

[G02] 构造函数
来源：http://hz.nanxinkj.top/gtnpsqugjb.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhixingplan.top/gtyrpyyfhk.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.shanyushiyangkeji.top/gtxznruakx.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.hnxiangtu.top/gtcdkeszbq.html

TS:   constructor(public name: string) {}
来源：http://hz.zhiwuduotai.top/gtjelngyyq.html

Java: User(String name) { this.name = name; }
来源：http://hz.jqgufenzy.top/gtfhvwolbo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.kuanghao11.cn/gtbrungphb.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yj20258888.top/gtodoaekkg.html

C#:   public User(string name) { Name = name; }
来源：http://hz.feifeiyinyue.top/gtfoljtjox.html

[G03] 实例属性
来源：http://hz.meibo888.top/gtsgazpmhe.html

Py:   self.name = "x"
来源：http://hz.0kj1m.cn/gtwzlvcfoz.html

PHP:  public string $name = "x";
来源：http://hz.yonumen.top/gtxxfbfdkq.html

JS:   this.name = "x";
来源：http://hz.ydzc1.top/gtdvfimvld.html

TS:   name: string = "x";
来源：http://hz.andypj.xyz/gtlcinjcpm.html

Java: private String name;
来源：http://hz.meibo888.top/gtyebfcenk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.pengpengdd.cyou/gttzjujcyq.html

Ruby: @name = "x"
来源：http://hz.yueranfly.top/gtbgusoxwm.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hysaishi.cn/gtftufieej.html

[G04] 定义方法
来源：http://hz.fzhhl.top/gtdtusvkmm.html

Py:   def greet(self): return self.name
来源：http://hz.zhixingplan.top/gtbldutcmz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.shangyingyoupin.top/gtarsxlpbm.html

JS:   greet() { return this.name; }
来源：http://hz.chenjidiqi.icu/gtqqnlbdbt.html

TS:   greet(): string { return this.name; }
来源：http://hz.gotoacloud.top/gtmnrgytpw.html

Java: String greet() { return name; }
来源：http://hz.xingfuxueyuan.xyz/gtplpwhzit.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zhengqikj.top/gtwnjkholx.html

Ruby: def greet; @name; end
来源：http://hz.jlsjyb.cn/gtzmsmubfs.html

C#:   public string Greet() => Name;
来源：http://hz.yj20258.top/gtnyzjuxjl.html

[G05] 继承
来源：http://hz.quarkkingdee.top/gtnsrljwpj.html

Py:   class Admin(User): pass
来源：http://hz.jianghu66.top/gthwwnqsbh.html

PHP:  class Admin extends User {}
来源：http://hz.sxryk.cn/gtlkxmwfjm.html

JS:   class Admin extends User {}
来源：http://hz.havefunace.top/gtojzpyhol.html

TS:   class Admin extends User {}
来源：http://hz.jianghu66.top/gtchuivqcf.html

Java: class Admin extends User {}
来源：http://hz.cheryme.top/gtfugnypdl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jinghuilouyu.cn/gtrevyntej.html

Ruby: class Admin < User; end
来源：http://hz.0kj1m.cn/gtkiuwpeuu.html

C#:   class Admin : User {}
来源：http://hz.quarkkingdee.top/gtterxmdte.html

[G06] 重写方法
来源：http://hz.meibo888.top/gtwlienkvo.html

Py:   def greet(self): return "admin"
来源：http://hz.9152youxi.cn/gtdbdrunzk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.pycfn.com/gtvmzcbqcu.html

JS:   greet() { return "admin"; }
来源：http://hz.hammf.cn/gthdxoymjf.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yonumen.top/gtjwnsaltn.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.haohaochexian.top/gtlovppfgp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yvedp.cn/gtkpbjmuxu.html

Ruby: def greet; "admin"; end
来源：http://hz.zhongyouzk.top/gtnzasemdd.html

C#:   public override string Greet() => "admin";
来源：http://hz.ydjk.org.cn/gtyvxlesma.html

[G07] 调用父类方法
来源：http://hz.chenjidiqi.icu/gtmwbuvfum.html

Py:   super().greet()
来源：http://hz.aizwys.cn/gtdiuqzcys.html

PHP:  parent::greet();
来源：http://hz.wangshuangyany.cn/gtxhqwemgt.html

JS:   super.greet();
来源：http://hz.9152youxi.cn/gtiaacylvh.html

TS:   super.greet();
来源：http://hz.c1oappe.top/gtrrenryas.html

Java: super.greet();
来源：http://hz.gotoacloud.top/gtfngdzczo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.chenzaomai.com/gtslzwpnqz.html

Ruby: super
来源：http://hz.aibaodan.cn/gtaysrxzwt.html

C#:   base.Greet();
来源：http://hz.shanyushiyangkeji.top/gteboatfqd.html

[G08] 静态方法与属性
来源：http://hz.xziqi.cn/gtdwtrrtmz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.pycfn.com/gthakcofrp.html

PHP:  public static function f() {}
来源：http://hz.guowangkeji.top/gtxesgngac.html

JS:   static f() {}
来源：http://hz.smart0.xyz/gtldaksojd.html

TS:   static f(): void {}
来源：http://hz.pycfn.com/gtzcgvgryl.html

Java: static void f() {}
来源：http://hz.quarkkingdee.top/gtjafanqsb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.kuanghao11.cn/gtpzlupfhb.html

Ruby: def self.f; end
来源：http://hz.snrcjt.cn/gtfcqafyww.html

C#:   public static void F() {}
来源：http://hz.chenjidiqi.icu/gterarzsgy.html

[G09] 接口 / 抽象类
来源：http://hz.pycfn.com/gtqywuqhgo.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.cashguo.top/gtotdtxpof.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.chenzaomai.com/gtjnuricvp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.hnqzz.top/gtxqmmcztb.html

TS:   interface Shape { area(): number; }
来源：http://hz.snrcjt.cn/gtnzfnkoit.html

Java: interface Shape { double area(); }
来源：http://hz.birdmap.top/gtlkvkhhpx.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.ppjwa.cn/gtdabupipw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.aizwys.cn/gtymvvsxex.html

C#:   interface IShape { double Area(); }
来源：http://hz.nanxuanxn.top/gtgklrmyqh.html

[G10] 访问控制
来源：http://hz.yangfankeji.com/gtzcjkpvev.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhaomingkeji.xyz/gtinfilaep.html

PHP:  public / protected / private
来源：http://hz.chenzaomai.com/gtuiklipgx.html

JS:   #private 字段；其余公开
来源：http://hz.jqgfzy.top/gtmqmpfdii.html

TS:   public / protected / private
来源：http://hz.wangdashe.top/gtovbdgceh.html

Java: public / protected / private / 默认包级
来源：http://hz.0kj1m.cn/gtpqycfunm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhiwuduotai.top/gtsvvaxwsr.html

Ruby: public / protected / private
来源：http://hz.tianlin.xyz/gtabcgcmhn.html

C#:   public / protected / private / internal
来源：http://hz.nanxuanxn.top/gtjlqxjlza.html

[G11] getter / setter
来源：http://hz.xuanzx.com/gturxnvgba.html

Py:   @property 与 @x.setter
来源：http://hz.zhiwuduotai.top/gtefpgibdu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.nwbrower.top/gtietrucrv.html

JS:   get name() { return this._name; }
来源：http://hz.bjfxy.top/gtanoepcpr.html

TS:   get name(): string { return this._name; }
来源：http://hz.tianlin.xyz/gtwfricivl.html

Java: public String getName() { return name; }
来源：http://hz.svipenyu.cn/gtwjdcnmtp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.quarkkingdee.top/gtowrwnjlw.html

Ruby: attr_accessor :name
来源：http://hz.iojbl.cn/gtgrmhtzvc.html

C#:   public string Name { get; set; }
来源：http://hz.kuanghao11.cn/gtznhjtbrl.html

[G12] 对象转字符串
来源：http://hz.jiagoushi.top/gtqewmokcn.html

Py:   def __str__(self): return self.name
来源：http://hz.jianghu66.top/gtnzirefxo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yonumen.top/gtmwmhmepb.html

JS:   toString() { return this.name; }
来源：http://hz.yvedp.cn/gtjonibjee.html

TS:   toString(): string { return this.name; }
来源：http://hz.jinqigfzy.top/gtclhftokf.html

Java: @Override public String toString() { return name; }
来源：http://hz.316326.xyz/gtyyxyorqk.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.nanxinkj.top/gtziiqdwft.html

Ruby: def to_s; @name; end
来源：http://hz.aibaodan.cn/gthavdxlvb.html

C#:   public override string ToString() => Name;
来源：http://hz.shanyushiyangtech.top/gtatligchq.html

[G13] 判断对象类型
来源：http://hz.0kj1m.cn/gtamlwnjif.html

Py:   isinstance(u, User)
来源：http://hz.jianghu66.top/gtbpsxukyf.html

PHP:  $u instanceof User
来源：http://hz.guannengcc.top/gtkqbjnebi.html

JS:   u instanceof User
来源：http://hz.snrcjt.cn/gtzwvkzric.html

TS:   u instanceof User
来源：http://hz.hnqzz.top/gtcjvugjnd.html

Java: u instanceof User
来源：http://hz.pengpengdd.cyou/gtwdrduhfr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.nwbrower.top/gtztpqapmr.html

Ruby: u.is_a?(User)
来源：http://hz.nanxuanxn.top/gtgymzoubv.html

C#:   u is User
来源：http://hz.zycfv.cn/gtcpkayvmb.html

[G14] 数据类 / record
来源：http://hz.jiagoushi.top/gtvxxgntme.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.redwolf501.top/gtixcvdknd.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.chenjidiqi.icu/gtqxeyigxx.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.dianchejie.cn/gtwqvqwwpy.html

TS:   type User = { name: string; age: number };
来源：http://hz.chenzaomai.com/gtwrqoyggg.html

Java: record User(String name, int age) {}
来源：http://hz.xuetiantiany.cn/gtsfekphtp.html

Go:   type User struct { Name string; Age int }
来源：http://hz.pengpengdd.cyou/gtjwvddelp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.sufxvd.cn/gtuzrwzzwq.html

C#:   record User(string Name, int Age);
来源：http://hz.ivvv.top/gtuxhhaket.html

[G15] 枚举
来源：http://hz.pengpengdd.cyou/gtcavdwomi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.ydjk.org.cn/gtouxnuxgu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.xylfe.cn/gtjodknoop.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jinqigufen.top/gtjvtdogmp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.9152youxi.cn/gtjvfhlzzn.html

Java: enum Color { RED, GREEN }
来源：http://hz.shanyushiyangtech.top/gtewgcqhkn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.gaohongyu789.top/gtpklbbtbv.html

Ruby: Color = %i[red green].freeze
来源：http://hz.nwbrower.top/gtwzagfkil.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.wangshuangyany.cn/gtdqymehng.html

[G16] 对象转数组 / 字典
来源：http://hz.hammf.cn/gttggeszmk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jianghu66.top/gtkgaqkxlb.html

PHP:  get_object_vars($obj);
来源：http://hz.hywenlv.cn/gthxapcrkb.html

JS:   Object.entries(obj)
来源：http://hz.gotoacloud.top/gtttrvzosx.html

TS:   Object.entries(obj)
来源：http://hz.jlsjyb.cn/gtxbsfxatx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhoulong.xyz/gtptqchwlf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.tanke756.top/gtcmvuprar.html

Ruby: obj.instance_variables
来源：http://hz.pycfn.com/gtjbcdkkff.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhoulong.xyz/gtspknzpub.html

================================================================================
来源：http://hz.jqgufenzy.top/gtdtkjzcbc.html

H. 异常与错误处理
来源：http://hz.shangyingyoupin.top/gthtffftqo.html

================================================================================
来源：http://hz.ppjwa.cn/gtiftynjyc.html

[H01] try / catch 基础
来源：http://hz.hywenlv.cn/gtdybohzge.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.shanyushiyangkeji.top/gtrfqbrors.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zhiwuduotai.top/gtvmdylngy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.sysykeji.top/gtzwrnretz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jinqigfzy.top/gtssdrkjhr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.aizwys.cn/gtwlqqkkqg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.0kj1m.cn/gtecqgmnvj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.fengsongda.top/gtpzsbzhew.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.xuanzx.com/gtsblazdwn.html

[H02] finally / ensure 收尾
来源：http://hz.nanxinkj.top/gtxtoizloa.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yangfankeji.com/gtqdkwrrab.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xuetiantiany.cn/gtvbweosgt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.ppjwa.cn/gtvasddank.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jinyuanbaomall.cn/gtexkkmnxt.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.smart0.xyz/gtjftesyds.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jinqigufen.top/gtlsjqfyme.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ydjk.org.cn/gtatdpxtnr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.chenjidiqi.icu/gtxarybjrx.html

[H03] 主动抛出异常
来源：http://hz.wangshuangyany.cn/gtvpbmysia.html

Py:   raise ValueError("错误信息")
来源：http://hz.zhoulong.xyz/gtwnmqqhkt.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.meibo888.top/gtyeciyojt.html

JS:   throw new Error("错误信息");
来源：http://hz.hnxiangtu.top/gtyrmgoizn.html

TS:   throw new Error("错误信息");
来源：http://hz.xziqi.cn/gtomnoiflo.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.tianlin.xyz/gtbuzdggjx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.gogol.net.cn/gtzrofwohc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.shanyushiyangtech.top/gtdaswclnr.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.meibo888.top/gtycqznday.html

[H04] 自定义异常类型
来源：http://hz.zhiwuduotai.top/gtussbqkeo.html

Py:   class MyError(Exception): pass
来源：http://hz.hfpthk.cn/gtdoedcinc.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.xinyue.icu/gtctrekyxf.html

JS:   class MyError extends Error {}
来源：http://hz.zhoulong.xyz/gtnwxlmyif.html

TS:   class MyError extends Error {}
来源：http://hz.yuanzhike.top/gtmgbjuclf.html

Java: class MyException extends RuntimeException {}
来源：http://hz.sysykeji.top/gtodnaleqs.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.xylfe.cn/gtqwdcjjnz.html

Ruby: class MyError < StandardError; end
来源：http://hz.jinqigufen.top/gtywosbooa.html

C#:   class MyException : Exception {}
来源：http://hz.iojbl.cn/gtxapvfidh.html

[H05] 捕获特定类型
来源：http://hz.fzhhl.top/gtakusnqst.html

Py:   except ValueError as e:
来源：http://hz.yuxming.cn/gtlhygzibl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.nanxuanxn.top/gtdroyeshg.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.ppjwa.cn/gtwkftxjyo.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yanxiufei.cn/gtcjwhbvge.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.chenzaomai.com/gtlixwkdtu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.9152youxi.cn/gtzlasmtit.html

Ruby: rescue ArgumentError => e
来源：http://hz.yuanzhike.top/gtrsyqztwp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.sxryk.cn/gtqbmqinps.html

[H06] 可选值 / 空值安全访问
来源：http://hz.cqqwz.cn/gtbszxpsso.html

Py:   value = d.get("k") or default
来源：http://hz.xinyue.icu/gtbwmwmkfg.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhengqikj.top/gtodrzlggu.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jinqigfzy.top/gtylwdqrus.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zdqjudy.top/gttgckhrzz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.shzxlz.cn/gtvsmetocl.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.kuanghao11.cn/gtunnbvodc.html

Ruby: d&.dig(:a, :b)
来源：http://hz.fzhhl.top/gthuohxtxz.html

C#:   obj?.A?.B ?? default
来源：http://hz.zhengqikj.top/gtwiqirnht.html

[H07] 断言
来源：http://hz.zhiwuduotai.top/gtqezticgr.html

Py:   assert x > 0, "必须为正"
来源：http://hz.aibaodan.cn/gtrdvxinpv.html

PHP:  assert($x > 0);
来源：http://hz.dianchejie.cn/gtmaongnwp.html

JS:   console.assert(x > 0);
来源：http://hz.nanxuanxn.top/gtyilmkwjw.html

TS:   console.assert(x > 0);
来源：http://hz.9152youxi.cn/gtutijzzxx.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yvedp.cn/gtykgcoygw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.birdmap.top/gtzqyvudtj.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yanxiufei.cn/gtxcrzgcrm.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zhixingplan.top/gtvzryatig.html

[H08] 获取错误信息与堆栈
来源：http://hz.zdqjudy.top/gtyuxbumaa.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jianghu66.top/gtsifbzjxi.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.xuetiantiany.cn/gtwtdyvrlo.html

JS:   e.message;  e.stack
来源：http://hz.zhixingplan.top/gtdjjmzukq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yonumen.top/gtwzxsuare.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.tianlin.xyz/gtzvojvmke.html

Go:   err.Error()
来源：http://hz.0kj1m.cn/gtpjfxbmkq.html

Ruby: e.message;  e.backtrace
来源：http://hz.0kj1m.cn/gtjfglqjri.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yj20258888.top/gtqxggmbem.html

[H09] 带错误码的异常
来源：http://hz.hnqzz.top/gtvmeymnls.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.fengsongda.top/gttbjxagqs.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ehwqpu.com/gturaaranu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.ppjwa.cn/gtonnstzaz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.meibo888.top/gtzspjmdbj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.quarkkingdee.top/gtbxqulkdp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.daxiang520.top/gtrhbcocgj.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.fzhhl.top/gtceocnxgx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhongyouzk.top/gtwvoebefo.html

[H10] 资源自动释放
来源：http://hz.jqgfzy.top/gtjedaawzk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.birdmap.top/gtolouizom.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yuxming.cn/gtamkcgrpn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.fengsongda.top/gtiihppivu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jqgufenzy.top/gtpxjrcnbn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zhaomingkeji.xyz/gtgtamnhpa.html

Go:   defer f.Close()
来源：http://hz.hywenlv.cn/gtrbkpzjqq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zhixingplan.top/gtzrpjzmqn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ybcxt.top/gtpnykbrja.html

================================================================================
来源：http://hz.shzxlz.cn/gtlqlwhucm.html

I. 正则表达式
来源：http://hz.ehwqpu.com/gtienyxpjo.html

================================================================================
来源：http://hz.dianchejie.cn/gtaifbmnbu.html

[I01] 判断是否匹配
来源：http://hz.9152youxi.cn/gtbmvddrfy.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhiwuduotai.top/gtdmfuaagg.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.havefunace.top/gtxruhxpyl.html

JS:   /\d+/.test(s)
来源：http://hz.sweek.top/gtzoowgnwm.html

TS:   /\d+/.test(s)
来源：http://hz.zhoulong.xyz/gtsgmucqci.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ehwqpu.com/gtgadntjds.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yj20258888.top/gthvflpkqa.html

Ruby: s.match?(/\d+/)
来源：http://hz.yuxming.cn/gttfukpxql.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yuxming.cn/gtsykqbtxr.html

[I02] 提取所有匹配
来源：http://hz.tian-w.cn/gtxgqsbxwp.html

Py:   re.findall(r"\d+", s)
来源：http://hz.xylfe.cn/gtgmouzscs.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yj202588.top/gtjlzfmbno.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.havefunace.top/gtqfpmvzwy.html

TS:   s.match(/\d+/g)
来源：http://hz.shanyushiyangtech.top/gtdzzcdtlu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.shanyushiyangkeji.top/gtvnkyzdis.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.xuetiantiany.cn/gtsfpjwgwg.html

Ruby: s.scan(/\d+/)
来源：http://hz.xuetiantiany.cn/gtlxovfofz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zdqjudy.top/gttgkeqydp.html

[I03] 提取捕获分组
来源：http://hz.daxiang520.top/gtdzfbrkba.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.cqqwz.cn/gthuwlafcp.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.ydjk.org.cn/gtcwwyorsy.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.wangshuangyany.cn/gtajvqiawq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.shangyingyoupin.top/gtnwfdnwye.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.andypj.xyz/gteofgndcz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.dianchejie.cn/gttbmnhhaj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.birdmap.top/gtatpiwtuc.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.ehwqpu.com/gtsadiqynp.html

[I04] 正则替换
来源：http://hz.jyoumei.cn/gtifpewgru.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.ivvv.top/gtfywczufj.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.redwolf501.top/gtbvlychjg.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.aibaodan.cn/gtuuzmdbns.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhoulong.xyz/gtqlamazke.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.gaohongyu789.top/gtayzoddmt.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.gotoacloud.top/gtblpatfdv.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.birdmap.top/gtecxlbwfg.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.gzhubu.top/gtzwqxhxor.html

[I05] 按正则拆分
来源：http://hz.xingfuxueyuan.xyz/gtrwnmxasl.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.svipenyu.cn/gtzruttgzz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.andypj.xyz/gtgvmeaaai.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.daxiang520.top/gtilgezrnt.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jinyuanbaomall.cn/gtlkxurlvz.html

Java: s.split("\\s*,\\s*")
来源：http://hz.c1oappe.top/gtrkauikwc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.hammf.cn/gtuadojiau.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.hnxiangtu.top/gtstkowlli.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.9152youxi.cn/gtckjcveem.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.nanxuanxn.top/gtiddrpqcc.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.iojbl.cn/gtzfnokqjk.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.nwbrower.top/gtxllmcokj.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinghuilouyu.cn/gtfjmeornq.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sxryk.cn/gtwwpzuvel.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.wangdashe.top/gtcunsjtkw.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.pengpengdd.cyou/gtvrpuhcvn.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.hnqzz.top/gtxpchfhym.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ydzc1.top/gtexnsgcrm.html

[I07] 忽略大小写与多行模式
来源：http://hz.316326.xyz/gtuaynhtem.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jyoumei.cn/gtbwxneqjx.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.quarkkingdee.top/gtgyllhatn.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zhixingplan.top/gtfyhlhecy.html

TS:   /error/gim
来源：http://hz.cdnleiting.top/gtavhbdpzf.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zhixingplan.top/gtvkhmmrkl.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.smart0.xyz/gtflcoconz.html

Ruby: s.scan(/error/i)
来源：http://hz.yuxming.cn/gtsetmrjpw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yongpay.top/gtcpfweejc.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.pengpengdd.cyou/gtzxajqhfn.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.aibaodan.cn/gthtepswig.html


<!-- 参考信息 -->