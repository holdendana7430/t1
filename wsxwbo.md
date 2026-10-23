代发 wailian999

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3zwbphjsn.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3biqyikap.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3hrtxjpcx.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3jaxzubsq.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3elukhimv.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3busfvtcn.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3xwhazlxg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3nzbthioy.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3otjgtpsc.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jyaksfyz.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3deduutko.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3nacybiwn.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3kfcssxpz.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3vdxydptj.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wdauadnc.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3bavvtiec.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3slidrnam.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3cmexlmri.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qztdhrmj.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3auqfnfoz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3uvubbbqt.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3tfoxlqlo.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3hcpwrazd.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3uhdiobqm.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3hoytkksz.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3wnerfuhp.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3eojntkkk.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hlpkbksi.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3bmwahysl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3crpthfdh.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3mczrrglv.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3tnxsmrcz.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3hbmpmmbf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3itmnwufp.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3fezfpahi.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3iorfzrrw.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3lehqlpml.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3oavpcnpv.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3sjieeujd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3exvenpbx.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3nikoohxo.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3dgrocfbd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3nqtgncot.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3mtxunpko.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3fvjhmpkz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3hdsaqbuh.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3kahailqe.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3cdzzefnp.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3pjdkxxmj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3rtbjydlq.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3fcoaqsgv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3xpfdyjqo.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3ynsacism.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3wwdfuzja.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lhtocpny.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3pbowdedm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3vyczcpor.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3zmqawmtt.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3vfongxqq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jdrybfnk.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3urneryub.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hpqhpnxw.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3rsifucev.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3jlelquzx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3knahczpv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3eetgygvd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3cvkcpztt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3zuxkopmq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3uvabwick.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3lduqzxzd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3ddpjjlai.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3njbkgaqx.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3qoxddbrc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pfbgsqzv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3himesexy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ksgtjmfe.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ujijgdtg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3ldtjsrck.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3analnlxh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tnktanip.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3dvbyviqw.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3kgkyqizp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rzrkwhyv.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3saqrnjqs.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3tdzviwrv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qqfdpdbd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3ytseknsg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3ezylqggf.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ckdwvnyv.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3eruzcawr.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3rtqrowor.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3fybdgajf.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3rjqoiklr.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3injakkzg.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3hbozpfkt.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3vbziekth.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3ulujzlio.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3kvqpgeqf.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3nbblfniw.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3tuoiyunh.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3upwfqiup.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qxuhcoit.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3spuwfpgf.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3diskkynw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3upqvqjma.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3rlssiakb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3njivblsf.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3ffgbbnwj.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3chgzunok.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3opgmruau.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3emtszmqb.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3yykwywmt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3apggnwmc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3ayoimibm.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3bxzevfww.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3simmkmam.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3yifljydf.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3vncpjfas.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3sinxzfzu.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zeaxgssc.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kcwlktcb.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3fftyvzge.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3fkxhtnwx.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3khtrbxun.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3nxzaobav.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3luwbjkqq.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3pzevtsef.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3bjkztluh.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3rnsfmgwf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3uqcwcgsf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3vvsxvgzq.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3ywfaxifb.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3zealwyni.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3ncrgtneb.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3psilerkr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3txicgdyj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3fqnnkfjc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3pkuemsir.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3zywaflgs.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygydjqad.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3frescwdz.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3uswgxbon.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3jxkurhhh.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3umqsqeds.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3nljahzmb.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3hcofbiyg.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3vqiyqbnn.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3doxiwdjy.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3budhpxbz.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3ubobomcm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3mrdrdsfw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3swjaxdbd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ulipspfb.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3vspxlbal.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lgftaykz.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3aettavub.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3mymeptzv.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zcauppwt.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rvzgrmcn.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ijgpcddv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3fzxdzmdv.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3chefghhc.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3yarjvqgo.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3cybmhibp.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3awonkxgi.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3vawauobe.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3zwcqoqos.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3huhlfphh.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3pwkcxood.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bhupsfqa.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3fmcdeowa.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3sajfpizn.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mdafctmc.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3ardoaizv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3taadpdej.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3dfudmvya.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3axihspku.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3klvdpeao.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3rzjsttfh.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3pxfxanty.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3lwlmfuwh.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3uzmyfzmr.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3aspedbsl.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3zvctcpix.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3cevvgbwc.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3roephdoo.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3gwxpkdde.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3nekbrepz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3fovmnvfr.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3beypbdci.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3yoceuoby.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3ockbmcbb.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3zfbpmkji.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3vmtqtnpo.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3wxhdwbtx.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3ovmyovjc.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3dhpiwexe.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3xirqswnu.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3vcptsibd.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3zpyizbbh.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3rworkvdr.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3zkzkbwpa.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3rzpdywbt.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3bddkazme.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3hrhretaf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3quuwayur.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3fylxulhb.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3nqbaehbc.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3zoejgzil.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3qezltxds.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3sxladtvr.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3gbmeqila.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3rtwmogmy.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3fjdlqnkb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3pnlfyjfn.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3npmpvjfc.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3jzwhphqh.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3ujvkkbtb.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3raasyvrw.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3crhhtpkt.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3nmvqjcrt.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3cnmeedsd.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ogakwmkp.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3qsoiwxex.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3vtcwhpmk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3zltlfhpf.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3jpftlmfv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vxcedsir.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3joofyprp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3doojyrlb.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3kzigmdqr.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3tsbuatfp.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3jcrdzopf.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3clfxwqmi.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3gpsnywaa.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3mztaxssj.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3bclvajng.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3hyhabdib.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3tjjvyuof.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3xkgrrquk.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3tarkxgri.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3minigxud.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3fyulbwon.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3kubcboju.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3ritdxiuy.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3mxcdcsld.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3ctxveext.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3pbkowszz.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3nllxarbb.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3giefelno.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3owkknydf.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3lgxmaggp.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3vtmepzyr.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3jgwzlsmr.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3oirffsuq.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3cmcexave.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3rmfskplw.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3biertrgy.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3hrxxcsmx.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3nfmdbdpt.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3ymnwiymp.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3bulqzqca.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3lwplizku.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yilkprsf.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3jsskqnww.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3drpuxtzm.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3tectpjkh.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3opmwgwph.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3cjvqoudb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3hvlqagjx.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3nrpczwqu.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3fvtchrxl.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3wytwqgjs.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3sftmilxr.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3kxtpnyfv.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3zprzwjjr.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3cpdgseen.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3uthwaqvz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3ciziilkq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3eopqmvtb.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3unqqvhny.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3vguitbrm.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3vwprhmfx.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3xabmtkmz.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3mzotmvef.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3mxpcsuqg.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3dgmkzdec.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3khfsevln.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3qweiqgst.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3ozkegbpt.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3mlpkrikz.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3prybortg.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3iyuefjry.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3blfctphu.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3incxgxcr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3hqducbhn.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3gadjhgxr.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3mwnmvdqk.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3zrcxadsm.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3gpozarok.html


<!-- 参考信息 -->