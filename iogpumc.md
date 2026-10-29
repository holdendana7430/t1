代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gufkokpjc.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gcdhyavcg.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gusagcjpu.sHtML

[G05] 继承
来源：http://baike.hesvh.cn/Article/details/gmzuwithx.sHtML

Py:   class Admin(User): pass
来源：http://baike.fehbvm.com/Article/details/gibgflkdf.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpnnwoiix.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gadoqhrni.sHtML

TS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gruvkowig.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gkjotilxi.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.hesvh.cn/Article/details/gjarbrerp.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/gyynbvjyg.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/gsbxunart.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/gyxeyztjt.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.zdbjq.cn/Article/details/godsxixvr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gkjkunyel.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gtenkzpbh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gqcvufdbu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gunkidwpi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/gqalkmnll.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.zdbjq.cn/Article/details/gjaissast.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fehbvm.com/Article/details/gukofmkms.sHtML

[G07] 调用父类方法
来源：http://baike.hesvh.cn/Article/details/gqbhltvyj.sHtML

Py:   super().greet()
来源：http://m.share.fehbvm.com/Article/details/gknkfzbjk.sHtML

PHP:  parent::greet();
来源：http://3g.hesvh.cn/Article/details/gluhjzepo.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gsykhogag.sHtML

TS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gkgmnfdew.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/gnjdyhvzw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/gsnrhosjn.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/gdpokqgdb.sHtML

C#:   base.Greet();
来源：http://m.share.fehbvm.com/Article/details/gekjpdzcp.sHtML

[G08] 静态方法与属性
来源：http://mobile.fehbvm.com/Article/details/gdlwxeiev.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fehbvm.com/Article/details/grlfclbmj.sHtML

PHP:  public static function f() {}
来源：http://wap.zdbjq.cn/Article/details/gwpojorla.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/gbwftitav.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/gaxrybaud.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/gkajyhxvc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/gyzphossi.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/gcinwdupm.sHtML

C#:   public static void F() {}
来源：http://baike.hesvh.cn/Article/details/gdjshcfiw.sHtML

[G09] 接口 / 抽象类
来源：http://baike.hesvh.cn/Article/details/gezkavxsy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fehbvm.com/Article/details/gfbojwkoa.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.hesvh.cn/Article/details/gcaqzxgkz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fehbvm.com/Article/details/gxnyrrfqv.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fehbvm.com/Article/details/gingzltic.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/grihejivo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.hesvh.cn/Article/details/gvivxkjxs.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/gyruqbxqv.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.hesvh.cn/Article/details/gjurgvhiy.sHtML

[G10] 访问控制
来源：http://blog.hesvh.cn/Article/details/grrpjdabz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fehbvm.com/Article/details/gqdvrlvhb.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gtxclrekm.sHtML

JS:   #private 字段；其余公开
来源：http://baike.hesvh.cn/Article/details/gtjwirycs.sHtML

TS:   public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gmwkxcevi.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fehbvm.com/Article/details/gdujnixip.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fehbvm.com/Article/details/gmbjrbgmq.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gfrkjihzk.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.fehbvm.com/Article/details/guigsqhir.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/geqvpjqzw.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/gluydnfqn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gpapjmgjn.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gcdhpmpat.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gneoplpyw.sHtML

Java: public String getName() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/ghitmpxca.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gmagugheg.sHtML

Ruby: attr_accessor :name
来源：http://baike.zdbjq.cn/Article/details/gpxhxsztn.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fehbvm.com/Article/details/ghxntayby.sHtML

[G12] 对象转字符串
来源：http://m.share.fehbvm.com/Article/details/gpkpnozku.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gnnmvstbo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gumxnqfzl.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfzhqdytz.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gzsllmpui.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/gglmpcghn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gnktvrxlj.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gotfqabvm.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gshggvhcq.sHtML

[G13] 判断对象类型
来源：http://www.share.hesvh.cn/Article/details/ghxxzlnzv.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.hesvh.cn/Article/details/gusnqccpq.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gjejfkquk.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/grlddnosw.sHtML

TS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/grfwgobnr.sHtML

Java: u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gmbiyjaxt.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.hesvh.cn/Article/details/gypzjhdpg.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/gmvsjlxnh.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/gwxhjxkha.sHtML

[G14] 数据类 / record
来源：http://m.share.zdbjq.cn/Article/details/gnqnlsads.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/gqfmpikci.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fehbvm.com/Article/details/gcyiizanb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.hesvh.cn/Article/details/gdjyybmoa.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.zdbjq.cn/Article/details/gerwcqqpe.sHtML

Java: record User(String name, int age) {}
来源：http://blog.zdbjq.cn/Article/details/gojuydpyk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.hesvh.cn/Article/details/gejhsjjhc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.zdbjq.cn/Article/details/grkrerxsy.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.zdbjq.cn/Article/details/ghkxcvxwj.sHtML

[G15] 枚举
来源：http://read.share.zdbjq.cn/Article/details/gbzmejrxk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.zdbjq.cn/Article/details/gumqgxadw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.zdbjq.cn/Article/details/gbifbjcaf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.zdbjq.cn/Article/details/gkmqpscfu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gjenquyom.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.hesvh.cn/Article/details/gvcfwxvau.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/gznagbhla.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/gcgqskdtg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gyhkpjvwv.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.zdbjq.cn/Article/details/gnusmfizp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.hesvh.cn/Article/details/gpbuwgysy.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.zdbjq.cn/Article/details/gruodukyh.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/grdupuxuz.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gjxerhcxq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/ghymfljwx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.hesvh.cn/Article/details/grslkvsnj.sHtML

Ruby: obj.instance_variables
来源：http://3g.zdbjq.cn/Article/details/gjxvqesmk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gpikqhxbs.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gebuzrpwg.sHtML

H. 异常与错误处理
来源：http://3g.fehbvm.com/Article/details/gvvicaijs.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwvznenbs.sHtML

[H01] try / catch 基础
来源：http://read.share.fehbvm.com/Article/details/gyozxlwxy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.fehbvm.com/Article/details/giiezvyyp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fehbvm.com/Article/details/gqqnrbbob.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gotbnpoot.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gwucrckac.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.zdbjq.cn/Article/details/gfpauseym.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.hesvh.cn/Article/details/gsnloroji.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.zdbjq.cn/Article/details/gphzzcter.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.zdbjq.cn/Article/details/gisfduxyb.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fehbvm.com/Article/details/gkmtpvneb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.zdbjq.cn/Article/details/gblzkqrtg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gjhtgxskr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gmngfgixw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gcpeaoftd.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gfazbqgyw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.hesvh.cn/Article/details/glaczgejb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.fehbvm.com/Article/details/gdekgicth.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gdrulvqpk.sHtML

[H03] 主动抛出异常
来源：http://wap.fehbvm.com/Article/details/gnryjerth.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fehbvm.com/Article/details/gevnryulj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gncoytgsb.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gyzjjvcrz.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/glasmtwqh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gljmzikre.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.hesvh.cn/Article/details/glnveedti.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.hesvh.cn/Article/details/gioinjtru.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gpxxdrnzi.sHtML

[H04] 自定义异常类型
来源：http://www.share.hesvh.cn/Article/details/gugmbwahi.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.zdbjq.cn/Article/details/gmedqtjgj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gjwqedmcm.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/gkqhoedxw.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gjnbzmgig.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/gvjbqpmtq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.hesvh.cn/Article/details/gjuniciqw.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.zdbjq.cn/Article/details/gbxibvxuh.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fehbvm.com/Article/details/godrwxyry.sHtML

[H05] 捕获特定类型
来源：http://www.blog.zdbjq.cn/Article/details/gyrtwjwsa.sHtML

Py:   except ValueError as e:
来源：http://www.blog.zdbjq.cn/Article/details/grtrypapf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.hesvh.cn/Article/details/gdqlgqord.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gnjaczddi.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gutipfpql.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.fehbvm.com/Article/details/gnwgwymco.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.fehbvm.com/Article/details/grqdihpwn.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fehbvm.com/Article/details/gcrevxvvr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.hesvh.cn/Article/details/gbgkpsawk.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.zdbjq.cn/Article/details/gigllcovc.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.zdbjq.cn/Article/details/gtwpfalug.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.hesvh.cn/Article/details/ghmwrhxef.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gvfcjqpwp.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gqhnuxqzw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.fehbvm.com/Article/details/gmlhuxrsr.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.fehbvm.com/Article/details/gididxkuf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.fehbvm.com/Article/details/gisuoommf.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.fehbvm.com/Article/details/gvyhsljkb.sHtML

[H07] 断言
来源：http://read.share.hesvh.cn/Article/details/gecpqixls.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.hesvh.cn/Article/details/gytozhhum.sHtML

PHP:  assert($x > 0);
来源：http://3g.fehbvm.com/Article/details/gktllzegd.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gmvqgarxt.sHtML

TS:   console.assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gzqrpdbyw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.fehbvm.com/Article/details/gdfkzsnck.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.fehbvm.com/Article/details/gawjgkgdh.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.zdbjq.cn/Article/details/gekgdtppj.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/ghvqsgtxw.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.fehbvm.com/Article/details/gahmqmvuq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.zdbjq.cn/Article/details/gdhsvmtsb.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fehbvm.com/Article/details/gpfervxic.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.hesvh.cn/Article/details/gbvuoggek.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.hesvh.cn/Article/details/grunrsqso.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.hesvh.cn/Article/details/gmhnbbjlf.sHtML

Go:   err.Error()
来源：http://www.blog.zdbjq.cn/Article/details/ggcrhrwws.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.fehbvm.com/Article/details/gkdyouvim.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.zdbjq.cn/Article/details/gzlqqpckx.sHtML

[H09] 带错误码的异常
来源：http://www.share.hesvh.cn/Article/details/gkyntxeuq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.zdbjq.cn/Article/details/gvxawtozw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fehbvm.com/Article/details/gfqojjgjv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fehbvm.com/Article/details/gtiojihrs.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.hesvh.cn/Article/details/gbfelvbvj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.hesvh.cn/Article/details/gfbktgoye.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.hesvh.cn/Article/details/gbqqcnrao.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.zdbjq.cn/Article/details/gkqdbbopf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.fehbvm.com/Article/details/giutemfdj.sHtML

[H10] 资源自动释放
来源：http://3g.fehbvm.com/Article/details/gtxohzlnd.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.fehbvm.com/Article/details/gtjcznwut.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.hesvh.cn/Article/details/grrgqoevi.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/gqaiorkzg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/gebkasxkc.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.hesvh.cn/Article/details/gbrcegwmi.sHtML

Go:   defer f.Close()
来源：http://www.m.share.fehbvm.com/Article/details/gggzqjhhu.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.hesvh.cn/Article/details/ghkzamhsh.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.fehbvm.com/Article/details/gzflxdwwk.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gaffkzgjc.sHtML

I. 正则表达式
来源：http://read.share.hesvh.cn/Article/details/grkpifrge.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdtixchvv.sHtML

[I01] 判断是否匹配
来源：http://read.share.hesvh.cn/Article/details/gxmtzjsmb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/gsjlgcdlj.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/ghqldulpg.sHtML

JS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/gkaxiypwc.sHtML

TS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/gzyltjkkq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.hesvh.cn/Article/details/gpfaukwcl.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.hesvh.cn/Article/details/gzuwymekd.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.fehbvm.com/Article/details/gsmteaoqz.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.hesvh.cn/Article/details/gawtsuxkf.sHtML

[I02] 提取所有匹配
来源：http://mobile.fehbvm.com/Article/details/gfiggjhgo.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/gzaxrfqsc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.zdbjq.cn/Article/details/gauaxafer.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.fehbvm.com/Article/details/ghjjudwtw.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.hesvh.cn/Article/details/gpgerrfoi.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.hesvh.cn/Article/details/gwtbfcpyv.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.hesvh.cn/Article/details/gozxeirvi.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.fehbvm.com/Article/details/gfrissmsq.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.zdbjq.cn/Article/details/gfjquwnlt.sHtML

[I03] 提取捕获分组
来源：http://blog.hesvh.cn/Article/details/gzrrmngsd.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.fehbvm.com/Article/details/gxvoyrcqk.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.hesvh.cn/Article/details/gcfwdkmkq.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.fehbvm.com/Article/details/gylfjfbhh.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.hesvh.cn/Article/details/gxeujjpvb.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.fehbvm.com/Article/details/gumprpmiz.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.zdbjq.cn/Article/details/gveiorryq.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.hesvh.cn/Article/details/gwcczescy.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.zdbjq.cn/Article/details/gipivkigk.sHtML

[I04] 正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/ggfuayqnr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.zdbjq.cn/Article/details/gowwkcsam.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.hesvh.cn/Article/details/gkenpnjvy.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.hesvh.cn/Article/details/gjnfixlhl.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gnvfatzdt.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.zdbjq.cn/Article/details/glwyhhdfz.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.zdbjq.cn/Article/details/goxrnuklz.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.hesvh.cn/Article/details/gztqqnvcp.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.fehbvm.com/Article/details/gmfvlyaol.sHtML

[I05] 按正则拆分
来源：http://3g.zdbjq.cn/Article/details/ggcevtkbu.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.fehbvm.com/Article/details/gmviujpgy.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gocwvmaec.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.hesvh.cn/Article/details/gibtmjqwv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/gogjmubww.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.hesvh.cn/Article/details/gkxiwbocd.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.fehbvm.com/Article/details/gtqaeaaaw.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/gmovfnsjs.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.hesvh.cn/Article/details/gzrbuyhtm.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.fehbvm.com/Article/details/gcveggfeb.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.zdbjq.cn/Article/details/gukisvdhb.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.hesvh.cn/Article/details/gnxocgrrq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fehbvm.com/Article/details/grxvnmjvd.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.zdbjq.cn/Article/details/gmmojtgws.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.zdbjq.cn/Article/details/giqitgyzu.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.fehbvm.com/Article/details/grntrxcxx.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.hesvh.cn/Article/details/ganijhghk.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/gghruoojz.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.zdbjq.cn/Article/details/gegyriigf.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.hesvh.cn/Article/details/glmjbokxt.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.zdbjq.cn/Article/details/grvjqsrdh.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.zdbjq.cn/Article/details/gcvihbudn.sHtML

TS:   /error/gim
来源：http://wap.zdbjq.cn/Article/details/geodbexdx.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.hesvh.cn/Article/details/goeauarpl.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.zdbjq.cn/Article/details/gjlqjzotv.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.fehbvm.com/Article/details/gaypqntsm.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.hesvh.cn/Article/details/gghrhpryu.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.fehbvm.com/Article/details/gfpfmctmf.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.fehbvm.com/Article/details/gnvggtczt.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.zdbjq.cn/Article/details/gsvamiyrf.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.fehbvm.com/Article/details/gtvqixemn.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.hesvh.cn/Article/details/gqcuslgmh.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.zdbjq.cn/Article/details/gzyqyanct.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.hesvh.cn/Article/details/gmivdmzqx.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.hesvh.cn/Article/details/gcadgbqje.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.fehbvm.com/Article/details/gyhhwhilk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmsxeladb.sHtML

J. 日期与时间
来源：http://www.m.share.zdbjq.cn/Article/details/gvryyzvhm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/glokfrrny.sHtML

[J01] 获取当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gdsltawgo.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.fehbvm.com/Article/details/gfiqniohz.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.hesvh.cn/Article/details/gynikgbgi.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.zdbjq.cn/Article/details/gicmfioyn.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.zdbjq.cn/Article/details/gztztsdgo.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.zdbjq.cn/Article/details/ghurmxkbg.sHtML

Go:   time.Now()
来源：http://read.share.fehbvm.com/Article/details/gusfzcyly.sHtML

Ruby: Time.now
来源：http://www.m.share.hesvh.cn/Article/details/ggcxlttub.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.hesvh.cn/Article/details/gaycpwikd.sHtML

[J02] 格式化输出
来源：http://blog.hesvh.cn/Article/details/gvmmwpzpz.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.hesvh.cn/Article/details/ggrhdhcil.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.fehbvm.com/Article/details/gphemszmf.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.fehbvm.com/Article/details/gndqlqaez.sHtML

TS:   d.toISOString()
来源：http://baike.hesvh.cn/Article/details/gityqrbzy.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.zdbjq.cn/Article/details/guvmchkss.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.zdbjq.cn/Article/details/glfqybivs.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fehbvm.com/Article/details/gneeglbml.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.fehbvm.com/Article/details/gssgovjwn.sHtML


<!-- 参考信息 -->