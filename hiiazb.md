代发 wailian999

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3zziczxtt.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3vmvdpkbv.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3omyakrvo.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ppfedakr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3srnlnohm.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pykwttvo.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3whbnazgj.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xmklnraa.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3mvybalcy.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3fteyvelo.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3fqbwdwcr.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3agpggkei.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3dwxjifpk.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3twtzwhbh.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gxcmwwxa.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qixcbcvj.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3bmyqvaab.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3lsburuot.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3tsitsyck.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dabwqyxu.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3xqsdngkq.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3delgaabz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zqnvjjsw.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3yrnxdlyh.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3orvygtsh.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3iiokzpiy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3bhrbfxrn.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3khfjciok.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3ydjdhake.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3siirlszp.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3cwjnvvrt.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3bddfruyp.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3yoxxfrks.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3yodtcddn.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3chlpyriv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3lecjcywz.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3lxzrrizb.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3cluhofqb.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3nzeihzxw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3lrfzruer.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3umtivjlq.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3gemrdtgn.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3xiighpul.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xepuxbjx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3meuuacoe.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3mjtjqlyq.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xcavjohy.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3mlyosbqy.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3piknkdhd.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3yrenmhkx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3mqaoucye.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3wxcvoggo.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3odqeexne.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3deyxjdrf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3oqpodpzx.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sgcwvohu.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3altaenqe.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3wmndhuty.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vqrbymyf.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3jbqjgdvm.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3klvcdwgv.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3ooabhjnl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3cfgvtwkl.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3olgwqlhh.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3jpvusvkz.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3evpddtjb.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3gtvgdfls.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3opegving.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3iewwqrxh.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ooqfrtnf.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3eismiuef.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3sdtybgrg.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3zlqbiqgw.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3woaddfnx.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gsdiolzi.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3dhtdyyau.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qegdsntj.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3usrkvqtu.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3injggaja.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3isecjvhz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3psimbqdg.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ljtfhjps.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3zodzpgoh.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3scrvhwgq.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3fbkvfyhs.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3aastrzjb.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fqtalsed.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ounatbon.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3tbmyaoio.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3edjindmu.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3wdryyulo.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3mbymlpfu.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3ufyxmmyb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3wuvnogpx.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3ineeuami.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3xaauuflm.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3iwrojgfc.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3mezqhnty.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3tlupmozb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3ufxekleh.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3mldzqqjr.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3geplorfj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3vodgzvwu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3dwpxjlgm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3mxxqcpbm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zrnkirdi.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3cqefwpyf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3zjwqsutr.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3mttzegmv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ootroolv.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3fdcigvrd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3xfnezeuk.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3zilulppi.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ystwhfof.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ufnedzwp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3mqtmbdem.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3tvkbbrdi.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3jwbkdquz.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3cturooph.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ljmvncki.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ovcagkxe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lruxdgip.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3gcisievz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3mgjpttdw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3eeuxijco.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3cnxusssm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3vfdzovoc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3otukzzbl.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3vpsocynk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3kmlqeves.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3eusxtawx.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3kzovlgvz.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3qytzsmza.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3svcihmel.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ocehshxu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3bvatwpsr.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3oaibotnj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3spiklpdr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3aoslemng.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3rrkwjuul.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3tfqynmux.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3jzhtwxuj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3poddpgai.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hoiuysxd.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3unxvhwse.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hwvcsuqn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3bckkollz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3pxznwlyi.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vududtwt.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3llcrvafm.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3bcywnrmr.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3douxcrpy.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3wedspgkm.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3ugchaihs.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3fpakaqmn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3vdrijljw.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3jyfzqlnm.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3aelnraya.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3yueijyme.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3nfkfukmf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3mztample.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3wmaromoj.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hdqcxxsn.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3eqruivzp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3tneolbmh.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3saaotwlr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jmpeawmu.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3iznnsmle.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3artxibat.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3agccjrzq.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3jzcvzvlx.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ovsgjsph.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3yxjbubog.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3joyavpuv.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3vddqqaqu.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3llbrsgsw.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3vjjhpgqc.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3svuphola.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mwnyotvs.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3whygybsj.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kwmjhotc.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3lemtvhuf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3prwwbyve.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3jvxobhpe.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3axrarayb.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3pdtjfkqp.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3fplvtxlu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3jjfhvnyn.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3auxobsop.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3dokxmiza.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3gldnytoe.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3atuiffpx.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3kcajhenm.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3infvetwi.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3nqcvumnq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3tdqgopcg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3yurgrikb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3acfzlfib.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3vyeywexv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3saatzgxm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3deexaegt.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3irmpaaqo.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3equflams.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3wciqzrji.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3huoczfok.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3gslhjvts.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3sntlpzty.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3ykqvazth.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3zfwkymwh.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3knduyiky.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3rhftlkmz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3svzvisst.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tqgagjvz.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3ksqhxnoa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pwlcjqoc.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3nwmveuzh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ljcszyfd.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3tkawmfbo.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3knrnknvh.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fwvtphse.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3jcblzwpr.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dvwffmux.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3sowtkexj.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ebzeafeo.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dgdrrsef.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3yzreknfh.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3rnirlmub.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3kyenpgjo.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3hjlgtfwi.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dhpoemyp.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3wrbnagnr.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3nczirmth.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lghiwzlu.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3ewztiabd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3wwtaamzz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3beiapjpw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3wfghpnft.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3jiiaxqfv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3nikqjahg.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3wmgjjxzf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3vclcgyck.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3yxswbtyx.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3hbikkkqq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ijymipqt.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ioisyzid.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3itivahxi.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ipbyxlmt.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3exogkysm.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ygsmfgop.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3cdmrwwhx.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3dcypjrxu.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3fprqkzpp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3exrgyaxb.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3nadsfeeh.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3ouwijmhw.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3rrwhfnzg.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3jgugqakd.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3qiyovrhx.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3ewjkyctb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3qhqiayih.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3iaynogkd.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3jmesvimi.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3ubslnwil.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3xtwqbyzr.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3sppehulz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3kyvtboks.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3mpzuvtht.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3xzatcnwc.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3aamzitse.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3owngrzmw.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3dhevbqmc.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3qzdoyvhf.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3bspumufw.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3rcngdkrv.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3stbbjzif.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3cmvvumez.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3tsexwesk.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3fyuirndv.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3muwhtudr.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3kfantucb.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3qginwxyf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3bygosnlq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3lohuqwmp.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3ttratlup.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3uxyouyhg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3yarunvaa.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3ptdqrfsm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3coltwotx.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3mmlisaqq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hzkyqhio.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3skeatdpg.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3iqccntcw.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3odlttfef.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3bkluwfeg.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3ywojnutz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3bllmkrio.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3jentpisu.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3bpotkfaj.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3hgyefhlt.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3xtrpyyuh.html


<!-- 参考信息 -->