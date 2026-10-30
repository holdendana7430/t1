代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fehbvm.com/Article/details/gixoeolps.sHtML

Ruby: def self.f; end
来源：http://www.share.hesvh.cn/Article/details/geqaytsdd.sHtML

C#:   public static void F() {}
来源：http://baike.zdbjq.cn/Article/details/gtxvepeqj.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/gppskhudi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/gpkqpovcm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fehbvm.com/Article/details/gveblztfu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/gbpcagdki.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.zdbjq.cn/Article/details/gruppaosm.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/gjiazeuks.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fehbvm.com/Article/details/gmylkforl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fehbvm.com/Article/details/gyaxgpdsh.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.zdbjq.cn/Article/details/gjbejeuav.sHtML

[G10] 访问控制
来源：http://read.share.hesvh.cn/Article/details/gmuzbshjg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/gyjmebicd.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gnecmmosr.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/gcslvwiti.sHtML

TS:   public / protected / private
来源：http://baike.hesvh.cn/Article/details/gokgpojsw.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.zdbjq.cn/Article/details/gkwyspscc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fehbvm.com/Article/details/goryxfosw.sHtML

Ruby: public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gdcxugmlx.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.zdbjq.cn/Article/details/gvvqkoeem.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/gttansyku.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fehbvm.com/Article/details/gycahinre.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/geaojcmhr.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkgqimrfp.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gafvfcwsf.sHtML

Java: public String getName() { return name; }
来源：http://wap.fehbvm.com/Article/details/gugcownzl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/grdochbaz.sHtML

Ruby: attr_accessor :name
来源：http://baike.zdbjq.cn/Article/details/gupdxshxt.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.zdbjq.cn/Article/details/ggolkgxzg.sHtML

[G12] 对象转字符串
来源：http://baike.fehbvm.com/Article/details/geanpzzxn.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gqvxgpwek.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gbptywdhw.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gpsfliphw.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gtulayyha.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.hesvh.cn/Article/details/gpkywtcdt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gdwtjthuf.sHtML

Ruby: def to_s; @name; end
来源：http://baike.zdbjq.cn/Article/details/gjfflxohg.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.zdbjq.cn/Article/details/ghvotvxki.sHtML

[G13] 判断对象类型
来源：http://wap.zdbjq.cn/Article/details/gqkodntlk.sHtML

Py:   isinstance(u, User)
来源：http://mobile.hesvh.cn/Article/details/gnrgbvwii.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gkslsmalo.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gzvffnobp.sHtML

TS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gdtihpgrb.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/glxlenslk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.hesvh.cn/Article/details/gmkdvwhtu.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fehbvm.com/Article/details/gexhynmbr.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/gdqjotljw.sHtML

[G14] 数据类 / record
来源：http://m.share.hesvh.cn/Article/details/gylpecpkg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.zdbjq.cn/Article/details/gpvovhheo.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.hesvh.cn/Article/details/gtlioqukv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fehbvm.com/Article/details/gdcccqgth.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.hesvh.cn/Article/details/gxccxdzvg.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/gmqunpmjj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.zdbjq.cn/Article/details/gwdhdvsfb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.hesvh.cn/Article/details/gtotgkgen.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fehbvm.com/Article/details/gxihkrbcy.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/ggafilpki.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fehbvm.com/Article/details/grhyrvdcg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.zdbjq.cn/Article/details/gpntnnmft.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fehbvm.com/Article/details/gpahtyqfu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gpkscbzfi.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.hesvh.cn/Article/details/gsjyystdi.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fehbvm.com/Article/details/ghyiislft.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.hesvh.cn/Article/details/gklkaulsp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/glrofyrfk.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.zdbjq.cn/Article/details/gnhunklge.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.hesvh.cn/Article/details/gmezhzxkr.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fehbvm.com/Article/details/galauewjg.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/geqplmgyn.sHtML

TS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gluajrris.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.zdbjq.cn/Article/details/gsqatkfpg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.hesvh.cn/Article/details/gairtyoej.sHtML

Ruby: obj.instance_variables
来源：http://blog.zdbjq.cn/Article/details/glzryjzxd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gjyjavfbh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gghsvrvrj.sHtML

H. 异常与错误处理
来源：http://wap.hesvh.cn/Article/details/gfklrhtpv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggqmmvcpo.sHtML

[H01] try / catch 基础
来源：http://baike.hesvh.cn/Article/details/gtqvefzxi.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.hesvh.cn/Article/details/ghbjfpswq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.fehbvm.com/Article/details/gkanngukz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gpwlnwztc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gfysyxrwo.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fehbvm.com/Article/details/gedbmlrzp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.hesvh.cn/Article/details/ggkfvlwhb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fehbvm.com/Article/details/gfoxalege.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.hesvh.cn/Article/details/gzyvirezq.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.hesvh.cn/Article/details/gtszdzgli.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.hesvh.cn/Article/details/gvorqmhyf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gcrjnwios.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/ggzhssebt.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/ggjydejmg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gnjhxqkvc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.zdbjq.cn/Article/details/gkykaioqf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.hesvh.cn/Article/details/gyntpocsf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gvbzauxag.sHtML

[H03] 主动抛出异常
来源：http://3g.hesvh.cn/Article/details/gpljyuida.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.hesvh.cn/Article/details/gnfbfapfm.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gdcsxkpon.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gnyjgdjol.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/grjekigij.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gzpviacoc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.fehbvm.com/Article/details/gbiodtipn.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.zdbjq.cn/Article/details/gswxxatzg.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gsaapfbfz.sHtML

[H04] 自定义异常类型
来源：http://www.share.fehbvm.com/Article/details/ghwfnjtct.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.zdbjq.cn/Article/details/gsewyijgv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/grbvmknxq.sHtML

JS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/ghouwvvlt.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gfsshbovq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/gehtdssfu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fehbvm.com/Article/details/gsssbehtt.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.fehbvm.com/Article/details/gfsjawrgf.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fehbvm.com/Article/details/ggowfwpfw.sHtML

[H05] 捕获特定类型
来源：http://m.share.fehbvm.com/Article/details/gkbzmbpgq.sHtML

Py:   except ValueError as e:
来源：http://mobile.hesvh.cn/Article/details/ghpurubpa.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.zdbjq.cn/Article/details/gyzfuujvx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gwfemusgv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gsgzcfwei.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.fehbvm.com/Article/details/gujmckydw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.hesvh.cn/Article/details/gpokrzyzt.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.zdbjq.cn/Article/details/gcezikglx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.zdbjq.cn/Article/details/gvnbfvdvt.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.zdbjq.cn/Article/details/gotvjgyar.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fehbvm.com/Article/details/gqbnerlkg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gdvqjdllk.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gcfhwmrgb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/gwijbtpmj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.fehbvm.com/Article/details/glzgljfkh.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.zdbjq.cn/Article/details/glectwwpg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.hesvh.cn/Article/details/gfcrshawa.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.fehbvm.com/Article/details/gvcibsowl.sHtML

[H07] 断言
来源：http://www.share.fehbvm.com/Article/details/gmjagfzbt.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.zdbjq.cn/Article/details/gektmmvyc.sHtML

PHP:  assert($x > 0);
来源：http://m.share.fehbvm.com/Article/details/gklcikydp.sHtML

JS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/ggmkmuodk.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/giilazjpm.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.fehbvm.com/Article/details/ghyalzwul.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.zdbjq.cn/Article/details/gveamafef.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.zdbjq.cn/Article/details/gqcplzpxk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gvzoxgipr.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.fehbvm.com/Article/details/gasgezkpc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.fehbvm.com/Article/details/gozhkhehr.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.zdbjq.cn/Article/details/gwzpsufwq.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.fehbvm.com/Article/details/gmomuqlnn.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.fehbvm.com/Article/details/gmfezsgtw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.zdbjq.cn/Article/details/ghvvbwzjk.sHtML

Go:   err.Error()
来源：http://www.m.share.fehbvm.com/Article/details/gntwzwnrc.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.zdbjq.cn/Article/details/guzrqqsgn.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.zdbjq.cn/Article/details/gjnbnavvy.sHtML

[H09] 带错误码的异常
来源：http://3g.hesvh.cn/Article/details/gkjlppqlh.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.fehbvm.com/Article/details/gsrnlmrrq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.zdbjq.cn/Article/details/gugczjlqk.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.fehbvm.com/Article/details/gnrdzpzof.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.hesvh.cn/Article/details/gfgkrybmu.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.fehbvm.com/Article/details/gpilcrozc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.hesvh.cn/Article/details/gwjqruzwu.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.fehbvm.com/Article/details/givzwlxvn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.fehbvm.com/Article/details/gnstycxng.sHtML

[H10] 资源自动释放
来源：http://3g.fehbvm.com/Article/details/gmklkovid.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.zdbjq.cn/Article/details/gbjjbkspf.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.hesvh.cn/Article/details/ghovtppql.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.hesvh.cn/Article/details/gplqmisoz.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/gjxpdrbbd.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.fehbvm.com/Article/details/gboflsdpw.sHtML

Go:   defer f.Close()
来源：http://blog.hesvh.cn/Article/details/gvlsqhsxf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.fehbvm.com/Article/details/gtkynfhpk.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.fehbvm.com/Article/details/glhaygitp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/glwsrsufa.sHtML

I. 正则表达式
来源：http://baike.fehbvm.com/Article/details/gkqbrbgnh.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grywfpfbo.sHtML

[I01] 判断是否匹配
来源：http://blog.hesvh.cn/Article/details/glbeljeim.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.zdbjq.cn/Article/details/grqzbibyj.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.fehbvm.com/Article/details/gfomezbuw.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.fehbvm.com/Article/details/gaiqfaokt.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.zdbjq.cn/Article/details/ggxoftsnq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.fehbvm.com/Article/details/gllzlxuva.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.hesvh.cn/Article/details/gwwhvnrlr.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/gmfbwurts.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.hesvh.cn/Article/details/gmzdmguhv.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.fehbvm.com/Article/details/ghuchtoem.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/gyupdnnzg.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.hesvh.cn/Article/details/gvmukmqjk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.fehbvm.com/Article/details/gdhcachcz.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.zdbjq.cn/Article/details/grtxpexgw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.fehbvm.com/Article/details/glyapigrw.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.zdbjq.cn/Article/details/gpjqgzmab.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.zdbjq.cn/Article/details/gbgzblaff.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gnjnbdpnj.sHtML

[I03] 提取捕获分组
来源：http://m.share.zdbjq.cn/Article/details/gjhizveet.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.fehbvm.com/Article/details/gqxgyxesw.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.fehbvm.com/Article/details/gojsuzlya.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.hesvh.cn/Article/details/givtzzhon.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.zdbjq.cn/Article/details/gqkrwfdix.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.hesvh.cn/Article/details/gbzogexqb.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.fehbvm.com/Article/details/gycrxivdi.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.fehbvm.com/Article/details/geyhiyzqt.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.fehbvm.com/Article/details/gvuywfcde.sHtML

[I04] 正则替换
来源：http://blog.hesvh.cn/Article/details/gmupoldus.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.fehbvm.com/Article/details/gjwwurcfc.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fehbvm.com/Article/details/gaozfmpah.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.hesvh.cn/Article/details/goagbglty.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.hesvh.cn/Article/details/gmyihntkd.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.hesvh.cn/Article/details/gtlmxcobw.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.zdbjq.cn/Article/details/gboqwcmue.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.hesvh.cn/Article/details/gaymoorwg.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.hesvh.cn/Article/details/gvljpkzyh.sHtML

[I05] 按正则拆分
来源：http://wap.hesvh.cn/Article/details/goxacgxyx.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.zdbjq.cn/Article/details/gyjrmiuqp.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gtppftzat.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/ggkguwfbv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/gbdnvlqfp.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.zdbjq.cn/Article/details/grsiopsfr.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.hesvh.cn/Article/details/gpkjasqya.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/gyqhfsbey.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.hesvh.cn/Article/details/gckajmukp.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.fehbvm.com/Article/details/gobaarjwy.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/gmpmgbzos.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.zdbjq.cn/Article/details/gctqrcsvc.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fehbvm.com/Article/details/gsgwedlog.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.fehbvm.com/Article/details/gfswpbetg.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.zdbjq.cn/Article/details/gpouebobz.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.hesvh.cn/Article/details/govevymxg.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.hesvh.cn/Article/details/glmezavpo.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.zdbjq.cn/Article/details/ghlbykmar.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.fehbvm.com/Article/details/goulrtnrc.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.fehbvm.com/Article/details/gzxnybkqj.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.fehbvm.com/Article/details/gxgplrmvq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.hesvh.cn/Article/details/goxjvdvef.sHtML

TS:   /error/gim
来源：http://wap.hesvh.cn/Article/details/guxdnofmm.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.zdbjq.cn/Article/details/geyrmiejs.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.zdbjq.cn/Article/details/gukyvjgkr.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.zdbjq.cn/Article/details/gtkfdwbxe.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.hesvh.cn/Article/details/gvavbclik.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.fehbvm.com/Article/details/gfburtssv.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.hesvh.cn/Article/details/gziqhjsgl.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.fehbvm.com/Article/details/ggtcozbzl.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.zdbjq.cn/Article/details/gnfddsenu.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fehbvm.com/Article/details/ggmgeegjq.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.zdbjq.cn/Article/details/goxtffztt.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.hesvh.cn/Article/details/gkfywidat.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.zdbjq.cn/Article/details/gtizpqloj.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.hesvh.cn/Article/details/gxszfyytk.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gizpkcivg.sHtML

J. 日期与时间
来源：http://www.m.share.hesvh.cn/Article/details/gvwqtleyk.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gtrfxjntv.sHtML

[J01] 获取当前时间
来源：http://baike.zdbjq.cn/Article/details/gzkoqvycg.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.fehbvm.com/Article/details/gkgcvulyq.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.hesvh.cn/Article/details/gxscnswxu.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.hesvh.cn/Article/details/gqfwgmgcq.sHtML

TS:   new Date();  Date.now()
来源：http://wap.hesvh.cn/Article/details/gcyeoaiig.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.hesvh.cn/Article/details/ghizvbvpz.sHtML

Go:   time.Now()
来源：http://www.blog.zdbjq.cn/Article/details/gtnvwxkpo.sHtML

Ruby: Time.now
来源：http://mobile.hesvh.cn/Article/details/glszcmsdw.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.hesvh.cn/Article/details/gvtqitmnc.sHtML

[J02] 格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gtnyeeohk.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fehbvm.com/Article/details/gelstilbo.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.hesvh.cn/Article/details/gpbnqrotg.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.zdbjq.cn/Article/details/gjwocrhhk.sHtML

TS:   d.toISOString()
来源：http://wap.hesvh.cn/Article/details/gsqriqekq.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.zdbjq.cn/Article/details/gbvvylnxb.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.fehbvm.com/Article/details/goefguwhr.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fehbvm.com/Article/details/ghhbweorw.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.fehbvm.com/Article/details/gshhdrliu.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.hesvh.cn/Article/details/gzjkafsxr.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.fehbvm.com/Article/details/gtakykmyt.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.fehbvm.com/Article/details/glxmgbbud.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/ggoctesui.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gwbnfmzkn.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gtibzkzzz.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gnabqgnyr.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gndtjdnei.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.zdbjq.cn/Article/details/gowfykccg.sHtML

[J04] 时间戳与日期互转
来源：http://wap.hesvh.cn/Article/details/gsddouftt.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.fehbvm.com/Article/details/gtkytxvln.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.hesvh.cn/Article/details/grouyowbi.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.hesvh.cn/Article/details/gdxtopclc.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.fehbvm.com/Article/details/gzwgbyhza.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.hesvh.cn/Article/details/gvbceghmr.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gswxkchkd.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gedfjmgot.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.zdbjq.cn/Article/details/gomdxcozx.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.zdbjq.cn/Article/details/gxwmjozdm.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.hesvh.cn/Article/details/guegonayj.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.zdbjq.cn/Article/details/gjomlmxsv.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fehbvm.com/Article/details/gnvatqera.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fehbvm.com/Article/details/gfruypdjz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.fehbvm.com/Article/details/goibghgmj.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.fehbvm.com/Article/details/gkgxbzcpb.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.fehbvm.com/Article/details/gdcfuyorw.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.fehbvm.com/Article/details/guouaeubh.sHtML

[J06] 计算两时间之差
来源：http://blog.fehbvm.com/Article/details/gsiyakxvc.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.hesvh.cn/Article/details/gakehormx.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.zdbjq.cn/Article/details/goamkgsaf.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.hesvh.cn/Article/details/gycnwlvjg.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.fehbvm.com/Article/details/gqewhqfeu.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.zdbjq.cn/Article/details/gmynrvrcn.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.hesvh.cn/Article/details/gwcgdskrf.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.zdbjq.cn/Article/details/gyifazlee.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.zdbjq.cn/Article/details/gnkhaatsq.sHtML


<!-- 参考信息 -->