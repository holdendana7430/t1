代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2siotuqtw.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2zhhfjrrt.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2fhxqgfcu.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2dkxcaklf.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2ezjrmlmb.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2idnjgjfv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2wrotcjzp.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2zqmfwpzo.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2phenvgjw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2bjvgtbxr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2bcukywry.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2mdulmnqk.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2vzvvavwc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2zlfauaqb.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2nitwckfo.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2zgprbekx.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2qhcwaqtn.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2mebtwbki.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2ftascxln.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2kqkanzwi.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2gpjmniaq.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2brqvctim.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2hmwdnrnu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lzuhkzei.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cfrruypn.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2jvjhidgx.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ymajdjey.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2bzpxgqoy.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2mpxxwgae.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2qyvdunmg.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2yecglsmj.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2jonmhrlm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eacpxpdl.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qqfdrmvb.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2zqzlupdq.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vzfaiaed.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2zcrrznux.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2vudsbhps.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2axpglykb.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2ntvuasiy.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2garjwkvv.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mrinkoss.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2trrqwrlw.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2facohwbd.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2thmofxdo.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2cydcqacg.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2gdusjsvw.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2lruxagps.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2hlittiif.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2dknwdpvu.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2ziwqgjvu.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2hyddqyuw.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2wuvjrwip.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bmejmecy.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2nstetvzt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2hicxjvnl.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2veeelbua.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2oxytjimr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2nufsdvva.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2dmlnekrr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2hgtdpenz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ryojokno.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2elhcarcx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2qbucnrlf.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2gaboxrff.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2vfscpiqy.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2aapqvctg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2hcpbjkxl.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2kxtgirzd.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2syybzgsr.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2xentddla.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2mgygjssl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2elfgvkmc.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2tarnlngl.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2sdfxuvtq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2owakciaj.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2pmrbixnn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gjryubzz.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2nswmndui.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2hooxondu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tmeddvob.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2yfccykgi.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2igilklrs.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2szoygilb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2cosuofse.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2envvbzks.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2ydjisvul.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2gavuxihw.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2ymzvwdme.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qzslglvh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xxuqqehz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hmsjopkh.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xrzczgid.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2yturkaef.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2tnuxsvub.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ibhozxvw.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2swxvyhya.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2bhnwhiuh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2juhxnnvc.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2irhnyzmz.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xezzramv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hcugoxke.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2ewklvifo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2efsstapl.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ebskbycm.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2cbltpaiz.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2lvsrfrnz.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2rxrzzxhp.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2rtghhdlp.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2iiehtbno.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ndohtwwk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2oktcwyjp.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2mehaopmh.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2ivklpxmm.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2bedfcvfj.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2bnzcmxba.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2gzfurkos.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vtpboyft.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2hwxrhsyp.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2uqjqnora.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2bzdpditn.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2slpnieyw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2semwrlsb.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2vvphpxqn.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2qwwevild.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2cbyyeoey.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2gjkpnipj.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2kkfnyqsz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2bjykzqzp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2soqwqmdz.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2qjyeswuk.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2juxpcqpu.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2mpeumfxc.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2nwhsczfc.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gwpjoztf.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2zlrpkjne.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zhdxkykx.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2chadfnvu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2udyahexe.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2sgnhpxgr.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2rtivltil.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2zawkxqbt.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2oojitena.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2jkuwassj.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2gzdxliec.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2eaghaivq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2tnrbleyb.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2cztykgwq.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2wbekrtvk.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2ztlrgpbx.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2znkkhuzy.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2hoiuoczj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2rwpgweqm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2bfcrfyjr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2gzoqurpt.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2pmbsvjwx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ymyddrxt.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2oltkwtbg.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2mnnxddpe.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2aodshbjo.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2rioodvut.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2luzknnyt.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2uwchznou.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2qhmccxoa.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2kyqjgbnf.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2lcjywalh.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2yjflsadp.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mbbgczvb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lkfdgdov.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2afktkbru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2llknsjsz.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ykdprkey.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2zubewydq.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ocnezypc.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2pwgflkuv.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2gmvpzuro.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2bjtlqbne.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aitrfwdk.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2cvcynicf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2awzrxizc.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2pnhtnfxo.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2uongbfiz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2lygrnore.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2bsrqazbc.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2ujvqikjd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2conopzfe.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2olwnmxif.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2hggtxqbw.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wizcuxrc.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2ncnrnctp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jgnjjvmo.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2pslmkauf.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2mjiliizi.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2plzwbein.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2olekrcsx.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2lrajcvjq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2gahuwady.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2aqspkbbb.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2fltkocia.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2uosbnxxe.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2wribqdgv.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2majrfdkr.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2akrsqjpz.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2gptzmhvu.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2lutfijsa.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2ltjhrnrt.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2npuafcfi.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2llyyirhx.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2xlgsibqb.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2traekzlx.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2itukupmz.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2lkifcsds.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2gzfzgqqc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2otpvlblj.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2fpvkgftx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2wmahympq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2zeyaonxk.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2mjzdyzud.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2wwocmqay.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2fcyiviye.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2vbihzywf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2zemsybfj.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2veqwyaod.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2ihfmucyb.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2ycqmxqqb.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2poxeaajq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2mftiklrv.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2tezubkin.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2wqwlycmy.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2rdkhubxh.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2mrpfdboh.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2ojyashim.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2udzionzi.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2ibkdknon.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2vljnoyrg.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2wkurqqoh.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2syzeuhvd.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2azmemiep.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2wkettivp.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2sgbgvxiu.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2zibukglf.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2bdqegybb.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2yynnlxzo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gvbzgwbl.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2mzdetyvm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wojfgkpk.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2fhwhawza.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2borcdlkp.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2gzolvcyv.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2hjkbkbpc.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2dholhfae.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2tmxdgsnp.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2hdcixmai.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2utowclrr.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2wpscfqlb.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2kenlpqzv.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2gxxlyzaq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2chfuptow.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2aglulwri.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2nlduroqc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2ampmgoxy.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2tjgbxgxz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2lidrouyn.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2ztxwfclk.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2tyzjnhog.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2lartcipg.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2ctatpieu.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2exvnbomb.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ocibuytu.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2myrjgyco.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2obugikdc.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2rpyzkxcc.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2zwqoykbp.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2dktozokq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2rzmuavez.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2oeizfhsa.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2zvdmwrig.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2lfhhqskb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2rsfqlytb.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2gmocikmg.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2awkbubft.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2zxtukxeo.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2vbsfomrr.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2bbuctuvt.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2oguwylof.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2xwtsgbyx.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2lbdmpouh.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2kirjxvvv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2exkxhphr.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2qadqxepk.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2ggspqgsz.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2plolcrkq.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2ewzgneub.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2xyognotl.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2htvxkaqt.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2yuimmpcn.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2ixnpwilw.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2kacaonvf.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2xffxvnmh.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2eesqmenq.html


<!-- 参考信息 -->