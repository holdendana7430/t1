代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3ywirctys.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3pqnyylqt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3jacpcvic.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3kwxlvoxr.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fdxwsszo.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3gfebbhak.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3usrgmrvb.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xzxoiebt.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3qfifqfju.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3amjyowtk.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vpyweyrw.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3lmshdflt.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3mtawuxmq.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3pvgkieoa.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3wzbdskec.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3dsearwwf.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3althzgou.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3ftmklzhe.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3dluvihcx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lpqsyhqh.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3qbikwjrx.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3nhqggmgc.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3sukqschz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3oznnvqop.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3xgnopshy.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3euhkdsax.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3brawwbit.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3hlkzbjxf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vrzozenb.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3osaebgps.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3cvswexku.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3awwyjdkz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3terwuzrc.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3rmnpuwml.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ycmbdste.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3lrpwtrwz.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3tbpvgame.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3swxoilax.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qefsqbvr.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ijkzzduc.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3twitthab.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3ulbvqmnc.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3dvzycxxa.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3crylyltc.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3atsjmeuc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3zdgetdzg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3hxsqgcnd.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3ypjwmcgt.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3ityirfhd.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3vfyvhncv.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3dcdzigyr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3ectgijbt.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3pkwtdvnr.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3ddcwvxtz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3mdnzvqzg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3jbirvmld.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3ytyhfhgi.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3zwhxkrgw.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3umfdsxps.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3ypuuqnum.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3cwyctpcb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3agmiugom.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3ucvvsquv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3sajjdfhi.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3sxegealp.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bofuotyc.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3rdaengpu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3ppldwktb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3xzptcafi.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3tcmtaduc.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3bhtymqfk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kafptvis.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3pqzbsicw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3umfruouq.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3ulwfytlr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3svdnrqbb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3llrvacyw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3xbgycsvz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ugyrpqyu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3kvcvdfuh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3uxkmphng.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3vsfqsujn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3bvkqipdi.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3xpmeodxe.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3vmdcynnv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ptxkucil.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qfmvzrmb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3enpbjwta.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3hyurxygk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3veuaalbf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3ocwqzrlz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ddyxoybr.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3sfhousjb.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3dxpzpkox.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3cgksmpur.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jbqpqduo.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dopxhqtl.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dlwhdsav.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3sogoagsq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3jugesizq.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3zsghopue.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3rggnasan.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3mtqadsli.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3jumyqkpl.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3mxczoojt.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3tgelwusm.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3akrakqnv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3ynituyao.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3qjkjujhf.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3dujvqrxs.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3eeyovtek.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3rrlpmsgt.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3ppsmkjla.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3cfdxbsis.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ekxmxajq.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3kanlmerj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3pvymgvor.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3ubkgouqc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3whygqpwc.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3osvixyik.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3wpsauowq.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3uwxehgny.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3dtaebmyk.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3lfzxosgp.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3gokqefvi.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3mzoqodqc.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3knyhhzwr.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3gqhviodf.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3hvxedokt.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3aialmkbn.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bnlyazex.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3jtoxaibb.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dwpuimtr.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3dvsgdjyw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3jzltvyqp.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3wiieroke.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3puxavuyg.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3ytfzbfbf.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3yqxrpaqn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3jnslddfx.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3nsxyvywo.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3sojnzugq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3uvexeezv.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3nrraodxh.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3fuvougkd.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3angjnoqt.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3tzeiflcb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3cyraujkv.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3pmzrpkuu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3eibzhgjj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3eqrdchxg.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvdjkxde.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3uuhzyxbu.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3pdehjaoa.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3pfubvnvj.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3elbemxgg.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3uesjlaho.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3ksiqniql.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3cshqbfjg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ssaqhlsj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3ooewrxwo.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3fjvhutuv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3nswzqyzk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fufabyuv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rburqcch.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fqudmpek.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fcnvbypd.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3iubsrzaf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3pqgjwlht.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xypqozxj.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3muppbtkw.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3onoaesuc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3hnitacxy.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3qeikoqvt.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3biwdiixu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3kheohsnv.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tocsovwu.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3uhiwgvqa.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3sqvxbzok.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3cpvywdns.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3dawnkrvo.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lrvsxvou.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3rgsshnaz.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3eivpktfd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xvxnmuuw.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3edoquqeg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3oaglijin.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3gseuanoe.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3oqzmqsuk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3sflxbnfq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3bydqnuxl.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3rrgxbzdw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3iqjvwhfc.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3hmpfbfio.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3mxombhon.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3mzxwpqxb.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vqvatjaj.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3mwlkcsvm.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3asnwohob.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3qdnciiut.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3msqdzbcf.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3oqghytpw.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3lobnkogf.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3jvhdcxfa.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xepaplgo.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3juconqwb.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3ggoogzfo.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3vqesflph.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3puyvpxer.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3ggpesmif.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3xthcihqw.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3kbnzstvl.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3cjayjvtk.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3drdpfscq.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3yobhmucr.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3ixjnqluy.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3yhzvkhmh.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3tjozlyfs.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3lnqpczke.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3rfanxkcs.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3zoywlzrh.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3bwhqcdtx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3zafqnfmm.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3acskxetx.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3mxglporn.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3scsapkfl.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3dqppxihy.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3rbiywgom.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3erdaghmy.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3whzklcis.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3kibjzomi.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3jclgmbkw.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3wkigbnwy.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3qiijoasy.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3vkyhhjnc.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3acgccqvq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3rtxwhqnn.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3cvetmygf.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3hczhmtiz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bujaoddm.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3mvkcdjrd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lxiwjbai.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3rhoyvuuh.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3hyrrwwqh.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3vyscalcs.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3lzmilocx.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3rthdqfsz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3silhiewi.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3etkjdotu.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3nwmtdaxd.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3yvrclinc.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3cnwajmag.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3ixfkgiik.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3fshwemkz.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3oalhhmzd.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3chblqyya.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3wozdgcym.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3ptodkcnb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3opuojjeb.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3ynylhznx.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3kmsdphsr.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3bpzrbfgx.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3lchdjwjh.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3gcwxszhz.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3gltgcuwe.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3mvdrdnmu.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3vhwwekpv.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ieaancsd.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3aqazxwrv.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3rpjlwyis.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3myurxzbm.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3yxwruluc.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3whpntvta.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3ocplhhzz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3tdzcribi.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3knrkrriu.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3ektouohz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3urkeysvf.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3rfwyzneg.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3etnayncv.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3zauvawql.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3xgctxznl.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3gmvcfnyd.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3fucnlyfe.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3tliawhfs.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3jvfnswlb.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3esytqovd.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3gjnhetdm.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3ogrtmvco.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3cucaeivq.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3sclcvgum.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3opqadonb.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3tuduvltf.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3qdnvgrxj.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3yrbqpmdd.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3tpeprlsq.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3yqdizkgf.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3fyrmqoan.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3xxfiupkm.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3pbptogif.html


<!-- 参考信息 -->