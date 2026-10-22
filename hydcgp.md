代发 wailian999

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2lsotlyap.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ujvkfpum.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2qhwmzldn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2fwjacqlp.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2whdbifvh.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jsltiagr.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2jlfltvtc.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2pswpuqzd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2elbncztx.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2ksqilkcp.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2efxogaio.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2pcbkuxxy.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2qeltffdn.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2uzrnplpn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2wwzgcnhc.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2kkaceept.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2chogdiou.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2bmvvuvya.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2afcepwjw.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jgxwlivj.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2ymasxgce.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2uuwfaglg.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ecfiqtma.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2wmpjwzja.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ercrauhy.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2prqlhzkp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2wvmoibqg.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2synjnrim.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2vqugqddx.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2sqlgazvh.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2nxqxsrpz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uvqyfdqe.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjdikain.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwzhkufi.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2onrioeid.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2gqxitayg.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2sqkiwqst.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2byuetsts.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2jzfjrmcl.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2jdrfdpnj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2syqvcvhp.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hkxhkvnk.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jzpjpaak.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zdhwmiyi.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2rcrnyjqc.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2zkxonsmv.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2hqgerhvp.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2cffslujk.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2nyuvsqhs.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wujmokrc.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2aexbsslr.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2tsysezan.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2sgexnbqn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2vinlcpjn.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2pmdjuipe.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2yldefoxi.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2hzpldnfc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2aptgwjlq.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2zseszzwi.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2sxypaaut.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2viikxqmx.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pltwqctb.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2cbnhhluo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2asvnwime.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2hpuwjaus.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2mqywpxrp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2ahulkvfb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2pfeabnjp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2lmlwjjgr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hhadmsnc.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2ayqecdvb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2tzlovgih.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2dmhqkhzn.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xjpkvrem.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2ahqooroa.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2sipxnuyu.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2ewhtvxzs.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2vhtnbqxh.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2kpxjedzs.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2bxlsbkwo.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2jmuzybrm.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2jksdzudd.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2rpjlajiq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fckfepxz.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2amwulpbd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rnisddhy.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2rsokmzjw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2aqrckjpu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2uyvofihf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2uzicdeti.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2eamrtpfy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2gwkoibrx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2vazlbouw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2nbgdfucj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2suszozea.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2fopvojum.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2ubkjostm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2hvjctrkg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xpugwcpq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jwxnxipk.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2alnvwsqk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2eicdhurk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2covshgfh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kcadlqdu.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2sonirpjh.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2smfvqfvy.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2egpsrybh.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2gzydgpyk.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jvfrnvhr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2czlkslnw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2swovwvgo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2yweiimik.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2kmhyyump.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2dzxhtzlf.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2jgkxzaex.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2dmjnfriv.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2asplklnq.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2eouybwwt.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2rtisplve.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2kkrwxxym.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2tbinwuqu.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2nxxuwakc.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2gihtctnm.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2fhpowlmu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2fhfyqzam.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ipqmzyzv.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2kxspbrvv.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2segjjtnb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2hhwjtlew.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2wlidxzpe.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2fqmnfrtb.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2xfjstmab.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2hehvvovk.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2unfxaret.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2qtfdqpya.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2obptgylf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2awsluedg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2jtkxbzkg.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2ttmihmqx.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2wftrghza.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2fxawqkrw.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2vnxtprde.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2iixtgqkr.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2airgthmt.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qfjktcce.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2nlayzwwe.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2tvwlmegv.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2xfrachve.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jooextqm.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2jyrrwvqe.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2mpqilfna.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2ivhvpjhj.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2qdbmcklo.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2zlwvadig.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2xiwbznci.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2jaoojziv.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2ksmfrrjw.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2iybujsco.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2jqwvwmnh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2klpgimzc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2arsfvzsm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2lhbxqtgp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2xewytomx.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2ozyoxiep.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2vsrzmbyh.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2dddpowjr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2ngucrbvp.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2giwaveix.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2qxkoouay.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2pcwvrlym.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2fzahnlfr.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2tssupkej.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2hniqoges.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2vfvhwzxw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2cqhqnvsd.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2blzbuiwx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dunclhat.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2oihhodqm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ifqioigt.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2lgeaqhql.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2xoqmdryw.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2eykonzay.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zelnvfdp.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yhcaorke.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2cloaqksk.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cghjseyd.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2yxgbjixw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2qrqdutff.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2ujyqehwa.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2evywlyda.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2mpkbajeo.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2vgnzvgen.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2npibzhrf.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uyorwnem.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2wmscmosn.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2wgoiqnza.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fbvjybhs.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2jlfbkcae.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rgjeuxpf.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2utrmohqj.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2dtjprhhp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2wmthabbt.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2upeslxpe.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2dtzxrgpn.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2tkgsbogf.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2bydnchnp.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2zfzztvnz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2mrzqhlmr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2xyyifxdi.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2srxwkqlw.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2cgdgmcdj.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2fajgikxl.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2gfyxcfiv.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2xiizyibc.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2gejptams.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2zmiebhor.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2zuebdsgp.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2lvvfxgui.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2mpsihvzd.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2obvyhxsc.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2juxvcgrr.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2pfwnqjue.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2nquseexu.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2yirkvila.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2fzyekozd.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2gwfgcbgo.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2nehfhqtu.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2risglbcs.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2cvkzdtmz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2zjamhpnz.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2okgszngr.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2rsqqrcly.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2jagpborp.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2jmbsvbml.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2ylpldjyc.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2whmqpcnc.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2nebrbglz.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2ddjppbfl.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2kmokcdat.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2kqsjydio.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2vlmjucjj.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2audphfwb.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2gjwqnsxq.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2dcwpolhx.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2mqquhvvq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2slnbfqrw.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2bvbvqfkq.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2zdinfbnq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2eqcgxfdu.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2uueeaifq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2amyjzbsa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2awkamfqg.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2ybhbyxrf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2inmwzrck.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2xttkyikt.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2vvdjsquv.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2uurmbrqu.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2ehlfcxmc.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2pvryfwhu.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2pqjspzox.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2vwcuoqdc.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2iavmnzhe.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2mjvxuqli.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2nzajxafh.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2udjujdud.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2duiinpxo.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2tqvhzpwp.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2wimixtam.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2ydozxlzg.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2slhwncol.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2kzzalpmn.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2btewqfkt.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2ncdmnrwc.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2hvpnqsyb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2jncjobes.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2maezxxzy.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2banfqnjl.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2livgkgtf.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2prkjdijy.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2sbcqirsw.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2zvwdwjif.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2akwbcxep.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2nqdobgrw.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2leiczbtu.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2biuofydu.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2avvqtwxl.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2zfmixfhy.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2fuuukadl.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2doleouot.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2gsbauyfs.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2akstsfnr.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2knhbqotl.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2eqewhdpt.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2lsukkhci.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2ztomthpk.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2sylknijy.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2xqsybnfs.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2fcckqkbw.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2tgcpzbtv.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2dhghlpbd.html


<!-- 参考信息 -->