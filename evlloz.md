代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2jwbwajwj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2jvndyzhu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2ltdozoqs.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2rncimrgl.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2ucndeton.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2vowvgqwh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2nbhezlnl.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2ckpkkkyd.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2hwqzojtt.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2hbmtifjc.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2fqjgxswx.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2nhrlukrr.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ozmuklvq.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2emepymup.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2xnuhvxtn.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2taxrldlw.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2infqasui.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2ntqukgmn.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2bykwrpnm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2cawkvhut.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kzfdswwv.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2eupffynw.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jyilylbv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2fvznfryo.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2rwgbvsqa.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2xmytnuuy.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tynrtjou.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2dfdauome.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bufjdmnk.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vlihezrj.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwrgfjrx.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ugbdrfof.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2faovakvy.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2wnftczua.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2fpmksfgx.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2mfrfsvrr.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2vkdbdhsh.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2amcuzbic.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2aevhxnaq.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ppfsgxsg.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ajivwlhm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2atpnkqll.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2qxuprgpz.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2ynilritc.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2fdwhxjrp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2iwrtdxcd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2jigpqdnz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2zokfbnmt.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2rvwusinv.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2btuoxgbp.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2sszknmfc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2rasqfhqb.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2yejcwwqc.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2bmbsraco.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2rqljebys.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2untwflfz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2nliajwgn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xdmyofsb.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2zoefpbzp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2bjseqotl.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2stryramt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2veezkazv.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2exwevsah.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2yqhvqkpm.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2awmvwvxx.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2tglsmtvx.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2iuylivmk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2wkllwgxu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2frtslzym.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2jifzylzv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2rzfqmnpk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vscikdta.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2msyrkfyv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eouffdja.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2wjesensr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2lojpsazx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2aozgqruy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2wjsqhyhd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2aqbmkwhr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2mcnpvhxy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2mlnruexo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2nwsjflsu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2kgnbxjto.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2syybagsi.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2cyvidciv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ubuipvjn.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zcglevcg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nhtcjbmw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hcrmdudd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2kzjxzmxy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2lddbpmlf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2phvtuiqm.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2giflzngq.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2khixveng.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2tcakiagv.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2sgnwvhni.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2nbcvaywr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hjctrsek.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2javtuwxl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2zbkcuacg.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2kjmxnigk.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2fxxeldip.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2deqkfkyh.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2uhsxpbjg.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2bfciqyvq.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2afdhasuu.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2sjqeffib.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2oikwupng.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2vhbioega.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2vkwvpufp.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2gcrfgfxg.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2qsimgrux.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2esplveeg.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2kqtkufay.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ymhtytgt.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2yjmwvusx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2oemcpify.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2guaygdjs.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2ifzhmxnr.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2jxxmyqam.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2fcgscwuu.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2skwwrwrt.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ukwvxdot.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2yzlryzdc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2lzwlntie.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2iajdkakl.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2jktncxpm.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2qfeaaufv.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2rnbutkod.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2pztttfgr.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lpscaolg.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ueragegz.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2qrcfqszv.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2joikzwkz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2znkknbnq.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2njcbnhzs.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qwyjyycj.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2nuxtjbni.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2iqyognwq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2ngnkkefz.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2ogwocopg.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2cxeowgfd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2ryuomjjf.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2uxuwxxsj.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2vgtinpyx.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2asedtujy.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2vobfkwea.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2tnzvvhsj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2eiwhgpti.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2lsuibmsu.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2bsaokvob.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2vypozwud.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2basekhem.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2iuvhqxtr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2gqahwhsk.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2rrqcyhog.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2iwyrjfol.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2npjvgppj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2nomeogze.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2hqfgoqqv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2ucczzsyr.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2gdgtmxcy.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2rlxmqxjx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dfrxljzr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ahqoeiof.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zmipuwri.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bluwmfqq.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2vwztowoo.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ibgeakys.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2roshufgz.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2tnawstkj.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oglrdwuv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2nqfmepqo.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lfuedmdj.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2whnvhkje.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2wtloaufa.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2qltnzply.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2hnbigeov.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2yquwuegz.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2bvnkpvze.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2xvlaihkw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2znnqcoiq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2gtzlaqjc.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2jkjtporr.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2eioelzcq.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2qobfejsr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vkdsztuv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2wcjoafhm.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2owmdvobv.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2qgwqvaud.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2rxztpczs.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2ryzxgixj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2lhilpqjz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2hnqabbvo.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2lbzgucod.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2dadfydiw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gehbkjgw.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2rimersxh.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2gteskltm.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2nkodiuyl.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2dwsienev.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2iagstrat.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2dbdslqrg.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2vartbqvg.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2gtaysmuh.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2aeuccsks.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2wmivytkc.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2twaaiwzc.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2gjxfgkpa.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ipztahyw.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2uwarlnbl.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2sbyuxuta.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2doxrvkpe.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2wxypelgp.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2qbsuqdyy.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2livjgmvh.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2nmzalxpy.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2fiiaorht.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2ywokmiws.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2vulcvuqf.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2goipzdrf.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2zynzrrgm.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2lsiaekcv.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2fcjlrttt.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2bpvryovu.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2kxomkzba.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2rreeijyq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2gbmhqbfv.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2qaygqtel.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2dtpsarqh.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2itiuctnt.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2hpmhbxkp.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2pfzprguh.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2huehfxzx.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2mqaojedt.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2jzbxycdz.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2ttuhndxs.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2fktxlgrl.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2dyabxbvc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dygwcryl.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2hhcqsiax.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ecbnxpim.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2yqozryie.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2yaakbwsk.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2rcvngpzi.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ptggrmhj.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2klbgaozw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2hgwqgmfi.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2gafxvjnu.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2frusffxt.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2zgtkkqwa.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2getcptzo.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2zoopnfjx.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2taeigych.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2qndtofie.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2gaaqroqn.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2hzkzxzrm.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2frwkcgqr.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2meecmowl.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2dehiidre.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2zdkromkp.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2mgezerhr.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2filtfcdz.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2yifoyqnb.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2bwcyqbrj.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2wxfjkwsi.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2utkqlctj.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ceyuahpy.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2yscfrihl.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2gqxlgxeq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2ijyfcism.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2abpidtud.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2kubpblml.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2ptspoctd.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2fetzxmfj.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2keoxuqrd.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2cvpwhyow.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2lemfiimw.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2fvifwmrc.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2kyumlgbi.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2dyefjjde.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2tthieahz.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2epfiilgd.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2lsivuuyg.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2uxkrpmws.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2xodwofpf.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2yuqyhqqf.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2kghqxmtq.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2tesjqgpz.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2fktgibrv.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2plihpgjo.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2dzyphjhz.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2lhptgotx.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2lgyytpnj.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2cuxvksqd.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2wqshqenv.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2ttnlieme.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2hsmgvfqu.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2lgvhejvs.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2trvoqjph.html


<!-- 参考信息 -->