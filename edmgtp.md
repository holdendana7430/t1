代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3psmraquy.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3maqgnzfa.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3xhhdjtzm.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jjqyictm.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3borhkhad.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3mmhqneye.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3zygiapnc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3ajhrtcqr.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3xparxamk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3nqctpoye.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3zahglhiv.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3kdvfipib.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3amnbsvdm.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bebpplnm.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxlyvpyi.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vtphaswe.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3nmumymir.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3vrqduwna.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3qtngnkkh.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3ymlyaqfx.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3nyuinbxo.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3sslwsrdz.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vyamoqcc.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3kaeruhut.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3byawxdam.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3rahovucl.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3iddlbeeg.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3tyazilky.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3bqfltxfe.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3kuzaubhx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3opqiewrb.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vfjxzowf.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qprrzjpa.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3caswlyqt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3ueirrxov.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3ivjswith.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3yswdkujy.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3ujwhenxc.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3setvmzcv.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3kdpahehz.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3sfyewqzx.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3dhjzscgp.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3occigxpw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3xdqqpyuo.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3tlbzhdrm.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rlepocrt.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3kaqzqfon.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3kifkigxw.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3izgskqyu.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3radaijdh.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3hibzjkzb.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3ygazjjyw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3ewarirsx.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3obgzllax.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hrmnelfo.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3pkhkiyow.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3vxhkuukx.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwktjlhm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3olnqgtpd.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3niceaskk.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ipunyays.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3eesiegxz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3gzuztflm.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3yvzfidgr.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3pofwsfjq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3uqgtyere.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3gckgbsgq.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3ztplxebr.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3hbxeqdts.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3iskqukvy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3ysgsatoy.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3yunfntes.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3erknujyx.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3dfphiyne.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3qxlttzbo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3txytdlak.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvjhmukf.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xxdkahqr.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3aiclxwhe.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3bagdivwi.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3vpndubxz.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmljvvtz.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3gprmiynd.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3hsuwmyfe.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3qjfzphws.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqtysynj.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rbmymzox.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ljixdpqp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3zjegxgyi.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3aakyazjq.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3fuckponi.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3hrabhtcr.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3edjamnwh.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3iupaxweo.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3uuuruxos.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vstevuoh.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wqduwsxp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3oucuplfw.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3jutbtzai.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3lsvwcpwc.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3gkyrgiop.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3jiqbnald.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3rphufsrz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3egzodqmq.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3ohvtmxyu.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3kwetycsc.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3oetecujv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3vbnakqpz.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3nzqgblht.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ehowbjpr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3lluolbvv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovgulihs.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3ospvepsq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ezpowtmt.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3lhbzewiy.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3zuwuomko.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3mvekgiwr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3oafiruoo.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3zjcoryqd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3crgqicqz.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3yxqpfqbf.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uxzslmhi.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3imsjqmok.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3qfnlcvgr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3uzoyaqex.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3qcybbyij.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3nlxjyfbl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rrhozilm.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3cchmdcke.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jloexfqy.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3hfbiwtjs.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3axhtftjj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3pbolrrub.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3zofyhtth.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3xjdtmtvw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3yvgpnrgj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3cymwycdw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3gjhetbyh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3itwlcbyd.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3utytqhwt.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3zuesgbqc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ytrwmihv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ryramyvz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xgxfylrl.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mxfsasen.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3bikqgoph.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3ticrouht.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rivefzqc.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3gjourjbw.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3lyibkrdx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vauyhhyx.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qlrkreza.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3eglqmdlf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3cspmguvy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3ovbhqvqj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3qneysiia.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hxdeaxqo.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3nudyikzm.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3khemviow.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ukbknjsb.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3tkksbvea.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3khypczba.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3feezszek.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3oxiqnurq.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3aqkzetfm.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3lwfpgpfb.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3bxbagomn.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3ljwveljy.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3vyjsmqqt.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qfvchkbw.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3bbrmqbll.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3uxhlqxrf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3gawoufct.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3rjvuvzmx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3rsonsdya.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3fpclishu.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3pywwjlpc.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3cmkhwgra.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3czzncchz.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3nvqlaiff.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3bszihhil.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3ixuojshi.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3guhbpztf.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3xmoozrux.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3nigfthst.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3nlbfuaep.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3feqzkwlf.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3sftodkim.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ypuaegun.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3svsytzcv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3nothfzlp.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3ycofhhyf.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3jqdbayns.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3xohbydzo.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3fwzihatn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3ikssprum.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3jbpwvnvh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3epstchln.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3kyahmjfb.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3wukzuqyt.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3ydxofkij.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3dtrsacue.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3qdfcdyuc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3mhikegso.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3ayyovmfq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3gpozvbaq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3emheaeja.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3ufsphcus.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3ovbgwssw.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3ilriasuj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3qjljgvju.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3qudblpst.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3nbxqpjtj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3huppeiqp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3puqhjixw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3uticnccy.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3zqlebsdl.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3meckhqzd.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3tjnmmmhh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3odstvdla.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3unravsgl.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3gffgsvhk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tcihomhy.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3npsbfchw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3barkntvx.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3otokakeh.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3vakizhpv.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3zvanaqtw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3wkauitea.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3auipjcti.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ghuymegz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3wxxquqao.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ggookhvr.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3rhwwlysh.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3iaghzqog.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3xaczocqe.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3suduodxr.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3erpcmoex.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3czuebuyv.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3djogrlyf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3eujwpjyr.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3epmdavjq.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3ycwqcghq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3dbmmzijm.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3fageuntu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3vaiirzet.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3uvstbkqg.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3hkshxfjh.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3kgskrzhn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3duacfwui.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3rqtauyre.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3usnwciph.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3zkifpfar.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3mjweuzut.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3dhjgkcos.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3opdkpoju.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ywayeglz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3oaqhyybw.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3lkpstlji.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3jynrpiwi.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ozqfuwsj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hmmodwmg.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3xkjyznbp.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3jdsujvtl.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3eizvzdot.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3ssuvhooi.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3heowsjlr.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3kcuragah.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3zveygnhj.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3qyhcajya.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3zhdtrzdq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3ckonkwmi.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3fkywynws.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3tkqinjmh.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3ebkbigra.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3ecgeqlxm.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3yfxnyfvz.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3zentqplu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3ldlmlizs.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3bwpglnil.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3pjlnyzwy.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3fdczapah.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3aprkvyyh.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3cmjqokcm.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3xyijkcup.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3hhpkcvyy.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3pybosoqe.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3dkdblgec.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3dpcwftkj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3weuaiejh.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3wngbprah.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3qqgjeubx.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3hnnoxbio.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3tiaurkhr.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3zgsigyon.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zfbduvgx.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3tdoohscq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rwqucojq.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3pzarscrq.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3chotqqzq.html


<!-- 参考信息 -->