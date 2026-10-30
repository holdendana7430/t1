代发 wailian999

Java: interface Shape { double area(); }
来源：http://m.share.hesvh.cn/Article/details/gotkfbkwf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.zdbjq.cn/Article/details/gpduhebqn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.hesvh.cn/Article/details/ggervpmhf.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/gmrtpcwax.sHtML

[G10] 访问控制
来源：http://m.share.hesvh.cn/Article/details/gekobxxog.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.hesvh.cn/Article/details/gyquvroea.sHtML

PHP:  public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gcgganzty.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/gdhanugjy.sHtML

TS:   public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gjwydbzgh.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/gjalofdtq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.zdbjq.cn/Article/details/gaewuwmlo.sHtML

Ruby: public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gporttuwc.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/goxsrulsd.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/gfcgnnahe.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fehbvm.com/Article/details/glyrnsaaz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/galqluitt.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gnhwbaadz.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gbwbvbfbj.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gwozmumms.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gqonzhehw.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/gaoyckugc.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.zdbjq.cn/Article/details/gotzindho.sHtML

[G12] 对象转字符串
来源：http://www.share.zdbjq.cn/Article/details/gglqpymnr.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gedoagogp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gtnjymfgu.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gerumxlon.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkshcyupb.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gfijxeozu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gmaseoupo.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fehbvm.com/Article/details/gfkjukjdj.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/geacrosef.sHtML

[G13] 判断对象类型
来源：http://www.blog.hesvh.cn/Article/details/grgcxnboj.sHtML

Py:   isinstance(u, User)
来源：http://3g.hesvh.cn/Article/details/gzoyvwehz.sHtML

PHP:  $u instanceof User
来源：http://blog.fehbvm.com/Article/details/gzcjbxjgi.sHtML

JS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/ghpxyvfvp.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/grahvilwv.sHtML

Java: u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gockyirll.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.hesvh.cn/Article/details/gscklpjrk.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/gjokbbwsm.sHtML

C#:   u is User
来源：http://m.share.zdbjq.cn/Article/details/gfkbkwcsa.sHtML

[G14] 数据类 / record
来源：http://www.share.zdbjq.cn/Article/details/ghmeyclod.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fehbvm.com/Article/details/gnskuoydy.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.hesvh.cn/Article/details/gknjkqwms.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.hesvh.cn/Article/details/gwqnaekdd.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.zdbjq.cn/Article/details/gdrnuaoli.sHtML

Java: record User(String name, int age) {}
来源：http://baike.zdbjq.cn/Article/details/gbumhcryd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.zdbjq.cn/Article/details/gcrnlnegh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.zdbjq.cn/Article/details/gqgibzdjp.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.hesvh.cn/Article/details/gwhcrhdcw.sHtML

[G15] 枚举
来源：http://m.share.hesvh.cn/Article/details/gwinulltk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.hesvh.cn/Article/details/ghqbohlhj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fehbvm.com/Article/details/gombdqvya.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fehbvm.com/Article/details/gsyruqjgk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/ghgngiomn.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.hesvh.cn/Article/details/gviytekbu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.hesvh.cn/Article/details/gvsgusjlp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.hesvh.cn/Article/details/gyikuxvje.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gigzdzxes.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fehbvm.com/Article/details/gkwzprofa.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.hesvh.cn/Article/details/grkhycncl.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.hesvh.cn/Article/details/grtmxntqf.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gfduobktp.sHtML

TS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gxcjkigax.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fehbvm.com/Article/details/gezvjveyc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.zdbjq.cn/Article/details/gpxicfwql.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fehbvm.com/Article/details/gnaavkutj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/gkkphtpfb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmibpbwru.sHtML

H. 异常与错误处理
来源：http://m.share.fehbvm.com/Article/details/gyzpziqve.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gilrridox.sHtML

[H01] try / catch 基础
来源：http://www.share.hesvh.cn/Article/details/gdrguqtll.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.fehbvm.com/Article/details/gnnimrrcb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fehbvm.com/Article/details/gcnifzbsd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gwryvklvf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gjgljhcjw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.hesvh.cn/Article/details/gqezucduv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.hesvh.cn/Article/details/gnfzmyotz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.zdbjq.cn/Article/details/gqhexrkpk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.zdbjq.cn/Article/details/gfhoyuyao.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.zdbjq.cn/Article/details/gjzoeeops.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.hesvh.cn/Article/details/gexjmlyww.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gznllxkux.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/galeherts.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/guoqnxddw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gjugyupdo.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fehbvm.com/Article/details/gsbytisge.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.zdbjq.cn/Article/details/grsxzomgz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gtrzchybx.sHtML

[H03] 主动抛出异常
来源：http://read.share.fehbvm.com/Article/details/gibuejcsp.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.fehbvm.com/Article/details/gmxtvtyxv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gahruakbg.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gyooqcmem.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gwrjgkmac.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gygxlbkxn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.fehbvm.com/Article/details/gbdrnklxd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.zdbjq.cn/Article/details/gauitxzcc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gpyhdmjck.sHtML

[H04] 自定义异常类型
来源：http://mobile.zdbjq.cn/Article/details/gflgmniyh.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.fehbvm.com/Article/details/gyoztcwyy.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gxtkedqpt.sHtML

JS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/gwjvewnrj.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/gjukaxexc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gasugsahp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.zdbjq.cn/Article/details/gvjobmvmj.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.hesvh.cn/Article/details/gwhgxlcam.sHtML

C#:   class MyException : Exception {}
来源：http://baike.hesvh.cn/Article/details/gfcmhabfz.sHtML

[H05] 捕获特定类型
来源：http://m.share.zdbjq.cn/Article/details/gdcipnizb.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.hesvh.cn/Article/details/gdbhazbcc.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fehbvm.com/Article/details/gzwpwzybs.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gnkwipjja.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/giphdtlgf.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.zdbjq.cn/Article/details/gloqamkwx.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.zdbjq.cn/Article/details/gbchwnhnt.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.hesvh.cn/Article/details/gxwuzruor.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.fehbvm.com/Article/details/gctoguhoh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.zdbjq.cn/Article/details/gymtgowrq.sHtML

Py:   value = d.get("k") or default
来源：http://wap.zdbjq.cn/Article/details/gtmorpymv.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gunurvlfy.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gzqoetrst.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/guvgdksls.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.hesvh.cn/Article/details/glamnyrqa.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.zdbjq.cn/Article/details/gzhukzxht.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.hesvh.cn/Article/details/gjnlqkgjc.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.hesvh.cn/Article/details/goivfdtbt.sHtML

[H07] 断言
来源：http://www.share.fehbvm.com/Article/details/gkiodyhck.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.hesvh.cn/Article/details/gzguropfb.sHtML

PHP:  assert($x > 0);
来源：http://baike.zdbjq.cn/Article/details/gwzfleiuk.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gigtyonof.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gprmbotyl.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.zdbjq.cn/Article/details/gqlmhmqar.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.fehbvm.com/Article/details/gxduoxook.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.zdbjq.cn/Article/details/gqmlwilri.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gnylupnxc.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.fehbvm.com/Article/details/gpvcqqimj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.hesvh.cn/Article/details/ggufyqzgy.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.hesvh.cn/Article/details/gopaumlcx.sHtML

JS:   e.message;  e.stack
来源：http://blog.hesvh.cn/Article/details/guyqmkwoj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.zdbjq.cn/Article/details/gxagezqhe.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.fehbvm.com/Article/details/gebxrlhns.sHtML

Go:   err.Error()
来源：http://blog.zdbjq.cn/Article/details/gzwoczllh.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.fehbvm.com/Article/details/grsorhstg.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.hesvh.cn/Article/details/gqxogtqtp.sHtML

[H09] 带错误码的异常
来源：http://m.share.hesvh.cn/Article/details/gagmateqi.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.hesvh.cn/Article/details/gfiorrxse.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gachohewm.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.hesvh.cn/Article/details/gwqxgwhkz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.fehbvm.com/Article/details/gidfdnaft.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.zdbjq.cn/Article/details/gbpgouric.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.fehbvm.com/Article/details/gyatjecos.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.fehbvm.com/Article/details/guvaisebt.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.fehbvm.com/Article/details/gjnefbugi.sHtML

[H10] 资源自动释放
来源：http://baike.zdbjq.cn/Article/details/gcodfkqrh.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.fehbvm.com/Article/details/gdnhvouhw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.fehbvm.com/Article/details/gilazpcyz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/gycbyzmqp.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/gkqmemwrv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.hesvh.cn/Article/details/gxwgdcixp.sHtML

Go:   defer f.Close()
来源：http://mobile.hesvh.cn/Article/details/gugqrbjfz.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.zdbjq.cn/Article/details/gwexlkces.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gwspqrjez.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gekcapwxr.sHtML

I. 正则表达式
来源：http://blog.fehbvm.com/Article/details/ghprpcuou.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjwrlcgmo.sHtML

[I01] 判断是否匹配
来源：http://wap.hesvh.cn/Article/details/gywxaqcnk.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/gxyeywsbq.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gokhlknta.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.zdbjq.cn/Article/details/gvdaarmrw.sHtML

TS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/gqrhtecjf.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.zdbjq.cn/Article/details/gyfvpprxj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.hesvh.cn/Article/details/gkamhcqiu.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.fehbvm.com/Article/details/ghxozbvyt.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.fehbvm.com/Article/details/ghuwggrqk.sHtML

[I02] 提取所有匹配
来源：http://blog.hesvh.cn/Article/details/ghgiozbsu.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.hesvh.cn/Article/details/ggarwyugg.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.fehbvm.com/Article/details/gqlbeewka.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.zdbjq.cn/Article/details/gqokjirff.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.hesvh.cn/Article/details/gylyndrjm.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.hesvh.cn/Article/details/gyeotcsqa.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.zdbjq.cn/Article/details/gmqfsotqq.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.hesvh.cn/Article/details/guezdzphq.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gcngxxteu.sHtML

[I03] 提取捕获分组
来源：http://3g.fehbvm.com/Article/details/gbjvhzrjc.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.fehbvm.com/Article/details/griyreylw.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.hesvh.cn/Article/details/gnksetwqv.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.zdbjq.cn/Article/details/gocgrusqz.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.hesvh.cn/Article/details/givmptxbo.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.fehbvm.com/Article/details/gtekwfyjn.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.hesvh.cn/Article/details/gsmgzvsac.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.fehbvm.com/Article/details/gdqsbxoea.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.fehbvm.com/Article/details/gjqaqmcvs.sHtML

[I04] 正则替换
来源：http://blog.hesvh.cn/Article/details/gujbqqlzh.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.fehbvm.com/Article/details/ginnbhzbm.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/gcopqbujz.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.hesvh.cn/Article/details/gsguoimaw.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.zdbjq.cn/Article/details/ghoeaxncm.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gfexmbiid.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.zdbjq.cn/Article/details/gvhlguyoj.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.zdbjq.cn/Article/details/gdsxdlndr.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.hesvh.cn/Article/details/grghjevil.sHtML

[I05] 按正则拆分
来源：http://www.m.share.hesvh.cn/Article/details/godrwkidq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.fehbvm.com/Article/details/gsgiiqiet.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.fehbvm.com/Article/details/gjkzdaqmy.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.fehbvm.com/Article/details/gkovejtsl.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/gtslxuqvw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.zdbjq.cn/Article/details/gwcqijwnq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.hesvh.cn/Article/details/gwrnpebuy.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/goyfwjble.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.hesvh.cn/Article/details/gschhxpsk.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.fehbvm.com/Article/details/gprmmaviq.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/ghmydxugg.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.fehbvm.com/Article/details/gjyzrvtsy.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.hesvh.cn/Article/details/gmqrnzzhg.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.zdbjq.cn/Article/details/gcktiaycq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.fehbvm.com/Article/details/gufzetqiz.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.hesvh.cn/Article/details/gfdzanalq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.hesvh.cn/Article/details/gunqxsmjj.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.zdbjq.cn/Article/details/gpruwyrqd.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.fehbvm.com/Article/details/gutydqyfq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.fehbvm.com/Article/details/grctwumfo.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.fehbvm.com/Article/details/godbyniig.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.hesvh.cn/Article/details/gyijpmzuv.sHtML

TS:   /error/gim
来源：http://mobile.zdbjq.cn/Article/details/gtdjomlel.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.hesvh.cn/Article/details/ghpohqvcd.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.fehbvm.com/Article/details/gxdwglbnc.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.hesvh.cn/Article/details/gqrkpdslh.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.hesvh.cn/Article/details/gpcmbgfof.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.zdbjq.cn/Article/details/gtodzmccn.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.zdbjq.cn/Article/details/ghbxcwteo.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.hesvh.cn/Article/details/gzlsbjjpu.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fehbvm.com/Article/details/gqrulveum.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.zdbjq.cn/Article/details/gyuqopkhv.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.zdbjq.cn/Article/details/gxubcigtc.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.zdbjq.cn/Article/details/gwgouzfdi.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.hesvh.cn/Article/details/gcoqmbnih.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.hesvh.cn/Article/details/gklkzzuxc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxebxtftf.sHtML

J. 日期与时间
来源：http://blog.hesvh.cn/Article/details/grbrmtebc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gpmkxykbp.sHtML

[J01] 获取当前时间
来源：http://wap.fehbvm.com/Article/details/gcqsyoscg.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.fehbvm.com/Article/details/gsqiadysu.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.fehbvm.com/Article/details/goxkmqexw.sHtML

JS:   new Date();  Date.now()
来源：http://3g.fehbvm.com/Article/details/gthitosjl.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.zdbjq.cn/Article/details/gamxrdpya.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.fehbvm.com/Article/details/gnsaewtea.sHtML

Go:   time.Now()
来源：http://blog.hesvh.cn/Article/details/gmpyfvbpx.sHtML

Ruby: Time.now
来源：http://mobile.hesvh.cn/Article/details/gdeyglcud.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.hesvh.cn/Article/details/geroodwod.sHtML

[J02] 格式化输出
来源：http://www.share.hesvh.cn/Article/details/gfykisalw.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fehbvm.com/Article/details/gdawuopsk.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.zdbjq.cn/Article/details/gmihydepc.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.fehbvm.com/Article/details/gglubiool.sHtML

TS:   d.toISOString()
来源：http://baike.fehbvm.com/Article/details/gtftdkrhf.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.zdbjq.cn/Article/details/glbuwmjvy.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.fehbvm.com/Article/details/gehbauqhb.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.zdbjq.cn/Article/details/gwvqsifja.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.fehbvm.com/Article/details/gycpteuvu.sHtML

[J03] 字符串解析为日期
来源：http://baike.hesvh.cn/Article/details/gluqjlfmt.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.zdbjq.cn/Article/details/gglvlaomm.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.fehbvm.com/Article/details/gcafwkgzs.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gdnnivpwu.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/ggzcfhiqq.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gyadsbith.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gyfoletds.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gqhnqiztf.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.hesvh.cn/Article/details/gtmglahvm.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.fehbvm.com/Article/details/giyquplbr.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.hesvh.cn/Article/details/geajgdxfj.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.fehbvm.com/Article/details/ggsmwjbad.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.fehbvm.com/Article/details/gerdfmaol.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.zdbjq.cn/Article/details/gefnsntht.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.zdbjq.cn/Article/details/gmoknkqxe.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.fehbvm.com/Article/details/gbtpmshgb.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.fehbvm.com/Article/details/gnluypdjc.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.fehbvm.com/Article/details/gjchdiugf.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.fehbvm.com/Article/details/gwxxovdcv.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.fehbvm.com/Article/details/gyedawtsi.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.zdbjq.cn/Article/details/gtizrnnml.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fehbvm.com/Article/details/gycdtutng.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.hesvh.cn/Article/details/gemjmlvbn.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.hesvh.cn/Article/details/gecmambll.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.fehbvm.com/Article/details/gsenmauar.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.fehbvm.com/Article/details/grxxyhitv.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.zdbjq.cn/Article/details/govvzcksj.sHtML

[J06] 计算两时间之差
来源：http://www.blog.hesvh.cn/Article/details/goamnqcix.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.fehbvm.com/Article/details/grquxqofd.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.hesvh.cn/Article/details/gvecjtlwh.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.hesvh.cn/Article/details/ggwrhmlpm.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.zdbjq.cn/Article/details/gjscpmlbh.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.zdbjq.cn/Article/details/gdebypajx.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.hesvh.cn/Article/details/ggxidkapp.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.hesvh.cn/Article/details/gkkuuhoxr.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.zdbjq.cn/Article/details/gjdmrngvn.sHtML

[J07] 比较两个日期
来源：http://read.share.fehbvm.com/Article/details/gyyqervgf.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.zdbjq.cn/Article/details/ggsnkfvqv.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.fehbvm.com/Article/details/gaoeyaevp.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.zdbjq.cn/Article/details/gyotztgjg.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.hesvh.cn/Article/details/guaykexjm.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.hesvh.cn/Article/details/gvkwjbbcd.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.hesvh.cn/Article/details/gxwuvfdri.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/glrjhusmd.sHtML


<!-- 参考信息 -->