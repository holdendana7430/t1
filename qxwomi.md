代发 wailian999

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3sfaenrqg.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3ymgnjbcb.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3oyffpkge.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vcllkjfe.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gubajcrm.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3wsznkgvy.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3djwxzasr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3powlcxdh.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3vdknunfv.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3twzdoice.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3ladzrzal.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3dhqyhdkt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zibudmep.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvlkkluj.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3mczmikum.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3mtvcdcgn.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3oqzagwdz.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3mfjpfbmx.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3resbqwqt.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3yqdjqgym.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3lmvnrdyl.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3zbgmuied.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3useepgrk.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3bsaffwjs.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ouxxsrmy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3scvhtprx.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3erubkitb.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3mdnkjmkw.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3jcwdydeg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3qjuqgbgw.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3puymsvco.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3ayshwuty.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3zrjjpcvm.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3xqleavaq.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3kydxwlgk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3xkulnugu.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3hkcnkbsi.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3bmepgnxh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3wkdsdriy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3mygzirkv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3mdggkkrp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ukcwhuuv.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3lvgbfncw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3ivfzzofl.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3hfieexaa.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3yqvpnouo.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3kpwflewl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3frbahogw.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3qhtkmmja.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hzwukvtq.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hexcwegg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3wjokqasq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3anmqpemj.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3bqitagks.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3htuvkkvm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vgqfnrwj.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3jspjislh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bbojunqa.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3smoyhime.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3uxtlxiys.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ifzbnqkl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3rrsnikzz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3tlokpese.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3yoaadcqv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3uzxxxuir.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3ajipijxg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3pfysmyzo.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3ysrptaku.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3azdxjvuz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3urpkrkrf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3cqmpxvla.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qsdauegn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xidvgzzl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3tjlsayyr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3cdjdktsq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vfvzhqst.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3pieyesky.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3hagmkfzp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3kxthozps.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3yqrvpjlg.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3tyejidzg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jzvreyiy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3qilwzlfn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3hcamthgg.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dlbzufmg.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3kpqwdeho.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3jwuuvaoo.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3bekqpckv.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3pzkcenja.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3molpjfha.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3cvshomqd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3fntllypw.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3gjbiljld.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3gntsldod.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3swyrcczk.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3gzuqxtbj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3hksjxvgx.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3zxdorpdu.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nybypnvt.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wiazhavp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3axudoaav.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3dvgyqdox.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3pgrixzow.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3uuzbbmfb.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3kheefgqb.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3juzvramk.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3hgnlafgr.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3cznziujc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3hkmqmszb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3qcsdazxx.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3xcqyhthz.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3kcztzaxz.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3crdgxhpd.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3wudlumky.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3atuvqnqz.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nmieignd.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3oqyzporl.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3yzyngjwl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3axiyjnfy.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3mlzuyrzg.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uapvctez.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3gtcfyerz.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3vfjqfdub.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3ohdkiqfq.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3zglkvrpb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3qmeqsgmz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3scfzhccu.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3aecmnwjk.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3cyonburd.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3omrswnln.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3nqyapngx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3rygawoup.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3awcjuaxw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3ibytbtpr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3ucmqnmia.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxavjycc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3tefbvzhp.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3jqaurjmd.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3mxksqpzn.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3bkvbvkxl.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3bgfjvfps.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3ytgzwfzo.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3fqbkotjp.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3niooajzv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3lpaipslx.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3cojapxpn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3nzprjcrw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mjizjoef.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ntrpfkik.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3yrjdouyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yzcytrpn.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3agglauhf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3bppvwmzi.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3aahqmnvb.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3fuglbfrk.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bgtzvfey.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3qnfihrjj.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3blgeqjwo.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3davvqpcy.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3zbkemywx.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3coulnmff.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3hakgjnph.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3umtjseus.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3vzulnpvw.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3tdouvret.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3zrutspmo.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3ogqafvjg.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3gcsjbnxa.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3upsjjjtv.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3sdskeleb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3pixitike.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3vdwotikp.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3hwwfbplk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3zrhsliow.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ojkadkfg.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3gtpevvjz.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3gaggoeig.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3qzpdrmyf.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3fwoyhoxd.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3aisyvdyv.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uoqgvygp.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3oozfsgsc.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3pyplvmdt.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3wdkfmhqp.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3hvvohoyn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3yfqnpluz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3lmgxhyaz.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ejhifxwf.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3qszojyux.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rvdgeqpm.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3qcdyretq.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3cbflqixr.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3vctqqmpp.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3gwwygfjb.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3itpzlpkf.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3mstuncow.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3ycukkdgp.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3wzpcrcpb.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3bocqqljc.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3glwfgsez.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3jleuykxe.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3rjbelqwu.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3xgpqmfnu.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3hwwufnxa.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3rcldqijf.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3qxaydvgy.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3fztblugh.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3zljsjqaz.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3loxmmlen.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3ountgdmu.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3xypsafet.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3lowpwxku.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3jnpbxgta.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3fmngwtnp.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3kuimicix.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3xrfazwby.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3nvphsgrr.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3ikgcccwb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3wktvibph.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3okdzzazs.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3cjbwpzoo.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3vkfniixe.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3ljvpuiow.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jbxruusj.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3dypsakrm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yhvdlupi.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3onziqlsv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3odwtdwqb.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3yoazlunx.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3vrsbzjrk.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3mianqjuh.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3lfubdmhp.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3fvnjhzpx.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3lddwxvpy.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3kueangsk.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3nmudosdm.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3iidoygdd.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3vdhadpfu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3mivkmgxa.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3lbpycldf.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3sekwfhgg.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3ieyknqid.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3ovjfnzjn.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3qfwdisvi.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3fbzdmrch.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3ygcaxzxz.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3wpbioict.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3mxxzkljx.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ttmrsmkj.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3iljxficy.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3enbsqkas.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3yrratagy.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3dknbvwsh.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3aqlfnppg.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3olfujyfv.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3mxbxmxlc.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3dzropjwd.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3trezncxc.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3kzpsvqqt.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3snhxzapz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3bcvdoozm.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3sbizemba.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3fguncxnn.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3tcrbztqy.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3oennqbkp.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3iglwshlf.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3xcubityl.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3hasbodwn.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3gjxvexkg.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3pedznnuu.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3rahyvjkl.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3nhczhycw.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3geuocakq.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3pohtqvhu.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3cfpgcmbx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3dbkrkdur.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3kfsdycpu.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3bykaylgw.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3mfyptbwu.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3iupymods.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3jgknjgdm.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ldqgzgit.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3zxqauojm.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3hkofytur.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3bpuazmrq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3jbhmsrhh.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3bbnaxxzr.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3twcvupca.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3wfdwisgh.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3opdxiwtm.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3iakoomoc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3elzzulbj.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3iasekryf.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3fozxksox.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3cqoghrru.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3pkqpraga.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3cvigxglx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3illikveh.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3syjmmysl.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3mdmwnirn.html


<!-- 参考信息 -->