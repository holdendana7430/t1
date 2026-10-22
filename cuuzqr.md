代发 wailian999

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2srozwezx.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2smskyxrj.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2vtjjducv.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2cxwkrsyd.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2smbnzruk.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2snihuhuk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2jrayppbk.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2laihxsik.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2ftqfjdox.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2vcyodopl.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2qyvzkkiy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2mftlmqly.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yijxqfzl.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2cdoefkji.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbqtpziu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2gfjxfezx.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2zvwpavqa.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2rclkuibx.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ayjghmbh.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2hqkrwmfh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjxdehsj.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2xtkzrtpm.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rxnnhfuj.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rozpobjp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2vhxpfztz.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2enzmdytl.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2easayipk.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2tjndoqrt.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2pqbdorlt.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ygqhveix.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rukytkgb.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2bbmuyawu.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ekbjribl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2yolwjfmj.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2vvgxffhl.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2khshqxej.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2alqozesh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2haoyegyv.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2bffoimfq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2zyqtzhth.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2eshyphrd.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dvvzpwec.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2psppnsdy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2wxdilcof.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2jxxlvmxv.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2oaacaybv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2pcqoiqjs.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aqjtfyaq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2bkdgctgy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ixobuemo.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2qtjihzzv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2kdfkpwsa.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2wnegqgdo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2evoorvsk.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2iwnqfcru.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2qgaxxomq.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2jtbfwnqi.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2etmsjilq.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nkaaixlp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2yzspvoyq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2ugvxdqrc.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2ezmarjyy.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2bbeikagm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sxyectof.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2czkzkron.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qvorbxvj.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2hhkwxhsk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2mughcojs.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2yqfzdlwr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2zmhkbrzt.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ghpuqopg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2npjgsabr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2blfkmhht.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2oovzpjpx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2ntarorcp.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2ymjhikoh.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2rgfwmvkc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2llhtsoaw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2awwbnnvm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rtadjbtv.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2prsrnzan.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2fcsxgerd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2fmdjsfbg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2swbzkzyp.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2hsxngdzx.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2iqmzugjo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vzsyguig.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rinhniuq.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vfuiquqh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2meftppzt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2vbkxwcrf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2easkwsxn.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2puzxaskg.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2fbvuxava.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2xuzxbwpg.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2lcksycge.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2niwqupey.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2tlhokljj.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2atszwqvi.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2oajcawon.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2uknskqls.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2nyeebqrn.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2bjftjhyy.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2yfkklrgb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2eonrjfjj.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ytfvrjxf.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2lfftoxha.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2envumsjg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2hqmjqvbe.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2hbutnwkc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2pwtmcbhl.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2zkkzlicq.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2pllovbdi.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2xtqofwox.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2qsodggcw.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2brjdzxfa.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2ftlzdkyb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2ukvcedmw.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2tbntprzl.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2zuqrapqt.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2poljoior.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2lyjrufqd.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2drnjdjqs.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2adwieqno.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ywphtzig.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2kbnsatbi.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2elbrorut.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2flhofgtz.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2khilxrdw.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2mucwietj.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2qjvtfbzr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2cinxnekd.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2hsgadiqh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2syylfavb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2hprxqjpo.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2vbskdgmz.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2jglvnash.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2ugebixlm.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2fcbfdclc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2jpzdhfel.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2tjhizgas.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2vjhgzjul.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2tjflgjdh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2bkspijde.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2jqdsffdn.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2ewrzckaf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2zrrgxgmj.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2xazjihrt.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2vxxzolit.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2gysvoolw.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ukbvlwuy.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2vkxlnscl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2dcwsazfv.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2ekjxicxo.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2rzaeeauw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wovaypta.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2clukikxw.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xpxxwmfu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2admgerlu.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ouzltrex.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2fouzybvp.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ptfmebly.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rxplvktd.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sleixict.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2xeynidgj.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2acdjzjls.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ksaxoduj.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2nmzmoigz.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2pekvgovu.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2eoucgroq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2wyuoutfd.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2cqeueaua.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2lewfikec.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dwcsfgxi.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2mscbijfz.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2spflbugk.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ozdgchmb.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2tdwytchf.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bgnrwzvl.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2qkvaqtzl.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2wrcycgqk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2pfmpjcit.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2xmvlbdoa.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2jyoymxce.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2zxaohnzs.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2aqvopvwf.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2gmnkfuso.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2regbqrlw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dwuivbza.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2gjfxqzdn.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2fwuvuipv.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ravvekum.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2cxgzndrk.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2ohmlsqog.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2jvfzhahw.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2snzrhxqv.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2hvidxqxa.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2geudrwdl.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2lwacadtv.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2qoraehgc.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2metyjmcy.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2uowsfjvl.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2qudeszif.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2aotxhnjj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2zduskiby.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2epqrxicc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2nehzwtph.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2fdpmzhae.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2tgryqmku.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2cszgpzsr.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2jvjtgxkj.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2bxgtvhhk.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2dkluimnu.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2xwhycrpo.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2ptaeeuxi.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2ivftmswy.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2wurjwgac.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2qotpjisq.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2siibrmek.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2ddllmnpw.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2mzaxftlf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2xzksbbnc.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2urvounmm.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2gkkjmkfl.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2qudiqebh.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2omdnpaso.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2ikdcshyk.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2qitfzvxt.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2igbwqxqg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2vrkwzqfq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2bmseugpi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iomewxrw.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2ovftsakb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2szoydoma.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2volseylz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2kvtoitmd.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2fhnyfyja.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ufhrjbrf.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2bzhrafqo.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2atrwsjvs.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2kzdbpbgt.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2hceiytxh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2kzxlqkqa.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ploliokk.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2bzzommiu.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2brzitoij.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2yaddxbue.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2lsvxrfll.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2omcjjyal.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2eimnwggm.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2riatkdrx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2yzvvroay.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2ckriqatn.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2zxcqceux.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2apgjqhyj.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2izzqcfwa.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2cnnbizxw.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2hdubssxn.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2yhaavjno.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2kpjeluhk.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2tpodfplu.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2bemgpyzp.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2irsktvnf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2jiwyjhbm.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2rtbhiafr.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2skittzly.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2gitessqh.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cvrhafhg.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2fztexqax.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2vzyoeowb.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2zuxbcmmj.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2xfnbuami.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2ootiojai.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2anujwqnp.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2psskneax.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2qifgrzws.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2ojiidtbr.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2pzdndhtc.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2fbntvowt.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2ybpdzpjv.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2jblnhxps.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2dhorahao.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2jvaqnwyv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2jmnhfjmu.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2szpnxicx.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2cfffhmyq.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2uvvaxrnk.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2tzcingqv.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2eqafrrcn.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2jtgrooax.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2ivrrvkjw.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2jjbxujcx.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2wmhgelta.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2jtmfhcqz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2bhpkcemp.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2phvqwyox.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2bjtmuttp.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2zvzotogj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2ctxmzyqw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2sdvomnxj.html


<!-- 参考信息 -->