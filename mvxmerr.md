代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/gwzlzxplb.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/gwamairfh.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/gcjqibnny.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.hesvh.cn/Article/details/grcwktwmy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fehbvm.com/Article/details/gcqwxtmbv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/gktyokmov.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/grjbaqcvf.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.hesvh.cn/Article/details/gacmmytem.sHtML

Java: interface Shape { double area(); }
来源：http://wap.hesvh.cn/Article/details/gmkuxmllk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/gnrwejvgk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.hesvh.cn/Article/details/gwsfxilku.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.hesvh.cn/Article/details/gzzymwume.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/grmejfxli.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/gusnjwwyd.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/gngrsjlxj.sHtML

JS:   #private 字段；其余公开
来源：http://blog.hesvh.cn/Article/details/gnbmfsrdp.sHtML

TS:   public / protected / private
来源：http://mobile.hesvh.cn/Article/details/ghltethgc.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fehbvm.com/Article/details/gdygnxqxj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fehbvm.com/Article/details/gedjmkdpy.sHtML

Ruby: public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gsxuspmgl.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/goquvmpns.sHtML

[G11] getter / setter
来源：http://www.blog.zdbjq.cn/Article/details/ghsfmsjig.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.zdbjq.cn/Article/details/gafwnwdwr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gpmrvhxlg.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gottridzz.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/grqnhxvly.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghvcjvvcz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gdrexwlbi.sHtML

Ruby: attr_accessor :name
来源：http://read.share.zdbjq.cn/Article/details/gbqgwucoc.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fehbvm.com/Article/details/gbxfixadm.sHtML

[G12] 对象转字符串
来源：http://www.m.share.hesvh.cn/Article/details/ggbopeclj.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gnwymrvaf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gvymmlffa.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gonpzobyp.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gzeazssyk.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gyfjvxdti.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gujfzltau.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fehbvm.com/Article/details/gtatiskcm.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.hesvh.cn/Article/details/gemveykvf.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fehbvm.com/Article/details/glbqqvanu.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fehbvm.com/Article/details/gnwlzueno.sHtML

PHP:  $u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gzgupexkn.sHtML

JS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gvwjqamaw.sHtML

TS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gcgljvxrz.sHtML

Java: u instanceof User
来源：http://3g.hesvh.cn/Article/details/ghfhfrxfb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/guvoqggrs.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fehbvm.com/Article/details/gdilkrcuz.sHtML

C#:   u is User
来源：http://read.share.hesvh.cn/Article/details/gwitigiyg.sHtML

[G14] 数据类 / record
来源：http://mobile.fehbvm.com/Article/details/gyjqegztb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fehbvm.com/Article/details/ghotfkmpm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fehbvm.com/Article/details/gxotvxquo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.zdbjq.cn/Article/details/gdkimvlpf.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.zdbjq.cn/Article/details/glsxvlgih.sHtML

Java: record User(String name, int age) {}
来源：http://3g.zdbjq.cn/Article/details/gsfvhiqbw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.zdbjq.cn/Article/details/gdkvzeaal.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/gtmfbrvcq.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.fehbvm.com/Article/details/gmmlkfztv.sHtML

[G15] 枚举
来源：http://m.share.hesvh.cn/Article/details/gllglkdak.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.zdbjq.cn/Article/details/gpberxgtx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/gqozddmhf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.zdbjq.cn/Article/details/gbqwcslgb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gkwbvtsoz.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.zdbjq.cn/Article/details/gyollwdzq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.zdbjq.cn/Article/details/gfvuvujzs.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fehbvm.com/Article/details/gsxyjtvcn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gusnzpxwk.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fehbvm.com/Article/details/gziwarjde.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.hesvh.cn/Article/details/gddgyfifk.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.hesvh.cn/Article/details/gnpimojmm.sHtML

JS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gzrlzbjja.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gjbbmyeof.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.fehbvm.com/Article/details/gpvqbihdv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.hesvh.cn/Article/details/gqjksjccm.sHtML

Ruby: obj.instance_variables
来源：http://mobile.hesvh.cn/Article/details/grgacuqje.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/grrnyzgyq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqeowwkul.sHtML

H. 异常与错误处理
来源：http://read.share.zdbjq.cn/Article/details/ggcjldhhd.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqcqyilqj.sHtML

[H01] try / catch 基础
来源：http://3g.hesvh.cn/Article/details/ggaznxqqk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.fehbvm.com/Article/details/gnfzhwfzn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.zdbjq.cn/Article/details/guwfaihkh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gkefqkryu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gbbhfcteq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.zdbjq.cn/Article/details/gjbivybor.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.hesvh.cn/Article/details/gmylcsiwc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.hesvh.cn/Article/details/gpjayikbj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.zdbjq.cn/Article/details/gprydnkkj.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.hesvh.cn/Article/details/gvzdshcbv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.hesvh.cn/Article/details/ghmiljabz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gmesxempd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gqnrjflau.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gduzfgbms.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/glqvqhykt.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.hesvh.cn/Article/details/gztfqpnsy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.fehbvm.com/Article/details/gjakcoevm.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gvchundfw.sHtML

[H03] 主动抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gloacliuu.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.hesvh.cn/Article/details/gxatbbmxm.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gdmulrmez.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gmwarcwjx.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gonwqsatz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gccljymzf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.fehbvm.com/Article/details/gkxjdibot.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fehbvm.com/Article/details/gwgwotoge.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gibanjxtf.sHtML

[H04] 自定义异常类型
来源：http://www.blog.zdbjq.cn/Article/details/gdmnnrffm.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.hesvh.cn/Article/details/gbgbblsiw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gslzvwdnf.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/geynzbhuv.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/guanoyjhm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/gbtubmvhl.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.zdbjq.cn/Article/details/glodqdgzh.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.hesvh.cn/Article/details/gmyqpunij.sHtML

C#:   class MyException : Exception {}
来源：http://baike.fehbvm.com/Article/details/gguagaeyn.sHtML

[H05] 捕获特定类型
来源：http://baike.zdbjq.cn/Article/details/ghttucgcl.sHtML

Py:   except ValueError as e:
来源：http://read.share.hesvh.cn/Article/details/gbmfahnmw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fehbvm.com/Article/details/gyhpevagp.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gudfdsvbx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/gvnqianjt.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.hesvh.cn/Article/details/gzvhdcdmw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.zdbjq.cn/Article/details/gumwdhnbv.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.zdbjq.cn/Article/details/gtyqhkemz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fehbvm.com/Article/details/gaiwifuhr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.zdbjq.cn/Article/details/gvovgpzzh.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fehbvm.com/Article/details/gofxnbtxq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gckphjatp.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/gtdznherj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/gnejswnzq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.fehbvm.com/Article/details/gmexdliim.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.fehbvm.com/Article/details/guelolkqv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.zdbjq.cn/Article/details/gdsvfrxvf.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.hesvh.cn/Article/details/gsljajwmc.sHtML

[H07] 断言
来源：http://read.share.fehbvm.com/Article/details/gksfqajyr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.hesvh.cn/Article/details/getgdwmig.sHtML

PHP:  assert($x > 0);
来源：http://m.share.hesvh.cn/Article/details/gjlycyoqo.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gdzbxvivx.sHtML

TS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gazzmggsj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.hesvh.cn/Article/details/gqkilgjgs.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.fehbvm.com/Article/details/gffuyskpr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.fehbvm.com/Article/details/gkqbhybom.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gdjijxyuc.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fehbvm.com/Article/details/glvgltciy.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fehbvm.com/Article/details/gshfinquv.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.zdbjq.cn/Article/details/gxrrtldjr.sHtML

JS:   e.message;  e.stack
来源：http://m.share.hesvh.cn/Article/details/gtjpjwukk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.zdbjq.cn/Article/details/gofqhzbra.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.fehbvm.com/Article/details/goriqrppu.sHtML

Go:   err.Error()
来源：http://mobile.hesvh.cn/Article/details/gwhdegjhh.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.hesvh.cn/Article/details/gkbfilomd.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.zdbjq.cn/Article/details/gbyojtcvw.sHtML

[H09] 带错误码的异常
来源：http://blog.fehbvm.com/Article/details/govsfmpfm.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.fehbvm.com/Article/details/gnuzjxlsu.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.zdbjq.cn/Article/details/gajooulzj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.fehbvm.com/Article/details/gjpkjfryh.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.fehbvm.com/Article/details/gzblkyiko.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.fehbvm.com/Article/details/guaxqikqo.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.zdbjq.cn/Article/details/ghsptbnyb.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.zdbjq.cn/Article/details/gwlsdsffo.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.zdbjq.cn/Article/details/gbwjfookd.sHtML

[H10] 资源自动释放
来源：http://wap.zdbjq.cn/Article/details/gfwaonzjp.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.zdbjq.cn/Article/details/giyksqrec.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.hesvh.cn/Article/details/gvuhcxhin.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/grolmzahy.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/ghpmoslcj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.hesvh.cn/Article/details/ggdjcinqd.sHtML

Go:   defer f.Close()
来源：http://m.share.fehbvm.com/Article/details/gmxozpfyy.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.hesvh.cn/Article/details/gwuwkbvhy.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gxocuthfm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gfmuzinwu.sHtML

I. 正则表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gieoibrau.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqprzieik.sHtML

[I01] 判断是否匹配
来源：http://wap.zdbjq.cn/Article/details/gktuwmdqn.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/guntheflw.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/glgvxmxow.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/gsreziwcz.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/ghabmvgnp.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.hesvh.cn/Article/details/gaxcrdppi.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.hesvh.cn/Article/details/gedxcagxv.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.fehbvm.com/Article/details/gayqeyevp.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.fehbvm.com/Article/details/grpvkoyok.sHtML

[I02] 提取所有匹配
来源：http://www.blog.fehbvm.com/Article/details/gznfzzxkd.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/gbptqqpca.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.hesvh.cn/Article/details/gcrxndzjd.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.fehbvm.com/Article/details/grkgtzyid.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.hesvh.cn/Article/details/gtljprfbm.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.fehbvm.com/Article/details/gghbikvfx.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.fehbvm.com/Article/details/gxtkzbxhx.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.fehbvm.com/Article/details/guqshewer.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.zdbjq.cn/Article/details/gcmvkxszh.sHtML

[I03] 提取捕获分组
来源：http://read.share.fehbvm.com/Article/details/gxlarmqkb.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.hesvh.cn/Article/details/gralkawgf.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.fehbvm.com/Article/details/gchihmkys.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.hesvh.cn/Article/details/gazflnncc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.zdbjq.cn/Article/details/grcibeqmj.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.zdbjq.cn/Article/details/gavnwpmur.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.hesvh.cn/Article/details/gdoyifwia.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.fehbvm.com/Article/details/gctvmdpqr.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.fehbvm.com/Article/details/glnsunrkf.sHtML

[I04] 正则替换
来源：http://read.share.zdbjq.cn/Article/details/gjgtngccz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.fehbvm.com/Article/details/gekyebevf.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/gdfnonkhn.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.hesvh.cn/Article/details/gcvpywmqb.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.zdbjq.cn/Article/details/gwyjokzkd.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.hesvh.cn/Article/details/gvwltdlml.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.fehbvm.com/Article/details/gpuhohsse.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.fehbvm.com/Article/details/gzcrlqwpw.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.zdbjq.cn/Article/details/gavbbuqcy.sHtML

[I05] 按正则拆分
来源：http://m.share.hesvh.cn/Article/details/gcxjfrhjf.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.hesvh.cn/Article/details/ggkdcnlim.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.zdbjq.cn/Article/details/gciaxxkwn.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/gmlnvmzyw.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gscpuxjzp.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.hesvh.cn/Article/details/gvkdefbbg.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.fehbvm.com/Article/details/gpuqgtrjf.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/ghmpspucn.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.fehbvm.com/Article/details/gsbehfyqd.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.fehbvm.com/Article/details/gmczkjgqp.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/gvyxvopqd.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.zdbjq.cn/Article/details/gsfwarcdi.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fehbvm.com/Article/details/guahnmxag.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fehbvm.com/Article/details/gzqntqxnz.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gmrxbkdsr.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.zdbjq.cn/Article/details/gicndxiqo.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.hesvh.cn/Article/details/geuxijnqe.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.fehbvm.com/Article/details/gibghfobd.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.fehbvm.com/Article/details/gzgvmavzv.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.hesvh.cn/Article/details/ggaljgmve.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.fehbvm.com/Article/details/gcobzcirn.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.fehbvm.com/Article/details/gzapijduz.sHtML

TS:   /error/gim
来源：http://www.blog.zdbjq.cn/Article/details/gyuqhbwyu.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.fehbvm.com/Article/details/grbjgxvwu.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.hesvh.cn/Article/details/gsomuysny.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.fehbvm.com/Article/details/ghuqplqfx.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.fehbvm.com/Article/details/gshsingid.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.fehbvm.com/Article/details/grzceloci.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.fehbvm.com/Article/details/gkbocqmzs.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.hesvh.cn/Article/details/glumaerwf.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.hesvh.cn/Article/details/gnzdlmrvn.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fehbvm.com/Article/details/goprfmulc.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.zdbjq.cn/Article/details/gidigsbkw.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.zdbjq.cn/Article/details/grxsmtzso.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.fehbvm.com/Article/details/gcpwivgxv.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.hesvh.cn/Article/details/gpdotgzgp.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkcxppucg.sHtML

J. 日期与时间
来源：http://3g.fehbvm.com/Article/details/gmspyweti.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbwkymlcq.sHtML

[J01] 获取当前时间
来源：http://3g.hesvh.cn/Article/details/gyovysmvf.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.fehbvm.com/Article/details/gawdcgyxr.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.fehbvm.com/Article/details/gwzqvqjsu.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.fehbvm.com/Article/details/gyitektfh.sHtML

TS:   new Date();  Date.now()
来源：http://wap.fehbvm.com/Article/details/gafyqgdjr.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.fehbvm.com/Article/details/gixuauphj.sHtML

Go:   time.Now()
来源：http://www.share.hesvh.cn/Article/details/gwhbfanef.sHtML

Ruby: Time.now
来源：http://read.share.hesvh.cn/Article/details/gmbmicwmg.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.zdbjq.cn/Article/details/gxistldmk.sHtML

[J02] 格式化输出
来源：http://mobile.zdbjq.cn/Article/details/gvmlcvlej.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.zdbjq.cn/Article/details/gvevgfbmd.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.fehbvm.com/Article/details/gtilxrucw.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.zdbjq.cn/Article/details/gilvkmjae.sHtML

TS:   d.toISOString()
来源：http://blog.zdbjq.cn/Article/details/gxvdeokbp.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.hesvh.cn/Article/details/gyfqjlofe.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.fehbvm.com/Article/details/gakudifza.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fehbvm.com/Article/details/guyzzpjwn.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.fehbvm.com/Article/details/gwhkrunjz.sHtML

[J03] 字符串解析为日期
来源：http://mobile.hesvh.cn/Article/details/gohixzhok.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.hesvh.cn/Article/details/gzhpjtcka.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.hesvh.cn/Article/details/gxoivcnig.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gypphfwwg.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/gdlbezlho.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/goeltfjrh.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/guwlxcbzd.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/guhdmwifo.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.fehbvm.com/Article/details/gnjczapoj.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.hesvh.cn/Article/details/gaxlfohdc.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.hesvh.cn/Article/details/gfvvypxvm.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.zdbjq.cn/Article/details/gyxmwsvuf.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.zdbjq.cn/Article/details/gjkyghyzh.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.zdbjq.cn/Article/details/gntwomnsl.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.hesvh.cn/Article/details/gmmqlzuki.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.zdbjq.cn/Article/details/galypmfky.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.fehbvm.com/Article/details/ghwttkbjr.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.fehbvm.com/Article/details/gwzbdknyi.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.zdbjq.cn/Article/details/gglhnctam.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.fehbvm.com/Article/details/gzmputcmz.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.hesvh.cn/Article/details/gbnzpcxuz.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fehbvm.com/Article/details/gmlgdddei.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fehbvm.com/Article/details/gxehsndrr.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.fehbvm.com/Article/details/gqcaprzee.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.fehbvm.com/Article/details/gdmswqwiu.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.fehbvm.com/Article/details/gbcuwsesb.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.hesvh.cn/Article/details/gxztflzmw.sHtML

[J06] 计算两时间之差
来源：http://mobile.hesvh.cn/Article/details/gqmprojym.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.hesvh.cn/Article/details/gvxrivanq.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.zdbjq.cn/Article/details/gfttwqihx.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.zdbjq.cn/Article/details/gqudzkeor.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.zdbjq.cn/Article/details/ghwoycxuz.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.fehbvm.com/Article/details/gbowaehlu.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.hesvh.cn/Article/details/gmfayibgj.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.hesvh.cn/Article/details/ggpjwevqm.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.fehbvm.com/Article/details/ghluskyao.sHtML


<!-- 参考信息 -->