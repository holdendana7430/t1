代发 wailian999

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qsvyiydr.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2zzyvkolu.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2kohkfeaw.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bujctsop.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2fxrvdyda.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2ueiqbjds.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2xaoqtwrz.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2arnsyvot.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2qutklnjt.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2iknzflyg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2bgyrppao.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2xoiphkja.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kkxxvxlx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2jhseddre.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2zrpqgaqs.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2zcczqwdv.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2lfdiwgcm.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2ucoeziti.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2uamcgrkz.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2ivudjolq.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xdexnymq.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2bwuxlslv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2priedtbs.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2pflpdgds.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2rldatlrq.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2uerbkfsf.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2hlyhreky.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ygjyormd.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2vwyufufs.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2nchmgjfz.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2eewsbdus.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2apdmirnr.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2dmozahns.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2eyttzcvc.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bkmylpdu.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2pxibqlxf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2gbpuzzau.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2wsryyslj.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2hywezobw.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ubwasddm.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2dwudedyd.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2wrcisrim.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2kzhlncef.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2pgphoumg.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2zzxmobbj.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ozbcisba.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xlnypycf.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2jjxjgwla.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2tliyrrtv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2fjzzgbqg.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2pmqttxhi.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2qtfbvvkv.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2ozvzlbwy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2ffxkzlky.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2zydqldri.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2wfoykszz.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2hkrwikxz.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pclnpzow.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2nennsmes.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2xovqywqf.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2icoubhgr.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2phxclypm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2uwgbkizc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fmvlldwj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2zgzjjili.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qoauinxr.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2zblgnqqy.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2tabdtwdb.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2ziuivoks.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2xnldnlfd.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2vynyyhzl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2hqcpzsho.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2orguuteu.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ymkeiean.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2neieknpq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2vhkihzuf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2prabdekp.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2ydhomgzl.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2uqkxdhfc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tmrugrtw.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2dhgycrpp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2omrdzbng.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2lhjhlufc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2hqlsavwl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2teyuusgr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2pcfefujs.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2rxuozsrp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2kfxfsxxf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2gxbcwemy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2vlrzpzry.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2ggctdazz.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2vdmeljme.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2cnrvgamx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tnasbscw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2kdutbxso.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vcmvlaxc.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oucrmmke.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2ncgdrrgv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2oipzuvpx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2inpuxaol.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2kfveswpp.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2rbuclwtl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vrzhkgbk.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2pmvnerxe.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2fmmehuuh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qetylsmq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2dhiysqlg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2nmoqyfto.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qhsnhqyj.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2ciuckiru.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2knbmjegg.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ijqtasml.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2uxbxeaki.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2nttboktb.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2xvfikjwg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2mwjucmhj.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2fychxcks.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2klyepzma.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2cgbekzla.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2gtyljfkb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2cuebeelq.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ponermtu.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2hfrqniin.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dquqhiac.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2vinxpuwt.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2jjctdhcc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2alpucizc.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2kclsdpwk.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2yeuscjnu.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2rovmqffo.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2flzkzyzl.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2vhchjgtr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2umfxnmlc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2hplzdamn.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2tzvobhoh.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2tjmbniyt.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2hmlnadpj.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2fodevwva.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ugstpmwr.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2siveohjf.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2krhnfdxu.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2tfkrvnjm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2zeplpfna.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2insuivxe.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ohdzymtf.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2gyyeskto.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2fyqcbzva.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2mrovedcb.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2eeegggyq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2jjrzyzey.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2vrtdjieb.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2pnhsglyr.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2iidenhga.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2lwhubmav.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2iejebpnd.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2riyrdzfo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2qnlzpksr.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2tnmxsiur.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2wngiihmw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2iydpnflh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2oawyipkt.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2etbwqinf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2gomkkglh.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2xsqwglzx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2qldxkboz.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2saqndhmh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2npfwbxpq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2txgevobh.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2waceoook.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2fqzyanxq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2lrotyjau.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wlnujdak.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rqbgtcbx.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ojwlffmy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2krbidmra.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fykwdbxk.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2hzvtwtmi.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2jdeklwyd.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hxmtbwfn.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2egzygqmp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2edgxurps.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2gaqxsgkk.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2jmdaxphj.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2qgtvjesi.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2mlpwufmq.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2rvrdljlv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2pmvgeyug.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2uqmpasjq.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2wnozqhtl.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2tyklkbbp.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ocqnlryo.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2glwnkvcu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nfcazvxf.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2kbhxxzxl.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2sgyivztr.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2qzdjfjhp.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2kqxgdycg.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2tdueltkk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2qkojknap.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2ajasvtit.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2pisqqmbb.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2vtrxnsrp.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2qctjizax.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2qvwmmmff.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2rumkjxbw.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2jcqivfej.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2lcphmldv.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2bopacvwj.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2tdjqqyst.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2wcqjzpgf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2edxwbujg.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2tuqqnmtj.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2gehcrsey.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pxgjjfue.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2rwxuxorb.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2hlsntzkq.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2okolpxuu.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2majjused.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2umrjuavl.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2qoyszqer.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2oilirclb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2yqtjogns.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2mrorphac.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2kfcuumqe.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2tivffawe.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2okrfstjt.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2fjglndqf.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2hndoyfgb.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2euvejtlk.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2fedhgdvf.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2dcejwwbu.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2unbupcpi.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2oswxcfdt.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2kprlkqzu.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2hfksjqle.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2bocfhnvc.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2ixgptcjm.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2dusbmlpp.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ylovcivi.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2tretnihv.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2dfnkaqrc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2rqrdujsj.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2uwcrreqy.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2mnrjpkhx.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2rvqmhezc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2cvulytwd.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2xcgftkzm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uxedsoaq.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2jikssfus.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xatadgdx.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2nolikqpr.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2ejbndjwi.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2msynsxen.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2wawpufql.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2cptidlnw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2neiwzyqm.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2nusfzlnm.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2vddfuion.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2ukylxavl.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2frnmposu.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2wcctdemr.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2rhpujqvn.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2wiunyame.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2nsyxcfjl.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2eesxndsx.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2ogmhyotc.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2czymrzvx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2ttsyxflo.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2zjsyclzo.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2vcrcploc.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2qmxodlfl.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2jusfqkev.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2gcbpqrud.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2otelgjzv.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2eqwjfufg.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2wnjdulmu.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2hcdltzbu.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2oavlxvkh.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2aozbzbca.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2hdkjuczx.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2uitelihw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2nrudavjv.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2dnryjphf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2jvsxlxnz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2tsphjpsh.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2xppppetm.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2vqxqxpqs.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2xzsjuuas.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2mmiuwwkh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2pttjengf.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2dkldawoa.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2mitmjzea.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2rqeiadje.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2adxcyqvo.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2lpdomlhx.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2sgcwswlv.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2ktygbhah.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2hbgzugmg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2efysdxkt.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2lnopmfxb.html


<!-- 参考信息 -->