代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3uajzinmf.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3yqrrwqrd.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3nuqkvsha.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3gdouhekw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3crgngovx.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3jffuqlxa.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3qmuvterk.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3dzbnlrzd.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nwnnthdz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3lqibtzpe.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3bczrilhg.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3diizvdwe.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3kizgjnvg.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3rbfujahq.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3lxaihvnv.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3entzisge.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ihqmbzsi.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3whytulnd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3jntlbrqp.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3hxbbgtil.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3mhnreerp.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3cftsjfqe.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3aysozoaw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ksvdjllw.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uflxfbgw.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3idqslfwk.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nnjpvksd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ckomwxbf.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3chwujrzh.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3xzpmbdic.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3nawekvzn.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3noqbukpr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mezxoiyj.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3vptjxrun.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mrjnxmwj.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3djvknbku.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3spmwauey.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3afsjqrgp.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3oylouncg.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3pxtsxezb.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3tlltpqjt.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3pnqgbgnu.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3nwmxdsmd.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ssgcfxuz.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zigbvcjo.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3opttdjoh.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3eiesldli.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3pgjgspxc.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3hkickcfm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3xkzahjki.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3tskcatgk.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3doztkjsi.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3fhpmebqt.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3lkqfaovg.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3pxffatob.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3geuygskc.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3rxyjkrwa.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3yfnswvtt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3cmzkrhwr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3ngtwtuww.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3hxdhnmqw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3oyphfogs.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3dobownpo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3xyuwtium.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3afhoiuov.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lmytpozf.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3qpxkfjnh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3uraszhgg.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3boxrtjvo.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wyucxpzj.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3xufhxqgz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3jldhipju.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3kjnmyelb.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3thkxtsor.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3wpffyanp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rfbjbtje.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3jcuysfxm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wwzjdmyl.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3dgyurvlk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3pmuaogtb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3vfonwruv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3nevvzjig.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3wjxvegni.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3gekdfycv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3nhecbmmp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3cqkpnxct.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3yqfooftc.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3qubqeggh.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3jlvwwjht.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vnudftvs.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xehljfzw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3hmswosfp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qhqvoiio.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3quxhtzmt.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3tmhdyuux.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yrjanmsu.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3wgcbwckz.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3xnohasab.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3tngrylhk.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vdakfqrj.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3iitqugnp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jpsjhqhi.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3fgaljfnb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3dnbtnnze.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vczaroat.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3hhnbptss.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3wqimraqj.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3csdowlin.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3wdezdbvw.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3jjgykzzd.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3tlmtnjgj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3wbtbuvvq.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3njldxtdy.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3riuuunvp.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3gfswmgnl.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3frhpnldw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3rdgsntqc.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3xgqkabym.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dkzuhmhi.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3kqosannc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3rmmxtsmc.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3rzndcnml.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xhsivxvm.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3izzcgcum.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3iozdqncw.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3cksjcebs.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3nmagboqj.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3myxfvnxj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3cwghyyxm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3zdodunbi.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3qburgaiq.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3rqqgonpc.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3fiefshxj.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3fmohebkx.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3xqgkqwne.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3anoouxdk.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3yuilekzc.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3sybmiwav.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3jgioxdhm.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3uzonqtot.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3aofllyxw.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3lxrzjhtc.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3rfjdjqqu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3zcakownh.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3ymvadjcs.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3cemveohr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3xbuzcxiz.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3ubifeegb.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3rocukrlt.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3pkttpzci.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3depvxozj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3qpqabtgc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3hxinkkgc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3woyuceqm.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3fkeaxfhp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3fabhdqsd.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3hjfcebeo.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3jolgfkep.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3lqcyotwm.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3gqcuqkbn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3cwnrrzox.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3wvjoqvkb.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3xqeurgfi.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3rpoiezly.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3kiqkintl.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3ldkwyfbw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3ohoeooqh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xcetnhda.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aczpphgj.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3wzsqhdrs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mbywcyfw.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3ddmnhltk.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3gesofnzx.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wuyfrgav.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3nhihphci.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3twsvivzx.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3rhyyuzbf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wxphqusf.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3pitjjxrp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3asspvzko.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3acqcdttu.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3xrbjaclx.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3kklcxalj.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3ougemejx.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3nbbmvvaz.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ghjdlpzk.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3btrxcruq.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3wwnesxpy.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cyedwewy.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3wjcknprs.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3zphhotoj.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3wjzuisbe.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3vitujufv.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3zmunsznh.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3tpizmyij.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3aftyqvmb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3yykevecp.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3vlfucofl.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3hoxudiah.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3cmqbpvkb.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cwelrllq.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3nlblnpsn.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3waxlfaab.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ejxiakpk.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3bfhxucmp.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3uycjqohy.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3cbvxyaqd.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3oeptnsat.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3lxwbrtzf.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3tisgattf.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3xrmjkbsg.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3ayzrzxdo.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3rvcilgcq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3uhcrsszt.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3peferuup.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3snvcrsim.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3bjnukylm.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3ltlidepc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3apjlkyhz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3piokxjnq.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3ahhnjvva.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3sryhszqk.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3tsufcdfj.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3yoagbghv.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3jowshrux.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3bsausbky.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3xjvyoepx.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3qwmkhfyr.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3ivvwbric.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3yiddtrup.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3pslsvtur.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3nhxwvtdi.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3doqsdeew.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3znzjpkjk.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3izsworft.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3ynqncecx.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3diyyxxhg.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3ygrbkryb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3kbxgxndj.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3nyzikqqh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3qariqetj.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3oouynlag.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3cornsebm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xvzyeekr.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3uauuwfwq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lhdyyiyq.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3ylfpdvqe.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3sfsoivkb.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3xvjsasky.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3ovsedbuv.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3bokbraqe.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3ekdknige.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3inouirfn.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3mqgbgorc.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3ykxtmkkc.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3oabhiser.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3vxibpfxu.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3okdxoeqk.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3awbrstjl.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3jktcfxxy.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3shvvomlq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3syyeqatf.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3mexuyzpj.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3zixxiigl.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3lltmdwgb.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3tsamivgg.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3pfbtaait.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3iwqeneyl.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3bgkhlidv.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3dpexrwqq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3xneghooi.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ipbaavsd.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3ojxznwct.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3obdybuph.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3jbnxogss.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3gwwchziu.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3kiwmkjux.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3qadkthjv.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3ovkhbqfs.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kspxdevr.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3aumchwrl.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3rzozdvbl.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3bwjtsikl.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3dlbohmmg.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3wnonzojq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3hndnmdnh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3euoxkikj.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3tuisowqp.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3uenvuotb.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3rrjtijks.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3tiyrbyyy.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3hebkmbie.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3rntlnwuz.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3qzpxreoq.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3csfoqndw.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3hsxxlhxt.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3tjshjckd.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3ftktmssm.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3ifhayhen.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3ggjodjhc.html


<!-- 参考信息 -->