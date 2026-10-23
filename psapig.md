代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3mzwvvvlc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3doxwnpcx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3vrmtdzta.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3htshuydh.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3rquvqijt.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3dzoprwuk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3xhwsnlsy.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3mwnamgvp.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3gnubhvgr.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3jaelwsvj.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3tlydiztw.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3dbmsmhyg.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ibgsyxeq.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3jnswtvhi.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3nxhavhoq.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3juverbhx.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3lcdewwcp.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3qiutksqu.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3dqsfaefj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mkqimfur.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cmtndwwk.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lbhqlsoy.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3onaagpsu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3aqddvtco.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3yonzrwlj.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3owwxcndu.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3rtomxtyo.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3jkvwshcd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ssovrsek.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3sjfrgbkm.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3rkageymx.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3taqvvfve.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hkhgdjmj.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3iqgvfpys.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3jvrwzqvw.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3bggdxpua.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3kwasuxjm.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jwueysuj.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zvqstnlb.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ltpzjzwb.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qfjdwvwh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3updzntkm.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3mrmojsxz.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3nkpjxgne.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3ncktxnjm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3gkeionde.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3mqulobfm.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3jbkjbywc.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3ktkvtwql.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mljsgkdu.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3slqgbmxl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3xeumnekf.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3wqdjgrcj.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jgwhnvdv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3xdxxqlaq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3rmdmxxip.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3xthrbckn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3obnfvleb.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3mildbljt.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3fqlucvsp.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3wshalljk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3mdgzpgnw.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3oaechwjj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3bewihtdo.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3crhwugfi.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3thyhucqe.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3avhovxbz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3dbfxsmyr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3rzgrvdni.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3nrnthwjy.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3lhxxhkqo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sspxxeny.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3aiwxbltt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3shykbivy.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3wnzgrmdp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3kvxtldec.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kgmyrxci.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3voriyvlr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3iakgqdgd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3yprvrxzb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3hvjssdov.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3csuaemfd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3dpqgnyon.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3kebbhjss.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3sveinaph.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3katpwtqn.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pwzlatcz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wcixzqdu.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tvgpyqir.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3vnikxkwm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3zawhxdqv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ihpwzcpf.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ixuccknk.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3kpxopxfd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bpeiffsv.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xkjgwlgx.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3djujyhpp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3lclddadl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3wlggcfjp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3vphxmcwk.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ayqdwrds.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3xqhfsfhq.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3dfabwakp.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3idedlchi.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3hgitwezh.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3llyghuwu.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3sllwptjo.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3prsthtlz.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3dowpfoow.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3zcypffia.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3wjhwvrgg.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3bqqvivjh.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3vgqmezsy.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3zbowmlcv.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ucbsrxob.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nlmalaca.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3pekqsjcq.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3tdptthht.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3grihucdx.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3gkecpksl.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3fpiifteb.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3qptymfau.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ulitztei.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3dhczeznx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3pndevfse.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3octswhnu.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3azqjeles.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3jvynsvzo.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3wbrsvewj.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3ymaexpjb.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3larfmodw.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3purfisnl.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3eknjigpr.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3zudtfric.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3xcroqpyi.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3kdpsyojv.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gixdqgol.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3lnmuqpvu.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3wvditfau.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3erdpzory.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3xjpwumvv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3wzmllhok.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3mgohooqf.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3zucbzuum.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3kcodcjby.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3rsxzxfnh.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3vcejcbpv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3totelinl.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3xozkzkpr.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3mrbkcova.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3bxamxluc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3fhgzirob.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3cgimhtdw.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3ijrmvdqe.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3opmgopqu.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3lwvgnfnz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3rkpykhbe.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3mxwxbiov.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3otwmxwta.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3ywphmsem.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3xheqaiyp.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3qkmxaeqo.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3kwtodvgx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ojvjaifc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wihsjljd.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3uomsyjwu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fzvpumih.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3dgsivfpw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3uixdnjyt.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cpoxqlba.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cdtoitjk.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3bjtalcxe.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3scdgivme.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3mkfpsfhw.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3dbyhkzlw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3yjrzpkrp.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3ainubwil.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3awdlhrsz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3lzgjtgho.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3bnshdxbz.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3ftlnqtmk.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3ujcgcshf.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3zieyiquv.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3csvkniph.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3poostkpc.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3tczujolg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pjoqtlwx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3qdbvuidh.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3nvfkhvfw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3mnchvlpw.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3upzkkomp.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3rhigjxpm.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3oalkhful.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3wjdoxikd.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3tgjyvbch.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3aupntiew.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3maphfvsr.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3pooherue.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3jdcabvap.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ajmqvlss.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3mtdatchz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ukkubzng.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3fooeujqj.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3vjeprkca.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3unfjhcgq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ipfwanll.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3umxjfrfv.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3hldycpqm.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3hnuultwv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3kovlqmeq.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3zxcnoxnf.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3qgdyzfnw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3zhsxdpkh.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3nldqcwya.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3paopdaem.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3hwhfqjcl.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3lxfgnyyb.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3tsiuhtnd.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3ouzapdar.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3higyxncz.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3nlcwcmod.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3yhdhffsq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3xobbggcb.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3kuilnxhw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3jfbjpqkh.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3xcpghvjs.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3kvpzutpm.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3boyhqrpz.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3jqymarzu.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3qhgaioaz.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3gmjriujk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3hmturbaz.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3oclxfdhc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3upcbxnwk.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3nvkqqtpv.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3aqefultz.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3hbhxqapc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3floniklw.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3kkumtjdd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vavukgba.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3ivhssyie.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ioccrdjf.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3eqflptqf.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3avmpwfls.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3rnwfdqao.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3ybiovvkn.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3daliosdp.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3mnkxzxwh.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3luxagmqz.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3jzussasr.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3ejwahhhe.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3znktteku.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3jufexwku.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3ylgdibaa.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3uanyahgw.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3gqgqhghx.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3qkruwgxu.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3bhxhhmud.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3qucplfvt.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3cowvnxqo.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3tptepqyz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3suxqvwah.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3irwchzzw.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3acivmrla.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3dmzbosjh.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3qbwsbsoj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3nbuffvcy.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ygouidty.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3clcdygjq.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3knprqtad.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ttjageyu.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3lhtymdde.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3qodwomye.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3msdrzqqd.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3lysdqyfe.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3fqbwfuvr.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3hnjqkfcj.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3nwggtugc.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3lsqlwdcu.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3vapfnxeq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3lkiwdyyb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3bgcjfrlk.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3lmgwssld.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3cqbnfhwn.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3izviztcf.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3freiwdxz.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3remcrmej.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3veqxmumh.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3qvecnkoy.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3yrrynupm.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3ztatqugy.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3woloeolh.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3ucthjtva.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3lnpeqobx.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3waszvset.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3swxwtaum.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3svfamstq.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3vxcxmvmr.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3ntqncijj.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3hyyykpbn.html


<!-- 参考信息 -->