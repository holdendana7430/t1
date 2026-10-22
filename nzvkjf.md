代发 wailian999

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2anaelddb.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2kzluayde.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2gcazakgp.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2gogniqrc.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2mmcnujtt.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2gylmvqsp.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2hfekrdjh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2awzmntmk.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2dozoxfgc.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2fbjgkrnx.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2abqsfgpj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2tkgxbuwc.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2kbnehkom.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2znjjsxcm.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xzbocoxj.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2wbzplerl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2khbrqscj.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2byxmmixn.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvygojlf.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yvvnzwph.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2svaqaepf.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2grxtzctn.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2clwfvqru.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2pkawggco.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2mnskgvuo.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mhpuqrjw.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2tbczoiyv.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ilvyckmw.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2arplcwov.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2gpbdtgcd.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2gjommaxf.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2dqqrfgue.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2zogqrhsx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2iqvkoqtu.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2juljwvwd.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2ksjocdgr.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2jkypipux.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2skprjlwc.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2glizdlvd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2awdximqa.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2arzhitio.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2wvmtfjtn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2drgttuvu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vlvdyiys.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2wknvzfbd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2kkrkcvgb.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2arewuoeu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2khpbsdnz.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2qwvqbase.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ditdlpll.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2yenwghoh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2kysqnvjc.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2byxgjran.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tackkfjs.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gxqdqyzz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2gditwxoe.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2gunzgaeu.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2lmjpefre.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2urxpuzjz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tbsydhgu.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2rawyazle.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hyqvteqi.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2fdoevumk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2mcwhezns.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2orwelpcy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2rbwjugbt.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ybqubqod.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2ilfxojeq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2lfykmrkl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2ljipcvxo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2oawdkcyv.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2tnyfczos.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2wabjdqgs.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2lrfhczri.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2heunmtej.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2uvligdch.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wevjfcui.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2vunoowwh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2bhffutav.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dwxlacpy.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2yyycfxkq.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2mbfhswki.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2lghvweuu.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2dtpjcpwi.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2curkdahl.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jvbxbajw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2qtgsuhhr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2wurownnc.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2kcwlijia.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2mdwmvfpi.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2uadafeeb.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ktnpyfal.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2tecjtbpj.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2lhlijbgf.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2fzfbswuk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2lpfialoo.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2dmywbfhc.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2cdljakco.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2wbwyksqc.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2gnjlsfdf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2dqysalos.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2psueqmtt.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2duzjewzm.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lopgddwr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2tdwbxcmp.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2kbmmfvgw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gxwxivlx.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2vdingdrh.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2bgvgmrpg.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2vvnpxsqv.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2fqctzzrs.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2xfaegetz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2pmxeeeuy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2zskydlnx.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2yhjjqxnc.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2sxbpytos.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2vvyukpms.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2pemxhpvb.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gqoubnke.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2foylcbjm.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yjzxhmmu.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2pfsusedq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2anahinkh.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2lwgxokiq.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qoxpmxeu.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2otrzmijt.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2nlvpinhu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2onmaffjf.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2ecpvsmeb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2khskdmwp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2lorhsnbe.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2dcqfrsyx.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2qwrlhedx.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2odporrna.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2xkodnjua.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2nluydysz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2xbcakjcv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2bgfcfzti.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2cugxhzkp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjbqpyyn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2mdvkponx.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2rorkluud.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2ugzundzd.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2rgupmpcx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2rqfiwrrg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2mlivbtaj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2wenvfzmr.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2xibkfhow.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2gqlsbiql.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2voqmzlvm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2qiuaioft.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qptiuowj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2itbwdboe.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2btwlbsnb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wzurxdkd.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2uoptvdmf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2zhippgqw.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hogtqqjv.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ghmuttdw.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2kiuexapl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2aebuuhrw.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dntmsgzh.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2nswszklz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2riatdfjr.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2sugpnruo.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2xivxohix.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2fgvmlzab.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2ldzgjakf.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2sukoaoiu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2onvtztxz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2zpzmqxky.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2shadlenf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2raooyqpe.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2ynulfmsd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2jugrocxs.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2terwptoo.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2lxqztpgh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2nqsmdvnl.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2zvznoken.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2smgalhmf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2znqdbadh.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2rcdpxtwc.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ztsmutwl.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2iqrxnddn.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2faakfcbl.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2qouoiwlk.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2vjdnymva.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2kkyymghr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2nbuxvjaa.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2oqsxmphz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2chwzyzbn.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2fdwfivel.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2kiptwbyo.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2cdjfympk.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2czcdixok.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2rwbbxljb.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2wlqegrlj.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2vtkfqchy.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2fhyzbwww.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2uohhtcxs.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2hbimjcjd.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2romxcwef.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2msgxirpk.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2uueidpbk.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2xqccnuwc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2kjpgyeet.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2xdbocmai.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2ccjxctfj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2lygnokxc.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2vvikwmkw.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2hbyhesvx.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2mclucpcl.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2wluhkodg.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2buuvtdov.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2kyztaevc.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2otqfigrf.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2bzujdcwz.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2kjpzfkcb.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2cnqmxtku.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2lngrgufn.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2grlflvkw.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2mshqpskj.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2dbnecbtm.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2vjokwlfq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2nogkmzdu.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2umbrryma.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2kwhffoom.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2utkewqch.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2okzsmqhp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rqkhfpvi.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2jqimaqpl.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2zebypepx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2xagawaab.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2jtvmayvo.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2aggsfjpf.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2acdekmhw.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2zakkeuhk.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2kxqnnqzj.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2nqnacvib.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2auursfdj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2gqehdcjv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2oskbxxpn.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2kbvmsonl.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2fsevvadn.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2xctmtmsg.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2nzsgiprd.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2xgcgkcsm.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2sftwndpy.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2cbljudos.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2yfgunbzf.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2kslbievn.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2cgivenrp.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2nzhnevpj.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2tatvakuy.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2olevirno.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2nwiarhou.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2qrmaaqex.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2drlnwzvv.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2dzrsnpya.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2ccercvnz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2dcppdhom.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2odognwki.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ptyflwqx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ihtgobov.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2zjrfwfju.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2ozjhqspt.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2lfvguipd.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2hvyxzamy.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2eeotisww.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2wsxzfaer.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2sqydmxvm.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2cfigupgh.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2dgojnkny.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2ecluykoq.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2lilziezp.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2cmxtsvoe.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2axdzsjgn.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2ohreoxya.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2cjsugfhw.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2rvtgjafc.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2xthnctzk.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2zcbnnptg.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2vtinljfh.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2otsmzluz.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2nnmpgsnw.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2nkpuwbzo.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2elxyewck.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2egltowhy.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2emcyfsep.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2gzabeduy.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2sfrukdau.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2mtmktatq.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2fukgxsfm.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2vdaibsbe.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2szeteddt.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2ierzqhfx.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2vxqhyuwe.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2strscuzr.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2taehxhce.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2tscoinkn.html


<!-- 参考信息 -->