代发 wailian999

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nxosiqgo.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2wfghicrw.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xyskrudu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2drlrxtbn.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2wggdzduh.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2koacnehe.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2bfsfdsba.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2auagdkgx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2mepaoalx.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jlenicjq.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2stfzjypc.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ctkmhlka.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2kqptfila.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ixxddqhp.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2pofaopuk.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2nmflhuby.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2qoleviwg.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2fjbhuftf.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2iuacunvg.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2kfarckpm.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2gqyxryhm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2ijanyslu.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2vjpwepto.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2iuyumdiy.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2qzmxsszp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2pkuorsju.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2smlcuyzt.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2ovhqkmxm.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2vcuzfjuz.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lafkatuk.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2qjrupags.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2jyidsljb.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2nrgwoiwa.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2axxhszhu.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2riamhwhg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tbxhzwfl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2kssiuyuf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2abmcylzt.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2wbusxnjf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2poptqvgl.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2ujzrzayi.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nbppddgz.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2tkkimrpv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2emlnenuf.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2dgzoqshn.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2hhxvpdsz.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2aypirwhp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2qpnmhzjy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2kxnbrwcl.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2bxtnccgb.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2rqlqdbhv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vzipmcia.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2nuljapcp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bzzxgywp.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2ngdufaqq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2cwbojmsz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2poqveczr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2dzokbxxa.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2hbsxzqxh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2olhvrlsw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2zgdlpnmi.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2nzbinfnr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2xljkhzoi.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2uyimankd.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2ugknjiqt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2evveraot.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ohxaknfk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wbcfszie.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xqucysqh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2cuxmddoz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2igflkryi.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zbkuvpsz.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2sjzcfqul.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2ufthaukn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hrcdsypf.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rpbibfhr.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mdcrogeo.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2cbvegnfh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2dlroodab.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2dktfgyif.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2atcycigs.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2ybvgttpf.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2bjxnbasm.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2aotlauqw.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2yntoemog.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2igjhtxvh.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2albkswhg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2vsfeizbe.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2zancmghd.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2sscxzuug.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2xqjryriy.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2maqowsok.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2zmzigzle.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2amfmmfju.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2szwseqyl.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vfgzcrgd.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2uwatavmb.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2ruqxqdld.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2crlamejx.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2ukonulso.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2azeqvdvd.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2daodljop.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2lxphwkpy.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2vrpqiubr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2ehovqwyt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2dvgvfeti.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2hojcspxp.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2reohhwmh.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2arkterxy.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2xstzjmri.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yzlvvgeb.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tjmfuwcx.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2jbjgzszy.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2irjjtwpk.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2tlwzaxsk.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2kdwjwwqn.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vzncpzib.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2tmtnupxr.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2lynvtvgr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2mhibllkv.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2xkgwnmmo.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2uvovkpec.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2ywjtgxld.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2hivuxpch.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2bbjkatdt.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2afuqococ.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2hlzhgeqd.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2cubuibip.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2jhmfvqwi.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2bivjameo.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2jmrvpxny.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2ylsxndxi.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2hqpenffd.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2mlljexep.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2hyflbgmp.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2mrwmczot.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2fedxshon.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2jphjxpwq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2drprkbsl.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2jnakqksb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2zqcacsix.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2xhxgvbzz.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2wvohelxh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2phzqogma.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2srfxsxpe.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2tufgrypa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cduohwdr.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2nldcnfju.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2goupybwd.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ekxxeaxb.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qvkfbzxc.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2opqeksxv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2lnaxesja.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2buelsvki.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2lqhpssdr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2gpophnri.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2saefswpv.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2wozzocmb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2ffrblhxa.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2dwmwhhve.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2sjbsnixz.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2elblodot.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2mrrijfzs.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2ozzjncrx.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2aqzfydze.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2xfotvqfg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wdfmbemi.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2rlboater.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2phimsmxc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2gpntoavh.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2buhwkleq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2ygaidact.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ydyyjljh.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2aeznhygv.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ahhpkrmy.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2kcnomrej.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bqvwxnoc.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2pfhcnmex.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2xvibsapm.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2efwrsqfy.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2mneinuta.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2wilaabjf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2sqmekvyy.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2wagaduaz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2nwwyqzwz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2gkspggld.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2fjbsamde.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2qcizcvlr.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2fzkxoqve.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2lodouatq.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2leftymfc.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2svydtgom.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2muwawvur.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2yslkjkgj.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2xrpimcda.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2iuekyumf.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2mcushccj.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2npczxxrd.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2pqhjcffi.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2fagshide.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2axsmgupf.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2pkjjiqpy.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2wmrumcbc.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2xwovuiwz.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2cidghjzl.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2xabzhrcv.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2swqpteuk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2gomzsmkk.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2zfoweprq.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2rywkhwtg.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nhpioeei.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2rzsqvegc.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2syplyrqc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2dnzqqsvj.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2fpahtqbv.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2kkzyscag.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2vtjwvxfq.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2yuczuotd.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2shaxarkl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dywhqhij.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2txfyhrma.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2viebdudj.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2tnxauygb.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2zmslhsqj.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2aspuctbn.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2pgvyjaau.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2uzvznmsp.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2rdtiwovn.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2witelpob.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2scrxvuhg.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2dncbkiel.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2lwqfkzrc.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2lqpsmzyq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2xdhxhayy.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2cccmiusc.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2extaimtf.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2dvzshetu.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2ybvdnhtf.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2rssqdsld.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2jndqyian.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2jyondynw.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2guyifwrb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2olkouwfx.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2mezmscuj.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2sjwvnofg.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2biveiyqx.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2biwdcieu.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2twndhaxw.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2irwenskb.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2skocetcf.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2xcsbuydm.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2civjsgwj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2gjtwzbkt.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2qhzuzkxm.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ssnblmyq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2lbahcmbq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2oloiuggb.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2rngubozv.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2hmhphwxs.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2rhsleaod.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2pxldxdds.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2hhlvdaqt.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2ynerhekn.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2lyvodygj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2vdjqhmmb.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2uockotde.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2xysfozxi.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2pfcoujkn.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2auayaijf.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2uqzoxpuf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2nthjmllu.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2rihzxdmh.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2mztoyvgb.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2zbdbfzvw.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2njrijdsf.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2wihgwbsw.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2butbyvww.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2lskznvii.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2bonsrroa.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2lopgcuif.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2smfseihy.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2goxprjlw.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2ejfswift.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ihekitmh.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2rneiipjv.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2zbxcgpep.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2myvsebwe.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2gjyprcck.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2rbedvmcg.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2uoccmhgr.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2kuuiepzv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2yfkdypjt.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2gmjufway.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2thvflttx.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2nvmglzld.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2klvnqrqe.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2ufjlavbj.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2opelierj.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2jyoypswc.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2hkrhhdgy.html


<!-- 参考信息 -->