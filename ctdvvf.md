代发 wailian999

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3mwcluimt.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3rzvzltvq.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3qobcavch.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3dnvjcpng.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3wfxmiawe.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3ytmfnfoe.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3qfqatnqs.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3nqwcjqkf.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3fcfwvquq.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3erjvlrrp.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3weliyfvm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ieueezea.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttuyvtbo.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fvjqxdyo.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qznzldxy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3rdkgqysu.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3qlosvfjq.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3eqgnhybt.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3rmcblukg.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3hymfljmp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxvmtulh.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aaprwkcy.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vpkkuzcr.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ywfapnmr.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3dtgvhbyx.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3myxmxiyu.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3luxvuoug.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3rwvejklb.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3jiypkftc.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3zlckxmpe.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3tnugnjgu.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3tnxcosdb.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3tjlebcoe.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3ztwaoyeh.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3eoesptub.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3vmorbnzg.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3oodqtfae.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3cjlchwsk.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3kbcynsfr.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3dpuhihtr.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3gwbyyrxs.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ejraegld.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3fimcrtcm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3mvasniac.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3dptestvo.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jaqwiryt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3baotcuid.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3pubkrvjz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3qtpqybhe.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3pxyegyhm.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3iblkgamr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3yttbtclt.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3tyhhkcju.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3suwgadlk.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3vuhzcohw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3nstorhyu.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3sowfplui.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3yokuskjp.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mjkrdczv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3vfpnfpdv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3rmkrmqdg.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3ummaynsr.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3fpnkyrmj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uggnceta.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3syileftl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qqvwyljq.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3lcmzbtxs.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3ujulbdse.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3prlvvblu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ldlogatg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ycuvlrka.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3hadqfsgx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3vxbxyozn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3mffpszyb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3hxbotgbc.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3covopvlk.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3vmtoljns.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dsutoriq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lpqtylps.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xwjjjocs.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ukfgabsj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3ncrkmgfa.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3ccjzsqjr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3hdqsapsd.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3olsijkxq.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3tuxnwued.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3eskolzfk.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rclphaeh.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dnfcouzo.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jvmvqgvj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3ztktaqjt.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3rypzwfmz.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3iietqpnf.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3mtfinhgj.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3mpugycsx.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3qvmvmfcs.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3svvfugaw.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3pjcznmsl.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3vucebciu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3ifwdisji.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3bdbirboh.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3qjkosvha.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3mbjfftto.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3kumshlpp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3kezgazsx.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3zofnxatk.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jqzvkaip.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3crqranxk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3tdubhytn.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3khykbwts.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gkvfvzbu.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3pqkxyynd.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3iejishbs.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ixffmgah.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3moieuhbv.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ntvtbuav.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3tcjxajeg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3zdokjxht.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3kfpdlpha.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3kuemioov.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3gcwzzpqu.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3zgaaeejr.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vvqqffyy.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3iklgzzst.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3dkdqwygn.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3eabmpbyj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3sxnczqqa.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3asonbyxu.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3oayggwbk.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3zyygebvw.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3adtnvyuz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3eobamevn.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3wgrzbzho.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3eavwclsi.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3mfhronvw.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3qyzioyva.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3yobenlbn.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3afcjxpdp.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3qfjsxciv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3pxoczdzy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3pmyescgv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3ngaebmvl.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3dhwaanvn.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3llssylsv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3bxdwzbkq.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3fqgdgzkh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3dgoyrfyx.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3qysdqlam.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3smgxeugu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3egawtjho.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3dkqgalex.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3tseapvhl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3mrkrydyh.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3zhvbwtyf.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3izaegrff.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ebneqzlk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gtboismz.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ajpotrid.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oligrmsd.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fxryrywc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3xnsnjerl.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3sodcdarz.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3ybaeikyq.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xunwtwhk.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3baouwjwp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3jofxyspu.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3qdxkyobw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3eeywlxgq.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qkyegvsj.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3uzawdhhr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3mlzkkwro.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3tpkxaaas.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3gmvfkixs.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3imnuzrdu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3qqqebptm.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3inevxuli.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ucdinayl.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3ygqhnrcd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3ufppyjzc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3gwdskyny.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3baopbfzx.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3jzgipaxd.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3qlsjdkbl.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3zznkieup.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3qpkgffkv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3byswnytq.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3aywodhps.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3dugmgwgf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wbkapeui.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3ecwyisgk.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3unwxmqhu.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3vooawzjf.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3squigndf.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3vpyzorkb.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3hudgtevp.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3jwjyrjyg.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3nvbuzdkt.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dotxbytp.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3kinngifm.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3nujtbjav.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3evejiqvw.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3iqucmyvd.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3cezreepp.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3bskykhot.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3pngioyjc.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3omibtzbm.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3rshafztm.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3tusqsxgl.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3yzmtxnci.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3frusocjr.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3falzbbdg.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3hcjtreot.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3zjjyprbg.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3vbgxflfq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3rtpomnhh.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3xlpcctii.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3swthslmx.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3biudnfhy.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3dloyxqoc.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3tmvbpgcc.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3nsezvbyz.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3xwvnqrbm.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fwdrliqk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3jyotvcjh.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3lghtvfpy.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3ajmtfpxv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3aruxwsko.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3enwpjqcd.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3wlxywnde.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3dmhhjjqp.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3tuohksro.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zuzdwdcj.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3nszrjlim.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cjmjywet.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3wrfkfbfx.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3yhrefoqf.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3qjghwilv.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3jpmvpiyu.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3hwtyfugt.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3qzkilbta.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3kqfeuvso.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3liiyvmcy.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3ifewqvim.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3opbcprld.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3rbbzxsgf.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3veipqqyr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3llixjaim.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3zlunkoif.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3jyluvtkv.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3wahpnrij.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3xuzzmkty.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3bvmnygqo.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3nfshgqqf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3zdfykaej.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3aynedrfw.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3qeltnbbp.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3mejjhzpb.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3shydsqbp.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ipwtdaba.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3fskozajy.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3ugmjwwze.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3izxdmtln.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3lgczsiyp.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3ljxbovns.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3pcxisrae.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3djoqqoug.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3bogchjnu.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3fupuzvzy.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3etqksskg.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3wubixwvl.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3irhebkah.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3bzwjbfyj.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3habrqmft.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3vmiaidas.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3yidieclv.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3lcmctoew.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3mqlegemu.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3mmfojybm.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3lnseqtsa.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3ijliovrb.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3xgzxzquc.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3ydszkvyb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3eiptzipd.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3uqianmgn.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3qlkwonwz.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3aiwrwskd.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3bigxxrnv.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3lsouenus.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3ynqlcvdz.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3fxsocpnq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3ukyaajee.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3tqdrywsr.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3czhczqgz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3jzoiqtlo.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3uthpgcnj.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3flkxptoq.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3egxbayzd.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3whaiendi.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3pjryebil.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3wltetixh.html


<!-- 参考信息 -->