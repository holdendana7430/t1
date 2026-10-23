代发 wailian999

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3wlwxrdlt.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3dgmakbpu.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3gkpmvkvh.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hyculalm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3tyqifnpy.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3lepvakmb.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3sgwqymwi.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3bnelkqxv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3gmnzftow.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3oarovvfu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3hjeyzmur.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3noncrnyf.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3eufkhnzv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3itvpnhyj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3ldekyzph.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rdlijlzo.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3aczqbbsy.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3bdmteicl.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3nqvkkzdt.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3bcwmfzab.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3afulgwna.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3hrhnjrdd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3pcjmtwiw.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ndhvxqwe.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3oyvsykkq.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3gdlffumc.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3nwdjvbcw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgrkgjct.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kepkmizh.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bimgkozd.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3mivymoie.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3dqxmozcv.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3lkhvyjbt.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3qgzydzpd.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3vvldejtw.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3rlnfxzbs.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3dulkthze.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nnkmlhbr.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ltqzflmp.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hdgeajqj.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3fwlrdkzg.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3nrusknpx.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ykdiisxm.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3fxuocpxs.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3zfwsawxg.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fmnzgjyn.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3eeaenhss.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ubytpnxv.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3yulfqpza.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3ebaiawcs.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3emicratk.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3prdyklpq.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3qvstgyfc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3vxrisenx.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3upxwvaqp.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3zhcamfza.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3sxxybwfp.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lvbumofk.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3jxhloxui.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3kiqernle.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3nkwhrehr.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3qnqeqarn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3qfeapaxj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3jocwvsvj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3uscapvsq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3wypepjxy.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3puiphrsv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3dvmcsuny.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3jaiiazun.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qxdmwsox.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3kqsipust.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3guozlezr.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3hmqcxgem.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qiiidwpn.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dcbptmnb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3uzzaazhm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3nsvumnla.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3gkvwohss.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3dyomumpu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aamujbmu.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3ttuyfxhv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cwyvzawn.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3hzuucuqa.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3sgoinkdn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3niidhcvq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3qyuficxt.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3nftjrugd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3yuvevwky.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3otkqzchm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3yrcaszeo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3wepsnhkf.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3ursdreaa.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3puvyaoqn.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3autvzelp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jfzeosmo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jimuktym.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cuhgxgly.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3ldpbdjtb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3qlshrmjb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ostdetmi.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3fklvlzgj.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3phdekmur.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3cyfpqxso.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3okliiqpl.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3souhwfxd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3kdkdixdv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3gtlsotqs.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3azpiubje.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3pbnvazkx.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3ghphppow.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3dxyceges.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3zpnzvttz.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3kzghisch.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3dcnlyrsa.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3krghskho.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3oxnutunn.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3fhrjqrqz.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3qjdkxidk.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3mgvibqfw.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3ikndxove.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3skpcmotm.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3nyzmovgg.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3iymbyocp.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3ohjkmxip.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3ddlcpvgs.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3gfpisumz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3szmdhfcl.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3auqwvwaq.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3buhnninf.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3drzwnteu.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3znhcwhwf.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3vwayyjtr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3phdaeurl.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3vkxaruum.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3mnougnub.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3zffsffcr.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3zoepeydh.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3ywtdxocc.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3piuterpu.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3trmjcnjd.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3frqxiqtu.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3iljwqvvx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3ixdqcsay.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3yhwivmnk.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3jcpiqeci.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3fulxhluf.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3spilanog.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3feloqfzb.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3ntluiaom.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3kwdkivwx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3avrbdgid.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3wewfnnxq.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3xtcnhvtu.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3hqxldptj.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3fcxdwfzw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3gnaaktqc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3vxydjjku.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3wzotzzqt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3zkfjrmgf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3przhasax.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3qfthevdx.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3eqnhemhr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3kdqfpwlp.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3meeoswxp.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3kgpmpcva.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3ezrebbjv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3jwagdxlm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3flbzwfjc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3piqhiyoh.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3cchnnxis.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3qxgfonmi.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ruhiyeut.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rhsxirra.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ivdgfzlm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nomnvfwr.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pymnwxxy.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3hytatjpg.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3texqtgmg.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3fcfzapve.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3itkesonc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3ckwyftoa.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zbjbpeiv.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3uauqonwu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3jxkpludk.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hddibgje.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3ormxbsen.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3uogubruf.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3gbfgfetq.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3lgmxbebi.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3mofzyqfo.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3grnvimho.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3ritrzelt.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3aitwfhjr.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3hdnylhxo.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3npeusaxm.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3dtguwpuj.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3jnbadmcn.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3dmjwdmwo.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3jkubqrav.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3fohumwfq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3fkjummtw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3hefzksim.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3vefkqcrk.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3oexudugd.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3bcpznjin.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3otfbavyt.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3tkxpqrge.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3aaxjhyzr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3iqgqzvir.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3nkawfdil.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3ohrbzcnp.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3ciqshmgz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3wlvqhiaa.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ziruzkbg.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3xbulteer.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3keqzwiyv.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3fbwqdnwp.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3kupwtavs.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3ywyndymq.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3rdktieqr.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3sgbqshwz.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3yvnduycj.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3mtjmoegc.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3lpqgnmox.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3kbsogmzg.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3dlunnlvd.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3avgqcffx.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3ibjtdejv.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3lkgorgid.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3qqlkbgbu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3hwotogmq.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3tnrsdjof.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3wwtfwccp.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3tffgtzlw.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3vgdgsvhs.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3lhvqfeiq.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3vmkezeeh.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3duixzpyv.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3vozidbzt.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3audxeimd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3ewedzoco.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3jajoafyj.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3dydlggci.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3ezbtoxhz.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3ysmlknwk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3rynbulih.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3qmgoicov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gvitbror.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3ybjmotsa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ktnbsfof.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3eywuhtkk.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3vlcnarpj.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3vhddcyif.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3sjdpuvzw.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3zoanytym.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3uqtvkxfl.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3tougolsm.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3blotxekk.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3suyyoppk.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3jymuzdnp.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3vjthbmtv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3zhahttlm.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3dzwixnir.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3dmbikdgk.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3nniajlge.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3hfrxgcba.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3uenudijo.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3harhswes.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3knqodtal.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3dscnxlwz.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3ydshkwtw.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3mwbtppza.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3wmfjpbll.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3fdqviuzk.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3tovfuiht.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3tpmagqaf.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3cprgdcmm.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3qttjlhxp.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3nocmngfe.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3thkwvcbm.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3ahixlthb.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3rvtaimst.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3jatchgco.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3lihtxkyl.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3nkykwqzw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3dblpraqb.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3snlgjehe.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3swobcbmu.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3txnrztqa.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3xyjozvzx.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3yzehomwg.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3isoyusrm.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ikhztdoj.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3qiypcnza.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3mokdtmvz.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3pjfzqvgj.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3jptokipt.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3qlizcqno.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3ffevqkwi.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3cigyfncz.html


<!-- 参考信息 -->