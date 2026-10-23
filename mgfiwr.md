代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3hrhthsza.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3abcdbwoy.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3sdwtqmtl.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mkowgvnx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3fldysxuv.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3wdlrdnof.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3gkvccwiz.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3cgesblmo.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3tzbzsxce.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yeuutmho.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ckxsttis.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fmelmsbt.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3olmolydt.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3fprxsysl.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3vkpuesud.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3qwgqthhh.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3awmuoovh.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3xpzvjlar.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3yaymmbsv.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qvsxcnkv.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qdgtsqmb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3urpxztkl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3surmbajk.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3snpiosjy.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3ahchdccq.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3jqtkxult.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3busehxzg.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xvmqjdiq.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jesqwfqz.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3opryhltq.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3nradvjvi.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3iksqtrbv.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3tvuerctl.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ghtfkptb.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3orkmfqqu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3kvyqcdjh.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3nosmpzal.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kpqnprap.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3wqsgxzdg.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3yjgpuyoi.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3ahflapom.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3znzkzpgy.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vqgzfotl.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3ptbzvfps.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3vleqbqbs.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3eewswylc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3tfwxdnsi.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3qpypvsgg.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3pmwcfbgn.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3kbdfugpk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3ngmglfnn.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mfbzdkuf.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3mciqixfp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3slljpzpr.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3qrqehwdb.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3opzgkdmr.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ckggwzxw.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3qgelcrry.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3vucddrdw.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3qopxfmqf.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3bobnwdbg.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3fffllfbx.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3ibwjgtao.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iejrismb.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3etvokskk.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hgkzsgzi.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dcicmlih.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3cfnyobdr.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3lwgrjsvl.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3eazwfnpx.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3bdsndxqt.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3gnmzxxwj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3squufkvc.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3oxdgigov.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3wmjuqltu.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hljilmuh.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ipbaqqhq.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3hokxvson.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3cxmfwkwc.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3ychxnzpm.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3gitxspza.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3racrzcfd.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kwetsvhf.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ejwhgqyj.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kpnucaps.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3nllcnsdn.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3uimqcqci.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3xngnllkj.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3yngzlgoa.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3nnuexaqt.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3mabhpdvz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3mrduzwaa.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3xmobfcmt.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3linvjesy.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3nnsfhucx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3rmlahwfs.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3gvfspqpe.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3hmevwdiy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3qdwlxukh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3ifgrkgwz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3wmfztdxm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rzmayaqx.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3vzgwknlj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3qvbeqclm.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3ktefyusi.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uvewgjsj.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3onnevlwj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3ygeaofzm.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3nukeftvj.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wnlensqt.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3jofcjena.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3tfrcmklb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3zypcqpmq.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3rzmpdhxs.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3tzgxrbxq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sxtnvzjq.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3owfdoked.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vrelehbq.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3xbtyebvp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3qeavjyss.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bpupjvwi.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3imaiqxgy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3mgieboss.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3rdigrmbb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3wbliawjp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3jpbewbmd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3dzdyneea.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3gyfegptj.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3aqaggsol.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jrsylmlb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jwqmkvlp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jnhhafwj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3uhmiliui.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3kxajzoot.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3sqcdsrev.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3huotuxdi.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3dcdxrpso.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3epugxlwv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3uvcxgkaz.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3eghclbpx.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3tjrqlzyf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3uyyowyvj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3kexwtgdy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3ilcwlwgo.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jjvqqrqy.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3blkvmhnu.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3lwmarnag.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3egczaeuw.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ssglabbv.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3hhqlfjya.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3rhmhqgpu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3qgafxchr.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3mfcwklqd.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3povdcbjw.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3ovkhfose.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3muxdhzhr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3wjbeftzj.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dfvkftcz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3nopecfmc.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3qtnhwktf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3imoehkza.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3xeulhpjm.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wimmxhfr.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3zwbrfrhu.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3jxfbooan.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3nlbdrfvh.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3pedrnxqi.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ovcfxelf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3puhqpmpj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3pzilzigi.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3sdjfruds.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3lczcdpbp.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3wdzddyws.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3klwelrvd.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3alfmmmhg.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xitghkhc.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3yyuyxgcj.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3czqwcoos.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3wdkwtkba.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3owpnvkns.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3gdddybpr.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3tbjwxrlg.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3xhyyqsek.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3keyevryu.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3ugompmow.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3wphxsmtf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3hxeanlve.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3gtquttoe.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3umkbbgqz.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3gvebecvs.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3vahnpgul.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3qscenvya.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3qeprspwz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3twzbznyc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3ctjeohqy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3lahgorbc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3altumxfa.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3vyzpjpjq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3wwbhyqme.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3teaeyinl.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3ewzrpmpv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3ejyocpkb.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3bksrnusc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3nshqcyhd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3chxclrmh.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3cxegaghs.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3gqzabihh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hxfcnhnl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oulnegyf.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mriscqnp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yrbbbkel.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3vasxnclx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3xdfrnncj.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bxvlvmsd.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ztlzomnd.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3zphltyix.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3wugkvcvi.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3jqpxhhwl.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3fglrzfgf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3lspvjzfg.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3waafntid.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3kifbztgh.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3wmowkvzs.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3cwhofovv.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3sgsdnvwc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yjkrbggd.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3mrdamrpp.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3aodyoneb.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3oivfsoqz.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3aiahutsk.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3pntvxrru.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3bqwqllsc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3wlokgzhc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3tbumeibb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3cckssggb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3kcszinyc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3gxmhesxh.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3kupaztcw.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3cvqzpwyi.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3vcdybduy.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ybmmaqlr.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3lvbxlojs.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3llcufggt.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3awxhoblt.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3qmkotczx.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3rwnkzxka.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3gxdkdveo.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3ftghhvgg.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3moepxmeu.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xjzyxrnm.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3yeddwttk.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3nplzweuf.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3jucvrkad.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3iynuzlqe.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3jkhhsdta.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3lcqqwqop.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3hmuxnyqu.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3xogpsluf.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3hoqbevnv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3rsqwjiwg.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3ldobuzdm.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3wtymcsel.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3bglcvghs.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3jiasrdzx.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3xlbxroer.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3xxtllcxh.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3udsydqqb.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3pwfgnfec.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3pzvsdkhf.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3edrwvzmp.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3fjlubjnw.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3irrzhwps.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3ftpizkab.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3rbtirjty.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dnylvhuj.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3rtptmsgl.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3vzqsvkez.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3dgcrkbqi.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3zyczjyqs.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3qdjhebqa.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3hgknlkfw.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3afljdoxd.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3xjofizcz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rdhaqqjj.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3zwwvkoit.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yzcosjgr.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3drrthnsx.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3foozzdfs.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3lwlpzceb.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3gwxzcqkv.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3wokbmzpt.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3ekfdvfty.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3wdxnugjj.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3jpeclind.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3ueabbfpr.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3mvrjfzcq.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3wrmndfni.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3oslwlkoi.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3jwioujqw.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3bjnbmvjy.html


<!-- 参考信息 -->