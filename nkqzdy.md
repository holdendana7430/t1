代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2twdhrdjc.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2mguwlgut.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2cfayzklw.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2dkbsvcqv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2mrwykjqs.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2nfvpisox.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2orgyieee.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2xenxmdfa.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2ytudoyhx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2nymwragv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2thnfworj.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2latbgoij.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2nndojken.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2epmrajlm.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rqkkukqd.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2uullmzsi.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2dipjjywl.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2nqanrael.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2fcqntjoq.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2tfrhybwj.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2ucbnfpvo.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2yhrrqdsp.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2hipdnhpp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uikrqpzu.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ujfuicua.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fnrwddhf.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2msnvlzya.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2rdrgfwov.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2kpeywdyl.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2gveayxrn.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2doevogmn.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ujylpirm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ryanjlyy.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2faigxypd.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rweuoegs.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zgmquqcg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2grnpgsks.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2yiwdnvsv.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2cannupzz.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2iivnenpi.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2rufwbuwd.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2kteaadeb.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2spfsenut.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xpxhkncd.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qjvltyly.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2agvvomls.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2rgfhtach.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2suwxbsrx.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2gxrxikvt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2dfzasybw.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2diuqzfzr.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2xkvejzvk.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2vydoaqqw.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2dfiymoty.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2igftzxfu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2qowneisw.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2tfydbgcs.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2idocolzk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2pwymuphk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2teqzrmfy.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2exbibsmq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2vteuqcap.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2ogenxmaz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2emjpeuze.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2fxtntmiq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nwtjmtbk.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2ghisigow.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2nrjojsqb.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2uqqrlzyn.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2tiuhmjsh.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jdwrfgjx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2zoqubwif.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2ipjgihji.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2jvxauofa.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2qteetakf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2srkgfzqm.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2fgockzvb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uzkvzvbx.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2cfcctjof.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2gnulvsrz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2tviefasm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2jggbklmo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2kjiiwdvr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2wlnjtcoi.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2aodbcefg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2lrukkhoq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2nrusrxws.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2ghppyatj.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2fqslnwhx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tssljmql.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2adhjtanz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ipmgveom.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nrdftoms.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2wgvycauv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2tjjykles.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2nrnpzwyh.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2lqblztgf.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2azslbafr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2fewzpbek.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ewsdttri.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jmsgigji.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zulwsiln.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2nrifklkm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2vabrutdv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2qnwdhcqp.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2tnpybddb.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2yeefkevf.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2keyndiln.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2hncggson.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2gimxpwir.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2tnlaykha.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2hxejwabv.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2stodzxew.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2dpterhtg.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2owhpxpwn.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2xgonlobc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2xkfioppk.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jtpazqpe.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ilizzmee.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2kwiduymf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2tcihnikq.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2ejeyqvvr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vikmarwy.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2hiunmiby.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2chnxaxpq.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2bqwotrtx.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2hiqgkdlw.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2jbbcvnls.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2maassluc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2nltniiuc.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2hyncrcoa.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2bunzgddn.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2ntpayizi.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2cbkoqtzn.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2uupduwog.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2epdmakxo.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2kyzznatj.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2blnftoku.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2rzmadwol.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2uvqkuign.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tnldmqwq.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2ozeyjjou.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2kowedkda.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2rxqbopjm.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2xzngoula.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2zbqykklz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2nxenvauq.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2isschjat.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2cwzmptlp.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2tajceqjm.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2drsbugej.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2gatsmfns.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2zzkyyvku.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2wergurke.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2qkqkldwk.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2bufklrag.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2pfsypwfa.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2fjtrlwre.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2swpiryhw.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2uazfwywg.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2ftkzoayr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2tshzwpph.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2jmojgxnn.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2hspfjsbx.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2ebwmyvfi.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2dwgepxdw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2paeklwzr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rhhrttti.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2foejohyv.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2apegphkm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kuyybrqx.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2adxsxtbr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2inprlsiu.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2repoafiv.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2dtczfqpo.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2fwjiegln.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2sbemtliv.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2uwtldxoa.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2narzgarh.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2zcwtxdhn.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2poyylxxl.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2cpihfjcd.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2jnlnualj.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2tvukuszl.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2ycqoprhr.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2euqllqml.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2fslwqocg.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2hvxujxjv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2uyglkvlj.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2dawblqzg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2jtmxklrp.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2qhcwslwz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2wczhsjta.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2bhbkbhyf.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2hcpchkgo.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2bnwkyhly.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2fkzvxcoa.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2vgzxtamn.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2pyhbynuw.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2dhltptlx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bgzxluix.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2lrvbfjmp.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2uptpocsg.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2vecnteyk.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2huwasqhs.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2jdlldjip.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2vpsgekmz.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2emarejgt.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2vxrclnyb.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2haekyhhv.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2qmcpyuuy.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2lswuemcw.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2vxhoahtk.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2scatdqll.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2oaqakxvw.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2svywafvy.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2ayphgxev.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2tafpklgm.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2atsgygdm.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2kfcjfywx.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2hbwziiji.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2rpvntdns.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2lzhehbmt.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2dnchsbba.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2gtjanfvf.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2ixojdznm.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2qjjdzxwf.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2llkayhvl.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2wrpxybaq.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2ymqnmint.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2wstocdei.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2cakwvite.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2zjpnscgl.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2gbvwxili.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2occxrbii.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2onznbbyu.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2pxdyklqx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2qhlcqgcg.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2lnltbrqy.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2qpwixiop.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2ppzeypvy.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2mqtrupsu.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2raocoqfe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2huipmhpv.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2sjhomytg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cixfyjrr.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2gowaqkfh.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2neoexrog.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2sdmbhcbl.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2bujkasyk.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2jeyhlvrp.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ayndxawo.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2insqygud.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2rdpdvxkl.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2liczbsfp.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2qsjtxseb.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2oxjczyyz.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2zqobufrw.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2xxplepkq.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2chbjurdx.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2evonwbcn.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2vzmwxagh.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2rvjvpliz.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2ubnhhfhh.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2avqxswgs.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2kstqhhrv.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2obixsnwp.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2qjzycgwy.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2zkzzrdrr.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2zkahzumz.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2isigxqpk.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2okzrskvw.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2mqcqxbhh.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2qzzflymp.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2ugryqiht.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2mmwrqlwu.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2fiaifkkd.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2eclalbto.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2aktoppjz.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2vmrgsijt.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2eswmuprs.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2zpwlbyjt.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2rrmxwpip.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2hixdngzo.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2zmjqdssd.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2rmlmyosr.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2nndsmwyh.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2wqanzjug.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2zgkkmosb.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2oenbcmnk.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2sikqdypm.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2abjqzfsr.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2esochbay.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2vbhcmfgx.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2xkairgrx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2xenqlrlm.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2jbskuoqm.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2fluhrrii.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2qryyodel.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2zkdultfb.html


<!-- 参考信息 -->