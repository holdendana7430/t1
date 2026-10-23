代发 wailian999

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ulnyznox.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3oqavygvj.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3dwhoixgd.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3wnrndyum.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3okywdpdz.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3yqsntmte.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3nlihggyf.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3xquyahad.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3wuisvgry.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3vbolwgeh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3lemqvnuc.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3czhnrvgs.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qxhntjbz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3dpnegxpr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3fbpcdyyk.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3beqaukfh.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3dywmloik.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3icrwdcls.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3nfuheoyd.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3kaksvqeu.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3akfxkpyb.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3imurczmv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3rsnxmuki.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3uuhhmnqg.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3tfdvstce.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3prdcoomw.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3aqixedxr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3uybrfijj.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3opweuwvs.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3namzomxc.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zpnbtojy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3fxykjhud.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3iszdmrqw.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3pvkvllar.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3ofaymlnr.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3mdvuczuw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3taovxwyi.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjydpisl.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tlmupetw.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nfqhumem.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3fpctsslf.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3dqoldjkf.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ceczvhfj.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3ykbgwdxa.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3yvzygfkl.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jssxufiv.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3myuzryum.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3eeyhrwou.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3fnlfyplb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3nomjsikl.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3txiwgjlf.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3qdbqufjd.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3daixnykx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3kivmwbqa.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3kntnmlup.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3olpvexrd.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3xmoehctt.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3npjmjmzb.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3krxunlfr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3cwlsjldr.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3aqoygtot.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3pqmkfvjg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3fksesmax.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wkgwzfgs.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3niqtauwo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3mmcbqztq.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3zduqakgu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3nnpwdwzq.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3suqqoffp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dpyeeaas.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3gdwoofws.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3fnbrauvl.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3gmmuaqcd.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3msrytqhu.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3wsyolzki.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3dmbdfggz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3kswnxvsw.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3yvwnmezb.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3dacogkds.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wmqniunu.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3rdlvbqla.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eprkxvdl.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3dcuthlxf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3sbqqopnn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3ejkubxwj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ybcrujeo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3sclijycf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3zbgeprun.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3uqbqubsc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3dytrscoi.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3zvvtwefj.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3eczuopsn.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3wxnqrddy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3afecrhcq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kuvwsobb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3swnippkd.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3drmeeylm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3ufnohzec.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3wqemaauj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3euxdnlxr.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3rauwjwpw.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3xujzjxgg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3kmvczmoa.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3conbtrbv.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3nvtjilmf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3cscxzywk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3xjgwxipf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3zknlenhj.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3oiuwofxy.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3qeklbrxd.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3qdvelmey.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3yyvhzequ.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3llbpdvin.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3zwtoxlbj.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3rfauoccj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3bedvihcr.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3rnykdsax.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3bdopekwu.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3tmljphri.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3pkxtqria.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3ioslmnnn.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3smgnzraj.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3hwcjqtng.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3cgfjbyns.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3akyfcnne.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3agzdlufn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3khxatyuf.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3xzcximdh.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3sxnnsscb.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3eqfgclds.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3cabfxmvz.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3hhstrvjy.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3agfubitt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3cipufrch.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3mruvslsi.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3okfvdctv.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3vvjpjpyp.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3zltqbfko.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3oaedxxix.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3zvsvofkp.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3lmeessmq.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3blnkkmgv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3phzckqoh.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3rjnvxrfu.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wpwsrykb.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3eyzztado.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3pgelxwtb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3dlrczltr.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3qmwgwoys.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3tqacmgwu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3ozdmwrao.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3okmbrvks.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3dotedbvh.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3cmhhwdhn.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3wcahssid.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3udajphwh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3fftvbyvd.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3vppbhmxv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3sfcxgyvp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3nsvabdjq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3xlvwfzum.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3ayuhjcou.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3tkfmntlq.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3ubfgfyie.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3qyasdcsj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3vxbhqfgb.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3xyqtsabh.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3dtciifsa.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3xuhuvtmx.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3buvotkze.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3etgvkaxx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rjzsttva.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3khdwkxjq.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3ltcegrzt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ofprrxpg.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3blvpzqbi.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3wkcrfelg.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3plwwpcyg.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ojoraica.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qdjwbbdv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3mqkjreid.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3luusedgn.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3eeyatwnd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3iixhynuy.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3mrbuufcx.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3dxpmkznc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3epbazaqj.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3enngwero.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3gsaxqzqd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bpohxlvt.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ankhexkq.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3bimxapyf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vhcjcdvw.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3mimvbozn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kvpmvaqb.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3zxjensdh.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3cvbehwja.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3npjnabia.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3fprynyfl.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3fmumrwvv.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3hlwtybqs.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3mcezaxvf.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3aipqjbhl.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3wjlzaxbd.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nitzoydf.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3brgzhgnz.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3xhdpubjc.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3ocrzcxpz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3axvbwhuw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3ztpqcrqa.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3jmyjdmji.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3opikieex.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3spnpaofz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bujlksmu.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3ixpghdxd.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3dwsulcmm.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3wkqvvfrv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3obinhafv.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3kfwyybhx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3ggsuammz.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3atqqgdit.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3ucjhjvsi.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3vysqsjsg.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3umtfdjpe.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3kezlxalk.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3srepcgmx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3lrdrbppu.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3eouazygt.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3jylgvhft.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3azhiaeir.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3uwymlqzu.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3spbsdzho.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3ntistyjo.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3rysevtkl.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3qmgknwxh.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3viuxsntm.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3pmnbuvvt.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3kwytqefg.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3knaepayw.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3hdhbguxb.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3nfasinmc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3wjbolbbb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3opcdgtfg.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3mfwwsuyq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3kjbhyxqm.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3ngmnnbus.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3rmpngsri.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3atyxyudp.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3bzjhvqfs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dczaazyy.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3zphqbstx.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3jdpqwluq.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3zamuotdg.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3zlerrfjv.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3ocwrcezj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3bynyssyn.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3lucclcaf.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3piaggipw.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3mlcwwxoq.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3lbpwasjj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3hayciqto.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3rgohbbgl.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3ticrscup.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3dlxijvtb.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3ryhslnkh.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3sdgytvnq.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3zfobkuqo.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3tgtnfqih.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3lkdnhgom.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3luohkera.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3ehhuptyq.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3uhbjamux.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3wijypojn.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ixgatoez.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3nuzflqud.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3xmgnxzox.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3ppxbxfux.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3gaotfljj.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3tbzqumrg.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3jchnfhkc.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3rbrevjmt.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3ohfeikxt.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3qgfvafgy.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3wzvlnjia.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3itwrqkaj.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3uvwouvks.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3hrlofvru.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3lgxegeop.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3dlzrwydf.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3igjynytd.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3umgvctbz.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3tbhgkvxl.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3kcjewpgz.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3hzmoaxth.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3fgqaaqjc.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3yybfxcup.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3hfgwmjtv.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3wgumsgck.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3uguezkap.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3suiutgis.html


<!-- 参考信息 -->