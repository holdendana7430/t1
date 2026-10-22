代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2rxcznbiq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2pkoqogrj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2rfmkwene.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2edxiueiq.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2olyxmljl.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2xxvvwgqx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2ghiuhhwi.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2arufkapm.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2zsquxawm.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2ydbhpewv.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2hpnkdigc.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2mbmlxwmt.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2sqdqjayv.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2xsijcskn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2cctsnjwg.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2enaxmsps.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2bgvdsuzb.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2vobtjjrb.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2mmwlysoi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2huazkfbx.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sltgniin.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cagoxslf.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tcwpiekk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2vatlfjym.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2wsypsgtc.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2mkijngva.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2gcwprjja.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2rtwcpaix.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2kalngepx.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tmbtvnnj.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vrooalzy.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2racvgycm.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2nrswcjtm.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2mtuyvhvk.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2owwalnks.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2fnycvepd.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2fgvrkvrc.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ymiswrkf.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2dmbdnpal.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2nlejmems.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2uyuvupkb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2ewekmyju.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2nopdftnd.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2bxnsmmxr.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2dsbegpip.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2szchxzcc.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2bzoqwdin.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2sdbfflws.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2srwfhysb.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2jyljxfjb.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2eokjzxxq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2ljwbakwt.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2pbmldzge.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2rnhgqhaw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ggpzdwnd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2mrbruzwg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2msgokdqz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2nlbrfjgz.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2dwkogpah.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2yfnuvxiq.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2acvwhthb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2sbhyngal.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2niotdwei.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2ntkkckak.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2lmnhlvnr.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rcdehjwk.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2igsxvsmm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2xifuehpc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2pxdigvnp.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2hcpffhta.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2plpsymip.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dgahgxof.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2fwobzslp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jaltlmjf.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2wxblechf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2tyfznlxw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2agcaabmz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2yxxvpwcf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2rlcrxesc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2lkvdnjtd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2hlitoygn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2uqkzbxak.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2oevaoiqs.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2bnadpadl.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2kuwkielv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2gbycyrje.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2kpchkssu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2esxgfgzp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2yncvpbjo.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2anjatueo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2avsnmagf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qnjlowii.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2vsxcczkk.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2bhgfevgm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ufrjnrqc.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zhyotsag.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2bjymuwnd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2sktyjhrb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2xnvhgwyh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2optdmqhc.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2cxhhrery.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2ezxfjztf.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2yutbslcn.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2uukigilb.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2uonfolem.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2elglhgyw.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2jpwalyxd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2okgqtqjm.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2ewaaljme.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2hctfglwa.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2lfphlnob.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2odxvsxqe.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2erwwtiwv.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ljohukiy.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jjuvhlyf.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2xuwchjjo.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2lkzaftpk.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2mqtjmhgb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xurmfkod.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2fyuladga.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2vixfnsbd.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2bvuzkspt.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ezblzeyt.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2tjikcbta.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2pzweedqg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2qmakvmdw.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2cyorntpe.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2kgpkwtak.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2mpaolegv.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2fyhgqunp.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nuqkllgv.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xnrmhnpg.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vmirkmry.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2fnvpennd.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2danfemzy.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2vuentjci.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2lwlrkybg.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2bpekzrtv.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2voltqvrq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2scbsxqhp.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2xhgaxoeb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2hwupujlo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2tgdhebhq.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2hpxtvkof.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2xofeslvi.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2xwfsoejf.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2zkctiepz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2cnlowopu.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2dckifuau.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2ndccipay.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2jywgphae.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2bumcemkn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2xuoinvzq.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2yjxmhziw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2kfjqwoqy.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2qcnodepx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2tjglkbxp.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2crkwlise.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2luolycue.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2xkshegkm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2zmapwldx.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2ihtdxujb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2oipjqoro.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ldcuyexg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sogsqaef.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2gwbluoyw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2alnifwkf.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2shtfxorw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2clnmfrkx.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2kpnyymxn.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pdjzncpi.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2acvjmfcm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2hrksizbq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qsuurvwu.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2bimdtpyx.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2rufemcrw.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fmwunmbe.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2rkcpfvsj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2qgfjflbm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2lndswcct.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2sjwacttw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2kbfxcngz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2pyhkhzpl.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2jifdkjxb.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2cjlbeall.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2tdydnnsr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2epkwienc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2vegblmad.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2tgcqqlcy.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2doahotrt.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2sotwcqpg.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2mslhvzqd.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2eafnhwnx.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2kfilycoq.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2chsalzjb.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2fnusznqz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kuienrjj.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2gkofyvvt.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2huechboq.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2zdhbllrc.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2azzajani.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ebokvycp.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2iwannpbc.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2bcaipbmq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2lhjsfblo.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hikbtyuc.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2gsavlfmd.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2jsfjjgii.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2soqkmkuz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2xhuvqthf.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2hhsrejff.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2pamhhjym.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2ilwoirhb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ipdptmrl.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2lqeeuvwf.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2fsudczoz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2bpuotcfu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2puqnmxax.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2zewxkkjf.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2ockxbhaa.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2vvlefwvg.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2galwjaxg.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2bbdxcbuz.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2emajjmia.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2xtepavfm.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2pbiyghii.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2tkuhwlhu.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2qecozfpb.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2jlyktxmh.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2tsllmvsj.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2qgytyapb.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2gbewduis.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2kcuvjopi.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2adutbnec.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2acznadnh.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2qslbshgm.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2uuvdntdu.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2nbtxedks.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2jcrdnyow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2apqydsim.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2zltyxssx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qxlpnvfl.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2hyxlelcq.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2biqhqnua.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2bcwbtvqb.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2ikpjsivy.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2ujyzsvqv.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ynnxhnap.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2vxewquzt.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2kyiskdov.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2bcckpvvs.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2zuudhfct.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2edycgfgm.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2augrrrka.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2eebqssis.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2rlyfqeew.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2posvvhcr.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2amgjhivq.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2ahqcczyu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2uorcuzks.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2dyhhiexg.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2djaxskdq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2bsjqzbll.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2wgwzgzsp.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2hpejqsmm.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2stmszugb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2agymeyjc.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2cfgmslgl.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2flfzisvp.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2sulxxdxr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2dljeyixi.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2tkjzuznc.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2xpyfqyqm.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2nazimide.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2fztgzooj.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2fcblapwd.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2kiwvzoqt.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2qpimunho.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2naatfcse.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2fnvorcdq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2jfjybuay.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2ccttrzis.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2xyvxsabk.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2offashks.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2jlftcdng.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2lkmzifsx.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2ifferpkj.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2cqhensbi.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2jivrnqyj.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2zcvxsjjy.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2olswvulk.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2ydyxkjqg.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2xozfpghf.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2lifywoyx.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2pqfcjjoh.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2zjratwdz.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2gxchpguw.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2qjwolhtf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2gptsubjy.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2nvtzlhku.html


<!-- 参考信息 -->