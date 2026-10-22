代发 wailian999

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2nkjimcsh.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2neelxcne.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2otlsrbyt.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2hrjulxxp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dcajgoar.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddclgrij.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2pjlmpoud.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ioawiqpb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2sjycbtuq.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2iiuxikcd.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2oviarjpo.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2idshqxln.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2aesomrqn.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jtewsnfq.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dpsbnhzi.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2yvltoebb.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2umduinaz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2jzmswpmo.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2emyrokow.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qbttdrey.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2tgjudotg.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2douezbkr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mepeblpr.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2evsuibxq.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gaqntlun.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ijbklpcn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2kytjbtju.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2ttijuyry.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2bvoboaud.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2ojloqdzs.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2itskxqdb.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kdfwapxa.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lahakcff.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2iimylcxv.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2hbwipwyc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2cbpwawvs.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2xfthieom.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2slhzupgn.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2awhfvxtk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2wpcxyccp.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2liwangkj.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2fdoxyraw.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2aehsyepf.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2kmnyaola.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2otajsdym.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2dlwojdmk.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lgpaxikq.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2pebhgont.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2qhdczfkw.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2shsrxtnm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2ujsiltya.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2bxngsfic.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2kmklkfje.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2wllelmah.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2pigssxvy.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2qqfvyxhh.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2fryigkby.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2wglvzuiu.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2hntoyncj.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2cvdeaeug.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xgoiqmre.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2hwsdjtbz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2mbwohmkd.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2wvypqrkv.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2kuqphnbu.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2ssniwfbd.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2buhppjxb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2abniuujf.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fftscupw.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tigllprk.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fxzseazt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2qazzciof.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2zujgbsbq.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2pzzivabm.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2wxxbqceg.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2vqzqeigt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2dqutysex.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2gvhxuojt.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2sccktwij.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cktooqsk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2thjaghsz.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2bvajugom.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2uwwgpmbm.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2cjdlbjgc.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2bygoswqz.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2lxzduvtx.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ewxrtkux.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ssaewcjk.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2lmqtymlr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2hmrrqmjk.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2evqfqwed.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2jczmdpmf.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2vaycbnng.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2xmkiesgp.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2kwtevqgc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2ixdtmute.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2xyvdmsiu.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gcfofmtm.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2fwysnmuy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2zugshigj.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2gzksvcjy.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2xragzbsp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ofkbuuqa.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2dzivblrx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2ezsznbqn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pgnlhqai.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2wurwikjg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2vqwiazpa.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2xkbdsjub.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2oiwtjisu.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2eplhmfew.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2qapokinh.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2tyhlpfhm.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uskiuqdc.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ymeuvmij.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2wsxqklua.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2mloqmxly.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2gzaxgjqc.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2mwgwrvei.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2slvzkpgw.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2bggbqsnw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2veaxbntq.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2bnfatmwj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2iszndggc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2junlpyvx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2tdzfwpkn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2wvkqxiil.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2saolgbqw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2zbcnrlfv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2zyqqcxmz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2tthitzzm.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2hitluxmu.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2cfgapjdj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oeauatee.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bhxblnxd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2szcmigys.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ylnofrdf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2fzegrqie.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2wajlqart.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tyrzdxkr.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2yghncwit.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2usriukcj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2nemplqqd.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2pocbrbit.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ucdvixmf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2qehfsoop.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2xvcqcjna.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2xwburcqx.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dfgmwmwp.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2tzdbceox.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2pomzvjdb.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2llrqvuhq.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2wzmddsyl.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2bynfwanc.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2vxqhuqqo.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2fauhpssx.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2ctvrvnhv.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2epjlhjda.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2nmyeocxa.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2brthndcd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2sucoqjnf.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2halrpbsm.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mxkgipit.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fxpxksgw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2pdkpjndp.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2sflekhob.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2cdblhqmt.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2rnrwygmu.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2vnutdubk.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2pcpdeqaq.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2emdmncrc.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2mrfnkwya.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2loyftlid.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2rlngkkba.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2wqmypihw.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2vmwvgsie.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2shohrkue.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2djfbzyga.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kfwofyrs.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ckinqdwc.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ydvhqlzk.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2lqkzqjad.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2hrkxjjsh.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2sbcbxntn.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2dxwjseum.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2zfuusqkz.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2myangfyj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2xjhamiim.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2afbqaxfq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2nkektnwn.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2mimmfhit.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2ayeygaul.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2urhzrfab.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2mrbgzsxn.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2zbkhzshj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2vttygcaw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2blzcnchq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2vhluwqux.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2thcxjunl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2lxwplgia.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2jopolwee.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2hnndujuy.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2ljvifqik.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2mkejjpjx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2blpuipaf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2evufuoqx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2odvqyhxs.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2lxeehyfs.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2fnbwgcnc.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2yovzqfma.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2igntftpu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2apnytfzs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mdmohuxs.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2iowwrxvx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zgmrezgo.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2siskpddy.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2fbehtbmz.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bqkloghk.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2lzhvkrvn.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qpfyfdtm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2kysbcqrs.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2koqqvtda.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2wbitufgs.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2jpdpidmu.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zlkcbmbu.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2kbldlprc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2zsqdgyaj.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2kwujgqmd.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2xuuvqade.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pwhufwzq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2qctnnmot.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2vqejutkv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ctuvxjku.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2taksifni.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2bjaohjsk.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2notrpols.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2ukcgccxt.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2onbvnguo.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2vgssaguo.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2zgpwaexr.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2yujvjedl.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2qnfigixs.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2rqozqirr.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2hzgmmkio.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2uhnhrfko.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2ivoyjzma.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2vqlvangd.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2anbmruie.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2kyhwlilg.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2apcywuph.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2dotkvpkr.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2wgfrrall.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2uadzncrl.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2eiuxjlfs.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2jvljdfud.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2ykjxpoqt.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2ntgussba.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2qvekjjgn.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2lkzbzvos.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2uhdruwtu.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2jqblodrn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ubsvmjef.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2eecagfgt.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2vyixovhc.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2yjqlxlnm.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2wtjytvud.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2zencnmja.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2lrwpcfza.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ojtgujxo.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2ouuzkidl.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2eevtmqrt.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2pprkrpfb.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2holclssj.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2onowoknf.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2buudpekn.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2sgmqxhot.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2luupreoz.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2fxqfhfkq.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2ktsfwpgi.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2uwrjozql.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2jvpomkzl.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2awluxodb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2cbovzxbe.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2ccfcyhwg.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2leynbriy.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2oejwsdqs.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2hzhzfqhp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2izqezenb.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2qztezuxu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mwzekodm.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2wgajqxus.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2aamveqdl.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2ctxpwwqk.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2cqmiquuk.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2kqfkityw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2gstrxxoi.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2eppcfsyp.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2osrqcdzk.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2vomokwmm.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2fkmcorus.html


<!-- 参考信息 -->