代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2sgzemqzl.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2dupwdzku.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2orgkwtag.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2iatsztcx.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2mopbnmiq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2gqyaanvu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2ciffzavi.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ttofknhj.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2gwmgztje.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2cmedyoqw.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2kneelvml.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2oxsmbaii.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2emzycplp.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2oinzoxsq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2gqhhqrov.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2uwumqpqn.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2kpibuejc.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2wkslqyzk.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2bjledymc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2jaghgbct.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ddjzxhsi.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mvxtfntf.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxohvoma.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2qgseoulr.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2kyjhbmjr.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2qpugfswq.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2uwpcktsd.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2oopnxlsa.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2sokuqrig.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2anpcxjtl.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nqsidmba.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pgfhsnyc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ulmnyktn.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2aqhzgnqo.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2jbgjufao.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2pdarrpkl.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2dmrpjgak.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ztwtdlfu.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2kxpnabji.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2sjpjdqza.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2pkgkuude.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2qobhfsbc.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2vpwcemlp.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2mzyacgeg.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2puaqtmgm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2pazbjphn.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2hhjzqiyx.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2vkmoamwt.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2sutgkvoy.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jfnajapr.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2layyogju.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2xwyqkceo.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2irppqyqw.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2tqvzjgvj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2kjlbdaug.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cpbzkfld.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2urjqscbw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ziachnef.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2gqrlwcma.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2hfyaaxtz.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2gdqybdec.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gulihvqb.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2bssarhue.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2jvjynacb.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2zwbwzvsv.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2wjtmgvjx.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pkulqjgo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2dxgehkdh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2jntmjpbw.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2etuzayhw.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2cbeprehd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rcilgenh.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2tzbtcvae.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cafhmpqe.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2cmnkkurj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2ppudpvoo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2imitogpi.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2jdqinmiy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2jwmxhika.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2mukoyrcn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2xjyfsrha.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2cwafuern.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2qxurexgy.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2poojeudg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2bjekegmj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dyddmagt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tptuokdn.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2msdmdmjv.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nhlaxkdq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2prmuckyk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2gxcccjqg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zhnjogmp.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2bkrnuoif.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2ctyzttla.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ntyqyatc.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rbeypast.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ngjvcecb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2pahljxnf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2fjknpegn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2zqfsokzw.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2bukkslil.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2fhnpvqwx.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2rpldimyf.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ceatnuvf.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2hqhmzqkv.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2puvyozpq.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2pmypknwu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2gnzjkaag.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2phgditck.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2vlcsoxfl.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2kheqiagp.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2pjielxob.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2btvssxtp.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2vswhdiez.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ebsyxkzp.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2xayxdgyu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2jlmnfpif.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2akztfjtn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2niorxswp.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2bjfxurwu.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2dttntfxr.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2xyvqjiyp.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2xdxootuq.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2fkzqoqll.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2lysssuil.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2rexrhobd.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2wujlzbso.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2rrakqvfw.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2yafxrkhy.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2uofvrxub.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2eoxkpotk.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2chpdzjop.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2fawnzfhr.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2spqgharr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2oqxfends.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2aehafgup.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2slmysqbx.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2kcepkxqq.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2beeniowm.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2gaonfbvc.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2emykqrty.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2zvozyazb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2fqaafynh.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2bydiomla.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2zxoyvwud.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2luojpfok.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2rveovmby.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2yzyvxmvu.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ovetmixt.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2tbdscvrt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2enkhkaes.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwabimki.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2meqmzcgq.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2gmwzzfyu.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2gaamqrhx.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2qjkvxghr.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2uogpaemd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2odmtvdyp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2lbzrbakh.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2bgzhcylj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2eikemmqg.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2maxmwuts.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2tydnhvil.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gzbyksnw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nxjvtcao.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2nkbrqcfr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ftudjdye.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2vcpuyqve.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2cccssaqy.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fpcwvidr.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2ciqpdodl.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2eghkeszm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2cztmwlan.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fpbnfeoz.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2lxhjacoq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2vaocdumf.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2xozimwfo.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2myaqtpex.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2lnuncdkk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2kvlrmwxy.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2aoobjriv.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2zfswpjci.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2hoacpfwc.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2yniapwxj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2kwakjavw.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2llvivwbh.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2tpscfiac.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2lqfogzct.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2tknizwpm.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2pzwqrths.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2dootdius.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2joxpcjtg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2npyvfhoy.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2lnigfwxo.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2kelzwsfz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2gsdwmkta.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wygdrpgv.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2hotftowi.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2wfjhpglq.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2knctapry.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2jepqzlhr.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2prhxppmm.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2htdktkna.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ltcraprq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2mvwpiyee.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2iwtybhoy.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2ampizqhp.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2ggqknpgm.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2iuwnyqcz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2xpwfmmzx.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2nufanwbs.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2wccmqrfr.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2siyueaxs.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2tlsymovd.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2bhyupatc.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2nqxvaodq.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2aqldjysu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2khehslow.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2uuvaylfi.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2fqudiphg.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2loctlcxr.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2csuazkpt.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2btaktfpr.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2tvvsqohe.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2bururujx.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2rvvykqeu.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2ihvzqiio.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2aaisnbou.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2jajckfxo.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2cojgrulu.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2gamvwbyk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2lltopbcg.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2vcvumxil.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2zjgdsylo.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2wwocjria.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2qnpjlbec.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2stkrgros.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2wmfdzfba.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2qraklmlu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ufszfwnd.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2gspfpxkd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jimzdqmd.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2mwrtagxo.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2iuyaimlg.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2jtqohkor.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ncrllqex.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2dtrazuxw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2xeexuhgr.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2bqcmsige.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2yobqaayo.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2nrjnqdlc.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2vwhlehme.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2attcijzc.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2wreurtyq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2ramnnarz.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2yvzcpvtc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2vfsqkvdj.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2pyayyzdb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2vnwltnco.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2frabcbik.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2whedqgyb.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2dwgezyhz.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2ddldvtid.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2oozotnxp.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2qvcrauzd.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2rbtagyan.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2jwygealt.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ankoxrzi.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2vbvrhjkb.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2hrsvzdqs.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2bbxsytej.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2gccxcyhy.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2wzdsyomx.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2qlcaqsyr.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2aiakxwya.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2kkurpluu.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2twgwdoun.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2vddcswej.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2wzbkudfd.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2gmvhezlt.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2bgshcyvz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2crmaonzh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2zscwnybo.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2zboygoxm.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xjhiaqrj.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2ollgprcz.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2twwgnnyn.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2fepjdqhv.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2enyrzvcc.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2vtgzzago.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2yaozkvdy.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2tnfukdrn.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2bwtuusiv.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2mzljjaji.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2fravnfau.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2lzfgodfa.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2aydrkxsu.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2bmvyxdsr.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2lkoejynh.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2avjjkkuy.html


<!-- 参考信息 -->