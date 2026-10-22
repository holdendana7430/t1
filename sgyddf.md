代发 wailian999

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2zpgukcmx.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2heobogou.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2zliknzto.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2jokddfxh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2gzrioekw.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2gxhfjgzw.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nxnrprxz.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xmafscou.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2qmrcyllk.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2dtdiwbsg.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2cbjpdgvn.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2sgfbbiqs.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2iccdytrk.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2odihomsf.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qnyotprn.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ukzgpkxu.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2dpnlxkse.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2bdrhmmez.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2bxpbmaxe.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2twshfcug.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2xceohndc.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2rwucsezp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lspifbnn.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2chtdzgqi.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfzsgvks.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tvfotvis.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2jrggyubv.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2fgqymgyh.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2iibusbxn.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2bnijuxbn.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2gextceco.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2yxsxkygo.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2grlvnfyk.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tuhyfzxp.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qhlsanny.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2zdabjxdn.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2sqoqucys.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2djbzkpxf.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2jmnlvlhc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2tgflelzy.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2ofshjblq.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2eqpkuyap.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2axygrrpx.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2obwdoreh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2pwwlfyhk.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2eouhqufj.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2uwtxyntx.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2xhzczjcz.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2zautohak.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2eknrxdol.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2jblzodua.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmtczfhz.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2bpznxoye.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2rqgibwjc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2xoxqaazm.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2ziiihbry.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2urwpfbkw.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2xdutsulj.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2qisroeem.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2idoxrynv.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2fjyibiyf.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2dafkjxds.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2eyvglqyd.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2yxymurwh.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2ivnpgkdf.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2niivrgec.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2luuskdlw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zarsmukv.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2oongvvxg.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2cxyrakmk.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hlitmvjw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2pobpmwlk.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2aplqzqlz.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2sgfjmxqf.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gktfhyam.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2unscacey.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2rtpaacsr.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2teafgcqo.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2fsnqumvf.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cewrqkjn.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2wlnitsrc.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2bhztgngg.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2synazpbx.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2fznwwffa.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2efntkgpo.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2dksinfij.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wtbpovfh.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rtyrtfod.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2pxryjtpp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2adwzkprr.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2oaxloevy.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2ymekbyto.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2peicajbu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2jbngugho.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2wmpvaksc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2xlzzgthc.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2rtykzscv.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2ktxphlqx.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2kxuksclo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2yluybcrm.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2xdqcypjd.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2hvivvgpj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2aayioeky.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2irbvigkb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2ivdwyysn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2soliguog.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2wtetwswi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2rvuotibm.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2iqxsnlyz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2jptouijn.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2unutjngx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2mocwnush.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2iwfnptdq.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ambuvnfw.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ndloavso.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2hggbcidu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2ncbxtdgb.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2olvqohis.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2tcpodyht.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bxhaepfi.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2zvamzpmo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kdclhagv.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2zxajzucx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2wxevybzv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2hxxynhhh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2tbhygqna.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2tfhghiqn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2ervqazdo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2svtkdqek.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2wevnmeat.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2bhcybbrl.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2hdvlwuim.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2xafvtqcx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2eattdzni.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mnfaajgb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mxdbkwdt.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2lxpashmc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2rcdvixts.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2iiugcyop.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oyoxwfza.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2mjvtjkzk.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2advlngjl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ocmowzby.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2wcbguqiv.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xdhiisln.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ghbvjyxp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2umywngtf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2sbulnave.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2lqrfjhha.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2ootrgsko.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2vmusllzg.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2qdbbjlyb.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2kbwupfbm.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2mvjqpdlg.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ouydpkdw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2ynhlnvpz.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2okwggwmk.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2xocgorpv.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2mhexmzrj.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2czzoaqdv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2xqtnnupt.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2izakyfcr.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qnbzfvpl.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wbcuuaha.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2lvwltdee.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2jtbjipai.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2xjfzhtja.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2xnstxgbj.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2wugbkszs.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2levvxaeu.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2mjrukgki.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2meqffakx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2npqidgkm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2ergvveqf.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2fofstpdj.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2gnxkmqog.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2gewmaabw.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2zgxldgku.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xrtghtke.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2knnpijrh.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xkoqnpyd.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2cqvriqdm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2zemeafhl.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2ezpgjxke.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ipjmpjvk.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2aygijnxf.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2mpqkousg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2yumhrdir.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2hrnnrree.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2imkmamds.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2lrcvtmas.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2jbgckjmr.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2cnpnjwwn.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2abmiwzyk.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2ugftuwyq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2tkmdxcbo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2niotkpgk.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2tkcuuvsv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2jmtzemva.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2tiqktcvm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2hjqpqncf.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2xkupbwmy.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2uygqtmsk.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2uhtumbmi.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2qncnjhai.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2uhnpvylc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2nlinhzrg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ytaopacu.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2ifxpkkeg.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2tccvejxy.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2afxvgqal.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lmbjftud.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oinxbapg.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2sclrmhcb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dneoidlb.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vcevcrmc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2yuzkcfgt.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zizniipt.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2jkvaepgk.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2fvjbzhcu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2hiwtbuei.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2ayfomeun.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2dajktqqa.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2bwutxmbj.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tdamjuuo.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ifvzhqpj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ihafawdk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2fkoimsud.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2xnxxlrtq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2wrcbyavt.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2lsrqpoiy.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2xpqihsmj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2duarwceq.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2ifzskhjk.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2ygcuucwb.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2auhogstd.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2usfozbdq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2jummvess.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2okyeckiq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2ikormjfo.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2havwuuyd.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2ksojadkb.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ssyxyelh.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2hmpglwmx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2eomladok.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2vbqfdngj.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2gakktvrm.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2zyxpoqht.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2njeapuaa.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2gemiaxrx.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2jxydurrq.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2gqzuckfx.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2ycbsnanb.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2fijqdosa.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2smuldbus.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2mvjupmqw.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2ipgjbyom.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2abhldkwh.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2bpjjhttm.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2mdzwwtuw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2keqkftgv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2yrgajxmk.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2xxjwaxqu.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2bcxrxaad.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2mxuwtfjc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2drdpwuco.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2pkcnibti.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2wcezagfj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2rexwkwmd.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2cdpqlzaa.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2xbrfurcd.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2jcydcqff.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2fdxhofsi.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2yqhjlqol.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2zksavsic.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2gbfvdtgc.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2hwpdezrh.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2jrcpmngy.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xbdswbzb.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2hdsorxcm.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2xkndnepp.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2jwzjbgvu.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2vljyqydr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2bcmkivxx.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2erkuwfel.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2kdksszbo.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2zouamgpw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cshqbjmo.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2crulmldr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fopnoymw.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2afjybmqb.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2zbgyrokd.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2vjqsawyp.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2rcztoevh.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2zwcjbubn.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2qfdynfmk.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2shrpaqkv.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2pxmlkeaz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2lilxusgx.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2zoypqpie.html


<!-- 参考信息 -->