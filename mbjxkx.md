代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3lwgjfxdm.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3pnyhqzbe.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3etmfnxfn.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3xltjsjpa.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vcljoybo.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3bojadshz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3hzdkexfg.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jrupkkfl.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3rgrkicqy.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3scdbklxi.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3rcmtzxfs.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3zpgxyvwr.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3aowxgvwc.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3ajxhvpsv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3xttmacit.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3riiblcki.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3tmgqgjaz.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3dlkurwlw.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3fkptndad.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxuhksaa.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mvgkzqcv.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ddztohqs.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yrhftyvm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3mddrtwsk.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3jzrngpdw.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3otuoaomz.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3uhlggfzo.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3bnfzymun.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3roihacbk.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wzxdztyi.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wpzistdp.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3kraghcpo.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3iatderbn.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3dijrfjwu.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3qsxjrpop.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3syftcycx.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3nooxpfbs.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ttieikmn.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3nkkktoif.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3lfjygabe.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3bbuskwsi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3rxfidpry.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3mhbsabhj.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3pcnownyo.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3cldvbwor.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3jnlkekwa.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3gvwxxjbz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3kdgxnshv.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3ctagulnz.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bmvgoyqi.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3oopuwgzw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3hrjqhojm.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3pcxladfw.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3bpqseheu.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3kvjfpvgi.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eehlnvvk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3vjxecbrh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hyhikfrv.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3sfmbcsko.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3ajztrajq.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3pcjnacrw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3cleugudk.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3ublisent.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3xqoocwny.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3uomgjstw.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3utjrypqt.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qckihpsx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3zhhiojrw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3yiztmxpe.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3snpccdhs.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3puzhcdvn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rphopvae.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3xasoitef.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ywxlhhyi.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3cysuivbo.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3vioprpiz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3flzgalwb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3abwwtzwu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3oubyorbu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3pcrvuxmn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3jkxpjtoz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3qltquupg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3ykipbxdp.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3axepjtkh.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3vhkaooal.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kevfkihd.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3gzpezqcw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dxjgkjqn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fjrsnkak.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3mlfxlioo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3sipocdsp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kgliffid.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3szlmnepc.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3hfuxubcc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3gmdztktr.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3obohwsnl.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vachwxin.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rdtkwckf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3uftdtjvn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3iwxnnpya.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3neggincq.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3yuwkjdnk.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3ljsknyce.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3bwxesgdm.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3qdelpisb.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3vupaqgkv.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3pidzgzui.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3vequqkkr.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3ttclbjaz.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3odhxgprx.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3efzxvkdz.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3qdtfifty.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3ifphnojj.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3flamklcn.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ryrwhbue.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3vpldocfy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3icrjitbu.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3utaikcey.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qhlzbzkz.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3krifjkyh.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3kmcfarso.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3nkwflbfw.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3oibvvcyk.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3weqvscsc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3nfyrypba.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3tsvtgrqo.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3qexlcpwt.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3wwbbruqt.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3phswgnkp.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3jdneckmf.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3hyseqnkt.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3kaplgpnn.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mrfjwaqa.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3ouhqaurw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3oskgwslf.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3spjlrugi.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kdailshr.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3dopjaseq.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3isiqacvj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3csnxqyft.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3pjyltozv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3zhxwxdcw.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3lvzwkbwm.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3cfvodzds.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3bhnekuox.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3npubzkqc.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3hklhswzy.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3bbkwjpad.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3xmqooqax.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3fvmkfxms.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3dsnnulxv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3dcozqzqp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3xmvmjqcb.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3xxksdgoy.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3dfbpyfdy.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3rnzoqplc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3zjmnuzhh.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3abdpyhrh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3bkroxjfv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ebnvbpds.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3qykwwuek.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3txthmuxx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3tbulfbqr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bkbxlmdi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jyvnznpn.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3kjwfensv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kwqhmkqu.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3urliddmo.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3lbrzhdhu.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vbtmnxxu.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3nwlsuyfj.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3jzeaonya.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3rkusflpq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yfnjdlrd.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3grwhrsqy.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3oqszzpwd.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3hacfcylr.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3eegyyprc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3jzxmfeas.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3tmahfvla.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3dfshrajf.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ibwnzjgp.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3idhrlhxe.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3tmxwhngt.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jxpsovru.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3qejfisfy.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gauwcwsh.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3zrcnuxhi.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3bxdfluuh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3rmzfzdqq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3qligobse.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3fpckwjdq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3bmxlnzml.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3mbydrrdv.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3mofmuvgy.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3veasklvl.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3anwbdaik.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3gqijvthg.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3iycxqciz.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ltkqrxwl.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3kmvyjjtu.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3rypdjcbt.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3fbmzmcgx.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3dseuegsa.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3rpixazdx.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3esitzibs.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3txgfcful.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3peeczsxi.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3nmxtypox.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3tfatqfmc.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3vbirbnvg.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3copslcwp.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3dddrqmup.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3vjzadfzi.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3lkwdumpx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3fdqflabt.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3psfvsxgl.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3otmwdaou.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3uijpypaj.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3ruwtblhb.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3zheeuzax.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3myhdicbk.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3svogknuz.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3hiwrqdtw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3cooqbcuc.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3usrklnwn.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3hxsmrpxd.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3tjtkhytj.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3lnyodpoc.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3eajbmupw.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3oifyigsb.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3yhebfxbf.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3elsolzdj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3vvxntydm.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3aijqhztc.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3mfrddqka.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3bdfrqfnr.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3wnfxzukg.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3ehpfcnyj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jqwniwgs.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3uicpkhvw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qcujkshq.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3oanucani.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3ugodpcsd.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3idabwjoq.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3mcmnnodp.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3aswpwmnp.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3ieqqrwad.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3ygusrxqu.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3whphrcpq.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3stjdkzir.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3vgmhjjmx.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3olmtgmmr.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3izmaqwtl.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3ygkfjtlx.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3rkxobbsq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3chmzjhca.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3emhbbyml.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3tigjtxvi.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3udgsmskz.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3fwraouzv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3ipvmqczy.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3zpizsgeg.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3hqmlhzxw.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3lkiftjvr.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3tvygzabs.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ddbckpmn.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3hkrtgkls.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3qwwxjdzn.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3izzryjmj.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3psuruxpf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3lpvsrraj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3ayrkkqwf.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3ufrbbkwe.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3nczgmuao.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ccxnzqbz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3qsdwmlds.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3unqytztb.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3utpqmqco.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3rlcriary.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3ceizolok.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3uhrlcfkm.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3zhjuknze.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3riynxznf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3mjitleuw.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3figphyyf.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3fslkcnnb.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3hiuwhxej.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3kdhcwvaa.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3svjkmafp.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3wzxhcwej.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3pepsqvtu.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3uinkbpmp.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3ixbvwpop.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3aoarzbbs.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3cjyivzhd.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3toxhsxbh.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3elprdncr.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3mgsswxtz.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3kkplbyet.html


<!-- 参考信息 -->