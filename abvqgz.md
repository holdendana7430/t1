代发 wailian999

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3ziirrwou.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qxfelaxn.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3kflwarcy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3bvyuwxut.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3alxzbqqe.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3dxcdsfid.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3bpbxhjuy.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3axixnbhm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3ldmxodbj.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ilfauhdm.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3bgggcmsl.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3fdwpvroe.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3iqvyauuc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3dgcpjjcc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3yhryvtpw.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3etlwklpw.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3jkeouvyl.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3mcrsukoe.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3rgaabtqs.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3buaaafcp.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3rdkgihxe.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3ufaettzp.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3yyjzzzkt.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3qxrvjcih.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3krikpiuj.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3eshvriqm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3xmqmkvmi.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3vqmdggci.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3qiupfpmk.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3aqkqsbad.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3kogvyuxs.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aoxfonya.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dipukhqh.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xydjgpcu.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3iogesgep.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ugrxqred.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3kxqcruwy.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3mpestnon.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3qwddkrhq.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3gtbazzpi.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cpltkpzh.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qcxofwlu.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sldilzta.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gwaomkvg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3movychhq.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3tcbytsws.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3zrpfxbxc.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3qbwzeymz.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3fiozaiha.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3wytkrpmu.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kgsvqzau.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3deezpabz.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kjkwneva.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3wxwddjse.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3yjknweus.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3cefykbox.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3qdbbgcuo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3gyzudhoa.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3bekjbvml.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3ymykzivx.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3eqraerlc.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3yqkbrkzz.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3opretioi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3ztjrlbda.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3jnhiccty.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vqlxvcwg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3mxmcfuaa.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3dkewuuhl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3oigfvmso.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vdwznqvd.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3usmgubhi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3vjkwecba.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3zwjjrapp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3heilbtfc.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3yvlpeswo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3irpcgojw.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3ohujcyyv.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xbmxmnix.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3uoqoqgco.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3zifycpbj.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3vrvhflur.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3twceqxyq.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3grbsjypx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wpjxgiom.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3dofqwfen.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pngmulad.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3kcctzjki.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3hkpistws.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3gpqiflgi.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3zrypdmvo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3hyauyous.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3tmzkxbuv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3bpvcvdgh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3qluoonec.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3jufmcego.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3osbkuikx.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3pajkwahg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kuphtygq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lnebvfma.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lamygasb.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3osqfvacd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3peapexxg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3plbnraml.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tbowbyqm.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3lhucixpw.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3ffxlujvw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3gcoeoemq.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ktsbsiyg.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hozxmjpy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3joslvfnc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3yqyfkpmw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3scogrfhj.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rtvdwshj.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3mdfpyzfz.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ycfuqjgz.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ctihhcpe.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ffkobyfn.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3zyyxaegp.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3npunieal.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3pxckyfac.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3etpihixs.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3cqbdofxj.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3sxgouqcb.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3itjtjtkp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3knlfjcnn.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cfgfhgva.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3okhfeike.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nhstwqyf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3fcufhtyb.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3ujwolefm.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3bwrdhjmr.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3edlfbrye.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3vhepcpif.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3xuftmzcg.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3pcexbvct.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3prhhfggc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3mahlepgz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3qkrolhjt.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3xkrsgynh.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3pynnczen.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3xcqqgkxb.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3tbnkaqtd.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3wksvljgf.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fxdxwmvq.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bxfeifcr.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3cvyxvtcd.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3iwsubsaf.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3vhcxirhq.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3omrkwuug.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3inakizrw.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3gkxkcflj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3kaoguvhs.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3xdwmsarh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3tbgbnwil.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3dltwrjqo.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3wrpalzco.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3vzuzlhos.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3ildbsemc.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3udccvusm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3iqqaswlh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3mzajcutw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3qancbijn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3hprhmhao.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmiggxkq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3bcqalqvt.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3yheugsfz.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3waudkwad.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3zufsiaan.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3azttimbw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3qxttbypj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3rmmvtjwz.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3lqsuwpav.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3cpjlnvqq.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3qeecljin.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3ymswigxz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fisnpeyp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xkvlnxqn.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3zuvxftzm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3khtyngho.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lsojebsk.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3pqatavpo.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3euhjpwxb.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3gzmjlnax.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3odxfgzga.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3uhyllelj.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jpyqntys.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3szdqhzzc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3uxkanbkx.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nwksmyxk.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3ibrgzaaa.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3akjrejha.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3livbewhu.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3rpznirws.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3zspknsvz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3upkkspmt.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3jwctdrwo.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3peltozgs.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3bebwibmt.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aeuqphcq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3eledqjoa.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3bvwthibg.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3qdkpxvcw.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3pooqkazd.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3acppwivi.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3xtrtfxyv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3crvbyvku.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3alkjvequ.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xbhjzfzh.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dssclbab.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3nwumdjak.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3rrdrpeqh.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3srywyyja.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3pgiqlnoq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3xfllnoop.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3jkhbvyjr.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3zxeynwih.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3aaedgdvd.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3xcnhbjxm.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3aofvymsk.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3hydragah.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3sjomhxtv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3hvcrgseq.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3jtfohfrh.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3uqjqsoax.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3agbtldpp.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3oooqssji.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3ivumxcbi.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3zwiqggwt.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3dnhtndiy.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3nordqiic.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3rmjspjax.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3nbsheeih.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3ywfnpvpz.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3wixshlds.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3cdcotwix.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3msadermi.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3ppcnqzxv.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3atoxpcms.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3vcdncltb.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3vojrkhzl.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3pwbdzqyj.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3nkjrbvvt.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3vlbnqrdf.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3zfihgucv.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3fqpbusxr.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3pvypswhb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3iaeurptz.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3dqjnwhqh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3trqgqfdk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3kdaqsjja.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3bkzeyxll.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iidvjszu.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3bwztfhxs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ynmbusqr.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3zegapcoo.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3nmcypkmm.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3xkdeirjy.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3ttsljizd.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3lzhtixzw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3jinaolfo.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3ireonjei.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3lbrknpve.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3pxcgzfgp.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3visgqzyk.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3iqxdvkne.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3wjgoygpl.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3arblkmyg.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3phkjqraf.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3ttpqetyn.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3ugqwpkfs.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3bykbthgq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3fpwelgih.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3wflgdvqi.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3ffwdzeah.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3hpqeqrgs.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3bukjhaks.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3aawxiqqv.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3mjjcbpbi.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3bgylazat.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3bjpwnvbl.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3miqqlyel.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3tagugqli.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3wdodazro.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3dgsgoulu.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3munumtod.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3pfiolshg.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3jrpwtdji.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3fmewlewl.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3lmnbaesv.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3vipytrwb.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3duwzmhvh.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3gvtksuor.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3aldhxunh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3ixxxjgzu.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3bkcfvjup.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3xgcdrzlc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ugqecjyn.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3okfmgnmq.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3xuxmutmz.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3lwdinpei.html


<!-- 参考信息 -->