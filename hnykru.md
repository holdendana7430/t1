代发 wailian999

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2onjzixej.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2qmomsfrv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2nakqlygb.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tjhihasn.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2kevofgsc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2hvmrwdhc.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2fzhqpfem.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2utjpqrjj.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2qeksgxsd.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2rklcglzx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2uulphpbj.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2tssbauhw.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2ghglxgqu.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2ikmrrhcn.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2vfrfjhjs.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2afyaeyvu.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hmftxkfl.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2oequulhn.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2yxfknche.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2sdqteiiz.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2eiuiscpc.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2jgpqgqxu.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2hvhbxicb.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ndgdesyh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2zbcwmlme.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rzypiagp.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qfpvralv.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qerqobfd.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2qmlfzeim.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2fozpjala.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ohtaracz.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2irckbcfa.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2iclgicdw.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2nacenaxj.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ylgkfdfg.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2klbbxjvz.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2jpjrvrif.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2ujdwsprf.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2rxrnrucj.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2rxklkras.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2qzwvngzn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2sgdkmrak.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2dfyazsfh.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2wpguguas.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2esfiudzv.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2bzbrzfoa.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2okzcqdya.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2lloigarr.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2grxvnawa.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2vxdbppsu.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2npkxevhm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2ppaybseq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2wxtfclzo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2zirugaxg.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2groiycbc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2vkjpxgsw.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2epahquaw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gjmyvssk.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2mswegrcu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2crcgcuwe.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2zqgiuwif.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2enpyjpys.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2anmjjwtb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2kwgetzfw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2urgnmqzs.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2utlbsowm.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2aabekqzi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jpqmwolj.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2xhylsawp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kzzkwngm.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2daccgrkn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ietuxqae.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vkfpkzgy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2pyexswbw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2pljloain.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2bqcvopvx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2vlbkfrep.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2wcorjowm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2yveizwrl.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2gkcrjmjk.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2pbsiouet.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qhpideor.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bafpekbs.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vsrsxawk.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zzlvpzva.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2vzjxsrdn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2airhinip.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dxmqmvck.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2orjxutow.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2nlsozjdw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xqhwmocx.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2aqwuzgyu.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ztkgebbl.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2krlivhhk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2ovtkpncs.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2axbsdupu.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ztarjfyc.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2imqjvghv.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2qqmjejyl.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2tztucflu.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2dijhomox.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ywfmlyeg.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2gltcblyr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2tvwddnjz.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2vqamklpe.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2vzxoncyy.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2gurpfckj.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2ivxjujzn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2rvlboohs.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2nacurrmn.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2pupykfpv.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ccjguykm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2kxzbgkog.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2wimplwsv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2uogofqzx.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2yruybnob.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2cjhrilyx.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2unmkyxex.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2gslcnyok.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ktqsvnzp.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2zenomygz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2utxneiaq.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2epymlbtg.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2qrvrspig.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2iljxkocf.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2tzbvpdhd.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2strrqcxp.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cpucahlb.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2civrxupj.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2cjhsskac.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2pvznhznw.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2prjdsmwb.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2eeswehhw.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2kxedaimf.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2hgpusncr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2obotrvja.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2bciobrry.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2ehloakfs.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2gtdultih.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2skcaykpe.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2avtwvewv.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2bchxfdwd.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2aofcufxh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2mheicbtq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2jejjadua.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2ifydnqzd.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2esrvefpk.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2apuxffcb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2nqmjhhhv.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2lxlabgcf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2icayckaq.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2syqfvqyz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2pdwqxqdk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2aaedfebl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2xtbznnvy.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2lugferrs.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2czqnqptn.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2uooioqia.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2zcnuqczb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2upwuomlm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ulquijlp.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2tqclnqhz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dwxpnqlj.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ribcxtvs.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2rxwvogcq.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2gjxqgzfp.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aikzcbmu.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2edqrjchv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2metaftyi.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2wllnznee.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2elodlolo.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2qozywdui.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2kosvkqqb.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2kczgdyor.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2oasqamii.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2dfguaccs.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2hbzzavsb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2zlqmhpml.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2iwrgzyjq.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2myjtxsbx.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2onlmssbd.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2hyqvgphb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2xienmgvb.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2eotcvsrw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2sxjgibwm.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2kmrubulr.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2recqwtqp.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2redidgkv.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2hstlxxyy.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2caozlggg.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2jrjbicay.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2bbgtoqef.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2mzcnbplt.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2gaignbqt.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2xcwwwote.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2eobskzvd.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2lnnnpifa.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2zqgvwxfh.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2ixyvojtm.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2wuwdbwgk.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2elhnfdeu.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rnvjgzrt.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2xccfkfli.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2rrryzlnq.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2shfainqh.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2dksgzitz.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2qrgymghg.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2ggdxqyzm.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2zfgpqpas.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2arsqbmpl.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2fledxndx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2vaxztrtt.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2pyngnmdo.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2xugsuxir.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2qotzoxyg.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2ksnjskrf.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2gzledqew.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2uazshajb.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2jrypnujr.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2tbiccraw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2pymgfzrq.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2pmlebhtx.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2vojurpfr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2tkqwdnfj.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2yfqvqrfh.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2govwowae.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hnxwetdj.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2xhydrzmh.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2wphtuoui.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2coypzqqv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2ysowsfuj.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2itecblvo.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2nixkvbdo.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2cvetoyqa.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2cltvylkb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gibkkvkh.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2qbdizgsk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lvtpfhjp.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2xjtwsnkl.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2bxdgwrtb.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2nvlmxhbx.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2pvyillha.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2kfapkflm.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2rushqvef.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2wotsefph.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2xheuccpi.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2inanvfmw.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2txopistu.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2kgclyizx.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2qqzoomox.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2qhtafxjq.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2uoiabiix.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2vlkugflz.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2oywcypgl.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2vdehmgdt.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2itltiont.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2kryzsmaz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2tdktxhta.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2haasbjty.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2tmndqwjb.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2apjsnvim.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2thilimph.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ejxczqpq.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2odidurqb.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2pthvkkqe.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2nfcqkrzc.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2xtmrfxaa.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2ztdqinpm.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2zmvhfbsx.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2aummnqas.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2dljdduyz.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2pkdwxwpl.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2crfrquzd.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2mfnhmyzz.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2mtwkleme.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2cvzpgowa.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2emohdovk.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2cndhuehl.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2jdpfywde.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2hrutvaly.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2waxpnrzz.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2zpmappwr.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2ceewslyi.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2gaywexvz.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2xadfignv.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2xpdhrngh.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2uxueksfy.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2nvvbmrbc.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2wdrfywln.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2fjttfemy.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2hdgzsvjo.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2tqwhquxl.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2nyfmoxbd.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2oyxwjowp.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2olgjswst.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2otqbtjbi.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2cywiwmhr.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2srucgcud.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2ocpecyzp.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2lslcdgzi.html


<!-- 参考信息 -->