代发 wailian999

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ivjbanos.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2ozqmsxyk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2dfyvovwu.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lgabvaba.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2uiboiewt.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2lreqzkpi.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2oxwravvr.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2cspprxwz.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2nldrwdtq.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2hmceijfn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2kfwxotvw.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rtquinsl.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2nfnegdhp.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2lzowvaxm.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2gbnredma.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfgfaebp.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ypushcjr.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2szymvchh.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xbbertgx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2rqilhswr.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2qfgzvrjd.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2twcgibfe.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2lnudijyz.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2jqcjtrbs.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rhijhkug.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2xropuacg.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wsbaqnti.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2sectthkn.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2cmtzvoht.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2wichkyvn.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2fhawlpnc.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2emwnakgs.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2vfxvxoqb.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rmddezde.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mdphackg.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2osqkbdee.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2igxbuosl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2cmsvnnus.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2agxkrvgz.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2rhpxevfv.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2epzdwigr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2hslqbwjj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2ejddtouo.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2wxlbocqx.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2dtzhblnd.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tgjiwijw.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2zqvxbztr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2hkwperje.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2xavmaymt.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2chsaivbz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2ztvjmfmz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxfvlkoo.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2kbkjowhx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2srsmjlle.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2xezgoldw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2hikttjkf.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2eoqakvku.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2awfilsri.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2kigrosnx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2qjbcmohq.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2bcbghbbv.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2frovotie.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gbyvtzqn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2pzotwowo.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2gvlbcvuw.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2umxmewca.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2lzqphoto.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qjwwkrhx.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2hfqeiqjz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rwxctvcv.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2mhvcavuq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2gmdpywob.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2scgmtctf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2nfpeqhgs.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2unzwmgsq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2uemowacq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2dcqcsark.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2tyzfoawt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2flabeziw.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2fpeidlcg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2ewkmcvin.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mhxrfjzb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2uublojgf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2sjzegtku.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qndaqdii.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2fabodilo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2pzpupwxc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kyfyehtu.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2kmtvnpgk.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2dzbpqmgj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2dbcdzhad.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wnpdbcxe.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ofqipyjr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zbrzgbeb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2txhmdzna.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2cijbtnmy.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2wjwojadz.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2pzftideh.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2vvvokaor.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2lvmjtmtq.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2eorwuota.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2gbfbzryw.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2dyfkprid.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2bxneldje.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2plzappzh.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2fnqodwjg.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2dfpesqmf.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2fekkmbat.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2zmujmguo.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vtaubdsb.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2egeqihjf.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bpfdvoox.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2zlvnspvm.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2eskqbrmw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2mapjyhwu.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2lsojsbmm.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2wgetakcr.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2psewnobg.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ahzabfll.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2cbzleqgm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2jcugwtmi.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2xilcugho.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2vyqtgnms.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2qvgxmtvo.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2sdxrlelz.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2cmagrofh.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2lfcznsep.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ydlumwrh.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2cwutmmha.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2usdsfrfw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2kofprnun.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2gsvnklun.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dwamishm.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2sdbudalx.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2pcvnnowq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2dolhxqjh.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2axufschl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2pftdqxdz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2ggqzbojx.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2dibglias.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2hncbnoax.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2ivgaojur.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2asdhjzwy.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2rpkrllpm.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2gsmqtlft.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2ljgjouxg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2rzrcqibu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2tyxdmmvf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2xffwmwab.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2jpsxdgem.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2mqphuveo.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2lmhhmwwu.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2nhkbhgzx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2uqikdfer.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2xuvlcmil.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2ekugjqtk.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2yjfbycan.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2igaaqmqp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2jevmyveg.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bngewfkw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lhqgezxf.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wchvrgtw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kyvqfese.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2igacplhy.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2mvqqdcpj.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hhjojibj.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rwfnlmbu.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2kursbczl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2zleiwxxw.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2szjbtpji.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2yazasjbr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2vmbjiuka.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2vhpeljwq.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2qacbdnvj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2qveffzfo.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2vjilqxbp.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2bviyliaa.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2ihebtpys.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2bavhnhiq.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2hqshidsm.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rdnjexmh.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2kyznlrdh.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2qwqwgypg.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2zrvmlcew.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2lysvfyam.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2khbtniff.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2drcnugyi.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2owcwufvg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2neosozof.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2ifpxrjsx.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2omcyxsdq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2qtvcyvdc.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2qefqnjfy.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2yfvzznyt.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2lmcbuwsa.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2pvqrkbxs.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2frrlanco.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2qnezvbie.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2ipmqrusf.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2tximdvgp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2hjmkcatd.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hjxilbjy.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2zslcnfpe.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2tsutsuql.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2nhbwebum.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2jrvgoese.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2tgmzkjkf.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2kagigzgq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2zvpunvud.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2apbybwpa.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2ceimueez.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2gwefgeda.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2owazdkbt.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2wjmcotdx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2ysmrlydh.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2lkpmuxsl.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2sgohbfht.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2mibbfzts.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2ilmqingm.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2zryashcg.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2vbzhwpvg.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2qpncgvii.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2sdeqjyuu.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2jwdtyfrm.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2nvmjfcqf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2iawbzehr.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2boloqiso.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2zedccvzt.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2fdbsrchm.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2scgcfbce.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2ydrwilci.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2dhhctpez.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2euvfzvhe.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2wpuicste.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2yysafjxa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mwwysqsy.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2ucjcihxx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ubticzsk.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2oxjgszsm.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2dgjssqpf.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2kczhvwlj.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2gbygpeys.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2tbhfxcxr.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2diunqysn.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2zlxkmoeg.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2qdzqjoid.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2udvpawbi.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2yqwsaden.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2ojyoufpf.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2psrnucrq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2zydcfaps.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2gxesbrvm.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2yjntvhws.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2ezsxtucp.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2astsmomp.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2rrrfgkyz.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2wokxgouu.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2jaycnywu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2utauzhog.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2vsqorbdy.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2sssnxfqy.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ekaukmkp.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2zsccdswj.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2enetzsfk.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2gsquxoya.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2tnphjvgq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2exechapv.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2xlrmvagt.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2zawtemjm.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2tkaqmrkq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2luqnynlx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xaqwwkuo.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2eldrcozh.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2kftvzjod.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2fahiljie.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2bclolfaw.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2jwitadlm.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2mlckvjts.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2bxnolsbp.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2skrewddp.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2nyjldpoe.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2akbjjhxb.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2bldgsmbu.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2iqvxifby.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2fwnthrgx.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2ayihgaxd.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2agefsjbi.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2bpzclqvf.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2mxxdwejv.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2xjjxwrer.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2efamgzew.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2nblfclkb.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2tznpwumg.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2zzwpybvt.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2kkoxviwc.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2helfkbrm.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2itismrdk.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2qpbipgun.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2soiglknz.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2uqmvihfs.html


<!-- 参考信息 -->