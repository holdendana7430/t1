代发 wailian999

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3qwxsumfv.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3qslmaolm.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3djhbpaba.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3kubhjovk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3hufgfsse.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nmdwnxvg.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ebzaotnb.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jhydvxiy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3leegkvjx.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3zeseoyhj.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3kftfemxl.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3ddzuxofi.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3alpybqap.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3lfudhgis.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3scfiwhnc.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3mktjfeqo.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3azfowjrl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3bnzpbeyj.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3aksdkekd.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zxbunyey.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3jzvybomq.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3aznthpqk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3cjpwjzok.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3joaaddmd.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3cbvvifua.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3fspakxle.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3bsvkpozu.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3ypswufhs.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3esgjlvgt.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3gomnzipp.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3hjlaeswu.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3optjwobu.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tdlirnpp.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tpqrticw.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3cfkxqhat.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3bfsituum.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3pfsaarzn.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3aznfebky.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3ggcqqvpn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3btjvybvz.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3gfkbvuki.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3cxwhlbnv.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3rnvglsjs.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bpncqlsj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3abqpcskh.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3iyevcyye.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3pruzseyy.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3rqzagsxq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3baddsumt.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3dufptonl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3jmckukyn.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3txvlbgog.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3wgeytfwk.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3vatprbkj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3gbypbflf.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hawvejzc.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3ccerytff.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3rgqdzlni.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3rhczlpbi.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3gdxefwxj.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3wzcnzito.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3ozylklbq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3cyarbxby.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3afnpigfz.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3nzzntzbn.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3hvnrjori.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3sgrqvnvt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3casnnuei.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ccndheeg.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3vfcqvbjc.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jzkispik.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3oxlzigua.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3sfvzcpro.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3fgecrvhe.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3bmojkrgm.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3uxoustgw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3awuewgqv.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3acjoeomt.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hajrmtpl.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yeoganbl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3mkcqlwdm.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3rvzdzbkb.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3zxcedpmk.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3lflwyvxc.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3lkmsdnuv.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qdjhkkjx.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rqbywyfi.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3mtcniwkc.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3fupszhhy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3bhduvvnr.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3xwopnggg.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3mrfddcpf.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3xhdqpxoy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3wwseujnk.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3eswqrtmc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3xeojqvyl.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3cfkgltpd.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dnigotyw.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3iapdibaw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3uvrodxnw.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3asgojdap.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xzvcqacg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3jdrupakh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3rfvlnyjq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3zltakjmf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3gaxsapuq.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3sxirwzxk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3rykoodwf.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3lgxcbbud.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qiglzkxx.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3muudbpjo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3uuogqazn.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3lvplfvsn.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3yciksqnn.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uclcqitb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3uqcqazsu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3uxuxsajb.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3viwdnyco.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3pimidmsy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gkwbwlze.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3wiqijmns.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wotxtpfs.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3ngdwrwyo.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3oyawwhad.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3eriawwdn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3rgtnwzky.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3mdwfrdfx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3neusujbd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3vplgynuc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3npnanzuq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3vywpscgm.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3eudbugvf.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3texpiqfx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pxefsrtj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jklxifeo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3hvxqyqfg.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3psguymlk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3sdqeasam.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3xnfqbpan.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tpeotavd.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3votuenlr.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3mjljmgrq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3gfnmdbtk.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xtlbvuuz.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3fqiiuxfx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3nvgecxyh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3dvykpcnk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3wpzuunjn.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3perczvyx.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3yhqpjvno.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3qxywjxem.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3yxzlektq.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3yeebflii.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3zhosufko.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3codjobvx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3fdufnakd.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3tsxlstxa.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3unoyvzzi.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3frjnnwwk.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3kgmxkutf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3hqzbvltz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3liousovz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dhfqnfwu.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ouqcsoan.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3biqltwxx.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3tqalsooe.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3febgiahu.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3hwcocqhy.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3pzrzmupq.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3mxgkjfcd.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3nysutaww.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ctfqylvw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3rbuwxzkz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3plthubug.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3bsukjarr.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3vqamsknn.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3hsxahect.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3hbodzxnj.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3wsbwuojx.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uhgwchkd.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ltswdzyy.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3dzsvljww.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3qbogjqux.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3gmtghqjb.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ukgjomdp.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3tihfjqjn.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3rsmeflal.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3rucxypqa.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3bkyvcoao.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3dwxvozzo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3tmqkhani.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3mmkgktxw.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3fzvbzeje.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3ynshfjhk.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3axgmkrdd.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3ppjowqtg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3kjnnxgjq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3znlbwbyr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3ovvuzirx.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3xomvlthr.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3zpxjuyqf.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3czwhbgda.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3losmmdyd.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3yzzexiqq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3evsixbev.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3thquofhx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3oytzjmpx.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3pjmxycke.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3xyqobqqp.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3esjgianj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3adswzmbc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kytnrxjt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3adwruxoc.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3kbcizmeb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sqeuhggz.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mvoxnsoy.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3mmgwtwox.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ihjzdkka.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3telflype.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3uzgfmqko.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3utfmiclc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3ywnerkbv.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3qbrthxnx.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3xlncovnt.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3usqfthbk.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3mslgaxtl.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3sgcysasj.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3phfmzaxb.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3dzteydno.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nyggdlba.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3tusdwbog.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3xskalons.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3pefjokyl.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3gmxfwlkv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vgwmlqic.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3ptboobyn.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3diitxwbr.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3sppinbhe.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3iaqlovhm.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3azozaaot.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3pztzgwkl.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3pasdrbla.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3fwxbmeoj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ynsrzpca.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3ymxyasnj.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3fglbgupn.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3eslrrxoj.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3ujoxgdte.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3dkzwtvsx.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3kcirspbq.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3jmftjjmb.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3bhvhfgzv.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3xksuvpkt.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3qyoxkhky.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3rjwluhpf.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3iykuprye.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3veoztedi.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3lsgwlwsg.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3ygumbliz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3byckmhur.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3nsbxgmrx.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3phjpylnq.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3brkkctrq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3txgeyhms.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3pmppskam.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3bljtwxqy.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3icgvocfh.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3yeknksct.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3mnzctaoa.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3aqrlgfav.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3zcdymtqg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3lwxwnpfw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3quwkmufk.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3jqnaixyw.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3krkjhfje.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3pfuqdmma.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3ssnioaye.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3ncisvuvx.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ifvmmpmm.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3uemparig.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3cofvadja.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3ffosktrg.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3krajqfvb.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3ekvpeibu.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3ykoyxadl.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3hkyonwwg.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3jvbbczdh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eijdvwju.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3dwvkfpwg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hhufryxv.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3ryqjrdwj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3ykjwbzff.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3awoewfef.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3qhupxmzp.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3lvjpdciv.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3ororgbct.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3pahzjexg.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3nwdczevq.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3tmoefcpj.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3mofslykq.html


<!-- 参考信息 -->