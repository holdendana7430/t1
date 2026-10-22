代发 wailian999

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2mnvlgpye.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2megcmnjl.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xxariuar.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2lyvcjemh.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rdsfrhit.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2ijcgtcfe.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2wckujhhs.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2jizrtxkk.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2vsgccnii.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2bqbvnoca.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2jatffkgy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2unryiogt.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rcgrcijr.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nbeuhelr.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mxbaktwi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2scorfvby.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2wvyxznsy.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2grsszrwt.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2edkeyxus.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2yxoyhcyx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zpepvyoo.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iflcaids.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ytgazunw.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljlicadh.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2rdexntoy.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2metfdojd.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2dwvkxmlh.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2fyipncav.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2mbjvcnfp.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rdgeflfs.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2dozhioqz.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gmjkxptz.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mllwbfzg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2jfcowdzd.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2pwetkybx.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2aebfcktw.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2viuhbvyv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2utyoaewe.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2xbcrjgob.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2qejrcgpl.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2kstscwzc.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2exrmgsui.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2jqlvjzmu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2gateaqgc.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2fdpdjuyt.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2vuidgjlh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2onllwhjr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2htmqjizg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2xciyblej.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wqnkqonc.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2tenszeme.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2bwnlbxjo.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2bzrulcsc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2snyjluvh.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2vafveuov.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2xwzteeto.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2noxroooz.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lmyetuhd.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mkfceifv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2gieaawdl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2dgwqcngl.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2qwmhkwoi.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2qtphjuui.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bxyabald.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2fbcmvwpq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aydvncrf.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2hpbatolb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2bjcycmjf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2xcpdyiik.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2esyozuxr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2tqeltgiu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2vzovugtz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2icyzrjoc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2cyxobvtg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2hsoitptk.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2zyvcixtg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2fbfeqxle.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jlytacqt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2kdatraib.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2reuokpdf.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rzlprjog.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2gfxjvuly.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2zyitmndc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2opyxnqhb.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2tarpkeeu.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2dvttifwg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vlgjbdsk.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2upsfurso.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dbblozoc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2sommyhbn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2lulpzuif.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2xjwxoorx.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2nwpmuiee.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2afprpuqp.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2zbzkswxh.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2hufhukbc.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2cbzsnlwe.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ypotpjgw.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2mtzddjlr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2sikrubsx.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2tnjofgzk.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2zvcwoghd.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2lsdjfmil.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2uipqunxw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2surhndyn.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uexwrjus.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uabyvyog.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2uwpvnxpw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2eguhexye.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2ibtqorvq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lgcbieyb.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2pfpoduoy.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2kgfccrrn.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2gvizkozm.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2pzznojar.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2aeqqhahi.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2rqhswmul.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2cgmkfmxy.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2hxxhkjbe.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2zfkuyobd.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2bjyuintw.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2ujmagthp.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2zxveuqee.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2lndrtdbz.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cwdmqncy.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2gjebadtm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2sfvwgmfp.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2yhdlskek.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2yiwvptad.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2zdokzcmc.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2bbrjzzjc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2wnepumhf.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2izssizdc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2tqpsdyla.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2lsnovxgh.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2prcduwur.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2jbbxiztf.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2otcrpndx.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2vxkmqtqb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2qtvrnhhe.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2xejleaqv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2dnkagywx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2fjvxkvqv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcamfrqw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2pvoyrtff.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2rbeikhgg.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2tsxslfzy.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2uctfgvyq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2oarjnfpe.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2idrsdzyt.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2lsuskris.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2rvnuwedv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2kroeiwue.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2uakjdnki.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2gcolwymm.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2irxvpkee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jqsublgj.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2xkoxejgn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zkcncwai.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2ufuosuhk.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2uekjdoxa.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ykmasgmj.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2yuukkbnw.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2ztiyplfo.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2cnzmjczp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2efempblc.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2hyytwpoh.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2rksuaskv.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2hsrtcmzh.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2yaatbpwx.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2llwbzkbq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2uhurlcin.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2khwktqwq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wddplvho.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2ugmkinkg.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2wsubkpfa.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xkkfzage.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2mxtqepzm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ngacwxmn.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2somyhsrn.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2hdixghgl.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2fxzouswc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2htmlrryl.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2vrdzpnwu.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2bxtabzqv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2jxufhlsy.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2iituzyde.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2tvhzkjqk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2zbybowkf.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2rolmywsu.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2tfzwwmiz.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2iudmhukg.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2yobyfhxu.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2otqksgek.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2hntksltz.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2zjazlbdk.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2gylgxogj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2eeertxuu.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2eqtvzxjy.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2pzinulqz.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2blvvqcrd.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2rurqhccy.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2yxzltjxm.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2dpchhovq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2rlejzsvw.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2uygykywt.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2tyiqbujk.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2jdwgzusb.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2uyjgjier.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ikrpqvno.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2biukpygs.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2lgihlgir.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2zzbpafbw.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2gipxxlwq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2vhuuglli.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2zjoazzmr.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2rkugkqhc.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2lkwbcjuo.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2zwssupyw.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2codvqwpk.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2wjvbkden.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2nuwyyssq.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2qrpfrxyc.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2zoqjlqpl.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2foliupqp.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2vufyrjsn.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2ofepzzzn.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2svcocmos.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2uxkhuoik.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2wykkivgt.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2ndnfjysx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rmqsswym.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2iqdwmcnf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fcmuemjs.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2jmnaxric.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2neekqktx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2biggpzyf.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2feidhpqx.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2dqmljqwy.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2xwuigkmb.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2yvkcljti.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2xvecdzgd.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2wlcacgie.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2jzglozio.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2jeuxlrmn.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2evbqzfnt.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2iseifppc.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2bylmsmqh.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2lklgjvax.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2tccggaqt.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2qozyixaz.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2fdokqhlt.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2fgtuqmmo.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2vawsizca.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2dhwjthlu.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2jejrwutf.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2kzxxsoen.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2mflvpikx.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2vywcrvjk.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2npwqzhna.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2lyialtyu.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2sppqeyxg.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2vqsowzzg.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2lxvhrjzr.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2quzgncdw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2yvujekyu.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2uqqpdmfm.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2uvcdwiuk.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2cqisgwab.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2fxgpiols.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2vgowttgp.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2kkdprqwf.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2muyoazkx.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2hrsdvphe.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2qjftjgdb.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2jerstksl.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2znhmcsfm.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2radwvngf.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2osfjiuwo.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2wmqrwesf.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2wmpefogu.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2kvqhpqgo.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2ysgdscrf.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2fnrszwfi.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2nmosqrzc.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2ttxygvbg.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2apmehszw.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2jteuzgfs.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2uzmngcyt.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2xwnfvrpq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2mziqruru.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2eottgivs.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2uthepufr.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2zfsqiztn.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2eqrsxddb.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2cnzetqjr.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2lyaxygur.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2qaxwcnai.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2jgsmwysc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2ugztnjtn.html


<!-- 参考信息 -->