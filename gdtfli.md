代发 wailian999

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ogsaznqg.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3ggwzgfpf.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3zepjllva.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3ictvidvy.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3qpfxuiqr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3bdumiqef.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3eollpzym.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3cikrlggz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3maiwhdwb.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bgmgbqpn.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ojvynftl.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ybjgevkv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3mlkjxuur.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3advcysnm.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3pnqylcyj.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3xjzssztf.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3zxffxodb.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3eodiixjz.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3stzzglcr.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nyrecjzl.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3txdaqbra.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3kqnhgdkx.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3ndvmyhst.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pstkhvfq.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3xboyiuht.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3awsuixhl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oucywtne.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qtlbqdds.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3sxdbqoag.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gzrpymvu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3buwwdjvc.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3zyivwacc.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3jnlvvnxz.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3rkmwerzq.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3gohlapfb.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3ajsvamyf.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3byrixrya.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qnpffqpb.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3myaahpcp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3uwauqtxk.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3ueeteosl.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3lvwkbvli.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3bibcwcmi.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3yoszhera.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3klyyxryo.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kfqmkfes.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3gbxmpzha.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3mepcsjzc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3bjwycuhr.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3cbalppej.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rrmnyuwb.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3mbhzdufp.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3beeqshyu.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3ozfprpew.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3otmtwrub.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3vzhgttkg.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3qmbufuhw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3vgswetzl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3wyngscmo.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3vylsuelu.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3tmnkfxmh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3hmehxygc.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3odkdqdyn.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3vyqavkav.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3avjvqhhl.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3htkjfdsy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3rgmhcudg.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3heswldqa.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3mppreecf.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3gxofaayp.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3dgcuixsq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3sxoivptr.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nyuttkxn.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3kaeyzihw.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ypqxwskb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3vzexrlfk.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3cglbieoc.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3sbvhkbjd.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hqicyero.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3inlxpphv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xrcsvmsh.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3unokigng.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iaevbkwx.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fpxoomzd.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vjjibqss.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3flxdwbfn.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ubvtdkjk.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3lodnilhe.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3eokqkuhd.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hqvlnpsj.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3kosuhhal.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rjvcngoa.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3mghndjrz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3plzxidzv.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3ghshrsgd.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3klnbcwhv.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3bmxrzjsk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3kquxvbwp.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3khdkjdjp.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3etgarkxy.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3ngnkxyzs.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lomaqnje.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3gmsuqrqo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3xtvtulbx.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3umsyhait.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3cneyyyuq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3gerzqgwz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3znbuvkxo.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3mvgkjsuf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ifwitnkf.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3uoyxjred.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3ihmigdqp.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3umasnxeq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jdsobvyb.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3qedahiuv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3rhaidwyk.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3malpbihz.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3vwcrpcua.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nwjnimkt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3mprbsvgt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3gvxkenry.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3cveiqoei.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3ediloxpc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yeyopece.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3rosyczsa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vdvpmzlc.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3rojgjokh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3ikbnaxgz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gilxnmhh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3qwkfldef.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3qlfxulqw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3mcjzaogy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3qxvxnafv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3jxudeiuv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3qklbjdxv.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3cvzmmiox.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3ycafmvbr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3rtwrekwc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xzixqclz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3falilvad.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gwnlolod.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3zqsweigk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3iwxkvado.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zkccjkpz.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3jczwvgwj.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3zqlqefmg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3cphsddey.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qdyhsivq.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bhudvsbm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3htenzojx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3krelxlhj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3klydlryi.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3sezpybjw.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3zxgvovvf.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3yosxdfqg.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3xcxvkycw.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3japervxw.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3nujmqnzb.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3xwfiuzki.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3oeiyjrdk.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3nftgwseu.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3npnyfnwu.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3zvcwwpet.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3ruzghjms.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3llejdrol.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3zszeaiyx.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3bkcqhnve.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3bsubpvzf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3xjebsiox.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3iimswidm.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3xyzidvpd.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3gdxllcuc.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3pufetxko.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3potkxafp.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3qigzhppl.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3lmqbhxsg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3tqmytxke.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3ezgswqvn.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3qgluicow.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3dxebvzqw.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3kuevihyl.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3pijsljbx.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3zovitfxy.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3saukedco.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rcxoyuuf.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3qkjzcxjt.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3zdnpsxqx.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3jhdqwwlv.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3iyistxve.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3sbvgdmjb.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3cyxeotcf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3vpmksgfa.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3pihktivk.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3qjkjxsvb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3ebuyodyw.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3gibvrdhq.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3kdbtzkwl.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3ksdkxybm.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3fdvqdxci.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3ixbeelbc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3gksaotfg.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3ftqpsgjk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3zzbghwzb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhtjtodj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3roognawn.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3ztjrffrq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3aludaxma.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3rtirndpp.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3swzcavzc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3jfsqeuca.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3zaggnweh.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3wtbdxjxl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3sipyfwro.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3lytuhqdp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3zmkabaet.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vjmthipw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ifaxoulw.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3jyejlxso.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zfippexr.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3jtnombwt.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3jhkwdcmd.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3dtzyjnfh.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3qdjdpniq.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3ixtdtpnl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3fjlqnulm.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dconmyej.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3mrsnurcr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3qdwftybl.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ophtylwj.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3milsqils.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3dbjmmtkl.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3grirpeje.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3fxfrxxyi.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mnmsitoj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3yuonuwpt.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3xfmkudsg.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xcctspac.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3sakbxdjd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3buevtxlv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3bfxvpdwx.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3nrwbadtq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3ktgoeovf.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3rwncpyup.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3axbtngnw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ywzuwzuy.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3uloboave.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3atjcwxog.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3fspnnmsi.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kldwlihk.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3hvuvthot.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3eyhdzywk.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3nykrlsyu.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3hwscyjkw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3diumxxeo.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3uimuxbnz.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3maryugat.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3dttzltnj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3pujfvkwp.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3wwwgntqq.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3stwvbigt.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3vwyhmznx.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3vjloxcfb.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3plfqkznd.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3azkylnry.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3yzstafbg.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3ryismzqg.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3kubfotjr.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3dpcgtrbu.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3mcnbgplu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3gynpsojv.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3kdcsndro.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3thuoqfym.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3vrvxjnye.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3fjhordmq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3elfgqfuf.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3ovrezvcd.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3benjqdvf.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3zhauhvwk.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3kgcnithc.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3lhjbnbcp.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3rfkbjwtr.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3pguiqite.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pzgayjvh.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3liykuhft.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3dtwqrxyz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3cmdwvsnc.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3ggmwybpm.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3yiktspha.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3vzhvysht.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3neherxtq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3ldagafyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rxizhhuq.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3ahzllopo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vlexbmlo.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3zxevswpd.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3gbmnfrsq.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3xtggfkov.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3fcghfrnz.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3pddkezhp.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3vtocaxes.html


<!-- 参考信息 -->