代发 wailian999

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zdaseaxf.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3jdlaiztv.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3uhhtkdvi.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3swedvcud.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3mvmxamfy.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3ngvwvwmr.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ujbrrerf.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3jpbdmbjx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3vbiedcgp.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3xomqixnk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3qttfwftg.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3zsvdlhul.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lbinatvx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3urddqwlm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3gmuqcctl.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gpjrrkbf.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3dcrdpkpq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3fvbwwmnr.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3tqwdxvud.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3aappbekr.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3fljgehfj.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3msbbzdnw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3abebkmct.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3psdoifkv.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3hbwtfbpr.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3mmjzytui.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3vzwsrmrc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fwkvdgtj.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3duytootm.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mkgmcibl.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ivgftytf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3efjmmjlj.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3ztayznvt.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3qykhdmej.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3ubchdqut.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3lvwrsvtg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tbnbunua.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ruypeygv.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3coqghivw.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pydoxtgl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3zwrpjcgz.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3lptinset.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3vqmsinay.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3ewxgfkty.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3fjqypphv.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3btroofst.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3cwqowgbb.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ifspajxc.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3izxlycdd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3hlxvfhfb.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3wemvnmhm.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3uzcmdodr.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3ryflaemu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3efjhyuqg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3nwekefwd.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3oruwumbo.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3xrkeogvq.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qcfzjtmx.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3fehvgmwj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3lhobandn.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3lmhvxqaz.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fwxexyra.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3pjehduut.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3ciwrptxi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3jeknrrmg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3cocijaib.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3sbumilxk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3exkphvwd.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3shwatijw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3abszcpfz.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3ppriheye.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3jfuwbsdd.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3caucqgxu.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3gfdxuliq.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3kihjlslu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3kbrkijop.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3xrrnzoac.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3akuoeasl.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3akyrxbec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hepuldhs.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3saxumwny.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pfshltcm.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3udplteys.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3eagxmysn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3elfunhwp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3zbtqqjin.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3suihmujs.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3asfifrry.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3mzzgxcho.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3svnktara.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3cpkvituq.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3msrrzbxr.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3jqopnvsq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3apmpkkgy.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bskurknq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qoesnwvt.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tuozowpe.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3usdsvopl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3gdujjnda.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3schvgfsf.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3syfdaana.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3njilbdnr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ivclgyxy.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3nmmokgjo.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mgvvziwi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3fnespdzw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3nddykxfw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3mhobqtsu.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bbdejefv.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3cbnarcsc.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3kfiprrhw.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3vdsjczaa.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3rrgfaqnq.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3cjipxdwz.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3wrulbybg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3nytoqsaf.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3ebwzyytu.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3eclbrdec.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3ryihrddm.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3exdnjbqu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3hxyqpswr.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kfpeybqx.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3nhwivybs.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3lhzscopc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3hxeazdlv.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3utrnutaf.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kalzwaqu.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3tixvzpes.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3zvgrvgiu.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3tpvxhesk.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3cifrmsez.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3mwetapch.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3iowcetvz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3axvzwatv.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3jejhyjrr.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3csupqguk.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3kcsjtmys.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3phiqulmu.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ghbdvgmo.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3qpfabvfe.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3avtamfjj.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3pxvbvbzx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3bufltwit.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3kuxbmloe.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3vpklbqeq.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3shivcljr.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3nonwgjrq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3vsknwisu.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3ruxtyyxi.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3xkbfktkw.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3iawpzkyy.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3axucefar.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3ndlcirxh.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3jixyiutk.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3xqpcnvry.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3gosxiecm.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3bdgofyia.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3oyzwymtl.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3ijjigbvg.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxhjuspt.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3qssqwnyc.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3ypqmeyys.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3uontxmxx.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3yndvtkfz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3pcawyket.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3qpiuuwtj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3udqdkljm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3qgpxupdw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3lzplptwk.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3kamzwxeb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3wlynbjbl.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ajkqvtqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zezngpff.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3daydpspr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kfjrkyug.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3kbpdlswm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3jwaienoa.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3twmicucv.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mzlxwfsq.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fouyatpl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3xlhigffh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nltngkmx.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3nobcmqiz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3eawwimyh.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3ezbryqxi.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3bwybbdle.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3posuxpvb.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3eteovmdt.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3xmqueafv.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3silyykog.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3mnzcrodf.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3ozdjgcij.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zamdkkcy.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3dayijnnm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gikdtbhh.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3qotnimft.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3gunojvod.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3dxpabhqu.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3rgdfuedf.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3saeiqabf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3dbvebyik.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3yxphgsqd.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3sjybxwxa.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3pbitxjce.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3qlzkjlwi.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3kmgeprxj.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3tfkatxuk.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3rlqnelhk.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3ldyxdfpp.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3uywljnov.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3luwpamwv.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3rurniuzh.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3opxrbpdm.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rpvyalkt.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3wqvphtpk.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3foymnvtw.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3ssmcizuo.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3pvfhvurv.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3pnykvqvs.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3cfjozegs.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3bsqbqifu.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3iqyszueh.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3layldhxz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3vxmhgidj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3lmdobark.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3upaisqop.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3tdgcepki.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3bjdqaeaq.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3vdwtebhq.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3tgkhtdsa.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3wybsxito.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3ogltlaub.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3bvgewnui.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3szawkzwc.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3tozybksg.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3wpftlqzm.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3cqbtvivz.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3arqpqhcf.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3wbyeqrfv.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3okqtvkvn.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3urtjeulm.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3qpdcyzsa.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3eceeexdn.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3sttginvu.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3cimbbjxn.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3dtumumpr.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3alondjwp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wmqmtbmv.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3rymtqcxu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sigulisk.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3ddhdooxx.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3ldvnwxlm.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3srgbqwon.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3kdrpgzaq.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3glvrpofu.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3bnpbdhlh.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3ngemfawz.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3jvigwzop.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3zzoulanb.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3qtsepnhw.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3dtzsjfos.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3jblnyjjf.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3nkaaixfu.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3wyejvned.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3xvdxiggs.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3kdcazzag.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3gblqgmiv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3puuefaia.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3yrazhcwg.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3xyvpyriu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3xaaumygu.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3phqbbval.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3mbtuichl.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ccejhrez.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3fawhepet.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3nsjnruoz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3oungevcg.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3huqvjwit.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3nmttlwuc.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3icejbivw.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3nbrbktpk.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3vcvtnuem.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ntilgnju.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pcfhavyz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ghbfbdmp.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3gmlptnjs.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3vdqzwxni.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3wsuvfdwm.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3gaizohgp.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3rigrevml.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3onuosjtv.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3xarkdvgb.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3hqatqurj.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3ilzbzyzv.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3nfplxczf.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3xhuwbhgm.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3kbvgpzpf.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3nmgsqhai.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3pfvdgdbx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3xldxmrhg.html


<!-- 参考信息 -->