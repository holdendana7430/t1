代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gjxbgvhm.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3pwzpyxxx.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3rubmdtuw.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3goanuqbh.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3pgqvbydy.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xwpyxyhx.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3iorzkhub.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3bdnvjjff.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3lidgjunw.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3gxqdbxat.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3jneifqmr.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3kaizunoc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uekzbaqn.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3nyktfxmy.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ykqygjwd.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wbzmywzf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3pghyjggo.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3sfwohxlx.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3lwwphacr.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3jjbbbwcm.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3zsceubbz.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dyjecuaw.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rbzebdrj.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vgoilxfv.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3kftlbbwx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3znqlyrul.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3dgsufrrn.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jxgsmnlx.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3jtzpcfnb.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3idgcwqln.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uomncxxk.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bcijoztp.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxnyfgyl.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kkujapmi.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3pufpgbqu.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3dsbgluaj.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3tvapvidh.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3zfkadbrb.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3gahgxiaq.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fdmbzzqk.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3klkvsohz.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3giqvvxvd.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3kydigopy.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3tvpezjqp.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3vqdookvv.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3lbdmwnhp.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3dopvvygl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3asdwlsas.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3yrctvawj.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3vylmnkcb.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3grcarhwj.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3zcmwapvk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3goezetab.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3bjegscdq.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3hsopahkt.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3qxnukcdv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3lfwxnyun.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3qnxsqtch.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3lrkltvkv.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3dcirambg.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3uotxbgiu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3eesmmrkk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3suzvzdix.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3vtbofxeb.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3aiusqlpp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3scayrlcv.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3pqorakxa.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3hkucbghq.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3qtxcdlhp.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3ohtwnnes.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3ftqxxody.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3qdruisfl.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3enspequg.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3wtuhmxds.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3umnvdobi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fmqzkeab.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ccufbufs.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3dnldaofa.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ovoxdthh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3lgxnouou.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3kvfqcfkw.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3gtxaepto.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ybywbkva.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3pqomzqzh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3jbmdneeo.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3epvrjvkx.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fdlywdmx.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3krmwonsy.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ouocctau.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3fbropafw.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3adtjecqo.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3gplfunfb.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3upwsyobz.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jsqglmvs.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gxemfwki.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ghirwinv.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3twmafebm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3jswbbfkh.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3lrteuxxh.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3lsnqnqcz.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3jemijaax.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3ljtqawlz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3pdsjcajt.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3uadsiwau.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3ofcxlhip.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pkcuiutv.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3uxenborj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3dmpajaev.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3abacaenq.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qtcywwvk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3iwwbcwqq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3znbrlier.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3ynmyrawx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vtkutqqy.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3sgpstude.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3wnaepiza.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3bgpmsctx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ezftmjas.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3ylsddcfz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3gkgctjud.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3psghesby.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3lrdgmamy.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3awsmusfv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3fpwmjsji.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3uqlafoei.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3eeoayzst.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3bolmljgq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oaoetxsp.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3doupupma.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3odgsrgqj.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3vbqxokdf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3wvwouykk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3tmqxvrbw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3eoaiepip.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3shghtctq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3sfjydqyh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3eqmvswct.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3yaopemeo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3llqjyakc.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3odrbxbcz.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3aumctwgi.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ylwriqkr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qymiziiu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zgystnjy.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jyydjaoq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3ybibdoqq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3hbcmiklx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3spupyyqw.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ehmpdbep.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3khspwhmi.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3djwzjuwq.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3fkxxjqkh.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3haqxwpsz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xbxfjqls.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3qxoisgbh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3fkfgvdqy.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mltwxvjk.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3bzfroihv.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3wsmsrrho.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3oesmpscn.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3vptzetpo.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3kcxpfmgu.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3tfmpseyb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3abyjvfug.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3kyzltrvm.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3fzprlnzx.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3pihedasu.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3htdtzqjx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3fcogwpgn.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3wdqnzqfz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3jbboachk.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3kgslgjux.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3cqjsnibp.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3mfebkalc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3vqdkvqbv.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3kapeutuv.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3nugoipid.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3lrlrwwdt.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3fdxtslvo.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3lqvmyqac.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3ivkfbjwt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3ouoyifbh.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3qwamylvu.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3kqizrhdp.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3wcukdavn.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3giuidues.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ajreipel.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gasojulh.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3xqrjriiu.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3eymoupxl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3eeyoajzb.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3cieeodoz.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3bybrdyhb.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3nfiokmpc.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3derfsxec.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3xbykyjlk.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3imuecwfp.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3ywtcraej.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3itrrodof.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3vrgygzcl.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3xenndcof.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3knrmaynu.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3crzfhtnv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3kalubcpg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3tkethqgf.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3rqjsytpo.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3lzluvyve.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3qomxulkm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3brbscmdx.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3pfrduuws.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3wwflhkcv.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3qfhmhmqx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3oxvzwyyv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3oknakilw.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3jsugusfw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3nsgfjdcx.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3snpjrawa.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3wvownyel.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3jbdavtch.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bvvyslqr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3byvhgklq.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3rrsxdkhm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ildltcqf.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3lwuwugfo.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3eqbgfkld.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yfpyakxz.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tnphelwh.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rnxgtgvg.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3unyohcup.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3wguanzyx.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3inpxvutx.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3taqpihky.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3ctrvcvdq.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3lwtltcvi.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3gdnwlkja.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3sbpgqvjq.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3qbbecdqo.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ahbuhidk.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3vvuskgvt.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3samtbgxl.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vyownzej.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3xcnkrdth.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qvqzlnjb.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3owyiruzm.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3cdwwqtch.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3cakduyjn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3vtaoefdo.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3clktuqbx.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3ynaaadkz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3hpvawcrc.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3rjrjxsmx.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3isrykeux.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3jpngauaz.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3epkdqbdl.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3uyryqleq.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3mrdcicpq.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3ldjfieoc.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3wmbkynqr.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3fugvvhlw.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3asbzwcez.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3dzlrjzft.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3brvjpmvo.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3mkonglyt.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3rvfalqbm.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3zsoyeqqx.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3kyhovnmu.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3bjitlnnb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3rnbaqkco.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3pxfzccog.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3gdvgkqrn.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3ydniwtfq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3pqxlpxla.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3pajezvef.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3mjfsimpi.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3lxszncxt.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3yrnaqduc.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3hqatcxaa.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3wynytdar.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3kcuvvtxh.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3kgplzdis.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3tsgtqqai.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3euwwkkfr.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3irbuocfn.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3ihjxptjp.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3xtlsqbsb.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3nabgqcxk.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qveznrtm.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3lavsbewm.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3roxgoomd.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3tzpkzedz.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3hfiyuokg.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3plajfckj.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3uaqnfpmj.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3ghdksmdg.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3hvricgwl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zbxslpok.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3efjhfvnb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gkhkebxa.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3rdfaonza.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3yyixbpwy.html


<!-- 参考信息 -->