代发 wailian999

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gmokntue.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2nocvlbjf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2ziqlccsl.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jdodoiqx.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2mohklvik.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2owuozwpr.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2byzkcptc.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2ypysdawf.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ifayhyjn.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2qinyyfxj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2btafpqhf.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2cepwzrcb.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2dzsyhysm.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2rppxkvaf.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2csjtegey.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lerrysta.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uoueylte.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gdekimrv.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qxigjxin.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2rjioqzfo.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2qgcmjwfv.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2dlzlbzhp.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vppbhdvp.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2fhhtzbrw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxykzdxl.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2aojcihha.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2exfxicyy.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dvutatyd.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ywullruh.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2trxkzlzf.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2iryagssi.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2lgmtmbkm.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2vmhjcrnt.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xgzuzcob.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wfdubzog.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2hgnvpsyw.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rfrctknc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2ufrbapbw.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2miwynfhe.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2afbyujzx.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2ysdinxwl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2mbvlxldf.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2ispophjy.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2jjivjypv.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2winjpgpl.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2jqnahufc.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2mbcmewkl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2icdlljuj.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2olxagsig.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2dbrygyye.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2ggiktzgr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2piscsyjx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2ppcjrevl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2nhawjlvr.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2turyyhgq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2fgdxcywh.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2qqusgurj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2cysqpjts.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2jddbudsj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2shhfnhui.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2vyfatupp.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2igrhrrmf.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2lcrqhxzk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2ktdokdoe.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2tueujzrj.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2evzmospo.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2fibaajrv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mjymrewt.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2kuipeiqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bpaynvnq.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2nxuahfdq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2lvqjoiwx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2acafvhoy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2rjpgrfui.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2elulbopa.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2yrnbstpq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2qilgmyje.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2xejdojzj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2uwiuqhaa.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2blegmcsp.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2qdfoesso.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zfiteaxk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mrqvkyhl.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pelitjed.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2obbgjqib.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2cawwsndz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2qlfnqbxa.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2uwhvbavp.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2txuhhghd.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2moxolmib.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vpmpbasi.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vknuhgbc.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mgyeqysl.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vztbxldq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2dfneqcsq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2yqeyqpdg.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qcyfkpcr.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2rmbuvxum.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2ecvzfexn.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2pjzdwyga.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2gohlytmr.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2zetjfdlq.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2szinxwlq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2yudjtceu.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2kzdkzcgd.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2xvbxwvwc.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2jltqrfrw.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2nzrfiusb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2wamlpheb.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lhyhilaf.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2dvvsjarv.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2nvmdrupv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2chbfqcfc.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2htzugxlc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hhbiguhi.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2oysnbdlx.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2traejjgp.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2xzlqanyk.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2vpqhkigd.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ilhswvmi.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2wlcwarmv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2ybfkdgsz.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2pxfyodfy.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2ofhoboin.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2aqvbqhhc.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2pfyukehf.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lrguoumi.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fxvinnzg.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2wvbpcljf.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2yivmmuik.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2gazqtfeb.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2kifparva.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2bjfztzkr.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2oulqivkg.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2nbcdomdk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2imauimtk.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2iiqkwesm.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2tuvxinrz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2jozihekh.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2lsqelokg.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2zgrnebyh.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2vfegrkmu.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2qvxllfqp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2ixhummot.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ijvqtbij.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2oydahrue.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2tuzbwpsf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2uldhcfse.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2zsuqcyyn.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2sxgyfbim.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2xomxztjj.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2rlpgxyug.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2ksycxjdk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2jpueyldf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2dtkimndm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2ryerwoau.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2cfhvhkjk.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2kggxbzjf.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2mzurcenn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2phzlkvyz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2isserjuh.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2kvfkafgb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ugcsjhdn.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zusbzmrc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2nfesccnl.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2smcykvvg.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2rvsafeic.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lqolrfnp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2xplpkacf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ronfhnli.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2sbfnmeii.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2asekgjvx.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2csrrzzpd.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2qmdhkrbs.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2oisdatcg.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2tfaoqkbz.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2honipopo.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2wftarlqa.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2slhymtal.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2wtwrlgil.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ghzjsipo.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2szubbdqe.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yavfbzyq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2xwebhdxv.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2keecpohc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2kknequlg.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2bleklakq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2uorbqepw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2dwemcagk.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2tbtlqzdv.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2laxynbbx.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2ptufndmz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2xbkqbzdd.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2gvgqakhv.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2gfmjyebf.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2qcspqedr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2kzoirzxd.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2yqezrsbb.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2rfsapatm.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2rmeabioz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2gtlattai.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2crddciji.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2kywenrbk.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2vapigbhm.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2kmbqckjt.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2fxaadsyn.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2wcuhcyeu.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2xdpgxqkv.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2xhrxtdiq.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2oaaueszw.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2fxgwqtyp.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2eoygxbpa.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2rqfuxaig.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2sanyfpsv.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2pgvpwklv.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2voqpette.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2enxniqxe.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2lqwosvdl.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2rwqmcypa.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2ftjylcjq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2ejkdxljt.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2xfewsgjr.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2yhorlbsc.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2oxcdjsjl.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2chevgbzh.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2uyuocuwh.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wcixfrgn.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2drytbumv.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2ewtlpvqv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2focxxjpk.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2krbaojzu.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2gjebahlo.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2jhvdaefk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2kpfuypcs.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2eonpatsg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fuzyqouc.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2sgnpekyp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2opepioiz.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2kvaclxgv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2kqksrprq.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2yxqieucd.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2qizypjnn.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2yswthesu.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ccgcpojo.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2zqnyqowy.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2qfszihfj.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2mffanfyb.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2gdnpgzoq.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2arzakeqk.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2vaqehetv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2ypiohybt.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2bwlpltkf.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2armncnba.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2bxsaolfs.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2arvdniae.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2ccgllkkk.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2qdmjxtkz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2vmyfjtrl.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2kmrmxwtu.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2dlfojmks.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ickqqplv.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2uqugpmkm.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2pzwegaih.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2uvohubtx.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2ssdsqohn.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2egpkxuhx.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2qazlhpzi.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2drwcsmla.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2rzkqxyal.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2eamkndaw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2kknlpbup.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2perodmyw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2nqiqwjye.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2xxdlngfd.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2zlnrsjru.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2tjhxlavh.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2dudiywmt.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2ehlmgwlj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2jiluoigw.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2nrlbxwea.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2bczmwghb.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2bkgpfest.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2xfzrsjda.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2yygyqdei.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2hvxuzsmo.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2bkutrrvh.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2enmmtuvg.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2ugjolpjv.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2gvspihrd.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2ysszhynm.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2latefbue.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2tftyumqp.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2gsrjrjqm.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2pgusjbbo.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2oshujipx.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2sdeirnaj.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2oaexhkho.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2pugbkmrf.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2xlzaehts.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2rhonayfl.html


<!-- 参考信息 -->