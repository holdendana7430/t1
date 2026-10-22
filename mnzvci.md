代发 wailian999

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2zhgyjmgo.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2lndrahww.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2qwrgyyzf.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2wsihxgeh.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2wnrwlhli.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2ktpzxhvk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2wzrygept.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2anyefmfj.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2flbjgpou.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2rhuptrok.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2osefxmfb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bareflqd.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hobazweg.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ahafwkvz.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wfzjhjls.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2vqiigwmd.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2tzmgsjho.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2hdcowssd.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2odtgqkut.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2tteydpdq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qevabgia.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qlkjjtah.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2hdalfumj.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zultkcnu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2dgtwlfxx.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2sntulrnw.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2iprljpel.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2vpqyzynb.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2dbcosqvn.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2fficymwi.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2gsdeioxr.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2peknoclh.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2srmpbuym.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2zczuzhek.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2tkkujwbo.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2higeumly.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2ycionqoj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2makeepxy.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2cxjhzeuo.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2oxcruscp.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2kqulrmuh.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mdjuqssa.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2dvjqidzn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2tapbmdjt.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2mljlltdq.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ehczzjqx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2wugfgjph.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2zhzyjgic.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2bukrbiry.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ybgcuuvz.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2rxmudjxg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2oomxnzyd.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2gkvujmgk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2cqssonhl.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2xnsmkzmo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2amwulpau.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2ofrbmiwk.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2tqhilsyn.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2hdsxstng.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2ziqgkpdn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2jtlkfpad.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2pcfirrvj.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2fvlektno.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sfuntffy.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2bjonvpkl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pvarsahy.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2cikbaokc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2bkuvnnta.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2dssdhwra.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2vxvyvbpg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2fxbtbgdf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2atcrykvs.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2nwmkfhue.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2ldvkcrnl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2xeydacoy.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2mqozuybt.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2pjeuzzub.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2dsfgeabc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rkirhbiw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ppmdalgq.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ydphorqn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2greoaabv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2lbnhafoa.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mmmoovyg.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2topfpige.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2czkwveaj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qonnlkor.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mowhmkzd.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xiimmzji.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2wxhafwqe.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2dcgtzpfk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2gqdoblbx.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qdwcttez.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2ahplxepo.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2ievsfcmm.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2upjktskv.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2tcszyols.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ntayusfn.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2bmfumklf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2cgprysnr.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2rzptorut.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2utanmykf.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2slcpeejj.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2drtsszsk.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2bdgwthyk.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xkysicmx.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2uguimdmd.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nizenqxq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2iylcaiky.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2uqsfhbru.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2srydsttq.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2uxfuciei.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2mguybtbk.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2nvpypyvf.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ubilgtkc.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2rwkcesfv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2zbwcojwf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2ogbuiamw.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2nqnivhpq.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2gybefdnt.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2lrktqole.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2rgfttxec.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mvqjrxdy.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qmubsjel.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2qnapcfbu.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2wpwaaqmz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2yamivien.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2tjcrnkau.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2msklkghc.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2oqxvhlfs.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2xxgcjyoh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2pgczdvql.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2jxzjgwgi.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ohgnkfcr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2ihxpilgr.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2jyjwuxxe.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2wlqgcgvs.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2bntaghhm.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2sjxhvhgf.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2olokbnlx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2lkrmwxvt.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2ntsqmkpb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2bhryzbce.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2ljwgctqf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2dqfufejz.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2hrhjvpxv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2mmgynwfv.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2oeghueqx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2oxkwmyga.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2tkskirle.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2bzzcbnqm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2jaxzhtsl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2pkragblq.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2biafhkvw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2iemqaeep.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lfjjosxc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2elhiuqry.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2uiaxszhm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2otvadlec.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2lbksyram.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2xxpiteqg.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2jpjhogzt.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2byqdetfy.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2foetvobr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2jvkfombp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2wnaftghe.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2baolvjco.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2qqwymrts.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rysfihxx.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2yxvyubxg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2neatpaqp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2srnzblxp.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2syakrhie.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ybywyput.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2naqdsuex.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2zzrzlhmq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dvhjzlbx.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2muswgqgv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2gbznkuxg.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2ugnumpzj.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2rsabkdnj.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2ztxtudcq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2xjvthrsk.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2piuldyxn.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2xhiyotdb.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2xwvpemle.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2mavyavyd.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2qwaeqtti.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2vzipzohb.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2thcwmgop.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2qrkqqtfv.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2rasfisqo.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2wtppqhyi.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2fmwhcade.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2xdmudocg.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ytzzqdre.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2zjysjefl.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ajyyaicv.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2hspxljlp.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2yqcxdiqs.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2dvcxfxld.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2keksoyiy.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2wnizbbds.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2byqpvors.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2hfgqhzxp.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2wuswlsph.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2jxgsmhbo.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2smivmgaj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2ydmcbmtm.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2oywxfelt.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2biijuozp.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2cuqmmrhj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2lexkrglx.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2guycvyyy.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2ymewjwin.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2fvbxdack.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2tlkebzbp.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2aouzklvp.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2toesfypm.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2reqqroni.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2jlbufomb.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2txgcavgn.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2ifemjoja.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2iedrxbdp.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2ysyvvrgn.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2cjqqpnsb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2nxcavbfs.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2hxmndcom.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2swmeoevm.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2bdnabutj.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2jkcvqaze.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fmpslzwa.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2lvpygxto.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2daokgpxf.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2qtrxvhip.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2lpoicktt.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2cjlgkayx.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2hofxfnsd.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2zqkjzljc.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2ukbdqshi.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2ufpftagz.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2aaffljkn.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2wuwfjdaf.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2bdfbtafa.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2qelnhslt.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2addpiifc.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2yjtfzpdd.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2gvoekyxf.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2hwinqnwb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2bvulwpis.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2qmplzyzv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2hpkajzex.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2ervcynxx.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2xcvzpzzf.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2xaotnisl.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2aqpgvdru.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2smopuctp.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2hednawbs.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2vvfjwrhp.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2zvhgjkwi.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2kgiqxhrl.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2surtptlh.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2eufjidme.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2qtiibjur.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2gxvkoldy.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2hcwpplxs.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2daivyuhx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rrrdgees.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ohjzaapg.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2msudzwtr.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2ulkejzkm.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2ylrrwriu.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2qvayakxb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2pqycnkwa.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2kekmpbge.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2lkdefrbo.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2akfaiuug.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2sfoadfzn.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2jreumljq.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2jmkvegfg.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2tlxezekc.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2srgmicid.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2smzyqzqg.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2ebmonjee.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2wffmmugj.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2memgwmym.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2nsouyrfz.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2gomxvmwh.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2vxmsazdm.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2wkzpxwwq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2vcbmcebh.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2drirhvrm.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2lupuhzgd.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2avanuoul.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2bnrwrrcw.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ntdzyvvo.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2qgstvxxx.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2ykthjloe.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2hhfuwjpi.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2gotpzpgj.html


<!-- 参考信息 -->