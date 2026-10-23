代发 wailian999

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3ozbyhruc.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3fgakwrpp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3rnueezvo.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3fthfucfp.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3nosvmkjs.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3iyfxzuwd.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3idzyhony.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3lfmgouax.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3egqdmbbd.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3htbwnspm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3cuqvjcno.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3qcvdvecw.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3pxoekhoz.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3hyjsryde.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3wujbpmec.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ftaxukge.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3kcjqoofh.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aytkpxcj.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rrlmgqle.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ufaiarlg.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3isdaofwc.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3vsudnkli.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mpespmbv.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3worpuwso.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3dkbsuodn.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dgelcfoh.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3urydscby.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3upnicygd.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3qpqknljj.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3myzjszli.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3xkvuogqp.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3qaqmxphm.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3kemeljbq.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3tvqulicj.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3pilxwywg.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hpqyquhg.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wihbtabe.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3fcylrgdy.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3mbqclaai.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3xiutaqiw.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3zgibupqe.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3wwwjxnyp.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3rihkcorb.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3hyuaauix.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3anjeqqxa.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3mbilpxvb.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3hxuywvxe.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3hyaptjep.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3gftpzeqk.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3mozzdbsx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3knpuecuc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eilnkqnm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3kvlmhqtt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jfxijfsl.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3elzhxbyd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3tfoeyiir.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3liumejxy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3hoqpjmff.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3ffcpgqyr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3njbtrldo.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3ruxuboqk.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3luldswrr.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fbhvncdg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3jjqywrhd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3dgdwgeca.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3lyruwsen.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3abzdtcyy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3atboqbit.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3inhliznx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yennulze.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3rnttyjgh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3dhgqftkr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3wlijqcko.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3wqxhnbbw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3yrqcjvrx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3sfrdpmjg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3srqobkvi.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3emysiabu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3iqzhufsw.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3wthsprwq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3tbxcbseh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ewgdcvut.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jrwmsogh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jtvrmlce.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3eucrwnhc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3jsxaypqb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3jmlklmcr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3iwegkxuj.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3uocueynq.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3wshitbec.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3tivotqdr.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3fzajqeje.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vwkgemgy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3orlsyxnh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3sxcwxmhs.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3npvemoei.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3livstdnk.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3mvudvwfh.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3tddbokcx.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3btlcgjkm.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3emrpflbt.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3nlhwupxd.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3vyaoheaz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3cnneyyqm.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3vqqaepmw.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3iidrhsgd.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3hsjwjdvz.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3iqacdqsh.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3dlyqupun.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nddqfyah.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3pkgdwzsc.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3lkqqorkb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3nquwyvxa.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3gkkwtkvs.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3jrhfkwul.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3dqmnhynq.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3nbhfbzhp.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3elbnpjfw.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3axbldxvb.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3pbsglsrm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3xvikrsyp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3xwgkvvdk.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3ayvoecuw.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3swxpshqv.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3szlsvkzp.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3pcbfawww.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fdagbhtz.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3czbxepzd.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ttzfgmam.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3spytgzvb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3iiqyrssx.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3rwtxgdiu.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3yaenzznp.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3huqkyysi.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3pacbmapg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3pjpzkxtw.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3khswmcev.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3daumjugo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3dmpcpcab.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3nbynmiwp.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3xqxedwpx.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3wohmprmz.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3uxlwwfrg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3vaphylyg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3xpagmhkw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3pjxtdedn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3rbvhrroi.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3jbevslmk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ubitxeuu.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3xqudqezm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3bjtlzirc.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3epqifimn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3jghgiqlh.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3smynygma.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3lvipaiiv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3ktjyjjil.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3ffnabncc.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3ewzkbwku.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3kvoshogh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sdtjrkpy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nnatsocg.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xdiwmfth.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3trepfvwa.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3ysemimho.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3wdxdvwut.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hckmfwnw.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ayxvwleh.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3srgiwfdu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3mamucyml.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rqfyegtx.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3nijbwwjk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3xizcuchr.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3jxkrbqtp.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3xsdzczbs.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3jpugypyr.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3xnnqbiyo.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3afhbmtut.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3snistvgu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3hsoghtzz.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3hdgxlaqv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3fcwtgwzk.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3tnfhgzld.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3yqzctjhi.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3ygiypgxs.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3ymftyzov.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3rueokrog.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3fupwikmt.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3vbyshcaq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3lfnpftbw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3sqqeugfm.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3urkkdqbh.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3cignkxjs.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3hsgrrrlc.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3tiilfxfu.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3fxwybuwi.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3cjirgola.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3aszarmlp.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3nlfhbkps.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3omemvkgd.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3lpdnuosc.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3jvhbxihd.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ykqnjprz.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3smmcrzvk.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3nlajictp.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3lpfsistb.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3tietqidx.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3rlxeeovj.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3eeywerih.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3zfttkhyx.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3pvthketl.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3jdfdzcnn.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3hifnigpx.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3kccjqqmt.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3efznyhrv.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3bptlukua.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3wlfbmtoo.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3sldyuadb.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3wwimfjiy.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3agvvatpk.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3ecblxumi.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3zdqdyvmm.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3shkalenx.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3gpebjzxp.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3fawxgbmi.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3tcrrdzln.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3mitfzksw.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3amspcvqd.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3xiyyrxgr.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3fytqiibj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3rkwugjcm.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3pdcqoqpn.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3vcwxkobn.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3fnzdrbmk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3mdgiqjhx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3uytpazru.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pknsnjzb.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3nfzyudeo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mbtzatqj.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3edmqoafh.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3lqtgnwji.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3qmmkslad.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3oynbnbbk.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3ihzzlxol.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3jwdqjmwd.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3eadqzodh.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3uwpicjrf.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3cxhylclz.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3boainitq.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3xkkrgrhh.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3qupwtxtt.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3qakdwisr.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3oapqspia.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3rfqknibg.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3hfctusix.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3maghgkhk.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3khtuugru.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3rqqcvfms.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3fupbtabs.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3fczydaee.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3posstwff.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3zpqdrouz.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3udmhfrvh.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3iyqgkeoc.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3kfsoxicq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3aobsufqp.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3qrkqkpyy.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3wmhfndfm.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3gmaptoze.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3ysampfln.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3nyzqtqsl.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3cmlvziic.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3seonkqvr.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3yppnfxvi.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3yplupvzh.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3iqoldkdv.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3xfhnqoxk.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3sdupwhcz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3rcemarpk.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3fsldfblh.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3iqzxobkd.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3hiewsppl.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3ekablzsh.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3jncfuola.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3ckyqlxlp.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3kxligdjv.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3yxgfustn.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3mfsriyzq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3kxfnhoko.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3vszhpugu.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3nqbswbiq.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3yoqdypns.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3jqdrcrvu.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3phsocrap.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3sjiraqfi.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3sgitxteo.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3ymxdcggd.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3nyhcjpqt.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3xtqdtmza.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3csogtpwn.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3qnnhseho.html


<!-- 参考信息 -->