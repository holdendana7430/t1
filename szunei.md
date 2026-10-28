代发 wailian999

[G02] 构造函数
来源：http://hz.xylfe.cn/gtacqdtgyo.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.ppjwa.cn/gthptbouwd.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.xuetiantiany.cn/gtcbnhrrzn.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.sxryk.cn/gtdqczdgsk.html

TS:   constructor(public name: string) {}
来源：http://hz.gotoacloud.top/gtvvhirwcj.html

Java: User(String name) { this.name = name; }
来源：http://hz.hnxiangtu.top/gtknsdaoue.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.ybcxt.top/gthvriaiom.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.vqdsnc.cn/gtxlpjfspu.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jinghuilouyu.cn/gtlhnszhjx.html

[G03] 实例属性
来源：http://hz.mhx1999.top/gtyloamkrh.html

Py:   self.name = "x"
来源：http://hz.cdnleiting.top/gtlpachzdu.html

PHP:  public string $name = "x";
来源：http://hz.xziqi.cn/gtqodukbqg.html

JS:   this.name = "x";
来源：http://hz.yuanzhike.top/gtrvxrqwmu.html

TS:   name: string = "x";
来源：http://hz.hnxiangtu.top/gtnxlzhlpr.html

Java: private String name;
来源：http://hz.yvedp.cn/gtvplemfuy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jinqigufen.top/gtvildwsvl.html

Ruby: @name = "x"
来源：http://hz.zhongyouzk.top/gtudiknbza.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jinghuilouyu.cn/gtskyigsuq.html

[G04] 定义方法
来源：http://hz.gaohongyu789.top/gtzdcrcadc.html

Py:   def greet(self): return self.name
来源：http://hz.shzxlz.cn/gteastepgv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.xuanzx.com/gtelsibxeg.html

JS:   greet() { return this.name; }
来源：http://hz.xuetiantiany.cn/gtkecviszv.html

TS:   greet(): string { return this.name; }
来源：http://hz.xinyue.icu/gtnfghqtfj.html

Java: String greet() { return name; }
来源：http://hz.chenzaomai.com/gtkclqiyug.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ehwqpu.com/gtzkjpgsmo.html

Ruby: def greet; @name; end
来源：http://hz.cheryme.top/gtemxjoryi.html

C#:   public string Greet() => Name;
来源：http://hz.gotoacloud.top/gtirwwiwju.html

[G05] 继承
来源：http://hz.hysaishi.cn/gtoohqqbls.html

Py:   class Admin(User): pass
来源：http://hz.nanxuanxn.top/gtbthmkdwm.html

PHP:  class Admin extends User {}
来源：http://hz.zhijiandao.cn/gtqvynjnrg.html

JS:   class Admin extends User {}
来源：http://hz.zhijiandao.cn/gtmgtqyafr.html

TS:   class Admin extends User {}
来源：http://hz.wangshuangyany.cn/gtgzwkkact.html

Java: class Admin extends User {}
来源：http://hz.feifeiyinyue.top/gtiryjifyc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hywenlv.cn/gtcznokqcz.html

Ruby: class Admin < User; end
来源：http://hz.shanyushiyangtech.top/gtcgnyeuob.html

C#:   class Admin : User {}
来源：http://hz.jinqigfzy.top/gtpaqjspvz.html

[G06] 重写方法
来源：http://hz.shangyingyoupin.top/gtdovomuzn.html

Py:   def greet(self): return "admin"
来源：http://hz.yuanzhike.top/gtyhrlsrsa.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zdqjudy.top/gtxhevekuy.html

JS:   greet() { return "admin"; }
来源：http://hz.fzhhl.top/gtiorkvyxk.html

TS:   greet(): string { return "admin"; }
来源：http://hz.guannengcc.top/gtzojmswwr.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhongyouzk.top/gtzstdadux.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.cucudq.cn/gtnuocnkbm.html

Ruby: def greet; "admin"; end
来源：http://hz.yanxiufei.cn/gtxqhykhbt.html

C#:   public override string Greet() => "admin";
来源：http://hz.yvedp.cn/gtmnhwglwi.html

[G07] 调用父类方法
来源：http://hz.haohaochexian.top/gtykzmninu.html

Py:   super().greet()
来源：http://hz.c1oappe.top/gtwihmchff.html

PHP:  parent::greet();
来源：http://hz.jinqigufen.top/gtrztjpioc.html

JS:   super.greet();
来源：http://hz.nanxuanxn.top/gtozycflqy.html

TS:   super.greet();
来源：http://hz.zhengqikj.top/gtyctwreui.html

Java: super.greet();
来源：http://hz.tianlin.xyz/gtxxbdtxzu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.wangdashe.top/gtbpabtlot.html

Ruby: super
来源：http://hz.gaohongyu789.top/gtucxrhuva.html

C#:   base.Greet();
来源：http://hz.hysaishi.cn/gthoqhbvpf.html

[G08] 静态方法与属性
来源：http://hz.zdqjudy.top/gtoflorktu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jyoumei.cn/gthbvxyrqk.html

PHP:  public static function f() {}
来源：http://hz.xylfe.cn/gtozhozabg.html

JS:   static f() {}
来源：http://hz.yj202588.top/gtyexnbjqj.html

TS:   static f(): void {}
来源：http://hz.xinyue.icu/gtyrcudivb.html

Java: static void f() {}
来源：http://hz.ivvv.top/gtaecyjjor.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.hfpthk.cn/gtygebhjjs.html

Ruby: def self.f; end
来源：http://hz.jiagoushi.top/gtlsxbnasm.html

C#:   public static void F() {}
来源：http://hz.snrcjt.cn/gtkiqhxmku.html

[G09] 接口 / 抽象类
来源：http://hz.52xcode.cn/gtbohrwbzl.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.pengpengdd.cyou/gtopfyjuxg.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.hammf.cn/gtzdhloeeu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.kuanghao11.cn/gtkqlyljpp.html

TS:   interface Shape { area(): number; }
来源：http://hz.tian-w.cn/gtphfwziex.html

Java: interface Shape { double area(); }
来源：http://hz.jinghuilouyu.cn/gtkmelfxqn.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yonumen.top/gtduclxjea.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jinqigfzy.top/gtutjurbvt.html

C#:   interface IShape { double Area(); }
来源：http://hz.iojbl.cn/gtjuylypec.html

[G10] 访问控制
来源：http://hz.zhijiandao.cn/gtjcmkiymr.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.guowangkeji.top/gtcmdtqdyk.html

PHP:  public / protected / private
来源：http://hz.cqqwz.cn/gtlhverfmi.html

JS:   #private 字段；其余公开
来源：http://hz.shangyingyoupin.top/gttlmlezof.html

TS:   public / protected / private
来源：http://hz.xziqi.cn/gtapkirrzh.html

Java: public / protected / private / 默认包级
来源：http://hz.zhoulong.xyz/gtgkqtafse.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.gotoacloud.top/gtxponnmgb.html

Ruby: public / protected / private
来源：http://hz.hnxiangtu.top/gtfzrudomb.html

C#:   public / protected / private / internal
来源：http://hz.nanxuanxn.top/gttsyefqir.html

[G11] getter / setter
来源：http://hz.smart0.xyz/gthlosonsb.html

Py:   @property 与 @x.setter
来源：http://hz.hysaishi.cn/gthhoyyodr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.ydzc1.top/gtwlfuztxl.html

JS:   get name() { return this._name; }
来源：http://hz.xuanzx.com/gtrmkjhkwt.html

TS:   get name(): string { return this._name; }
来源：http://hz.guowangkeji.top/gtmzjlkadp.html

Java: public String getName() { return name; }
来源：http://hz.yvedp.cn/gttymjhbmc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.gotoacloud.top/gtyfqqshku.html

Ruby: attr_accessor :name
来源：http://hz.0kj1m.cn/gtddnpwdar.html

C#:   public string Name { get; set; }
来源：http://hz.feifeiyinyue.top/gtybcrrayi.html

[G12] 对象转字符串
来源：http://hz.tian-w.cn/gtvxzulzxx.html

Py:   def __str__(self): return self.name
来源：http://hz.yueranfly.top/gtlxrbmxdx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.dianchejie.cn/gtxezjstpx.html

JS:   toString() { return this.name; }
来源：http://hz.smart0.xyz/gtmlcbutox.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhongyouzk.top/gtoawowexu.html

Java: @Override public String toString() { return name; }
来源：http://hz.zycfv.cn/gtqaoukoqf.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.fzhhl.top/gtuchvvuav.html

Ruby: def to_s; @name; end
来源：http://hz.havefunace.top/gtlgzyihfv.html

C#:   public override string ToString() => Name;
来源：http://hz.ppjwa.cn/gtsevfpbjk.html

[G13] 判断对象类型
来源：http://hz.hnxiangtu.top/gtzzsnrnwa.html

Py:   isinstance(u, User)
来源：http://hz.xylfe.cn/gtwclzwvep.html

PHP:  $u instanceof User
来源：http://hz.jinyuanbaomall.cn/gtvzdfhliq.html

JS:   u instanceof User
来源：http://hz.hongshengwenyu.top/gtrnsdvifs.html

TS:   u instanceof User
来源：http://hz.sufxvd.cn/gtaqfpzkum.html

Java: u instanceof User
来源：http://hz.wangdashe.top/gtoabhssdd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zhijiandao.cn/gtsjofrxpn.html

Ruby: u.is_a?(User)
来源：http://hz.pengpengdd.cyou/gtynjuzbme.html

C#:   u is User
来源：http://hz.ywan-chungtsiang.top/gtepucsgdr.html

[G14] 数据类 / record
来源：http://hz.xuetiantiany.cn/gtwiusxpra.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zhengqikj.top/gtsjarpcdi.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zhaomingkeji.xyz/gtozunzjmd.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.daria6918.cn/gtoklixtav.html

TS:   type User = { name: string; age: number };
来源：http://hz.yongpay.top/gtqzotnhvq.html

Java: record User(String name, int age) {}
来源：http://hz.ehwqpu.com/gthcasxvjg.html

Go:   type User struct { Name string; Age int }
来源：http://hz.xuetiantiany.cn/gttgvcgeto.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zdqjudy.top/gtyiyrbcmx.html

C#:   record User(string Name, int Age);
来源：http://hz.cqqwz.cn/gtdozgenqk.html

[G15] 枚举
来源：http://hz.havefunace.top/gtphmbwadn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.wangdashe.top/gtuendnyvo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.nanxuanxn.top/gtjspecukn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.shanyushiyangkeji.top/gtnzezgfrp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ywan-chungtsiang.top/gtorpiwqrf.html

Java: enum Color { RED, GREEN }
来源：http://hz.iojbl.cn/gtnqhnlxpr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yj20258888.top/gtnvsssqrj.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yangfankeji.com/gtexohugjx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.nanxuanxn.top/gtnpeohmfa.html

[G16] 对象转数组 / 字典
来源：http://hz.yuanzhike.top/gtzczadcse.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.xingfuxueyuan.xyz/gtwduyjdnq.html

PHP:  get_object_vars($obj);
来源：http://hz.vqdsnc.cn/gtwfttyeos.html

JS:   Object.entries(obj)
来源：http://hz.aizwys.cn/gtysicheur.html

TS:   Object.entries(obj)
来源：http://hz.nwbrower.top/gtellkxnfg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhaomingkeji.xyz/gtrynzhxuy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.xinyue.icu/gtifkooand.html

Ruby: obj.instance_variables
来源：http://hz.shanyushiyangkeji.top/gtabdlbefp.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.shanyushiyangkeji.top/gtvpohumdl.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtjnxomnqv.html

H. 异常与错误处理
来源：http://hz.zdqjudy.top/gttdghdova.html

================================================================================
来源：http://hz.jinqigfzy.top/gthrjravhj.html

[H01] try / catch 基础
来源：http://hz.pengpengdd.cyou/gtcxrfwgrl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhoulong.xyz/gtxbpaloqp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hongshengwenyu.top/gtjjgnfcei.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.ivvv.top/gttvezxpvj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jinqigufen.top/gtkldpxylm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.cashguo.top/gtmzoomcng.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.redwolf501.top/gtpdlylqun.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.zhijiandao.cn/gtaibohrag.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yvedp.cn/gthemrbxmn.html

[H02] finally / ensure 收尾
来源：http://hz.daxiang520.top/gtwpbeyipz.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zhoulong.xyz/gtizxmwfhl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.nanxinkj.top/gtaanojafe.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.ydjk.org.cn/gtcwbcknlm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.andypj.xyz/gtjihosguo.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.ywan-chungtsiang.top/gtxarhfpcr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ehwqpu.com/gtnacnpwnl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.pengpengdd.cyou/gtehdnlygc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zdqjudy.top/gtuyxviddh.html

[H03] 主动抛出异常
来源：http://hz.hfpthk.cn/gtjmqftfyg.html

Py:   raise ValueError("错误信息")
来源：http://hz.snrcjt.cn/gtipfotgmw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.pycfn.com/gtbbylvsko.html

JS:   throw new Error("错误信息");
来源：http://hz.yvedp.cn/gtzyohpmxi.html

TS:   throw new Error("错误信息");
来源：http://hz.hammf.cn/gtdxzslfvr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jianghu66.top/gtovrhhcai.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.dianchejie.cn/gtilejkcwz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.smart0.xyz/gtopprcafe.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.316326.xyz/gtqxetpmkl.html

[H04] 自定义异常类型
来源：http://hz.chenjidiqi.icu/gtpaptcxeu.html

Py:   class MyError(Exception): pass
来源：http://hz.snrcjt.cn/gtsjnnsnhh.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yueranfly.top/gttmexvzhe.html

JS:   class MyError extends Error {}
来源：http://hz.mhx1999.top/gtayqsvgjn.html

TS:   class MyError extends Error {}
来源：http://hz.52xcode.cn/gtvvjdnogn.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jiagoushi.top/gtcrwdwkxk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jianghu66.top/gttsrdpjkb.html

Ruby: class MyError < StandardError; end
来源：http://hz.hnqzz.top/gtgdeknpdk.html

C#:   class MyException : Exception {}
来源：http://hz.hnxiangtu.top/gtsfokkhhl.html

[H05] 捕获特定类型
来源：http://hz.yongpay.top/gtvqdxokdj.html

Py:   except ValueError as e:
来源：http://hz.hfpthk.cn/gtcqpwvfdv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jinqigufen.top/gtbznexeot.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yueranfly.top/gtzmoxmcjr.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yanxiufei.cn/gtktlflajf.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.daxiang520.top/gtxzuzcpsv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.smart0.xyz/gtgnnlkiph.html

Ruby: rescue ArgumentError => e
来源：http://hz.hammf.cn/gtguyvamni.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yvedp.cn/gtzxtriaoa.html

[H06] 可选值 / 空值安全访问
来源：http://hz.wangdashe.top/gtsedrrema.html

Py:   value = d.get("k") or default
来源：http://hz.gaohongyu789.top/gtcdqmjskj.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hongshengwenyu.top/gtwvvnltmp.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.vqdsnc.cn/gtbbtyacdo.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jqgfzy.top/gtohizmeye.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.shanyushiyangkeji.top/gtkjgrxtzy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.svipenyu.cn/gttjxuldni.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jinqigfzy.top/gtgpltuysh.html

C#:   obj?.A?.B ?? default
来源：http://hz.yongpay.top/gtxzvggwnm.html

[H07] 断言
来源：http://hz.yanxiufei.cn/gtcayvihji.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zhongyouzk.top/gtujlfhpci.html

PHP:  assert($x > 0);
来源：http://hz.gogol.net.cn/gtzzwzukhj.html

JS:   console.assert(x > 0);
来源：http://hz.feifeiyinyue.top/gtbozihouj.html

TS:   console.assert(x > 0);
来源：http://hz.jinghuilouyu.cn/gtlcslvxvd.html

Java: assert x > 0 : "必须为正";
来源：http://hz.smart0.xyz/gtdrkwutrj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.mhx1999.top/gtxoffayld.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.wangshuangyany.cn/gtbhgqngml.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jyoumei.cn/gtqtxrsemv.html

[H08] 获取错误信息与堆栈
来源：http://hz.jlsjyb.cn/gtthokrhph.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zhengqikj.top/gtkitmxqbk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.nanxinkj.top/gtasxaauat.html

JS:   e.message;  e.stack
来源：http://hz.gzhubu.top/gtyfgushbw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.snrcjt.cn/gtzqerfdtr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zdqjudy.top/gtyoiubhid.html

Go:   err.Error()
来源：http://hz.chenlongwang.top/gtehpceoqb.html

Ruby: e.message;  e.backtrace
来源：http://hz.hfpthk.cn/gtovtybutp.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jinqigfzy.top/gtiltxeqdu.html

[H09] 带错误码的异常
来源：http://hz.yanxiufei.cn/gtpeztethx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.gaohongyu789.top/gtlfwrdyuq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ydzc1.top/gtjkgydszu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.chenjidiqi.icu/gtlqpgpmot.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.mhx1999.top/gtitsbypli.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yanxiufei.cn/gtsckwvsnv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zhengqikj.top/gtpnlccgoa.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jqgufenzy.top/gtxhqgjtuj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.tanke756.top/gtudhtmaqi.html

[H10] 资源自动释放
来源：http://hz.snrcjt.cn/gtkvacoeyo.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.ybcxt.top/gtrnnxcdmw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jqgfzy.top/gtgqxspumx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.tian-w.cn/gtttscgxdf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.52xcode.cn/gtfxweuhch.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.cucudq.cn/gtwsrvyccl.html

Go:   defer f.Close()
来源：http://hz.shangyingyoupin.top/gtpcsfdlqd.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.ehwqpu.com/gtlzgqpwks.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yj20258.top/gtmfisfves.html

================================================================================
来源：http://hz.guannengcc.top/gtiucqboxf.html

I. 正则表达式
来源：http://hz.gotoacloud.top/gtusqmujeo.html

================================================================================
来源：http://hz.jinqigufen.top/gtlkcbakdn.html

[I01] 判断是否匹配
来源：http://hz.yueranfly.top/gtefjiunlb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yangfankeji.com/gttfpellfk.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.svipenyu.cn/gtlbyakcnu.html

JS:   /\d+/.test(s)
来源：http://hz.jinghuilouyu.cn/gtlfyiaavh.html

TS:   /\d+/.test(s)
来源：http://hz.gzhubu.top/gtdijrnrdn.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jinghuilouyu.cn/gtrepctwnk.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.pengpengdd.cyou/gtobeedkso.html

Ruby: s.match?(/\d+/)
来源：http://hz.zycfv.cn/gtifsslkdk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.52xcode.cn/gtfjtustwo.html

[I02] 提取所有匹配
来源：http://hz.yangfankeji.com/gtyjrlgzyc.html

Py:   re.findall(r"\d+", s)
来源：http://hz.dashuyun.cn/gtwmkgxzsv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.andypj.xyz/gtxjboxhpx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.tianlin.xyz/gtjmwbcciq.html

TS:   s.match(/\d+/g)
来源：http://hz.havefunace.top/gtigbdxycp.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.gaohongyu789.top/gtzrtroxsx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.shanyushiyangkeji.top/gteachxpmf.html

Ruby: s.scan(/\d+/)
来源：http://hz.yj20258888.top/gtvihdyhir.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yueranfly.top/gtenqnwoxx.html

[I03] 提取捕获分组
来源：http://hz.tanke756.top/gtgomhaoaz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.xziqi.cn/gtsymrygks.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.haohaochexian.top/gtipinnlcc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zhiwuduotai.top/gtvmuprwst.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jyoumei.cn/gtzooxazzo.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.gaohongyu789.top/gtodmgapku.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.snrcjt.cn/gtalllkcyx.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yj20258888.top/gtkmmkabuf.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhongyouzk.top/gtpalolmwv.html

[I04] 正则替换
来源：http://hz.zdqjudy.top/gtjsltuiwg.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.havefunace.top/gtwkwbzlao.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.quarkkingdee.top/gtchdngbap.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.aibaodan.cn/gtgpsdgbgd.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhaomingkeji.xyz/gtpvqrnhyj.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.tanke756.top/gtwqbgmrhm.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.quarkkingdee.top/gtzlhoqtjd.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.gogol.net.cn/gticvclrqs.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.fzhhl.top/gthsucmusu.html

[I05] 按正则拆分
来源：http://hz.yj20258.top/gtjlfvajyy.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.9152youxi.cn/gtlgpdxwis.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hywenlv.cn/gtenrrcfyh.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.guowangkeji.top/gtokyuqssz.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.sweek.top/gtsbxnbxnz.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jqgufenzy.top/gtxzimbewq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jyoumei.cn/gtvukljzgl.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.havefunace.top/gtqjklmmzf.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yj20258.top/gtxzloyvrv.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.316326.xyz/gtpwsipctb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zhaomingkeji.xyz/gtchcbuzwf.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yongpay.top/gtubzdokwg.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.quarkkingdee.top/gtgxmrwker.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yvedp.cn/gtuflpvgam.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.wangshuangyany.cn/gtkexiysxo.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.52xcode.cn/gtvzjlhcjh.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.hongshengwenyu.top/gthivleygy.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yj202588.top/gthuglhmeb.html

[I07] 忽略大小写与多行模式
来源：http://hz.jyoumei.cn/gtcarefckf.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.haohaochexian.top/gteyawtuud.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.vqdsnc.cn/gtddgnsshm.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.ybcxt.top/gtpmqiabqt.html

TS:   /error/gim
来源：http://hz.0kj1m.cn/gtbhewbirp.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.pengpengdd.cyou/gtzouwlklr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.aibaodan.cn/gtukwxfnil.html

Ruby: s.scan(/error/i)
来源：http://hz.yuxming.cn/gtkdvimcok.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jianghu66.top/gtjvkrccoc.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.9152youxi.cn/gtuiqnsizd.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yvedp.cn/gtfoafulzf.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.gogol.net.cn/gtecnazish.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cdnleiting.top/gtjlypbyhb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jianghu66.top/gthobeenbw.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jyoumei.cn/gtzhvqiqwm.html


<!-- 参考信息 -->