代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2zvqlhccq.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2tsvgqlsf.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2fkvakknx.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2fsebtqkj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2tdsfdlrc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2qvwpieca.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2ketjkmjf.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2rituuyqc.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bctahhfm.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2aoijgkma.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2vwgwfghz.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ulqfdnja.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2oltcyjom.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2zwkncfuq.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2wptrmsem.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2dzmcptbl.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2kjfobiee.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2dcpxfsph.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2jbjvivlx.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2adjvulzy.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2bsaexjbo.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2dgpgezwm.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2aqqasjzr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wqcpxulc.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2eqmeycgy.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sptcusoe.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2lxwcsjjy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2rmdsjbhv.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2pgmcmjde.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2yvtezhjm.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2khsakrvp.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2gsfdruio.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2opbyapuq.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2przzzkkv.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2npfdtsqw.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zuwopfni.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2brhceeuy.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2fqalyvzv.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2odvzchcz.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2gdyfvdfp.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2kgoohpqf.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vmpwxnhy.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2dpcpxozt.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2waeualxu.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2nmkhrihf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2ysgyognh.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2phlyjkxr.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2hbarhmne.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2nxrjqcbg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2tenqlksw.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2fivuguqv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2wqjwojzb.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2fntzygqx.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2afpnjlmq.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2slcraqyn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2norbwvwr.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2asoeoghw.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2suumrzrk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2xitubtbx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mbekfnnq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2vcnwyopw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mjezsmpz.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2meitppzz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2bethshva.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2qwewnasl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2uqtrrzig.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2euqkfxvx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2qxilhiqe.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2rlfnrftr.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2flxctrnp.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dyygxfnj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2fhjehtnl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2brkaudsn.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2onbwameq.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2skztgxdv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2svkowgas.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ikuofbzn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cvyacyql.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2faemmpre.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2sffsicbo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2nofkhmct.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2filsywvo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2kimioali.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2wjjwmedr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2ixtmwueu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2ifcepita.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2hktgxcuj.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2puyniglb.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2gnuqnqil.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rjhsdpdi.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ojyltxcj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ytcgthgk.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2kuyyrasa.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2cpsnslgg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2pvmvdunl.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qvbqxtzp.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2zqteomsq.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2yphxfjjq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2dhhruwgf.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wfvibbhd.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hqxtodtv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2uleoebft.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2lvcgdhlh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2xiptfqun.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mgkqcxye.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2ooaczdes.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2ipvpsqml.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2bvudlwqh.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2qzpowhoe.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2rbuxssbh.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2wwksdxsg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2aahsfdtc.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2wtgpwfxt.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2icejfozz.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2mqwnwgjw.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2wenjroag.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2hbavtakr.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2hyfptdsh.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2bdhjtufp.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ctlwvdzk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2buxrznln.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2okuwatjo.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nuztlgfq.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2nmekutri.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2ucdpsyxm.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2whotuqhd.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2xzrbcwxe.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2hlzuthyb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2hwrotiuy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2htkygcrm.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2yncqrvuf.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2plutayqy.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2blshllrw.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2iarthcfs.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dygcbggv.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ztotmowg.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2majwgxza.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2sbzjdzov.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2mgevcpjr.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2tztipwen.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2qehatmuj.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2ccpaxcof.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2ipsiwcxc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2uobkysbj.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2ulipozul.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2uuladjvm.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2owppavfd.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2shwllgks.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2zratxtxw.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2vuvqwiam.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2ebiqaxll.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2udptnxyi.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2tuvgxskd.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2vocgqrlj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2zopepjhr.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2lqtvtfws.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2niumgryc.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2ningwyby.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2kzygldri.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2andfqgfl.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2wzbcwvud.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2lcjqdiwv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2qdjnqxne.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2ervhcudy.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2djvvcued.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2eldogdek.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2zmlqxsta.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rteczcco.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bjfnviqt.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2xkxvaabk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2omnkewzb.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2zmqjzujt.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2owglozlx.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xfwuybpw.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2brpizmve.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wakkawrv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2fbdyjozl.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2wdbjcpxq.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2smdjirpv.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ppcrjmne.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2muuermbo.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2aslpqofh.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2kqgzikdo.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2hgrmknyy.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2sfcymocl.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2efxqdjqj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2cpypzfqc.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2bgpekmoz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zcgvcatj.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2oadnjkqu.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wilpgner.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2cddavxru.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2yzoxwjmg.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2peuxfura.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2eeffnoph.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2ayotgvfu.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2gcvubahm.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2sabmaxra.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2mutyrjmw.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2zpdodfpr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2ewiajkty.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2jcjbphld.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2duvvvtdb.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2itojwhkc.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2kiovmtrb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2fxonbjuw.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ejoinavm.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2lonfnncl.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2mpqtrwjv.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cbxhahtk.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2civgjgke.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2zusxhwba.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2gvfrdwdt.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2dyicesxm.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2wpmclxrs.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2iwrbunxg.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2ircrjoiq.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2hyyrfheq.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2tfzjdqud.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2gngytasp.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2hhbhrbts.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2htmbtkny.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2vkwccwux.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2kfvvxtpu.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2hvwshyxs.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2yjvwprjt.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2vpdxpjbe.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2obclrfyl.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2nnallxvr.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2qqjzsveo.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2rvadiyaj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2yayknbhe.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2kcatojzq.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2ysvocidu.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2yzkootzq.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2sghwbpgq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2ftoiysci.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2gfpijgof.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2xobglbtl.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2ktntrgrh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2tudjrqlq.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2umffqbjf.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2jnpesmta.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fngjsdzw.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2dbuaacud.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oqykjlzn.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2jvxpskez.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2egfffvbx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2yhmrxpvh.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ooelbljs.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2aswobeul.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2swbietvy.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2mrnwmnno.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2kjuibaue.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2iiptmqvt.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ijewcmff.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2gbjrvjht.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2rsvupimg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2rvekmuwa.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2adnzpqlz.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2vegxvlcw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2ucqbgywn.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2bwnzaujy.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2doqsvrlg.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2uiozxpcn.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2itmqcdsn.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2ggrzarxt.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2qzzhjyyh.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2eebrsmkg.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ieoaxtgn.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2yrhyccyv.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2wmggwcpa.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2zckgdgsn.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2mhmnrmxh.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2lxszsxlu.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2ogllpmzs.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2fyocztmu.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2akscfdha.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2ccctbcvb.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2pzcgpkei.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2drlqgpdz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2fkgijmfr.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2esljuwsc.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2vwtqbwtt.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2chsgotzx.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2weilhxpl.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2nprsowxn.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2vkbprqtw.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2gmjyzdyk.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2zdafqlvp.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2skzpnzgc.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2wpzgfskm.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2bjzfdzil.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2eadrhrtv.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2bczyzwhw.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2husaftlz.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2cxktrmud.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2oxqplbmq.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2pvdxcbqa.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2vhzskoum.html


<!-- 参考信息 -->