代发 wailian999

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mrtaybfd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2rdwwktev.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2fqhysnji.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2xrrywjzr.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2vwleufjb.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2peraxtvy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jkmmcvwr.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwxaaapt.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zvkbcwnz.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jrlwwdnp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2cmfszvif.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2dgzeuhpk.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2piekamtq.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2vxyzuwvd.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2ktblneem.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zpzierxw.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2evezwdyl.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mzcmtihq.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2mwrmyxvg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2ymygpaoh.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2trwsuaes.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2yefnmkyo.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2mgmpjeeg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2ztuzdkwp.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2nltqphuf.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2ljyvcchr.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2sbemvsbb.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2uzgrqiyh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2vcnvpyol.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2lwpkffss.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2btrerlwx.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2pskyxtfu.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2qekfumkn.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2ceozfvch.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2okzyyhpv.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2ovpseoxu.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2daqtnwfc.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2tivogkkk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2samjzpan.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jjmimvzg.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2amxecucb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2uvjkhmau.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xqlsoygt.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2xolbbzwe.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xipgegww.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2bkgzxrmh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2fafpgxkw.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2dxjtdlpa.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2nnzvaxhj.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2zcbwlbgb.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2weemwgcn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2fdkcupsb.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rxrtdams.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ubngtwbh.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wqbrocrr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ohigznsm.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2swkomqpi.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2azqzgijx.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qkafuieu.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2gmjftocd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oofrnbsc.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ovfxorfg.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2knybtohj.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2njhzxlkq.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2jdnyomuv.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2jgtgwymp.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2xpihjlnp.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2mezxvsso.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2wbrbdonl.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mspgecgd.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wcwkwzfh.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2hmzyqaae.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rgixwkvi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2yilkvndb.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2iglzkmvo.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2zrdekfpy.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2qzvbhjmy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2zbxavyni.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2qmppipnn.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2esfjpebb.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2nejshfbu.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mosgxgst.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2vlbhulou.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2ipqhihqx.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2iwjbhelo.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2diilwphv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2qiphwddr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hgyzsmkf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2egzujnot.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2pjtplofa.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2lparevue.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2fptmeqjo.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2ugutfusv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2wvhtgxbk.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2dexjclsn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2wcptuupg.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2apdudmjc.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2rbaxdfbb.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2lwtjvsrb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2nvietpve.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2cauammti.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2ditxxhnk.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2wprkfdik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vtdlbutj.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2tpxywfzl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cffvhsbl.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2cdrkqzbn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2nkivtmem.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tqsjemvr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2zpsmewmj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2jkqokauk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2gvssocce.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2papkaiwf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2xcdipdml.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2cqqupzmu.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2uxluppgq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2hvmsfkxh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mcmzzcra.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wvhknbuf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2llmsuwei.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ravfuwgm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2orfpqpba.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2xhudynvy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xbfffszs.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2eltgddtk.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2avvotddx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2qujbvhqu.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zzkplfzb.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2pqcqdfpk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2arxzheeo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2qljrbfad.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2wbamfvxf.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mevyrpoz.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2kddvkicn.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2jdkcsjsu.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2zltrlmck.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2mcbqgehi.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2vclotyfq.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ugxfnidp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2lebknvql.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2twwcnifb.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2immfwbzh.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2deadmzmh.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2ztohxhyy.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2muofwoao.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2cxphjakq.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iurfaiju.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ybiiomiu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2icruikzm.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2lzzzdted.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2rkbjytlo.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2tyhwfrpt.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2twfwnxbd.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2rxagvqvu.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2rhhvdgww.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2hpqtxqls.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2phlqrzim.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2ietfsyko.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2hisjpbud.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2oyruckvp.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2krhyexyb.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2mckuyige.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2oglgwtok.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2uuethotk.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2jvyzdgsb.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2jyrlwuks.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2fslepakr.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2osnxuqzh.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qpqgtuex.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2ikyqgtwi.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2ctmiuzvu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2ssjhyxep.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2kgeetfep.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2bugdgoqk.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2jouvqnqy.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2uhjdnaas.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2ogiotxdd.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2yivprkwb.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2lgsqghhy.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2xuzbbher.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2oyxoxfxt.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2okqjvrhg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2vbrrdptm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2phtcbcvo.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2lvzgrsnj.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2bvswdzoy.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2vhiuxpsa.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2jkmjkity.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2nhxomted.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2eqzbzcsy.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2xcmysvuz.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2wayoctyh.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2ahjmdgka.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2cxwhykrk.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2sdpuyhfj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xovunhiq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2didmptny.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xqkzqyyn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yxzdiufu.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2vziolbmi.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2xuatoyrm.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rczgvmai.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2wbzniluy.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wucbedsz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2zpuazjfc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kysbxluo.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2awbkodrh.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ttzvqxcm.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tiakwqox.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2isgfjpqn.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2rmdtdshb.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2pkstxpnf.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2ocqmkegg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2zsvscsgi.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2qecllryo.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2omycaxfw.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wnvtmlsc.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2jtwnwkqi.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2xgflqkij.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2fqwdyoca.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2blbqplur.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2abdyrznu.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2qhlxfmsn.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2yoycjsdw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ztuztjug.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2wtkitigs.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2odybghzl.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ftbohffb.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xltvbqtl.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2noornkwl.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2zyyqkgpd.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2hcvjfqtg.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2kwxzkmyj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2rixbmvny.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2eaupyuta.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2rowwydsh.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2tozktnce.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rhorrgwu.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2etsovfcf.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2nmyxhrxf.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2egviepqx.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2avslwnbg.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2wxrgcsep.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2zpaqkrsp.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2oaxxiqts.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2wpvzzjat.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2zhzihhuk.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2ppduiyuu.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2iioiyxoy.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2iincmqiw.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2oyfcrjpc.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2cgfsnxrs.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2stghifdy.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2qwguawkv.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2yuzgxowa.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2ghfcqhso.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2vefxmkhf.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2pdtoasuq.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2srggkejf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2ucgxynrs.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2akdbyrka.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2rbvjpfjc.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2wcfxnuzh.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2wgebzzyf.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2gnrvxlvh.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2afmqrrso.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2wwvdffoc.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2fofqstpl.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2lxmngihm.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2kucymncg.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2bumfruap.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xahdmqtx.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2tuhcvjoc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jrjpqanz.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2awnmdmkc.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2avlpyefc.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2yzyokiww.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2jsmuotiy.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2mfmkgiyd.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2fycntmkn.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2otcgpzti.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2lmoogriv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2rgrflyqg.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2acyhyvzh.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2honuswxm.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2ewkqttqv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2ftdulnpf.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2nmpvnfrx.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2ntmrailn.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2ffbwcibj.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2qplpagyl.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2bicjgphk.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2iqeeegsr.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2pvxpvuvw.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2cjzehqhu.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2sjcuqdpf.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2jtwcbhxm.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2aetuxstt.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2gciiwymu.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2pzgewwon.html


<!-- 参考信息 -->