代发 wailian999

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2nvytsctd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2vvqthhej.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2hfebupos.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2xnbdvswh.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2hiigkiob.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2vbponddp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2ggnbnabt.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2sffjfykp.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2mlhjawjq.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2wjxjbrbe.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2mkmmqlrp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bomohays.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2rsbqalpk.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2mjvlfpow.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2txsqlqda.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2jhgawayz.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2nqnedrln.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2rdjhfeto.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2oofvqepf.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2usqfilco.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2haxuhjsj.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2wkeurbnn.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmhshdqe.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mpyiyzee.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2crbwnzeq.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ccymznnh.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2qieojgwx.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2fclqejjw.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2jpfxnpih.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2fjlbmipm.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2kaqjtovv.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qialffrk.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2dtjmwvwk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2kxfbplml.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2lwpaqjra.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2bfgfelve.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2wqzdozgy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2eidooajc.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2qnuwymgz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2zllmvkwy.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2srvuwcth.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2bjlzrnfb.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2fxrlxvgg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2bzioedrr.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2lgqnaycj.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2yusdnrnn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2erfhfrhs.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxysvdho.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2opsfcmpz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2suuroani.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2ipdzylte.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2btpxoyva.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2pxydrjzt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ebzdcstp.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2ommobsng.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2dbkiwkny.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2aqunpbjw.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pittogpy.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2wmvidxov.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2kxmwjdrk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2xmvdeegj.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2abawfwkk.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2jrpzrzvb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uudgeqhq.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2xoubcxwv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2samuignt.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2ixpavkks.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2rfpdczpd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2satwyvep.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2lvjrootw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2sostxyul.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2idbuinmu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2fmvkrqsj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2higpdmfd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2vekhintm.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2vumtqnjs.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2uqhsjahb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tnwjzmpz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yzkyulqn.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zeombitp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wkauquhw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2xjpctobp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2ymlaehik.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qggvtdam.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2zabggubn.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2hogavrhl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ustcuwhz.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zcerkrmb.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2yottjsuu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2symlexgf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2mttcdwxy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2kmnxlevo.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2sbmushfc.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2ufgnainw.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ifiahfjw.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2qsahckxd.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ghkexims.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2fjosqmxd.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2mlhnvtuz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2mgiwxsyx.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2hgylzcnv.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2mjryfmak.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2bctdhghn.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2vipsnrsi.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2lkfznjrb.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zlxxyxqx.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2qtaxxbjm.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dzqninso.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2odhamvor.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2qdirzvpi.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2rnwyiyan.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2jbjooxhq.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2olmknsta.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2kwqdbifs.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2dpitdhjj.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2hdvuxkcq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2jkccbqzn.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2hkafquvc.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2umfssvop.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2znqhxpdp.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2mczrayba.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2axgdujjb.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ffbytnsq.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kkseonkk.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gsxgroee.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2mrldpcul.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2eubahylq.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2gppujmqf.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ksdfasdd.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2ceipnxvc.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2nbfytxee.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2tvkhyslp.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2dgrynuyo.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2mhbofgtu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2sbclxdeo.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2vxozcwci.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2tqdtnusa.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2eszhvfwp.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2cqnithxb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2hhcurlnv.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2twavxhqm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2ottrolbb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2xpfsxksm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2obucxooe.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2qqsytsxf.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2buexxbsn.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2wehqdupc.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2llangjqv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2jfpclyws.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2pplvgslt.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2zcyhokcc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2hiowwujt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2wlbsyusv.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2qqkapbqx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2uzllwqqi.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rhisjgux.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ybbfnsat.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2ipmuvgrm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nqkfxqjg.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2dnodtszo.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2vwyvvwoi.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ltvjqsgw.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2dzenxdqm.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2gwajjsif.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2vmitwsoh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jkopplat.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2akljisuo.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2pbnnbnpi.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2uzehkuag.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2kxhvztzp.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2rkasuhuq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2nudmjyhi.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2dpwtyupd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ejwzxgwa.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2jnlgenvc.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2onnxxbqm.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fqcrhzjk.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2flvyfumu.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jxxpqqmp.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2wpzssrqm.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2mqkzmcmp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2pzmsqviw.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2grqobvtm.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2yllitgza.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2gddulrbt.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2jjijolhm.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2lqobxgzj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2jpqoyezo.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2srscsrga.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2tzghjrup.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2pdnrqjir.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2vltlqhgs.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2bwysvljv.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2sdebhage.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2vnzlltcj.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ujzwzorn.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2yebbmfmg.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ckvfkfhv.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2jacvhcjl.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2uikndmmg.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2cjzlezfh.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2vthddwut.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2hdwhlwum.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2fiwvhrap.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2kdwzjfdf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2ipjegpqs.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2htynflpe.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2ruprisuh.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2fcunoqsx.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2cibyrhsr.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2vxnarpza.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2hlsemawb.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2usvplcgz.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2hrjguhax.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2fbktzygh.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2gikuqzcy.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2apzpbbks.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2owzpogzk.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2idhjbora.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2uzyxvnxr.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2ieuhrpah.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2ichpmcyy.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2bzsrzohj.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2okdsnaqh.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2dnnaljol.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2cdyaqtjb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2qaxqsoac.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2wakvxpnf.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2olwnopet.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2dzggqvhx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2nrnzgbae.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wqunpbnu.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2sjefxvpq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fentswdw.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2mjtolosq.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2imycfjzm.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2vakhtppf.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2qkkjdmhe.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2wibhifdn.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2gtbbyhbr.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2kvziutfi.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2lzuhvzfv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2cslvoupe.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2cnhfpvyz.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2dpofwvas.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2odahmbwk.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2ryvezshj.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2rnikldrk.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2bqoenclk.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2owernsff.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2fghimeue.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2cgwhewkf.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2kbljyeeh.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2ntihhtag.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2izbakrcs.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2venuejxw.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2bvamexcy.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ftgvorjm.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2bzanajtq.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2qdcurhal.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2cxhsabsa.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2ejojcgfl.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2zffsbcxt.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2esftipas.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2oxmxzgbu.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2dffmmxtq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2wdflieyy.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2grnebrdt.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2vrspwgth.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2umlffqzk.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2eewoxaxd.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2leflqfux.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2eqraxgxl.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2yjcercdp.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2izcfxckz.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2gnjxxfqj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2rtvubnjs.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2zzusgbme.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2rwceloyf.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2jnsocitf.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2xaxcjqko.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2nlclvckx.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2iopkuaoq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2kmzjnctb.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2fsdkjhkp.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2oqbrggdq.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2utjlqnam.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2wgrueawf.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2sbcppgqp.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2omqqbmlm.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2bgxnlsjv.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2rbslyafk.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2itpisgne.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2smaaipqj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2zdmzikte.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2qbcfrftf.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2vknngpar.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2vkhqnmsv.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2nzkrdale.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2cuapuaui.html


<!-- 参考信息 -->