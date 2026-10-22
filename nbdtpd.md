代发 wailian999

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ndlqztxy.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2izxlynoz.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2mukfjrdj.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2uxsmfyfq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2xarqmaee.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hrdghnxa.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eebofhyu.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgdladgn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2hrtiooiv.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2cugtblwk.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2jflgawmy.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2yjbmvxti.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2snlvcpvg.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kmztygwl.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qymatlgs.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mmefdnuz.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2livruhul.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2fqjfsfby.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2lwelatbc.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2ernpkrpg.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2qluypstn.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2geuznuui.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wupkoadc.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xipygcxt.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ieecsxgq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ibkmlxxh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2rnhukiuk.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2usfspmur.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2jzkincaz.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2tdxwovyy.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2ceqjnutb.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2hdbtmysd.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2uumhljrt.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2yyiwmbqw.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2mgtzdszq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2hcqvzbsu.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2fixnmcnb.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2iigurfsy.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2aysiefou.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2fhsdbsje.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2wxlsskac.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mtpriiqc.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2hjdaejyv.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2gpzuwsba.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2pxcbrwae.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2dkwwkbto.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2pznaloyk.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2iqplrswv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2gidxklpk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2opjutfbm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2czldifdy.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2ibcqwohl.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hqlfjjcp.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2eeohqioe.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2hincfidk.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2tfcthrbm.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2eoafhkay.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2iezpyyfl.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2udxqniqf.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2xoapdhwk.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2utielbdx.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2uyklsovv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2ghcjkqcq.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rlrcdqcv.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2uqqwwqjo.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2syseihfm.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2czagpzjt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gsxhmsgi.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2jkhuzytl.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tdjzwdhg.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cnisqjhj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2dmqvgpsd.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2oectnizk.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2cshiylss.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fwevgkng.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2yuggifwj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ckswpjmq.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qntzsofw.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bqwghyty.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfzufsor.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ilwzmuhs.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2wwzyzdzk.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2cucqoctd.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2bltbewqv.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2iyjdboqh.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wogpsagv.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2fsrtzcfv.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2liufdkeo.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2adbjpnhh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2tqygxegd.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2dkczvvoc.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2bqohyifg.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2pmvreiry.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2yekueotl.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2ohaqkdvm.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2guuosdvi.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2ugttxryp.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wcjbfsjk.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2pvkursxd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2rdrdxhdl.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2pfvjjoah.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2dpgsojnr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2kxvyfquz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gplrtkwx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2ydqoycjx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2qmjkvyst.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2dmprifvq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2zgdwtevl.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2gdmophve.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2lxedzmsr.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2kjglkvgh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2qcptgygf.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2sagconxx.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2chwopyxd.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2zjmnjryu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2atwllcda.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2swwrcjmp.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2jmatuaxv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2jpothxrc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2arbmxrkl.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2kpmcrdqk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2peonypii.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2yvtxahte.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2alnjmjlp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2myyoncxi.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2lsogkeat.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2evzspbxg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2krkjxgye.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2gapfsxfl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2orykvmul.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2vihsblvk.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2iaegduvt.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2usihwsyc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ygcxujde.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kgpphehb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2grrvoxxv.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cnzgzuev.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2qeykipsz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2kfirheym.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2hanzrprn.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2etkioklw.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2okpndufl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wqjxbajb.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2erydajpv.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2aideyxee.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2nckgyuyk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2fhxocdbm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2xubzagku.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ltcmvbuu.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2immpwqkb.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2ymvzbfvq.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2lmiormck.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2hnrqvsnk.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2fitgikrd.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2gkqgacwn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2vspfkxrv.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2knczsdir.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2bvfeywpg.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2ybksiidw.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2znuvcklf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2ykpenmwc.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2azfrbuvl.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ovqxvigb.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2efkutspv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2ziabqkef.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2vmeshvlo.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fpwaywmc.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2oxrujcoz.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2ddvatfxb.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2lntmcaqa.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2belhgicp.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ugxytlxo.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2ichltbkn.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2qqodwder.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2gevttjkx.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2aukyomsj.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2auyvoeov.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2tkbwfxlv.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dktfklya.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jolhtlsf.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2alvurwoh.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2oaxaqamy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2qneppazq.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2ujsjcvzm.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2eypsqtqd.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2gkurrnpl.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2gksucxbm.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2sxkmkcpi.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2igldxpyx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2hrsanpja.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2gogsaijs.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2vkalrhfg.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2vvnzkwkt.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2zltyppxt.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2smaplcvh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2tixgsidi.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2cvgqlfcz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2vtgwlcld.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2ueyqrohv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2psuexybb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2yypkpzko.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2frwugheg.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2tsadwbvx.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2bdhgmenw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2wiacwdew.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2zhujkern.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2hnsyucag.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2ryzcdcqv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2hljjfuyv.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2aligiuob.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2bxijaupq.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zulgsihr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nlxogcrh.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2emziicwb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mytcnipd.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lphynvvw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2uwygfmps.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ggbkczcj.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dmyygajz.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2rnzxpxuk.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2egrerrth.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2wfjwtsgx.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2bcdhbvsj.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ziyfzdru.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2fxpbcleb.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2nbdyaizz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2pmgcnjet.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2hudkdlnh.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2xdcrmrfg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2atqsdpkx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2zxbjoigh.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2xulhusgx.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fwdngtds.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2kiljcfxw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2ruwokacd.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2asbwyvjs.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2renwxjwj.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2zlplbgfe.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2sclekwnh.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2rsomabhc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2ucqkqauk.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2fwcgkjly.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2ovsnwsug.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2xhzgaqms.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2oudnsrbo.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2slnapudr.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2fozfdjig.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2lhirntev.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2xvfnqfis.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2owbeljpp.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2xfbyxdgf.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2eivklmnv.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2tbioejkd.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2fsusfivw.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2zmzvjzsf.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2ovsurydz.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2ksghrurd.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2fabggcck.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2dnydpjiz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2uztxvhtd.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2muyjglha.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2lhnmdgzs.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2ndnntgfh.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2aynftokt.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2vujbogjf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2wpbacvtz.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2zcaowalx.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2ucrmredu.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2vnucavws.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2spswxqmz.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2lojugmce.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2qcvmedor.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2plpsvfuu.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2vafnaqtc.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2ldfgwifk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2afeixafd.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2lwvgcllv.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2rfxfyndj.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2vkkcsmya.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2ijsqrpil.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2pdfzlzzv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2hwiaepsl.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2xesokfvy.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2alesfcco.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2fengokfs.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2xwdzxzzs.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2xvfkzwic.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pyqvbixo.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2uiqeavtr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pbmnkwby.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2aeqmfsuo.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2anekgrbj.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2pihjevrp.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2akuuzqcb.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2yvyqovjc.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2vrbhntez.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2kpemcbsp.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2yifaafpw.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2byqmszmj.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2gtfqueft.html


<!-- 参考信息 -->