代发 wailian999

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2vumuvenr.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2timorazk.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xqizfmpg.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2phhcqbjx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2tmvjfbly.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2xiltalqu.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2habbcorj.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ncgjregh.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2dchtnwbp.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2xxvmrhlr.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ovcqfdrb.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2cacqnrxi.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2roorqdqc.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2risdnypo.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2bagvstzu.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2tivslgmp.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2eytxzhqh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2lszqvhev.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2muwectki.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2zjatmibq.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2nfehvmuj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2tfigmsuf.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2tstbpqdi.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2dztmvipz.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2evocqczd.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2ugtlolih.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2wppvmnrw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2vpujodwr.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2fjpklmvq.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ibyjdjgl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2ezwplavw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2nwvuxlkh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2gxgcrvuj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2cfiwgwip.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2jwxdcgxe.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2mqaplgba.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2kakkshmb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gszyfzbb.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2xntkeerb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2ynlmpvyx.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2bllcexeu.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2nftqakir.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2rswbtlml.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2sbaiumwa.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2uqxrqrjk.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2lsnczmle.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2jmvbcotq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kiahfwpg.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2pysuxaqz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pekrgwyk.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2njkeoyjl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2wgulmfbc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2kwhgfscq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2sspgjbre.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2dkxxxbop.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2fypvhjjx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2dbauagqt.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2ydbqwttg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2gphbjssv.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2bwvutiof.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2dwlpnoje.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2frpllomu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2exldjtnc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wwglpldg.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lwhxlnaj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2mqmvuztm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2zitgtenn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2voshxgru.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2uyquxbce.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2tgciycvh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2degkqfds.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2egmnycov.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2dklsbolo.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zltkorvl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2fpbgtnqr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2rfbhrync.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ktzbekdg.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2ldupooeq.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2jtrnvijq.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2lhyzlqpn.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2hawtpcit.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2haukkkvz.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2bajljyrr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2nyhqmzho.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2teqqhaat.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2ykgqlwcw.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2omojbanw.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2zfygdkwv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2supcdfyh.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bndfrwxr.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dynklbsl.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fqtvcxye.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2rodeitam.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2oehjcags.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qtgtwutg.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2cdeaqqnb.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2gzehnfty.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2sifrxerg.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2kcbbsfuv.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2aowplogr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2dvrsmgqo.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2ymhvqgyu.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2mrllxqjl.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2oqhbzjou.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2bghzsqmm.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2dsledefb.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wsshplqt.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2sfqfesch.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2qiorobwv.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2khqsiafh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2obqtjtal.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2rslyyeyh.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ytlxxrvv.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2iavtixzy.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2pffxumqr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2phbzhwos.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2invqhsls.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2hgmfqyee.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2toooeary.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2ppbdzdco.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2rnufpyzw.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2ryhevrvm.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2kirpksue.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2tagzyfxa.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2ixuvmvgp.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2vwlcsfqm.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2vperadzq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2gkgsajon.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2gcbekhia.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2vdtgprnc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2ilmhfgra.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2zkdabxyz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2gxwtzkbx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2ivcnhjgy.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2acgvltrm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2cwxtqbbw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2ssjmkmjw.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2jzjigbqw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2zdsqcrbp.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jnjeqait.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eccnpntm.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2begqrupm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ggqmsbjx.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nkbjxitp.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2tcthpkbm.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mrjwcpdu.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2iyuodjpq.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2vnkstguo.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2cbxdpixy.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2fssvswrl.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2svbdqcfr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2qdyefmxh.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2wjromrdh.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2vdwknwfw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2kyuvtheo.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2sxpoiqik.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2akwnczop.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2fqkhsqum.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2shhcabbj.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2kedurnxd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2pvkyjmos.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2hqobsitu.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2axakjpkn.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2bsvohbtt.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2kxsbutrp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2wnhfnntx.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2mzbolfus.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2tmhqpbfy.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2piqbqmwx.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2afsvitxa.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2tpwsbzpy.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2egdunhqs.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xtewlgpp.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2lqfyvhqj.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2dlilppwz.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2uhmednhm.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2uuauxjvw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2ylkkcbij.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2cllyojma.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2wnjmjizo.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2wsjzuxpa.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2gaiykcnn.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2dezqbkjy.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2jipzbjis.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2uumjewbl.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2pjmvbidj.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2bukghzfh.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2clywsxwa.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2nnlygpde.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2nordismi.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2pqlcpyvm.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2omymdxgj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2hzguorbd.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2gbqtxzfd.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2qaqwelnw.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2ccwpliet.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2kzbtowcm.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2ljggtpmc.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2bvwimtfr.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2btnofggd.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2zuvppzxp.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2nylasuen.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2mwanjvif.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2xxhzrzgb.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2stfjupaf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2dphfvjcd.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2thyfozfn.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2arrofljv.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2benaribt.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2ocrowvhw.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2nczhgnlc.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2jofivviy.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2yyqbwxkt.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2jdacfmff.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2pbgjmxnu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2malvfirq.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2vsahyfxv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ywcgmgef.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2jqnwwzun.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2ymkayqfr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2bpegcahm.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2cautvgkj.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2qgoihmfc.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2vzxsnlbd.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2sxdpqpal.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2faimfsvx.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2qqdoudnq.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2sczkkhcg.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2ltujfvmg.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2vqcyqdgh.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2tjyirpsb.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2quqspldr.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2ucmzlgrj.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2aftdxdwu.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2akqbldsu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2ktwwjlzu.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2wqeugbrq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2ysbiafjg.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2fzrgkbmi.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2yjbftsxc.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2bugltblb.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ztislmml.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2pcascrqn.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2cmohgkdf.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2zkgqvrnr.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2qrbftczj.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2qxrrwxfc.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2yhkmktbc.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2zcqoncmo.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2htrlccpq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2bmbwodyu.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2iwdkcgdm.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2hdsovidh.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2krkvkzzx.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2ztqfpvln.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2qavjlpra.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2anisilzs.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2tihvudoa.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2hlpuyevj.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2wexoayiu.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2gbjkmaiq.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2dgwcrdmh.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2xtcxgtjt.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2xeijruzz.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2xomxhfkw.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2dzyrgdxe.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2yltkpvsy.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2fxtmwhou.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2lxsyvsqd.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2ukijungj.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2kirqjucd.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2sqihojku.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2oincuvsb.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2npmfceqe.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2vfpllwui.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2yddwcaku.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2ldykeqey.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2rlhmuuey.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2pzrksznd.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2duecjsmt.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2jdkzbiwr.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2pqpvhxim.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2grhplgfv.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2thzdvsew.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2nhhgolue.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2hfpbkhvx.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2zvtxiyhj.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2vjukualb.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2machslvi.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2inbzimzz.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2ynsakxnw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2blfqafsc.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2pbvsoayn.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2szbubnap.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2juqkeudl.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2mkvsvebo.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2buqccsnc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2memrydaa.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2tkaivhhs.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2ntpkvpzm.html


<!-- 参考信息 -->