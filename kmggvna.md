代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.zdbjq.cn/Article/details/gzxmkikts.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/grsrcfbza.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/geaftowkr.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/gghoubwov.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.hesvh.cn/Article/details/gcycflven.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fehbvm.com/Article/details/gfnhrdslu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fehbvm.com/Article/details/gnsrrvnev.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fehbvm.com/Article/details/gspfuwqwq.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/gkdvspced.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.hesvh.cn/Article/details/gwqmzlzcs.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.hesvh.cn/Article/details/gxnbpjtaj.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/grqzoclce.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/gpbdazyrm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fehbvm.com/Article/details/glbwmerzp.sHtML

PHP:  public / protected / private
来源：http://read.share.fehbvm.com/Article/details/ghofubisu.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/gubkhvmzh.sHtML

TS:   public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gghynkhhb.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fehbvm.com/Article/details/glnosnxqn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/gcgdwvzza.sHtML

Ruby: public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gytrclxrm.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fehbvm.com/Article/details/gcwfzpsan.sHtML

[G11] getter / setter
来源：http://www.m.share.zdbjq.cn/Article/details/gnuuysbtl.sHtML

Py:   @property 与 @x.setter
来源：http://wap.hesvh.cn/Article/details/gtbridhxs.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gwxnnftkm.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/ghjcrfcuf.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gmchvtygu.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gymvrvmih.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gcykrlowb.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fehbvm.com/Article/details/gokbymkhj.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fehbvm.com/Article/details/gtygnyywg.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/gobcugrmf.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gtazjzfvo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gzczbdrjx.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gcuulaoic.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gwhuwirzo.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.hesvh.cn/Article/details/grqhopjvv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/ggttofrlm.sHtML

Ruby: def to_s; @name; end
来源：http://blog.hesvh.cn/Article/details/giymujrch.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/ganxxpzky.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/gqznhgoxp.sHtML

Py:   isinstance(u, User)
来源：http://blog.zdbjq.cn/Article/details/gbtanvfqe.sHtML

PHP:  $u instanceof User
来源：http://blog.hesvh.cn/Article/details/gemynimdz.sHtML

JS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gjkqohgln.sHtML

TS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gvtfcsbyt.sHtML

Java: u instanceof User
来源：http://baike.hesvh.cn/Article/details/gdmaszjmz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.zdbjq.cn/Article/details/gynxengyb.sHtML

Ruby: u.is_a?(User)
来源：http://3g.zdbjq.cn/Article/details/gzqimquqi.sHtML

C#:   u is User
来源：http://baike.hesvh.cn/Article/details/gfkoxteny.sHtML

[G14] 数据类 / record
来源：http://www.m.share.hesvh.cn/Article/details/gdvcgxhlj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.zdbjq.cn/Article/details/gjumrdkyp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.hesvh.cn/Article/details/gathyucgq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fehbvm.com/Article/details/gkdihckmj.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fehbvm.com/Article/details/gqskisfcr.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/gnqvrmczm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fehbvm.com/Article/details/gnkjtmtiy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.zdbjq.cn/Article/details/gftlqfxwr.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/gbwmcznjc.sHtML

[G15] 枚举
来源：http://www.blog.zdbjq.cn/Article/details/gqbubxtio.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.hesvh.cn/Article/details/gpnpeqavb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fehbvm.com/Article/details/gkzenhdxi.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.hesvh.cn/Article/details/gfnppjhok.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gvlercfug.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.hesvh.cn/Article/details/gjfgsqrpd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.zdbjq.cn/Article/details/glzuauazs.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.zdbjq.cn/Article/details/gtktedhdj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gvtarfzpq.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.zdbjq.cn/Article/details/gquahvene.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.fehbvm.com/Article/details/gngqgzduu.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fehbvm.com/Article/details/gznybpwnv.sHtML

JS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gleozcquj.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/grkgtqwpd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.zdbjq.cn/Article/details/gdraolbbx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.zdbjq.cn/Article/details/gxiuslyeg.sHtML

Ruby: obj.instance_variables
来源：http://wap.zdbjq.cn/Article/details/gdflogspj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gsjskyido.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvnkdmvqx.sHtML

H. 异常与错误处理
来源：http://mobile.fehbvm.com/Article/details/gwjxjmhpv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gecbwqxpm.sHtML

[H01] try / catch 基础
来源：http://wap.zdbjq.cn/Article/details/gvsqqtall.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.hesvh.cn/Article/details/gpjiyylsw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fehbvm.com/Article/details/gawfmfzof.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gedjzniem.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gfanjniab.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fehbvm.com/Article/details/geymjwrwq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.fehbvm.com/Article/details/gtpmqczxf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fehbvm.com/Article/details/gzdtzqcfa.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/ghwokobhn.sHtML

[H02] finally / ensure 收尾
来源：http://baike.hesvh.cn/Article/details/gvhjhgkzl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.hesvh.cn/Article/details/gedjplggf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gzdqivbfo.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/ghwmznoqp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gcvejvcpy.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/grmhqggxw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.hesvh.cn/Article/details/gzdlbryih.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.fehbvm.com/Article/details/gzudplmkv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gvauhwwko.sHtML

[H03] 主动抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gfvrapkfu.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.hesvh.cn/Article/details/gipusshjx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/ghiuzmsze.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gqtvrdebc.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/guhzgkknh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gjjbphzmj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.hesvh.cn/Article/details/gwhazalqt.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.zdbjq.cn/Article/details/gcdxldpnx.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gglqiepku.sHtML

[H04] 自定义异常类型
来源：http://m.share.zdbjq.cn/Article/details/gaygymqff.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.hesvh.cn/Article/details/gqzojzucj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/givesjbxe.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gtchrwrmk.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/genckvghi.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gooejnhdw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.zdbjq.cn/Article/details/gzoqebztc.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.hesvh.cn/Article/details/grzdbtwxe.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.zdbjq.cn/Article/details/gulwrhufv.sHtML

[H05] 捕获特定类型
来源：http://www.share.hesvh.cn/Article/details/gosstmqwv.sHtML

Py:   except ValueError as e:
来源：http://3g.fehbvm.com/Article/details/geyzatkls.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.zdbjq.cn/Article/details/gmtzxtrpv.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/guiigxbsu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/ghbcagnvb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.hesvh.cn/Article/details/grnibvvps.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fehbvm.com/Article/details/gxesoilbm.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.hesvh.cn/Article/details/gkoxigecg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.fehbvm.com/Article/details/gzgmxqrto.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.hesvh.cn/Article/details/gbydtjxtt.sHtML

Py:   value = d.get("k") or default
来源：http://3g.zdbjq.cn/Article/details/gfhmrsqil.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.fehbvm.com/Article/details/ghahabgsq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/ghxtrdypy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/gssknkmfe.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.hesvh.cn/Article/details/ghboncgdk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.hesvh.cn/Article/details/gviricfto.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.zdbjq.cn/Article/details/gqtczoxoa.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gpvnaufag.sHtML

[H07] 断言
来源：http://www.m.share.fehbvm.com/Article/details/glwqinguj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.hesvh.cn/Article/details/gwiikfnun.sHtML

PHP:  assert($x > 0);
来源：http://mobile.hesvh.cn/Article/details/gvpcvmxjy.sHtML

JS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gljexecnp.sHtML

TS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gpjykqqjf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.hesvh.cn/Article/details/gxxastokx.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.hesvh.cn/Article/details/gzwktnvxw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.zdbjq.cn/Article/details/gzwvyqpnu.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gykobzgoh.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.zdbjq.cn/Article/details/gelcynyjh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.fehbvm.com/Article/details/gsrozffbi.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.zdbjq.cn/Article/details/gviznuzru.sHtML

JS:   e.message;  e.stack
来源：http://mobile.hesvh.cn/Article/details/gwcoatpyb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.hesvh.cn/Article/details/giqmfefee.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.hesvh.cn/Article/details/gktbwehtr.sHtML

Go:   err.Error()
来源：http://www.share.zdbjq.cn/Article/details/gmywqbqis.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.zdbjq.cn/Article/details/glwabaocu.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.fehbvm.com/Article/details/ggudupfrb.sHtML

[H09] 带错误码的异常
来源：http://read.share.zdbjq.cn/Article/details/gfntjpfqv.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.fehbvm.com/Article/details/ggfvlqyrh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.zdbjq.cn/Article/details/giguqpudj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.fehbvm.com/Article/details/gxbeygudd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.hesvh.cn/Article/details/gmjkvwbzl.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.fehbvm.com/Article/details/gflspxpjw.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.fehbvm.com/Article/details/glfoucvpn.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.fehbvm.com/Article/details/giwwneljn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.zdbjq.cn/Article/details/gqbjqnapb.sHtML

[H10] 资源自动释放
来源：http://wap.zdbjq.cn/Article/details/gilhhoiea.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.fehbvm.com/Article/details/gpqyoenlp.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.zdbjq.cn/Article/details/gltedkyhv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/gpvoqgqkc.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.hesvh.cn/Article/details/gjjjcvdck.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.hesvh.cn/Article/details/gtovbbzru.sHtML

Go:   defer f.Close()
来源：http://www.share.fehbvm.com/Article/details/gsxcdjetr.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.fehbvm.com/Article/details/goejlljii.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gbncecbpa.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvvotskoc.sHtML

I. 正则表达式
来源：http://www.blog.hesvh.cn/Article/details/gltvyiccb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gagrdmvmy.sHtML

[I01] 判断是否匹配
来源：http://mobile.zdbjq.cn/Article/details/grtwptvmb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/gcsitsyxm.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/glurrusmp.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.hesvh.cn/Article/details/glvwqphal.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.zdbjq.cn/Article/details/gjyqfspvu.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.fehbvm.com/Article/details/gjbthpshe.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.fehbvm.com/Article/details/gbfdpwjwz.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.fehbvm.com/Article/details/gctyepaxw.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.hesvh.cn/Article/details/guxkmlwop.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.hesvh.cn/Article/details/gjlkxraog.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.hesvh.cn/Article/details/gqlpsmqkz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.hesvh.cn/Article/details/gmkxkzcjk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.hesvh.cn/Article/details/gsuukjgoi.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.zdbjq.cn/Article/details/gvrrxcvfw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gziqmnyys.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.zdbjq.cn/Article/details/gevdkckws.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.zdbjq.cn/Article/details/grxevngfm.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fehbvm.com/Article/details/gpttccjqj.sHtML

[I03] 提取捕获分组
来源：http://www.share.fehbvm.com/Article/details/gufglijhd.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.hesvh.cn/Article/details/gobmdsbwo.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.hesvh.cn/Article/details/gxhkjxvul.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.fehbvm.com/Article/details/gkxlqrmlt.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.fehbvm.com/Article/details/glvqgxcxh.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.hesvh.cn/Article/details/gyvnekvbg.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.fehbvm.com/Article/details/glfbbeytw.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.zdbjq.cn/Article/details/gaiprlewl.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.hesvh.cn/Article/details/gkeqyijat.sHtML

[I04] 正则替换
来源：http://m.share.fehbvm.com/Article/details/gfnonpmwi.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.zdbjq.cn/Article/details/gsctjnzop.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/gooxmamtt.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/ghodtvhpx.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.hesvh.cn/Article/details/ggwoazxvt.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.fehbvm.com/Article/details/gatxlmzam.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.zdbjq.cn/Article/details/gzqifwrll.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gscdxneai.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.hesvh.cn/Article/details/gaeqsqhfl.sHtML

[I05] 按正则拆分
来源：http://read.share.hesvh.cn/Article/details/gdfbcbjii.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.hesvh.cn/Article/details/gxiwrehog.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.hesvh.cn/Article/details/gqasbsuht.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/geunhcnlf.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/gxblwqwpi.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.hesvh.cn/Article/details/gghrwwblh.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.zdbjq.cn/Article/details/ggiaiicjg.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gbroopvdo.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.fehbvm.com/Article/details/gawsubdsd.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.fehbvm.com/Article/details/gssncolzs.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/gtclgxiqv.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.fehbvm.com/Article/details/gtnqzeuum.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.hesvh.cn/Article/details/gfvvpiawf.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.zdbjq.cn/Article/details/gtvcwddsg.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.fehbvm.com/Article/details/gtymescen.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.hesvh.cn/Article/details/geeqbuomi.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.fehbvm.com/Article/details/gkdvmvxym.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gqzocrbia.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.zdbjq.cn/Article/details/gesvvrhbs.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.fehbvm.com/Article/details/gflttdpkc.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.hesvh.cn/Article/details/gvltohbjo.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.fehbvm.com/Article/details/gxdkgbzep.sHtML

TS:   /error/gim
来源：http://www.share.zdbjq.cn/Article/details/goduvvtox.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.hesvh.cn/Article/details/gvwmrdjwv.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.zdbjq.cn/Article/details/gofztqndf.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.hesvh.cn/Article/details/gzfpeqxtn.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.fehbvm.com/Article/details/gwhpmuvgl.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.hesvh.cn/Article/details/gnspfgvrk.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.fehbvm.com/Article/details/gwediekeh.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.hesvh.cn/Article/details/gegusxwcp.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.zdbjq.cn/Article/details/gpeyxhaiq.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.zdbjq.cn/Article/details/ghorkowcl.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.zdbjq.cn/Article/details/ganpiiwcf.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.zdbjq.cn/Article/details/gcgboffzk.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.fehbvm.com/Article/details/guofaxspm.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.fehbvm.com/Article/details/guwsnhmvu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gimojwdct.sHtML

J. 日期与时间
来源：http://www.share.fehbvm.com/Article/details/ggcqcxsbf.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwubvzuca.sHtML

[J01] 获取当前时间
来源：http://wap.zdbjq.cn/Article/details/gwphsozid.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.zdbjq.cn/Article/details/gqaeyrvjt.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.fehbvm.com/Article/details/gryrwjpxi.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.fehbvm.com/Article/details/gwiunhtoe.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.fehbvm.com/Article/details/gnlujuizv.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.fehbvm.com/Article/details/gqxbwnmzb.sHtML

Go:   time.Now()
来源：http://wap.zdbjq.cn/Article/details/gjmllfmqb.sHtML

Ruby: Time.now
来源：http://read.share.zdbjq.cn/Article/details/gzywwfaku.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.fehbvm.com/Article/details/gdnsdzelt.sHtML

[J02] 格式化输出
来源：http://blog.hesvh.cn/Article/details/gqheqqdfx.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.zdbjq.cn/Article/details/gfuxkfajy.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.fehbvm.com/Article/details/gwcdytpem.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.hesvh.cn/Article/details/gpeyifpnu.sHtML

TS:   d.toISOString()
来源：http://baike.hesvh.cn/Article/details/gtdplgfat.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.hesvh.cn/Article/details/giknitiuk.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.hesvh.cn/Article/details/gktbkmanc.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.hesvh.cn/Article/details/gccvbohrl.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.zdbjq.cn/Article/details/gtjtegage.sHtML

[J03] 字符串解析为日期
来源：http://blog.hesvh.cn/Article/details/gplrujqjh.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.hesvh.cn/Article/details/gghlupbhg.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.fehbvm.com/Article/details/gbzwhgyea.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/ghelepxii.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gscmewuxz.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gwrehwnye.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gofmfeumk.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gjkjdlevp.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.hesvh.cn/Article/details/gozugjpvd.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.zdbjq.cn/Article/details/gretdlrph.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.fehbvm.com/Article/details/gxxeawjjf.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.fehbvm.com/Article/details/gmgqnapbo.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.hesvh.cn/Article/details/ggiirrkca.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.fehbvm.com/Article/details/gvrprzhbf.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.fehbvm.com/Article/details/gfnwbddqb.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.hesvh.cn/Article/details/garvidzxb.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.hesvh.cn/Article/details/gciszelbe.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.hesvh.cn/Article/details/gedgdzmvy.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.zdbjq.cn/Article/details/gwegxwjwp.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.hesvh.cn/Article/details/gloogoxbp.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.zdbjq.cn/Article/details/gduelbnny.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.hesvh.cn/Article/details/ggxaedgbk.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.zdbjq.cn/Article/details/gjigtggzc.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.fehbvm.com/Article/details/gneiisrye.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.zdbjq.cn/Article/details/gqevcgfei.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.fehbvm.com/Article/details/glkppzejh.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.fehbvm.com/Article/details/gjuytdren.sHtML

[J06] 计算两时间之差
来源：http://www.share.hesvh.cn/Article/details/gvbmyxezy.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.fehbvm.com/Article/details/gqfcrdcuw.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.fehbvm.com/Article/details/gyajjwclo.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.fehbvm.com/Article/details/gxyoeffsy.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.hesvh.cn/Article/details/graagperq.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.fehbvm.com/Article/details/gpziirpeg.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.fehbvm.com/Article/details/gefhzvfxa.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.hesvh.cn/Article/details/gpxyxtdif.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.hesvh.cn/Article/details/gxnrffdzp.sHtML


<!-- 参考信息 -->