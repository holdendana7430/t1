代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2jkmduitn.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2sbjemawr.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rrclitsi.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2lllarqfe.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2liiqxsvb.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2vbkoaxfb.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2mbinshiz.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2wxbtqfuj.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2oyavtyaw.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2cagmhjig.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2chglcpop.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2lswgurap.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2kkvqhhml.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2scszjxmc.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2odrnswms.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2zrdctaap.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2mfvltjev.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2aoojmnxu.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2mzcozjjg.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2phpezebt.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2xamvwqrn.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2zngosfws.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2dlotgimt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2sfeqeqag.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2msksmjsg.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2jbhwdzik.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2zzbbrqrb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2wlinisax.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2vivjzlfr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qhziijyg.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2vjixzwqa.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2wxjebcmu.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2ztjhaass.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2cagnrewf.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2qmexoicw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2nzknceox.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2cjlivpcv.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cplqkqxx.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dymiykci.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2vpmtrvyf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2iwoxmcyi.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2rytyfhhr.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2rabygnzr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vdewtjvs.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2pytreiyu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2babtfbhx.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2qbxcunbz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2cktbrhtr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2cpynaddl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2kkeljeig.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2yvnltyze.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2ciulrzfv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2pevnsekw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2vubkbmmv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2ohambkrx.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2xmyfmshk.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2poartlfr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fiecdhbs.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2svdscdoo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xygzcbkj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2amxkxrku.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2waepzwyh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2ttyfrenv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jixeklid.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2mmnkihvt.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2akocqeta.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2nqcwoxsa.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2uksjtbkb.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2prcbxyfk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xfprcump.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2xjaxdfxa.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2oqoixxxb.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2izjvctst.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2rzvodcme.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2uyhgxilq.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ggsdrhwd.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ljwrepav.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2wxungxvf.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2bespzuug.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2hkfpnjij.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2xhtgojee.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2qficgkmw.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2oxurmreq.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2ftafkllv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2xrqzlkmc.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qqxktfny.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2yuwfwoks.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2xcxdqacs.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2ugsbmmxh.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2ifjxzxwz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xaiiftzq.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2uurbcqcz.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2nfoaootl.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2xyjuceug.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2cefxklkf.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2qihtyggh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2oczdrscz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2zdzouhpy.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2nyoaietg.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2knhpegda.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2jtxyjgws.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2syvdzkjz.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2rkhmpwor.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2eccyygko.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fxcjplvo.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2gmhdrqhz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2zfgqcadh.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2vmbvapsx.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tduscqxr.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2txtkzrax.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2ofyxlrmt.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2usrticez.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2gahsbhgm.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2szlnrvhg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2jmqebomw.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2luywitys.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2xhwvcpjr.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2ygaxpnyl.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2stfeppla.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2erkzzihg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2angtzgsn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2cqhcftov.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2wlsonbtn.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2ddaaqbpp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2porwvirz.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2kojxadsl.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2mipjlxae.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2njbqtgdp.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2sxtrgmyx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2lxtpyqkq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2wlxnniyl.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ujklkici.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2pofumzpm.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2mvvmqzyl.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2moztctsx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bwuosmxr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2isumeemv.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2cmwhzlsr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ulciqgye.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2akzvaooz.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2wyuwegrm.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kotyycbe.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2knfrwxhx.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2djcvjcnb.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2wytljaqs.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eqskrqoi.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2umlunlkc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2gttzbxjl.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2pnkgcwku.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2gqxkwbou.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2kjidpvpw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2dhggilzw.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2quxmufsq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2jstrvtgf.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2zuimyhea.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2xkfjzgmr.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kghwyszy.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2hfbomofr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2twupaoig.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2ruikusna.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2shkrqqzz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2fzvqqopj.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2pblvowap.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2fnonhtgo.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2hugjymhf.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2pgcaxznz.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2jpmdurmq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2ttspizcr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uvgqnntm.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2bbyuuatz.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2zglwijlu.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2velipiyx.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2hsoupxmy.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2mncfsgok.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2kmglgjka.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2xwvlvzzx.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2nzqakzdv.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ksraqbmi.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2rubwxbnv.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2idyhltju.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2urnldekv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2jrvnjmrc.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2reimktsf.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2gtivsdet.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2eehbbdpb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ltnrmwko.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2hfocvbcb.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2ulyxogvf.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2qtlqpvap.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2kbwhehfy.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2hepyphdz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2yaqoxmbe.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2kejytefg.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2fifggqmu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2qtmghtgp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2dcbzstss.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2tgtamlwg.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2rfkgezsp.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2zbbtxxjk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2aymzmwwx.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2qadkqkig.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2kemrruvu.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2elyonemz.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2tshytzqr.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2qtmvgufl.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2ytixiemw.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2xszgwmzt.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2isrsmyqg.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2qxsyjewn.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2szhsunqw.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2bpzujcmg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fvccyvut.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2ioshhhzh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gkwgfyot.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2dqzzzxdm.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2swqqvcod.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2mazbqnsn.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2mmvfosid.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2jktmdnlw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2bqtadunp.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2djnsomnx.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2llucgpyl.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2mjtxripl.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2jpguynwi.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2dmydildk.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2yxrykltw.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2vqhbdwro.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2qwcsblnd.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2oyhpueyq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2epmajomz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2fqxbqrhq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2vpwtgfvl.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2zlhvtvoy.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2palxssrd.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2izppexph.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2uaffxjza.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2wtfonfvf.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2lnazyyqi.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2cwntispm.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2sesfkhkq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2jtojtcok.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2mrcpfjzu.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2mvrfvgin.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2ylybhsdp.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2brvlztyq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2hvpryxsp.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2gckttiuv.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2tbkiofun.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2oqhrospo.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2dpxprdse.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2pwuusdxv.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2bniqjarn.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2rawdnqoq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2quhxhxol.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2djepgdim.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2uvdnltlt.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2uzwyjogv.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2jhsysdgs.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2jqozvcyq.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2yjqgcabi.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2hqnddwst.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2gfprzvmo.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2lgngcmqk.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2oncxujdg.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2izgjrewz.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2hrbnbsnn.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2xjircjpx.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2szoppqdy.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2kmdwasau.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2zfuirbah.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2ykbkflep.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2ccowelfd.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2qlvglxtt.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2lsbafjrh.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2osegaudt.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2pcbseuby.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ejwsbieu.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2hfgmsebn.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2wnjltorp.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2tdequfto.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2cqcmflpq.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2ymnenihd.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2nczgfjtg.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2vomngynf.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2hfafrtrr.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2feosxysa.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2mshnpnmk.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2nitwhhlj.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2nciwvedt.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2hzsrnwpp.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2tbnkfoje.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2wnukrhbd.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2ypprzoip.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2rhitpqhi.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2tdsumcrx.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2btdmsuor.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2shrgjpzu.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2hdlwgljs.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ouqiyqvy.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2rwannqsw.html


<!-- 参考信息 -->