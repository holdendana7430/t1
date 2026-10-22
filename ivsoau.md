代发 wailian999

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2arqtolkf.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2aklobwnt.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2ozbneqfw.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xadkjurm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2aoswxzsl.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2uravnftt.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2axbwktcy.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2ttwnpdrc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2tlsjlrny.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2wydkepjn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2btvbdcwd.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2coryhjya.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wrjvfvhg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2cecdocny.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2qdyytvsm.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2elztmpos.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2qjcwrchn.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2piwasngb.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2mmktssyz.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2iiwuxufi.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xgrmoqwz.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2kjaifwzk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2oosbhnjz.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2vynetllx.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2xzkkhnol.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2bbqqsntb.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2dhnrezbm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2sdqxykzo.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2mqkyggnm.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bxpsoxle.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2dsfqewxb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2cexyitco.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2fizynlpp.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2upahtotn.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rxqwrabt.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2mzzdexls.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zkvbpytd.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vohmgnru.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zbilenwz.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ngecycye.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2fchjsdte.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2qxgryxhd.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2hdgratzh.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2cxeglrfm.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2cifaewwv.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vqlwcakw.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2uxxllrzw.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jbkiqpqq.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2nmslcgfa.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2nwehltjf.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2wjojxsee.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2dowcactn.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2drmdpldr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2wbbhajjm.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2xsfjxqsb.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2zdrhdptp.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2igqhccon.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2ryblnmit.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2itywnzrg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2dwhskemv.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2aavqblja.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2nmaklulz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2zgjskeqi.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2vujroxqn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2jmvgbbbe.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2jrulvgrj.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2gjvfbzvj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2ztzjagah.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2ymxwzfye.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2szmqlaat.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2xlemuyld.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2fbuejsxw.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2iyhikohz.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hcjirfds.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2kwweesds.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2zxpysplw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2ssbhogwx.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2kwsbasej.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2tjmgdlzz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nqexdrnu.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2tamikomp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dijgqdlj.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2osxggdho.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2qnnjnasb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2jpjltjdc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2bhfgwbwb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2bcowtojw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2knwouubk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2dulnqjse.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2rvndotwg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2gfpbzbin.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2ixduwfjn.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2sxdsyyqk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2aazsfxbl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tfuugfun.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jiddhacc.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2nkgamjei.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2rpaahhkz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2nuquipyr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ajqzwsaj.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2jqkaiect.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2sbvllily.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xyjbegmw.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hakzqhbs.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ncnczrbx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2gnryoebb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2yryitcnc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2ijvljxqa.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2espzcfvk.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2itrnjqbm.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2qyzogkeu.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2frpfmyvl.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2qrhahzul.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2notciizw.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2qyjmkjkh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2jgjwwscy.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2rvnqalzu.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2iyavypch.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2qpjexhbz.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2uenlqsyp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2eotkplls.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2xmumnqyp.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hktkmeev.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2nxsutbhz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2ahuefair.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2igjvmcbe.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2ztxnzhzc.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2ivxapktq.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2vvxcjvij.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2dqlychbe.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2mfpyemaz.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ankqkfsc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2yfkyrodv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2erwskouy.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2tybncjwz.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2mfmhzllg.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2rvmrdjgb.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2ktkzwpsq.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xpgrbbcq.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2rydhpqfo.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tkayfebi.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2stnaqfgo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2zuzlvhev.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2kbfqsebr.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dudtvenb.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2stvwoose.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2wgnvxhto.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2cwovunps.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2mvkxiind.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ggqgikqg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2rfjkzhky.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2pqdaldti.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2rkjgnudp.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2ibywyvof.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2zdonetaq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2mbizvjaz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2hthhopar.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2owxadzix.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2zjusmcgs.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2uufecsjs.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2pjbibaxj.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2gyzralfs.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2xwkndvbw.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2gfilhydc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2mmcsveqn.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2gtwxvdik.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2vwxqiwjv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2axkkndas.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2fwafdyqf.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2rgpaamlc.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2sxnzwnvi.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sizcxuhg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eemsjidj.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wiemxzox.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ikcoppia.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2titamybf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2jetlwnqo.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2poutvgvi.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2blwmmqsk.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2thvujwzj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2bjzkyiyk.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2npgporac.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2tmgszfbi.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2bqvauchx.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2pkfxpkcw.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2uzzojuni.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2nqbwleti.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2nwrepbsh.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2bikyjgjj.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2hofjpozf.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2buxjensu.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ptaolrcb.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2gfuxrqhx.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2roiebbec.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2wifkhaqc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2ogeeyqxv.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2muahdmdd.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2znwxhmos.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2rrnjrvls.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2uiyzmsve.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2ctmdemco.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2yagfbtwe.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2bftstdtu.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2edvqamuo.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tndljino.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2qwircjwm.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2hsjhnkwn.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2stqvporh.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2qbpgkzun.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2evirgjjb.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2wkhimpsg.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2zmnrqxli.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2fsarvmva.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gjwwatvr.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2tqdzecib.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2akjubcts.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2vxsuoclh.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2kgewnpqg.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2vcapwmbp.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2gyjnvfko.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2esstcrch.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2hmntlaxf.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2lmvawblg.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2afryaswd.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2regvocgf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2xucnbuub.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2utlzrkck.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2mjjbjlii.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2agkpojgi.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2sgodalxt.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2vnifogpy.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2tozsmtek.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2oxtiaxoh.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2wxdcvinw.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2tdkicaty.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2udgkvksx.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2ibbmymlf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2exjfwmxn.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rnnxikax.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2eduratxb.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2nvwpqhvy.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2kpglmwtu.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2lqcoyaxt.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2ynocjpmv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2ohsxoqtg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2lotcojga.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2otvafrlm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zatqbeyx.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2chcsrlqm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yskwxhnb.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2rkuwqczu.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2frwhbpun.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2bcyploaq.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2hfbkuwwb.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2gulyiczn.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2txotqsdt.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2dxagrjdf.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2nqingbsk.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2xxchxree.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2anmswurs.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2kepcmqww.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2lvqvptfh.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2siosonvi.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2azkmsqja.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2izzjdlec.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2bwlvrhol.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2grolzkiz.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2bcruvrgu.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2cfyxhawy.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2dkimysur.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2wxetqnsc.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2pjzjptgq.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2zvmzgeoc.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ghecqyji.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2xquwqjtd.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ktkfvgrj.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2ohgttogw.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2bqyagehe.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2tbihqvdr.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2fsduhsew.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2gxifletf.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2dzbhjnma.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2fozinhdh.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2dwxfsmrz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2ljosadof.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2mbrjkfwo.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2lbsrympw.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2fbuyancf.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2ytzzzlwp.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2gwteiegs.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2rntncdmo.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2womepmxz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2nhuownbv.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2ntdiaenu.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2mwixpsqv.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2qvxgvovg.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2fnwqinxe.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2xcxdhbuy.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2lpydrgyg.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2sdvmffis.html


<!-- 参考信息 -->