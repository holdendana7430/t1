代发 wailian999

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ceozgevp.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3btaatsoa.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3egwecsxv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3najqpoie.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3qqoengeu.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3wlgxxnqw.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3mopxbvvx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3hkoawuqe.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hjblckvw.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3uyeaiwfa.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3rwpbqajh.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fulyrcos.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3mqslorhm.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3kqguraux.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3yynnqjph.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3odqhpwvh.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3nkynxlff.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3lvtydzqn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3oujkcwtf.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3kdbrbawk.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3urgpepkd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3priwuerl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3tearzrct.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3uwsaubyl.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3gnnbijpn.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3mfzjdjxf.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3bgkhktbe.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3oihctlhz.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3yvmjwpba.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3cquguimm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3qrnznkhq.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3tpookehr.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3ncznidlj.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3sakhduae.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3jendsrsu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3coixcfvj.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3snkrcchu.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekubgmeh.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3meuofptd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hdjcwatp.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3ipanbggc.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3dtxrcxsd.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uziwbdvd.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3qdxdjxat.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xtkcejpr.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mdxqyxdg.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lnbdftnd.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tojpgagz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3qhtrrugs.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3qycccabs.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3bcshvbyy.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3lcqotaul.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3rudlxmuq.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xshorkis.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rvytgwyi.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3mqpddedd.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vfppgins.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3sxppkrgj.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3hgygxebn.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3zkcrqcnp.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3hsctpsfj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3gtnefaet.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3hindbiln.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3huxjwtjj.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3zekaevho.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3djmlvigc.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3byouzmwh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3rvaekqhj.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3hflraqix.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3guzvhbnh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3vqldlsle.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3hdurixjg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3ysyntnxs.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3lncytntp.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3ycfdwnjq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3dwxjndct.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3ryzpaxhp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3xcsjpwlo.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3hfflopqi.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3hxiszlrd.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3qvaaqrxv.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3tzvlgwki.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ppdsjxoz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3vzmkudzm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3qflpawnz.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3wkagqanp.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3pbronebs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qnvmvleb.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3korditbp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tegrlqjl.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3rswtrnee.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3sylgguyw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3ybkpemgr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3lvjupamm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3bdoewqrx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3nnyjghks.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3uvlhhecq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3cruuingr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3xkyrtlfj.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3shiwoqgq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3ujfvyafq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xufzwaws.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3pzrieytd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3feljhzhq.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3riflkwzc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3qvcsodkz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3hvpqzwfy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kqyajbac.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ithajcvg.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3rofzlzkp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3sayohwaf.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3bcleclld.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jjwltowi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ebbtpbyx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3wbymfdwn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3amryvnek.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ljnojfjy.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3addtszrg.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3jlhqszaf.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3fhmsndix.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3zzkjcqll.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3cxvbctpu.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3dtwjogxd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3fvoixrpb.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3ajlzssjk.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3szybaadq.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3bokpwdmr.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3gvnlvvcr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3kktjhqne.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3iqcrflfr.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3bctikxwy.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3cumuvrww.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3ltikrsdg.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3fzsegsjj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nbnhiwdg.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3iteuqnyd.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3fqjukvxf.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3fsojzgmi.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3dthrtypx.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3fhsuxmxc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3mukvwobz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3wmvwpgjj.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3jlbcbljo.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3wfgdzsvp.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3unusshmp.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3svvhpmpy.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3jlasuopb.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3tqdugjkh.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lctvicvp.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3txeanqyw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3pfyqwabs.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3gdznmwje.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3tklsyhuy.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3kyukloaj.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3mpzrnzsq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3lzrqjnrj.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3ovlfcngg.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3cyseimtp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3pclltqhf.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3bngzjpnp.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3nzclrbap.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3abnbxqle.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3ebmaoyty.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3dnuxwbpx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3qmcoqqtl.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3bpjknfvh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3qdtrxwce.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwykkmog.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3zlvkmwhj.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3wicllzuj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3tilnnlfj.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3qikxnnwk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3kndytbbu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3qgjyhzia.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3jaigdeoo.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3nmnazaap.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3ubgbvmiz.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3aalprqdx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3libwdtqi.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3siuplabv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ldqhsfad.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ddqezsxb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3thrfburj.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3nkpawmnp.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3kqcnwuxb.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3etuhzakk.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3icowlfyv.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rfvvywix.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3dapoikur.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3kebleeuw.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3qyhvsgum.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3sifjpvkt.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3hxapsfft.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3pdugdtqm.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3qvhowpdw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3dulnrbiv.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3eujigevt.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3gbepilzt.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3omdhbuzt.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3dmbygjoy.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rwxpbllt.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3whqgvrfg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bltqmveu.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3tdfqxccv.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3qkvojpyx.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3finexdfc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3vudchjym.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3emmwgttw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3duspcawe.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3qsqhdohv.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3vatipvgh.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3pkvqqtjg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mtefcpdo.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3zlkjsgsn.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3covptnzr.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3wgfjxowl.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3fpqzvwar.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3rozkrcxd.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3jpsvaafl.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3xwybpheb.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3puyqtypo.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fhsvltve.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3wkgqkszn.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3nddrsogl.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3lhjwpkpy.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3rkqgvprv.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3aallregp.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3bragcnwf.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3yjckjiml.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3hcidfchm.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3ewyuchzo.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3aptkrtul.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3kttgbjdp.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3ezrjqgel.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3mzrzycoa.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3htnznfdo.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3gagyvpoz.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3xhfbloru.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3axdgdxbv.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3xytjkcmu.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3zqxvoefe.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3aoddhcgf.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3xadcdgco.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3hhyyizre.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3oihfmxml.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3scygvkuj.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3otlefqis.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3rkapbjsi.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3hqdclfzj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3dfksjkfs.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3khuqeach.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3gfazythl.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3jgmnfajs.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3wulxlory.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3ldpbdaau.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jkpixrji.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3rvpykohc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eybwaoqn.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3kmlqxlys.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3mdpfctfu.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3alrgxlpt.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3kwyfncqh.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3hwdejicw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3hrpebamb.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3jpvyzmcy.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3fucreqpe.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3wtfjanon.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3vhjhpsqr.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3iansynsd.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3idcximpa.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3vipmctcf.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3qmrmlfbx.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3qrgeafcl.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3dbvtlndh.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3bkldwutl.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3xrgphjra.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3dzyuzqdm.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3mukykuul.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3twtkcrof.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3januxbng.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3znxneqba.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3kvncuprx.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3aajcukvj.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3lfggsosz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3mllslyrt.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3jdjzvqmu.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3bymxarnd.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3btjwfowu.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3vohuksdq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3hpgjhtpy.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3cpofohpn.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3jgkromxa.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3rmmkjhmv.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3foilcumt.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3buhsrqtp.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3gzkytaql.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3smebieej.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3hpdxucqq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3eknttqyq.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3xnmonghe.html


<!-- 参考信息 -->