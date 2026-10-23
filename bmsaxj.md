代发 wailian999

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3xwzzvydk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3labwcaky.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3ogqbbxln.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3cdojavey.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbwdojua.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3njiuioua.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3bfyxtpqu.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxgryhpz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ietmrdrz.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ommqvdyp.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3wffqpaqv.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3tfnzmegp.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3jdwwrfvs.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vkigjkqd.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vxgbculh.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3uynwbetk.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hknpgwaz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3yeebjdra.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3jykekglp.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3qpclpbsr.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3atdxtauh.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3nitppdxx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqyrqyuk.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3nxigrwju.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3sayzfdud.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ickzmwgt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3mizlinuq.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3txhgyxag.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3tghxqnts.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3wujlmuyy.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3rvqxysht.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3bqxvgihv.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fofydiwg.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hzubdaol.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3akpbsdwy.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3ewljseah.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3uipgxcnk.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3cmrhhwim.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3lkslvbcy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3pmfcmkqi.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3rhithbxy.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3cchgxsiy.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3nrcswyfk.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xxtlbpqg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3dseyjpgd.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3updnwnry.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3dejlgogr.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3tbovvrqp.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3adcgtuqq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmbfdybl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3ochcidhx.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3yqlbcspj.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3opqxcivj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3wynstjfe.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3jwyfxvdi.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3yungonxn.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3fgjifcka.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3lblbbofo.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3hcomozjs.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3wxsyaidy.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ryoctzss.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3flbspqog.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3ktxhsxxl.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ahbonojy.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3favhdhid.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3emxgmvon.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3qgtebalo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3atzkhmjn.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3yxztxhjc.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3wwqjskcq.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mcooactn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ymekyepv.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3degqprni.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3icyqdoxl.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ivutkntf.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3mmjpvgzj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3fjjepcdp.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3drpolpak.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lltfehwz.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jrbkhmas.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3bpgnuole.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3wlblnbhe.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3qrsgckzs.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3izofvdkg.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3hvqllpwu.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3aepwsasu.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ixxhpbxy.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3brxamzcb.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3mjempgej.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3vlzrkxld.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3bbqbtdty.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3ktpfcnlb.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3jnmudxce.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3tvuxvgxh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3cujcftqq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3afbapevf.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3xqcbzviq.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3ziefjvab.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3umkwrvbn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3qatydbxt.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3dbzdtswx.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3vkhzfjwy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3hszyppde.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3bylbnyyi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3fngrxkro.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3huctbdsn.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3jiimodvg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3mknzlfnq.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3miuwwexl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3pnoowclg.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3jepyujuq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3iwslltei.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3hkygtkun.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cuinumrq.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3urbcblqf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3jgwfhxtf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3fmzuwavj.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3pykjlzyf.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3skmhkcqc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qrxtxjqp.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3eldmzmww.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tuqpkhja.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3oajworak.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3gqqcthpe.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fibpxuyp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3pusdsgpk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3bpzfpalo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3inbmlfqj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3abbjztii.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3guhprddf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3vytfbhab.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3ncewivhs.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3hqedxhyo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ovngzdri.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vlvimulp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3heidddts.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fgbyxeck.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3wadslevf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3fbzxbqzs.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vxwcwnza.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3dipezgin.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3spiyuckc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vetmseyt.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3blweckad.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3gpehcsfz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3uoyfcruh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3blfrajhv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3zzwuqagr.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ljfgwvjs.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3xyistuwa.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3nhwmkldc.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3cbcriwzz.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3kzvgekjk.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3fabxlczn.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3aqorvtbw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3jauzgfhe.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3tslksita.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3vjsrvmxz.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3rnfzvhfj.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3xnzzhryf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3bwzzczrc.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3nofkjftj.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vqtfbmlk.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3lmdrwxjg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3xahvdebc.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3iiglnloz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3dtewcusy.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3njclkqfg.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3zljqaooj.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3cqqvdcls.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3uqithuml.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3srjrepan.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3rihnbfib.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3yhwhwcgc.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3keieybcr.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3dtapaxwe.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3yoyluvwp.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3pymmxggy.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3xptbbxcj.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3kebkmuyv.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bjqedbsh.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3kvkypofh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3ahklgloo.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3sqvagkym.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3dzarundy.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3vulneozj.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3oivqfino.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3vbyywctl.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3whfoyfbt.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3pbyvpnte.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3ntiolyzo.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3kqppkczc.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3yktsndyq.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3cssnscji.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3yedswbob.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3rfhryixo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3gldqpruc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3fauaodkd.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3gtilehps.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3vncfjnns.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3bgcwyhvq.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3smnnmuzj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3qysfcylr.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3vvpcpspv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3fuhbgmvn.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3grjwxuvd.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3pkpehvda.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3slaazvfc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3jyctiewo.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3pqnedmts.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3jfatsqeu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lflojvzz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bdkuypus.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3sfehmkbp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xbugvhov.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3yfaiwcxv.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3vhosghep.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ktuctpbq.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uxygfuje.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3cimwkgmh.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3rpxketks.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3ugfvbktp.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3lvpzebfh.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3xuzliuqc.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3xyuertkz.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3iwegdech.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3anoifgfg.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3hmdrqdew.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ipkyvsgc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kpwubvap.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3weppbmjq.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3efdtmkgt.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vnlagsri.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3nojtwnqn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qjsfaebh.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3yeshclyq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3gtewdskq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3hpjenkfg.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3wetipyxk.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3cczdlusi.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3szunsaml.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3utghwbkb.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3jpnmymbz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ohhswqev.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3vqmbicrl.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3xahixdgw.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3gxxjnyam.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3kberxczn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3pfvcuthj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3vbnaigib.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3bhrgcovc.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3yjnvjkvi.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3gdftqeok.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3juhtcina.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3icphxauy.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3qvnfcsmx.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3xebkobzq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ckscdrvr.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3bewxjqux.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3xytxzuje.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3jncjlchk.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3ujyrhhgk.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3qcyslprd.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3udqknamu.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3hwtlkkfz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3jgyyuwfr.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3jmlmnzeb.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3flyhqfvj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3kdewvwew.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3ijhemzrp.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3mrcjzuzh.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3laxoovhj.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3orkokian.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3gpyhptxm.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3bptudwik.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3gqscjlck.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3tjppsuwi.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3pwwfovib.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ajkxcrvw.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3ojpiscsc.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3oogrrkep.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ydpkbpcd.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3amkbdiit.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3dxlvcvjb.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3anahdciy.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3xyttfywe.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3imlvyifu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lxndbccj.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3btljvvdn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yqdoqojd.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3skaqepox.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3zelqffay.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3iduyvzdz.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3zhjljiae.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3nbjwvhqe.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3orrdpqhl.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3zvhojubs.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3jfixvopo.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3ldnqdszv.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ydrzmzji.html


<!-- 参考信息 -->