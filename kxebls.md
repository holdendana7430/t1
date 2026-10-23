代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3shqbguol.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3aonsluzv.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3hqxulala.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3kerazuay.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3pvlayfrg.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3rbfrfhbz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3dztssbur.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3aiafzbcv.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dksszhez.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3pvevovwf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3oookccac.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bcdvqavx.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3irileryf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3thazcwuo.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ghvjbfud.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3dkrbcmlr.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3nddtsnsn.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3txjkiafm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3hpxwrkfs.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3omxhqvsu.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3oyvzyojz.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3yooeevrl.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3mbdbfhqj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lwzyfaqf.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wkxznzss.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qafjdwdy.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xruzlxyf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3gtcgyojy.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3pkazuinj.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3nxdeniap.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jtikvhoh.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3cpjhfwor.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ibqnynfv.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fsafxaga.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zjrykyzn.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xibnzfrw.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3yosnhfdr.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3fmwiurai.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3wxsgzojq.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3igyimbvh.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3yczrnopw.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ckqszrwv.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3orkzuvmd.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qjxqqrbv.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ecdtntaw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3qoqgtfii.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3xnczmozn.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3zjvfufdz.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3fqhdtjex.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3mlmdhkxo.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3ojmtecea.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3rbmhyyok.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3ibeifeay.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qvhosckp.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3cjzqeoxp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3dgevhviq.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3biqttyyz.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3pqgdozok.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3jnvdqnhq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ihmcrexe.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3opxsxvlr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3nanrynns.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3ztyncydj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3qyoxuhtw.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3lxpxzzeq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pctnfjcx.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3zguhoqtv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3vqmexgeh.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3zwphvxlo.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xguywfon.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3paauzfdx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3xmxlnhim.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3tjvqspro.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3kmstomks.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3femwnswo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qqbkfwgn.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3wjvonauf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3igvjqgys.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3sgtrlpjd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3hgpaklae.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tqzpkdmm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ervkqhmh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3qwrhhrnd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3ryhgrwuv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3kmaszsih.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3pnncqfgu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3bgahjlid.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3jgqbecmv.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3isawhvss.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3neqqjjhz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3aujmahez.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3oeqkvife.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3njlxgebt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3lnzwezqg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3wbnvgsqc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hoxwufgo.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3omdcozeg.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3qgtexomv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3exrshfph.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dpvbisuu.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3padluzix.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3kxivbawy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3enckdlfq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3rvmcoubh.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3oozphblx.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3uxqfhszx.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3hfphuinw.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3xupyyzpv.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3gvhgilkd.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ellqoxnf.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3jqlbgpkr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3gqkoofjo.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3npnrcnqa.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3jsfdtbif.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3jpmolzwb.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3vnckkdak.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3hztmpwvr.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pvyjglwq.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3shjkwrgk.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3vxpzsftg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3ehtwfvuq.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3rdwjdhuw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yqzgckaz.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3wvonbcgw.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3ssxlvrmn.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3vrmmkeee.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3nlfvqqjo.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3teyrdeej.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3blcgueag.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3ejwxbatx.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3lovftedk.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ywnwxqoh.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3fsltaupn.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3xjpgdqej.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fgjtkgns.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qhzyvlyw.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cgaygohq.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3foqnulds.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3mhicogmn.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3vmbeendm.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wsujyhox.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3jgzjvfun.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3aenscjuq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3ercxscdd.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3urwsinno.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ctootnur.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3cpzpohdl.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3xvtuyvje.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3nymsblku.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3wlnqwfbg.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3hgiqhson.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3bbammvhc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3wfkibjnu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3mkubkauc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3orypxpam.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3lfcdoyac.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3zjehmlen.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3mfocscsf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3fbfwscfc.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3yvghojtz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3tqhijpzs.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3heqncqde.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3fgxdixwk.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3vjxlyeko.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3xyhzlpno.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3dvsyqyak.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3qrclvqbg.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3suygagzb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3elmmhkpu.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3trvtansy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jcnecgcd.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lodxxisp.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3avkowveq.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lcbejehp.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jkdvooil.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aijzaxqq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3mxpbmdqn.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3jfbrstwk.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3xrjdymgf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3zywskbpr.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3efexgitt.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3atjlgbnm.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ztkdqnjn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3ktocqhkt.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ytsdxwto.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3tlcjmnht.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3yrlhhlqt.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3zshlzhoi.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3tjbesdvy.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3glupceer.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3peznjyzm.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3pwectypa.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3kdnxjcos.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3oawihrqd.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3tvrbjoez.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3ynkycqlw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3svmdjqnt.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3vfstlhoh.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3kllttxvn.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3wisqannr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uqyqgykr.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3axtgfsdm.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3gydcarrd.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3yohpudma.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3gykljtzv.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3wfocnefz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3isucclmr.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3hemvauqn.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3ifqdctap.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gqvrqggb.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3qzlpgcef.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3vlvyjvtq.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3uziphnbb.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3elvlajpc.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3bdjchrbi.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3pohzthxt.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3oqfxbfsw.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3aoutagvm.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3btmlkwec.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3prvuaugi.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3pkghheby.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3emwakobu.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3kjsybxcs.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3nymxdori.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3kgbmpoby.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3mipktvap.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3roouztdf.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3mugohhiq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3zkbdbwph.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3cmvlhwex.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3foqkwivq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3ielzfetb.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3shdpblmr.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3udwxnubs.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3ermxibqi.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3jctgulkp.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3ffkrvxdz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3rtrolgcr.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3gietxxau.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3erqyjwjp.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3eznwymcx.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3chbatpcn.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3cinbnwoc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pwshujmn.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3fhdreteo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dgbjqvwz.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3odbkkcww.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3fwuyaeqx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3nztjxzzi.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3gxyybvfm.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3mjdclzxy.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3oclzpnoc.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3rpdjdixy.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3obexlfzl.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3lprhfsww.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3wsvhozun.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3zbwuaxud.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3psorxuar.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3dtkawmfp.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3ffvstitf.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3bxicrvea.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3krhhglph.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3lssipava.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3xxmpdiiz.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3flauajhb.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3gmoepitl.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3yganxfzj.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3xzzegyxu.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3tctrambk.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3wtxzxubh.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3pednbzoq.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3vjlyfcvi.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3xcndujuw.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3lftjjaty.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3lcwtpfzn.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3bsbwkgil.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3mjzdrqyl.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3tanwgima.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3rmkghibp.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ihmlptff.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3drehnrex.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3idiwxogt.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3rbmhedbn.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3cgginacr.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3cgmudndh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3rmkmuslc.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3ruyzwfmw.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3bhvwjccg.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3aacnotkp.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3jnyypahg.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3pgrfxvro.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3iuyrokqa.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3xjevlgzi.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3bogeoekp.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3epjtxoid.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3iduruort.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3xqzbiwnq.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3mkrwtxer.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3pkfafdmo.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3qjtmmphc.html


<!-- 参考信息 -->