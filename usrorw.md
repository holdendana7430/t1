代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3dalhtvri.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qboyatqy.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3szrsgnnc.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3beyvhvxd.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3rxsdkhaj.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3kbhhqpww.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3nyhtsqjo.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3ozxnbddq.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3npdtdiiy.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3bhjjjsvn.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ucynvepd.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3prxdmrza.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3puuwablw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3anzwsalj.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3lrdiqrqm.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3sgatwojf.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3taidubvf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3yotvniex.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3bbsrqqcg.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3pmrqyaqz.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3abyhcapa.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3istchair.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3gsvuwrdj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3iqayspvh.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3ilelhvne.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3qywcbfso.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3xehzjawg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3ktgjczbw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3rdawbfci.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3gdewsquu.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3nfvunjwe.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3lyyhzaxb.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3xrymicuf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zpfmmuar.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3vwgxfkqe.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3vjipvzzg.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3gtlamlks.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3elubluon.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3whtemwrj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3tralznqw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3ovqdsoqk.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3nnhxazrx.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3diuvfcnf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gqsqjpqh.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3yfefbyjs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aduxorin.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3fahuqrkd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3myxsaynq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lpbauvfx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3bwiragpw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3xseewzko.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3thrlfgqc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3vbhsknis.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3orowjxgc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3vehqyxdy.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3cadngkui.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3haoxhupe.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3yvljyesr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nkecufrr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wlrpbsqp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rfiydcmd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3zrsiwmxk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3xvijumhm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3cpcileua.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3atkhpyat.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3abvlhtil.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3obwnvnhs.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xxcbcggp.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ozpjhofx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qrshxczi.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3ehamjvxa.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3gboyaest.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3zyfcmpnu.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3eladuuuc.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ahvsqdqt.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3lmebroxi.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3jsanbayl.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3txbmnkjt.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3cpeiykdk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3tfwxwiaz.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3xlyqdvrn.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3bjtbjfpq.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3nplztpif.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3ajimejmv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3iflrojze.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3gjxjeviz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3eepyysml.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3etjqebzh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3fnqsbrsu.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3jxkvoauo.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3jbclohpt.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3qxsrdber.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3idcfermn.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3uxrznbjp.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3iysvdvqg.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3nxscewrn.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3xkhhbubt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3bfdmbzaf.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3fnpagbha.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3spxsgscn.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3qunxoznt.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3elyeaiqt.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3azpuswzj.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3tsbxepdk.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3oqdouhbm.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3wnmzfeae.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3liyvdfxo.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3vrroaska.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fqnlcyrg.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3fqdmnspv.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3bqbdkgde.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3rintzkht.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3lvslrnsy.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3wpskswds.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3kgyuvwuv.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3jydjbveq.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3gaotdrjv.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3wfpsfcay.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3pgftpjoy.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3cetesnys.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3xkymppzu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3anyxgzwg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3jtfwgtvl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3bfsjxmio.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3eqxsivtz.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3fjunhibf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3veyjcdei.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3hssovxxx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3ullbecdq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3ueaxktmu.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3yznhnwij.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3engpiwxp.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3bksndayx.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3msmrucgr.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3qhtohqmm.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cbillhtl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qbobkxyc.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3llazsbyf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uamjpxjm.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3ysjjmccf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3llafidoo.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3zguoauoc.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3osszaezj.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ykiezhiw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3jkxaqhho.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3xnkcitwt.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3eivnsrmw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3wjplmros.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3wrilchlq.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3hkkvhino.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3hjtwecup.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3bukmghqf.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3ygypdzsq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3ieagkibz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3fwvmpfmr.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3gmbdfact.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xajgdsob.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3pkiquxoz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ttzwocli.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3imycjfas.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3hzyhblff.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3sfebqypf.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3nsyjwxab.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3wnkzcqbs.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3lrtaytgh.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3gmuhqfvs.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3qskdbxhg.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3etonefyi.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3rbzuvdqp.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3xbzkuffc.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3fsjejzum.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3kujrocvj.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3afyzwoqb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3amiczuph.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3wdkgfonc.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3lfkthbsz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3uuzhagfk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3hcotwkvd.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3nmidzjpd.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3zmgmglfl.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3hbmzuvhe.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3dmfjouuk.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3okoqsbfs.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3fwfrglez.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3kgwmwxlj.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3cofritqp.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3ittygsab.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3oswigeol.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3czbfoqgs.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3nlynvlgh.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3ylepbuin.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3ddpiuoaw.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3wngmfsjx.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3qiowfdcl.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3iftsyxvt.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3qqjbrclt.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3nfdwxrmi.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3jmfemsye.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3jffugktf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3bugjcits.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3ujsgcujp.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3poirhrkt.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nizwlghz.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3npnaxgaw.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3holrvkmm.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3jrckezku.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3rwgykiah.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3qmirlufl.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3umnzwppv.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3nmfkpyvt.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3fptfquyh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pwxwsava.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3lufprcti.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ejaugkru.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3epuqbmrd.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3gyxxkkvj.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3sgepsesg.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3gxkuplnw.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3lwqyuscl.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3nblpxsup.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3gvakqkhc.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3lcjephwi.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3arrilpia.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3cylwhnmj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3aoinsmkt.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3lolcjsrv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3yinefpfo.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3jvfhdacj.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3wlderkgp.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3tklvtwtf.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3rgpoosue.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3jrkfhmcg.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3cigsvsdd.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3jcqsralb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3jzdntjso.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3wqgmybro.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3dzbhjiib.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3tsinvwjr.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3vizxexyw.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3cqpgiqks.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3eoadkrpg.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3zodmzpzv.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3dqmlsdte.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3eitleuum.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3tvwtxhqf.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3idaxizyq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3orudvezn.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bfgqgpco.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3agfkcrvs.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3slwlknsa.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3tqtkhzjq.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3gtmncmhh.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3cdilbbog.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3szlyjdae.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3eoitnerq.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3wrrqubnq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3qjeebhws.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3eecoixst.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3yvhjfqna.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3fitdozhi.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3lmpedzjo.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3kteoenyk.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3awywqbrm.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3nslyurly.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3wzbywmvl.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3lnldaizg.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3qeviuduz.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3zalotspm.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3bjayamqb.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3sjlofftc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3lxociyoq.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3pbsrpxgj.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3xxrucihe.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3eiiplldk.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3bjxsdbbo.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3jxojgqqn.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3zapezqsp.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3uahrumqk.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3dyochbob.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3bvbyvxue.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3hxulvhis.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3gotvnszb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3fqjfnjly.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3pvoocxff.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3pvrxjlgu.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3bdtaobgk.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3pplyedow.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3yaqcsspk.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3hvojxcli.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3brcduoyv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3quteuziv.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3mdpbgsxs.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3plzytdxa.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3xswqjmed.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3duzlhlau.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3qjszhife.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3qmvdayah.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3kvchrtya.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3pqjnwjpi.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dgybwvcc.html


<!-- 参考信息 -->