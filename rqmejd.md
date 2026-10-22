代发 wailian999

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2fmdwzzxe.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2kzzbgwkh.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2diqcvtsl.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2kbldzhhe.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwnpixpj.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nemdrjey.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2heabkcvr.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nktizfwi.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2fliwpoju.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2rzvyhnfv.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2fmdnxfxt.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2hfztxour.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2sagymqsd.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2encwwkjv.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ebktsytb.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fmroxuuc.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ngwmztkr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2pnccfojx.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2vxwjbhoj.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2zvzojvvl.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2ubhkgdyj.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2bahlhxca.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnphymyu.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2tpopvikd.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ovkyvxlj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qlxrekaa.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2zpjmpdsl.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2kjkqhafw.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2nktgczqj.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2ojowubvx.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2ucszmjqc.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xxdczfxs.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2sontqkgi.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2dbcoyqjl.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2resmuhit.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2muvwbfks.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2vnnfqtzz.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2crqjpqea.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2zkmkwuwh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2bhpdiedk.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2etotrddm.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2xyduszvx.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2tplwdohr.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bjxmtfbh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2hpmnpreg.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2dqpuchmb.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2urzmvjdr.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2tpyoohhk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2threzlmr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2lizfucyp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2szwdhgej.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2premqgsp.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2qyzvdajl.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2pjfvxiva.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ynrvuamm.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hovmsrkt.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2txswiqzq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2hibvtgyw.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2fqwvhrfw.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2bvcodqrz.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2gqtjmzmh.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2priagumy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2bvjztwvw.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2vsiaqedz.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2tbfkzsjo.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2hdbvtevr.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2xnqclhla.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uiforsgf.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qusqbfns.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qwcsvinx.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtiipmyn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2liauimqm.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2duktdoea.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2alesuqtt.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ddomvmxx.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2fdsxqygp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tebxigdy.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tfqfprub.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2hfqkwmfu.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjfdiftt.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2wgroiujp.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2rqgblowa.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ccjuaarr.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2xkeunyuo.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2filyukym.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2boplnphj.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2bbqdwblo.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2kvjeyxos.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ikqlxlyz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2raixvtvn.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2azrsordu.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2tilsvvqw.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2mqxlfkmf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2huxisaxk.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2evgdrcru.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2kpufjard.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2foimlbdr.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pdmsgqvq.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2bahirhez.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2utiemoue.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2bjjhgnga.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2mmsykzpx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2tprusxui.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2ziltvtad.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2urgxzzvj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2xjrzuoky.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2mpnscbrw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2rfdrdije.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2xbocgnmf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2inaxplcc.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2vkmoshsx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2scigygqu.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2emlqizva.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2nwfkzdyd.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2gvslecuj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2lxhrsumz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2evjvxcyq.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2xhcsdiyq.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ddxridol.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2glkqlimq.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2gqpxckbm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wgcvvbre.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2qucppepq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2hijgxzzu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2btnptkmn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2hcwpizrw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2qsoivqyf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2fofrqtsr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2xhkevrbg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2zrjwdcze.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2ijzjsvar.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2lkqrcuvo.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2netuerru.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2klgugaxt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qvuysjsx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zrmubere.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2glslemhg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2tifqhlzd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2ncswhgtb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tnoenfce.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2jxnqmhhb.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2polpjnbi.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mrlfesdw.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xfcgeqys.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zuydfkgh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dctbxxvq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2gvaemtew.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2dwpdnsud.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ultfyoid.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2cdwiggjd.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2cxvlewqa.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2vmrsjqdg.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2tuepkozj.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2xleffkkt.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2nosemiap.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2fzpwykbi.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2pjvcpklm.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2gmpkawgk.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2gorubxvm.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2nbsqtbvr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2efrqrjey.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2klwmudjr.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2jnairgnl.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2egjlazzi.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2pjhcjedn.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2seuhdkgz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aixkqxtx.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2qybzkkyx.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2xvstdhab.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2wufthvlz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ddffoayx.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2krgmylfa.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2vjfmouom.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2muptvinq.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2roudzdhm.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2gvtoaeye.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2tcxetaai.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2rpcgwrug.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2cleysdwd.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2qmdcixuf.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hzgvrdih.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2mtfiniyw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2rvrrrccz.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2medkwsci.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fywkhirb.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2iqllbkpq.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2bjcjiqug.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2ekulviia.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2mhpzqzno.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2nusshfde.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2kghibvnd.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2bwmslcya.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2mksgzpuy.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2nnaxrzwl.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2gfilajzx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2lrikohoa.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ypdyksgb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2mthuwpmo.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2skccklbh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2pgffflbv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2hnhysxkc.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2cfmdshsr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2wvprmtiw.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2znvuhyfn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2fhvdgdti.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2dgvpuqzo.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2jnnaapkc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2wbdtfbwh.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2nuynteap.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2leqkghry.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2hftjzkvv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kxmxkyjk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zdnzivsp.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2vuyqbyev.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xisrsfxt.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hglaqasw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2tislhzzk.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2moesapto.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iweikmqw.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tpkfnneq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2qgsgfqhm.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2ccrsadbh.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2zbcpssrx.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2isdeqwqr.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2eisjglgw.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2vapquthn.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2vnqpqewj.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2vnywmpqr.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2erqhymon.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jadtmxze.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2bdqvhkdm.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2cunngudj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ylnvocvh.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2dynblusn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2nwcbyfhf.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2fymgwerf.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2peruamzi.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2wcxpgfia.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ghvhuied.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2hnigzpcj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2qpnefszo.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2nexxhnkq.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2svtbpfks.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2elzztnqz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zkehhshv.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ivdzixnu.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2shbdopxy.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2suhtgdyw.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2fcovitcc.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2nitjcdwq.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2cbxeowix.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2jlzyujvu.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2nuhnnsiw.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2wyrqnnzs.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2hhikkcuc.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2qlrusxbm.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2uooxplcw.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2jnikkbsf.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2ptigeknv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2kxkifrfl.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2trbwmusx.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2pmcssnnt.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2ygynlmda.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2euzfnffz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2vyjtcmqs.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2bjnqeoyf.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2vdqgthou.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2vqgzydnr.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2sqwheamd.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2enrzmxef.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2dnrclxjv.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2nyyqufmz.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2dgxbdwjm.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2cmjthqxc.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2qwnzkbyz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2frukvzwf.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2zxozvpdl.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2orosadfd.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2rlcthhoi.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2thgqhusd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2owmqqkru.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2bjqipzoe.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2spuqanga.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2cordkmok.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2cqrdwrof.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2klbmbxid.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2fyspgvvk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bccihclj.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2ghsnvioj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zienyqng.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2cidiqpso.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2azfgfeoy.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2xomnfhxr.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2urisuyer.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2tjgwjqvw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2apqkfcpa.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2hqcccozi.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2uarttbqh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2sdwygnlt.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2zcfumfnu.html


<!-- 参考信息 -->