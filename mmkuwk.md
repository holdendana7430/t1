代发 wailian999

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2nydmkyfx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2fdeybnkt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2berhzbgq.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bmsgxxaf.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2eddjmpkg.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2xmgqjcja.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2zkdnvfpx.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2aczcnucn.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rspgtkue.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2hrigmfxc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2pdneftcd.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ozwksvur.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2werypayb.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2cbacygef.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2kmxneghe.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2samgygbe.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2usirdhye.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2klrvslsb.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2yugzqvwr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2mniudrdn.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2sihwoczn.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2zcveiwsw.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ynkccdhg.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ublmuyqv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2cuzkxslf.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bbxqhrcz.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ketmpnmw.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qikforll.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2shszcmap.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2egirgoki.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2iwrxrxfb.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2qizqtvdh.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2faonavhg.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gmyfeuan.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2lmvplzff.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2imrxtsqn.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ttmujxsp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2ekriamyd.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2nrarptuj.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2eszdpywl.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2szuxhwux.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2sqfokfxz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2hubuxzfb.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2syaskgnb.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2dbcmpvnp.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2hqxcgukw.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2dsbxknve.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2pkcahwbn.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2fgnimeiw.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2tblpmwgw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2wtrpjkxt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fhshbtpk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2nqdfhobs.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2twnteaih.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2krlqhsrr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2yhbqdjex.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2yjwvhtif.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xksozglh.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2wrfbzajp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2iaqolkjk.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2bynplwen.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2iltcefzk.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2idlgcvcz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2ihouapzw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2getwxitl.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2gttezunr.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2hxlyykwe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2khmrbnxq.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2vccvnjtt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sauhkvyy.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2cefuglkh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2vnsjnwes.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2ykwxport.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2hnjnldmd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2fmjtiajo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2brbswtwy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2ftwtwkps.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2cirkelfn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2stspfgam.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2qsiacxtc.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2plwtmbro.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2hukpettl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2grcyfdfe.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xbpgafdg.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ixngeafg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2rvyrlpsz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2npykhnto.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2aqzotksl.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2jcxdruzv.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2wtqnqksi.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xghqyvxd.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2qzobejrr.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2uqylvbmi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jqudhpkc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2aqyggorg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2zooocjbc.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2sdskmmzj.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2azhwsjko.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ojecwsdo.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2gyyfntnr.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2vkstqjdx.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ntntwzod.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2cvnbnwjb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2digluhxh.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2gczgtzhy.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2gqkuzavo.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2kfsvpode.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2fciwmlbm.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2hmxutrdx.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2difkfjjz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ptufoxmt.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2kcjxptmg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2pumcefjx.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2aagzifyt.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2sqmmsvvp.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2qpgamubk.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2cmcrqzvf.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ncmrjsuu.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2kuwsoaue.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2mqnxdilh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2hfczfqez.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2gyrfildc.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2clwxctdz.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2wwuzfbzb.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2llaouwtz.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2zuanthry.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2gudfihrg.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2czvffqly.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2hswjuwkj.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2mxkirozk.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2helplzfp.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2jkestfbk.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2dhinyzkt.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2gfmeotgg.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2iktbvmli.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2ezxilpvn.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2pvboeidv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2krhjiakp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2hiqohrjk.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2mfixrvqm.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2ubkfifsp.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2amqzegyx.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2dotmdjuh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2yphxqqrp.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2tmraqtpj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2qtkobdgx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2tiszyfls.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2nuaqequh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2dfiqnjsu.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2fhuhtsfs.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2ckhejldt.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2wyqjiqrh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2mnasyhcu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2zokpydeo.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2bpncehxx.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2wyrwgurn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2qgiwvcik.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2jwckgthv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2lpsxxomo.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bgnbmrkl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pnxvxtfc.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2qubzfmug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ihuirzgv.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2refbfbgj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2ilwhbjqu.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ygajppxk.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gndgrhyf.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2symtdnro.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2vmdbtedf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2bauqwmdi.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2xqthbfam.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2qyigujgr.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2skhnlmsj.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2nawshvnr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2umftfoxm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2ctqbpgak.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2uywopahc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2kbcpzldt.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2nhckipft.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2dnhpejit.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2oyexkyoz.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2auvrgrcd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zswcbztv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2apndxhun.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2ywboboyr.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2eplfacjn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ufyfyalc.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2lcknnotg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2hxrbsuzw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2yfsepjgn.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2igaxhlme.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2lyinblms.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2idmysmnf.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2elzxrtdb.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2vuwdkkof.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ediahiqd.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2dliaxtro.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2cwwihdvc.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2eyojklrw.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2elewszxt.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2ubtmldfm.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dosxejqj.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2iqicaipk.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2iewneduh.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2cxrfpczz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2vepfihji.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2kfsrdryy.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2wssjeshf.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2fusckxbg.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2pclwieql.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2jielidxn.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2danyvpnu.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2gbcklbkr.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2wsroxllp.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2nlfzitrj.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2qkxcljmy.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2cwowgmyy.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2agzavjxi.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2lznfmixu.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2txezmcxo.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2rzkxdvxs.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2uanpilxb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2tmdrffvd.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2oobyoode.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2dchothup.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2xmexdsvh.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2enxoouah.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2iwglzxhj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2mobuimzi.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2mcyhvbhw.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2mxlrqzla.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2ulgzzvia.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2fpfwluek.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2zmeucgzu.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2anffeote.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2chgqsssl.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2xlgbwhzm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2athdzoet.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2gexmqbqa.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2revkevex.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2qkxesqrh.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2hslyfzvk.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2xyqxjhnn.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2udvdgcep.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2xlnhovin.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2tmynnexu.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2wbuwbfyw.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2rulmiyap.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2xymhxxpr.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2odihrwfx.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2ubtnfkcz.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2zvhujfas.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2hkjmxchs.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2puiuudhl.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2rmczegky.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2xlwfjplr.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2kjpmyfqh.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2fzwuabqe.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2jjwcdbin.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2eczrvbyz.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2fbobhowr.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2phcmkpyr.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2hfquctoz.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ivldhrvs.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2bxdoobbv.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2lzyzkvbc.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2qkjlbgbi.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2zvidhxza.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2etxeqoyl.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2tezznsxg.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2dcpwcmff.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nlzvyfoh.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2vxyoeuxn.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2odbxdvwj.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2wubxhlnn.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2qgfdirjb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2nzynwjaj.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2evhohqsr.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2ntkjkqdy.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2jmlyjnyp.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2fiwjinmk.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2joknaoqy.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2ejpattcx.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2kwcqbgyy.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2ffwhztxl.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2tonaqyli.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2uaqecagv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2qgzuawts.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2gbpkxzjh.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2yphjpuwg.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2sgmfahzs.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2nyldyzxn.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2unqymokt.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2uihzvhzm.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2kqzsnbmn.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2stppmmpt.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2jlwsjoaf.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2wcgcgzlp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2brtguvri.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ylljgvmg.html


<!-- 参考信息 -->