代发 wailian999

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2psuedtpi.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2uitrqvqj.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2collyvgc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2wesacmzu.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2hdpgoizp.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2pvhnocjt.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2phnyabla.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ozrehool.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2qgrlwvco.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghpuemws.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2jinnhzwp.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2uzmqwtpg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gkjhivxy.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bsfyqhsi.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vvnpnkll.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vvacccta.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2wmthssnx.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2grhazltu.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2eegeqyuv.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2ifsosvjd.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2rshflzun.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2cnowwgeq.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gznbyxdj.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2nomwhzxa.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vpokmfci.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2rkdohazc.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2wopkgmeu.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2uhoclerp.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2cerwuooq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2jegzvtik.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2yulfrcbu.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2yytkwdva.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2mqgqqyeq.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2ojkpjaua.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2ftzaxbbn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2pucdnhbo.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2uyhchyfr.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2oorgrejc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2dklldjmr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ywmkxajt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2ddgsshij.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ricuvorj.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2qmowevkt.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2sawwbafp.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2flsgxgvp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2svbgopfm.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2mhamcnpw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2ompadock.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2luomcwrc.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2lawyqbwt.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dnmpdnus.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2rqochpkg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2gblwzisl.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2corsmryl.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2yygbidfz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mmbicibb.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2jhcfrryw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2skxipohk.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2tlahxttf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2pqaxwhxx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bbbkajmy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2vkmithkh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2hlhxaitp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2pofiiquo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2efyhzyfe.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2epjvounb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2vbberbdb.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2zdovudfq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2ibfdtyys.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xazjpozr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ubtrfein.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qkagbdxh.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2shdofwal.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2quyuyfsl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2gcemzvsv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jqsizmur.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ytjvcccs.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2wppmgjuw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vdiuchdl.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2oalfqrde.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2akwkyyrb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2czdcegdv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2edhwdnee.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2hoavxbun.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mewjtwfx.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2bfeujlih.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2jfqfoydj.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2eeaoevyh.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2xwlirwue.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2wdpewnda.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2jwinrgjn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2rvzhmexo.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2szobhzlw.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2huvjaalx.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2elvmoyhn.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2hlgoijbs.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2tgpxvqoy.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rrysrott.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2sufcteai.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2ordqcedp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2pbfbhzhe.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2sfhyziik.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ynlgcfeh.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2nxgkwcxr.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2ghxkduch.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2brwkinep.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2vwkvsexn.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2lcfqupnh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2yvhkespj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2gfvgckfc.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2bmikcubt.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2asnfrfoe.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2hfploqek.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2ohbmbnqy.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sfybqzxa.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xrtdwpom.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ofsfflcv.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2ydghfczn.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2najcmbkn.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2jakigfqm.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ktoaqgsc.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2mletcmpq.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2fpltqxks.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2dxdkvwtj.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2qmrpsyeg.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2ltvuunat.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2pwtrprgw.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2osjdobsj.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2wxmmfaiu.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2ffcitkue.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2fmdeugnr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2kkctsrnd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2bkehhozr.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2grpysufr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2whbmndsk.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2ithujelx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2yuvaenrx.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2kggdwide.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2ifepfjhm.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2meibalxi.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2fgthtemg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2vxhmvufp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2wrycmkvm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2pwvtylgk.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2ftqlwngn.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2coxzhycn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2dtfcmznt.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bloebnfh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rzpxnomc.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wmgauwll.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dtuwopsz.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2givcsbju.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2kmdvwltt.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2gleyrtzd.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2hsctveyq.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pdvcqhwv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2bspssbnx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hqlkywbt.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2hcfcevil.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2grzvzdxz.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2khyncpvy.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2xzcquetj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2ndgitoza.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2cenzlqwx.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2tpisampz.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2gphzaggg.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2jobcdpuw.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2zxfzwszr.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fpkafxpn.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2mwzbqkhc.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dgfurofl.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2cdijihxf.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2nroecxjt.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2fmurwpoi.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ammpgyzr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2fcivqsls.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2ohskmafa.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2cjstouha.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ixvabmuk.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2psflqcft.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2rxyfjqid.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2dnyknosu.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2cofsoncl.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2poyvpxxs.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2iebembgd.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2knrbqvfs.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ohfwbmqn.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2etiguupz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2jxtlgoim.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2tlckkiwo.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2szttxwzm.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2vxhzndcu.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2zwzbgpyy.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2coryntzj.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2nvkuazmx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2eggjyenw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2ifgisojf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2apszfvnk.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2muyxopmn.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2xlyimovb.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2jrsskxty.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ezlobhbb.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2yohrgpkh.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2ipdmxssm.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2zdnieegs.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2fpnunaon.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2kowlmtmx.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2nvyjmdya.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2njvifffp.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2mlrpqrax.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2lhtrxyor.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2twkocfmc.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2texjwpwh.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2ifzriayk.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2blrvahbk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2ypztrmtt.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2vbnlhffh.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2dgnnyvha.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2mcpeypne.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2hrpuqcjj.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2rbvpyqdm.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2yjopzizk.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2uavdwxoy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iizlehwv.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2wqhhwvzh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eadyiabs.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ixifhddy.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2ayiizysw.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2vqluvvcf.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2oieirszd.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2vwtfbqrx.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2aodydhjv.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2npbizswm.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2netaioqe.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2krxxbjvz.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2nnxvdifj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2eddpbzqs.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2qyxlqgtb.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2csiawpis.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2gmexdmnu.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2qemnqimh.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2vifcgcmx.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2yyxwtkrz.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2oihcpsgk.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2wvvvebwr.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2bmipssss.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2datuudjz.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2uzceustk.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2fhnfsdrg.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2idfhcdxz.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2uxpfcvnm.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2zawucuba.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2pynbyyzz.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2jvfrgmjd.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2gzycyirf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2rxhntxbi.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2etpirpbs.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2gyeowyyj.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2myvdpqfl.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2iyvmblyp.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2gzdqpvnw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ypobvkup.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2rnpvkufd.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2mifvpnox.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2pidyqeee.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2cosobfwr.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2szxcqohw.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2tuxbjqmc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2oyntynqo.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2bqqsqgdq.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2dfsshuph.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2cwsispzk.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2tafcnylz.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2mrquiruk.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2sqslmxmm.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2nbtqepzb.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2ljlsnpmh.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2rmcpfstu.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2laaskzlm.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2ajbehqmq.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2ulddhhzx.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2uwhptrmh.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2rliyhwuc.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2uazdhzsc.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2uxkkorjx.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2sorqrcoo.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2zlwuyjmw.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2nicoulbi.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2qihukgdp.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2dybxvcym.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2nwxlullc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2rribqpem.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2qclidlji.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2bciriqse.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2gdlbsxpr.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2nredxpjk.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2kikfonvx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2vmdyamgn.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2klgjruva.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2uhdcsbbp.html


<!-- 参考信息 -->