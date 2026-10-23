代发 wailian999

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3hjjcqdiz.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3mznwjtqp.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3zdwjqhgt.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3kdirzsrs.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3nugagity.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3nygrvhpq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3riixswch.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ppwdcwtt.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3dsxbrnps.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3xjqzmstv.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3vlevyjwz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3dmxrssha.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qurzagim.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ukwexoay.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3aqyclylj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ogrgvnmq.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3cmbhngyq.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3soxtdmyu.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3adqvlbis.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ojiahuqn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3mjpvjzny.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sinkihws.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tnludysh.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3yqtairfl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3yvjxtysv.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3pabyonik.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3qvejkzua.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3rohthzki.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3szhmmvcd.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3obsoqqyt.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3pyvkkmhd.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3biififet.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3tyysycix.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3dvjwdhvr.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3jdtdyujq.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3edfxpayr.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3jdzumtfd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3mqyeqnjj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3aymfwkes.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3wvxllrpu.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3nmqkgtty.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3awcetmvp.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3aofrpptv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3qwzzzilu.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3dptcnmsc.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xylhomda.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3zcnyillh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxrsxolt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3yonwikwo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3prasbmzd.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3odhkicot.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3akqlyypd.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3cqqoeaoh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qljbvjwg.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3kjvfdsvp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3qgmyvaoi.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3kerceeut.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3kjeqtflo.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yvduwiet.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3bvniuadc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3zevykrdo.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3pkhztzfk.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3cwtabomg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jovdlfrb.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3jturfugy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hewazchd.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3nulxqrjy.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3izqdcncx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3vwrllrbh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3jqjirwjq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3nxnatlzy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3rwdpixyb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3rodbbbhk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3auagzdki.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3xxvjvhlx.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3qopsjuas.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3dhtxsqyd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nphatroz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uaxpydih.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fxgyzmwu.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3gaorjxqy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3fnfappew.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3cslwmwsb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kkkyvgwg.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3renhcxor.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3fntpeivc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3suluqmbc.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qvqfmtfz.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ekszrhja.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3awdkndku.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3bawovhzp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3fkclyzwo.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3elvtdudd.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3ztrsnmun.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3ahpxqxhk.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3mhvnmatj.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3flstnynp.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ykwdtdod.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3msbirghi.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3zjrnqvlt.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3qvvhcyhj.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3kebaokun.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3rbeleijr.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3qditenss.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3hxwhjqjg.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xqgydcnb.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xuhqjrpn.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sbkcntga.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3rzfzzuoe.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3vkcuwhzs.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rwpioqqt.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3cbazmsml.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3vtzwhxih.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3bwjhjlrl.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3otroprpr.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3uwqmzzlf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3sdiwajpj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3lkgaeatr.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3eedaqffe.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3xhcvllas.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3beyokdaz.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3ixssvpnz.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vtvbctae.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3urtcfneo.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3pfgiupmx.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3xmskpvfx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3gvyvbjvn.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3dchhzgjx.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3tkbcwyis.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3guvttujb.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3wtpwxhkb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3quabakjf.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3fjywxthi.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3fhhtyzgk.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3dvtaxpek.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3mgxmxxzc.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3invpojzf.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3hvsbxvfx.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3tmqguppn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3ufzpszjx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3mbbpkrwg.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3fomrnvux.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3qdupvopi.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3jawpmfys.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3khbwskok.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3zfpwhyvv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3kyxrkonk.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3snyqlrqk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3zblxphjw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3zdjdeumv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3vzjmswck.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3oxzinmnd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3dcqzwhkl.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3vderwhwi.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3uiqwqjwi.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cjdplpcp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3emwdwtjh.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3trwnohft.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kftvoccq.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xjutbopf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3vdapijno.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3djzflpzm.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ugsesxta.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3yelpipse.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3mzthyvpd.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oetsuoog.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3ycnapcip.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3clvzqycr.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3kublgsus.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3ssncmsza.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3xkuzvcvk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3cnqphsdp.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3vmswuypg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lbzezurv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3tedvhztr.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3iclwcjrl.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mrraipxw.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3eibonzwk.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wknfkwjo.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3wgafigmx.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3flqaleqt.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ubavdwxm.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3sijxzgga.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3jezpggcn.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3dbphipan.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3vgrxtboc.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3qlerydir.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3yumdvpnj.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ntntyinj.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3cqjtsbxh.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3ztpahnbk.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3rtiigwwz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ayqrzzkz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3ruimnubk.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3lopggecs.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3lwzfcako.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3wnejuqfi.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3elffsmob.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3ccghthts.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3shpmhrvs.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3gfkgmkzt.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3oppqsdvi.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3dmvowhtx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3ezqvujot.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3knesvqhk.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3oylqrsqb.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3pfrkrqpe.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3rvedbiho.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3qtixekmt.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3jdqgybzr.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3skmbhqzi.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3hhcvqtzd.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3ywqutiha.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3dgtljflq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3mypinfst.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3azsqxjam.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3bmroclqh.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3idonovrq.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3apazwxbj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3yuiuquir.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3yocyqfqe.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3xhikuyaz.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nayvlgoi.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3fpqiawpm.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3otwdztbr.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3qpetgrxt.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3lnupgjrv.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3zbebohox.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3qmpeiuid.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3idbbcfas.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3urfobywx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rbdnnzli.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3ddfkxruq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3prsnambt.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3lmozexrc.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3veawljdx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3sreypoir.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3oemalbfz.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3hdqmzfgz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3ugwemppv.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3udcfcijz.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3exsvedns.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3tabbmeui.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3uknvbzxk.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3cpxhqhup.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3wqasvjcq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3skiwtwfk.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3vecgddzv.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3ehqwundi.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3dsacsvrj.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3hyrahzib.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3tkxjdzph.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3cqhygzkc.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3wdmqogmj.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3ddfcfzxt.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3puifpswf.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3eftphadp.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3jmztvloc.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3gqssxfvs.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3fexwougz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3mhkmywxc.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3kpmakipb.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3kxwsqdnz.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3nsutzgxk.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3waeqlbyn.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3wjvtanbt.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3bkcpskal.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3gltqhpew.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3pguqsmcp.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3pgqlltmk.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3icmvltlp.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3ymzqwglb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3keiyccbk.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3ykxmgrrw.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3sclcvsgh.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3vpocremj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qlcxcbug.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3jynnhuwj.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3rxlixfdr.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3iodxqhed.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3kltsoscf.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3awsdkubu.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3mopyftmu.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3vhmglzzf.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3crdjvdgh.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3xkknlbuf.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3lhwrpcyc.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3vshcioox.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3efldxivk.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3eucdhnkr.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3kqwfkftu.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3ilxeazdm.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3bcrodmav.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3jhhbmhgy.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3qntvsghr.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3fnjektjx.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3wflufxis.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3qrqybopm.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3gjiecojo.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3izwkckqu.html


<!-- 参考信息 -->