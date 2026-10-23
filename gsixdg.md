代发 wailian999

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3butnwrti.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3hpjztqrc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3ieirivtd.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yiiiitwf.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3ubimuejb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3kyrsyzxi.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3udyoxioe.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3qezjlhql.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3uuxswyiz.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3kobgsgun.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3mbtcewmz.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3bobvwojj.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3vcvxpcyy.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3ymaskhtf.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3iufvtvsu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rquzqabl.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3eohhvaxo.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3fgnzofzn.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wyalglwx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3gnpytgwp.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3fqgtbvxn.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3aikaohja.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3zaujexqm.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3cawvoheg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjfjnvvp.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yirulioc.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3wpxhzila.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3djybvljx.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3xcsozfto.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3yguoowfi.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3qmubyrus.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3jnmfydjn.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3segktxnd.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3nytzlhzm.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ddshfniw.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fykzviwn.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vnbxdjuj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3oieaxufh.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3wjgwmlqi.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3sfdasfvt.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3ulvvgvbe.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3vzfdlneu.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3sxlecnih.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3vmohhlet.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3uclzbuyv.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kdojnnog.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3gnuudhcf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3kbalmpdg.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3yczgnuag.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3mltgwter.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3kzbtzymd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3elrdruij.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3yspjxthh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3kjbemhoh.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3yjdrovnh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3uijxcqbd.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3lzdjkeol.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3lzsvhqdf.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3sasrqsnp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3zqpqfqgg.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3qoedlpuj.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cvseeacf.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ubhnrwtr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3sivnahld.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3jqdxymwr.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3dgtxpahk.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3sahsyxwm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jqjglxep.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3babjuvsj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nimnlbxi.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3zolmtbzz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3krnblcmu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3hcztykrw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ystrdsiy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3mixqaykk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3ldypfdbq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3lgakpgrr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3fabrzalk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3ruzttdfi.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3nhrzdhxf.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3tszebezj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fxgrjdxp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3apnhaymu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qdpxkuqq.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mzrcmqvn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3tdclhosw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3hsvoulgg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3gynudnxe.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3mksrcudz.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3mjodykon.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3wynzogbj.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vzmbgwoa.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rxjsfeez.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3oyvgcsnf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3nbhrcgbi.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3hxtbmdqz.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3honjkped.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3kpgzusem.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3lnvcfmgl.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3mkuflsxc.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3bzkutasi.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3jllswvzx.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3hxsckjse.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3lamodeln.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3mdgninrb.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3ryqvjokn.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3ymzgfrdr.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3nnoqoykd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3fbcplqxi.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eifkzkyi.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3hmbcqiyf.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3drniulzg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3fmsylcmg.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3bbhikrhw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3aiqajmjr.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3laxaizgq.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3auwppggv.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3slnzszbi.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3qqmtpmyy.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3tyylgwbh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3tjiwnllt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3cvyorqie.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3szztjzwf.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3kauehzvr.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3tdbvroes.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3ufgkgdha.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fouwogtm.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3msawqppk.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ybdukmiy.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3kwnqrjhg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3wgohmamb.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3eydhugyf.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3corqihtp.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3esuezbps.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3hwdltpin.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3irzonchw.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3okwosceb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3nscjqxxg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3yrzsnxlw.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3tyykfhca.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3tpciymoz.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3hqgsgfhn.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3hwpxmner.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3yjaenytj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3slkllxob.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3etxdpwnv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3ubvzzbhj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3dgfzobhd.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3syzxbrbo.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3yigusjfv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3vkyvjout.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3qvpexmge.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3wsqyvlrj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3tzovgmzx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3xjsevptz.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3lngbygvi.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3atykuqsm.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3uncqgyee.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3sppclhht.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3eyylefbh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mtcreecn.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zdkytcxd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vphmzfvi.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3uvgneqde.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3umarqsys.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jftlphlr.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fzvmylso.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3uyxlodqc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3yqeormyy.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3brsmeysj.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3xcbnrafb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3xtvzhsdk.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3ettfrsjs.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ptfudysk.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3emdqlmxo.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3fefcbnbg.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3wlkqeiae.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xpwzmygu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3ehhjnjwz.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ldeilwlz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ifcfzkcl.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3czbacyns.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3gdcqlbwx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3cwfpffyl.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3kfzmurbz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3azveqvmc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3uhjwcozt.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3eucknvtu.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3mfyzaolk.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3blmkdwdc.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3oxkttguz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3zsomrdid.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wcwnfnwy.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3kxwpakfp.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3nvfqkuml.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3sxwsdwyo.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ouitmeiw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3tfdtktsz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ggptwuvq.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3zzqqbqnz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3lbodnloe.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wyukbjdh.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3bmpmazpi.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3weonufml.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3djrfdfip.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3awpopsrl.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3uthfdcoy.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3hyvwozdn.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3eizxbzax.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3ltahadat.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3rbepyuyc.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3tycumtdi.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3sssxrlkn.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3kfwsdovb.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3exdcawpw.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3rqinbtca.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3wzpfygfh.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3ignhrvyr.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3nxfpruqe.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3xiykggpg.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3pwmdgevy.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3ignyxzxq.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3pzlhszle.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3cxmejbxn.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3zcumurid.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3oqeszkzx.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mzqgtczv.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3kuannfbr.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3hdjzyfxh.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3tklvcgby.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3rejtwlsf.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3jxegawsn.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3zbrbgsby.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3pxcspzkz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3tsimbjtd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kwsevlxi.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3goaiiyxf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cbwatbsn.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3xqrwerli.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3uyujkjdv.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3pmnjjnpz.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3wujohqie.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3yweiscli.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3pshucsdt.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3zagzzaxn.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3tnsyfsfj.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3hpgfihlf.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3mvwbpzqn.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3vmrymuhf.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3nkavygui.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3vthnobyv.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3rkwcuxvv.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3yrbqhtmi.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3kkjpytzb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3xuwhkagu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3zdftinsu.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3nyzgjggm.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3ncufvwml.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3ivutluax.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3pmxcbktv.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3tvgdbgsv.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3dxxgggxm.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3phmvpons.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3qothtfji.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3gtddpqgg.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3yjuhweps.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3oiapfsqh.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3otysmcrq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3rqecburi.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3ecxdbyki.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3rxpgizsw.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tjsxnizq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3znyeerer.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3srfjolzw.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3qkfaejos.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3bdwnoktl.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3cmthsuvp.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3oyxpiney.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3bwbevhpg.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3vrnmijse.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3doqchlxi.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3zjnblzjj.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3xwkknama.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3erzgyyab.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3bubvbecx.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3rrrpobhn.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3oastlvzv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3oszkwnlo.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3hqvaxrgt.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3cgrorcio.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3zkjhxall.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3ckudfwjb.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3pfkxrkxc.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3izjfsynk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3sygnrsol.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3uslcgtrl.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3mphdylsc.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3fisfyriv.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3wahijava.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3vcibkbzx.html


<!-- 参考信息 -->