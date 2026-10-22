代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2esxmnasj.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewteffiw.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2adgmxdsz.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwbmdkol.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2iyjvrujz.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2qywxghjs.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2jxnxvgyd.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2fcteyxgg.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2wnqnorrr.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gzacflcm.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jbumyjkx.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2nyoezaxw.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ggfnhpnm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2gnxzwbiq.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2vndmnccy.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2uujudgyp.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2lfbfxpde.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2bjwiqhva.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mhjzordf.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ggifmdud.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wxuvsdwa.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lqbwxrhn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2obhjgqgk.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2sdbgyjuj.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2pxwnisay.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2ndryskep.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2rhagqlqt.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2vndwbjfl.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xxnirmnd.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lpazutse.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kvdbllyh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2itaxaglh.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2mlkmomlm.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jesytecz.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2yhgfbnet.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2eogzecam.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2nlhkowgq.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2qodukzwa.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2stogwrdj.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2uluwikbz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2goyebwdv.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2rmgxvfjv.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2psybumvu.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2whwjddtq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2ctmwqjov.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2fynqqrby.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2xbonrsjb.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2fgdcapim.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mzdublys.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2seyjkfqz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2uwlbvqhh.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2hqencskv.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2kcrwdeze.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2wfjlhcnb.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2wuvizuyk.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2fhjabkhf.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rhcngphj.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2wcmoczkp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2pxokgvje.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2tbctwsis.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2efpjvkbb.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2xbjqbuut.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2uynaeflq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2uwqwisqz.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmeztlko.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zshbzyml.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bavzkhgz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2vepyziho.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2mjczsjyl.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2fzqyhfws.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2xdlcekhw.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2tyssbsah.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2msrevjri.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2stlighad.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2faolhche.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwdgyyty.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2nzvlwtya.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2onmwfvfx.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2fzdfeukk.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2ofxtozqc.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2kfgcvmzp.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2fbbhpbxf.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ouumiczn.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2pmmbtpjz.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2hdmxsnbs.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2pquapqdk.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2qeyoxumy.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2jobqzgnq.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2rzrplhkb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2dudsvdpf.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2erpnkwnw.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2iueayjvw.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2cqsfcgke.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2saosclei.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2cpekognl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2byzyukcc.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2pvknnvrr.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2awfsnqmx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2mxwsastk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xtqkhdzh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2pqurinnf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2dwdgxcfg.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2ershktim.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2dkspanxy.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2xwbylzqw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2vswhpuub.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2yirozvai.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2isbccfii.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2ifbvjcrw.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2xnryzvfa.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2wusuxjzi.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2reaxrhxc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2muoyusez.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2tdzgtxsh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2bqhxzbtv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2owtmwvdt.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2frpeaowj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2khyktffd.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2pwqhfpic.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2memncjtp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wdwkpzxg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2tkbybdhb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2jprxsiwe.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2hdiciqte.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2tutdtowm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2lpzazmmb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2paumdhcd.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2mxobjrhk.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2exsjnsam.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bssbmkki.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sbgjfesu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bebxpyxl.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tibfppzt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2ipltwtab.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2dqkyrcta.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tpthehgj.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2rmdssvru.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2omcficqm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ccjejdfy.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zesasdxi.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2djxxnptj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2tnhqrlat.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2ptmvjjbe.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2uglnwrbk.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2afmvnnzd.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2vkzbqqxu.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2modzobld.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2atoykayz.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ghbuuprn.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2pvkzihem.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2dojigegg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2rkwukaod.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2xvqlysbc.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2gmbmjyil.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2uuxupntm.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2bkzkxoil.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2oytajxgz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ybdgzyyz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mfmrzily.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bfecxfrj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2aysvubns.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2rzuyfpxz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lcxyblee.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2xqdglqxc.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2cqxsxhqb.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ztoognvp.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ygtduzjw.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2qilgniau.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2jrehcben.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2buxwjoty.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2xtpkrpek.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2syveicee.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2culhxgru.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2tyrramtp.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2csivttsk.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vbtvkvhh.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2honjtnbq.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2ghyngjgn.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2oqcbqnke.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2utdhvdxv.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qdxgkkon.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2bzpvvkxp.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2aabfbvvo.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2ocdzgrbl.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2vvgskaic.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2rhbxfila.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2vnuomjqe.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2xxdohqgx.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2pkohawrz.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2pvfnuwjb.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2ojqldvax.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2auivdqli.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2flcgwbqq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2uiaimwoi.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2tlwvukaj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2mpdqnexp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2rdrnqace.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2nwvpqnzf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2dighfzxt.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2tbkargfz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2vnmfuuzu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2lahtpwmy.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2canerslt.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2odghynuf.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2hwjfuxfu.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2ydnjautc.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2vbbercla.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2shlynpda.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fvcfewxh.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2uqqktlau.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kpmdwbsw.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2fjwzedjt.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2bwjdingt.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2afsgxkrl.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2vjftspkf.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2cahdfqjr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2znackudp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2zezbvcsk.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ybyrmnaz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2lfleurdi.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2piewcawu.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2qlynmcar.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2tdsyvekj.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2jjodiqeb.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2gvyfpktd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2totpxuqi.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2ujlcailg.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2rvjqiktq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zhesjqun.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2vciqguoa.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2mfhwhesg.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2bxeeeuad.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2swaffsbw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2urzgjyyi.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2sonxwejz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2jlpcwzfc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2dwecxraf.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2urhrlyss.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2qmwkypng.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2cjayomva.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2jmihnkny.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2qpzddrib.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2zpehvkow.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2mhkeamgp.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2xnkybmjo.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2kwwtkssl.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2vrlwgjrl.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2klgjfvrt.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2wmdtmpde.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hzpdhjdh.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2xjyzalwm.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2qnxhqpmt.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2gpytcwjq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2ozmtjqsr.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2bxgmvmuu.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2wwbpxuwk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2gdkuumir.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2bsfyucof.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2srnvawwi.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2wcicxrcs.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2ncnqegaf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2szbfssom.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2njkcfwuc.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2uasdykib.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2iyyjevqq.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2qqjcaivh.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2ddajnouk.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2lrliydgy.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2jgibpvre.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2bdormoka.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2zesznfpq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2qvwsaabe.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2jwmapgzv.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2acojlfyd.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kjxgvcxm.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2rszvwchu.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2glndwzak.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2patfsrnn.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2bkgwgeoa.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2buklhsvv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2ewoixtlv.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2ewqpuwuy.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2tkgbspsg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kknicazd.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2gsosqqws.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yxumqvur.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2camhjmkx.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2dqaotbfm.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2xqjuafjo.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2wuytimpd.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2hvclbxmm.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2zojmurbt.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2vkxkwmhr.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2gxtbltkk.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2ellhicty.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ldhrndli.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2szqunahe.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2kdwitkqh.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2kiyfclqh.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2vngqqyqx.html


<!-- 参考信息 -->