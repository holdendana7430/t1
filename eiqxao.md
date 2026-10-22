代发 wailian999

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hafsxnhe.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2kqgjgcez.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2oiezgnpv.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2mygrzomt.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2byjtuyho.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2awrixlyl.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2zqjgdjjx.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2lngwdtsh.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2tjhuyrtg.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2csjpmrzd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2axaidezl.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2uybszvmy.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2ftcrpeaq.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2jebzlzza.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2mcgbzyoa.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxegrbia.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2jwunohxj.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rukorxcn.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2dcyongck.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2kallgoqd.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2enwqudni.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2jchvzcpy.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2fktnxucw.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2uapeqqua.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hlyvuoij.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2waaypfth.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zvyuusry.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hmkmucdg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2hxuimill.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ikyitlwx.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2xwngtera.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2jdkijark.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2uyrvzuyu.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2jyjqcido.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xhzjvnil.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2bbxrlcpc.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ywrgglrv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2naeycdan.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2zfflorsd.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2frczztpd.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2elbprreo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2bgjkpphs.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2vwqsugst.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2tyvjjiju.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2fcgprpbh.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2voqlpiop.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2vjrewjbd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2tqmdmfcb.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2jabvcsoz.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2xeyrzpfp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2oyxhfbtn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2dhyxkaod.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2fpsswdgf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2surnsccz.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2duvrkxee.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2mxzjtlkz.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2qvrzhcrn.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2opmrholt.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2xrorzmzk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2tqjenkdi.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2xlezluql.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kldsmtdx.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2hosluyvn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2djwfptnq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2xaokskam.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2obguxrzd.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2arsqhboi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zinrbhkl.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2jctagdij.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2onujbcpe.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2ximreiee.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2lrrqmfyy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gsqclqjl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2pqvnxoof.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2pnetobtc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2xghxqgkj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2nbosmowk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2acpahkso.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2tjmbwkzk.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2aksyhigw.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2cmukjebo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vbmdvdnm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2quzborto.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ihlqccpy.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jxexnycz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2cmjxqsnt.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2ientwllu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wifsxery.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2zbhcfhmq.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2mejjqezu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2bnwynqau.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2fycbjilj.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2osbknlap.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2egyfsyys.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2mlgzvzuj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2hxokvjhn.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2majaljws.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2sfdkqwem.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2eademhbv.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2zpeitfpe.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2voafjbaf.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2erpastoz.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2xwnwykfr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2ykoesltw.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2jlvmqxpv.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2haxulpse.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2xjgxqmdg.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2cdfujydo.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2hllhlblk.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rsmjdoge.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2gnygnsex.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rosjpess.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2czgrwbrg.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2hpmpfmfp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jwcpfyyq.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2oexucqow.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2vwaqjypx.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2hhjaqowb.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2wezwjeor.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ptjgcfmo.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2qhcrlfgw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2szjgkfmj.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2qeoczwfx.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2wsmqmuyf.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2xkgimxqn.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2usbbltuu.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sxivjifn.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cvtapdyi.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2rvrtohdy.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2rcgspnzz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2qgtxwbcp.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2acpdgsei.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2kiaobubj.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2ytbpqalb.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2zluqeodx.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2oixgyggj.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2haqhoxxm.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2nfqokxup.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2yeldtkte.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2rykhimso.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2ykostaqa.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2hwykdyvg.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2qjnmvvru.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2inbdjzbq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2rnfyjkgu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2ihhviyqn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2kcjglakf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkovsgkw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2ddmjsict.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2ugqafopt.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2fmrlfwhr.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2xbakvhrx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2bakfvisc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2hcaoxcdg.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2jexfzkma.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2dektvboi.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2zhzvqydm.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2bdgteezs.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2bkpmyccr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gjwfkxyg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cvykuljs.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vrfijwfz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2viwzdmqp.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zrxawkmc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2mniydlil.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tqsqsdff.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bjegyhby.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2qzfvndqh.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2tgbcwkuc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ttwcrtha.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2uqtrgrpv.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2pjwipvyb.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2onlrsnnq.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2eltwnqsc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2insvevnf.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2hkzhbgdm.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2lldhnucl.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hddtaont.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2tomhegmy.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2jlijekax.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jbywzprr.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2vraadnoq.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dvckgegt.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2vbjcwvqe.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2vbfwtlle.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2kskrhnnc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2ejvikcsz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2vjynwffc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2bwymhufy.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2tjehibbm.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2wnsptfqe.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2ykostpuv.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2qftjhwbb.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2wtjqjtse.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2dwklxtgv.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2spogetgb.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2qcxkfapj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2dipydvqe.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ymsylzon.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2zeolhcaj.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2mhvyjgrj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dbvcdkil.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2mreullvo.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2ffaqqxss.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2zklllqnq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2wyubmqfx.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2dfpsjxmv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2fxrxgeaj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2kbhhvwmk.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2nspjidqw.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2zrupynef.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2htswpwof.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2nvvkizia.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2ywbqohyy.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2ahkgimvt.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2qktkyime.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2adddysmu.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2saygzfxu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2bsjnmcfd.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2iyjxfjos.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2gssuyxin.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2fqpswajr.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2jjsxjlse.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2kxkmcxap.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2ihgfpikm.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2rxfkmhnc.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ldpkjuty.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2yovsrmvv.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2wyeqdwgg.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2bkfffqcl.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2vsashoyf.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2zdtauoko.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2mggmbryt.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2oxcsmfhx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2swkauoyn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tjwbqwya.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2ymimjxuv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xhgjgwkt.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2wyktdowa.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2wigzqqdd.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2hqcwxrue.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2ypsujedi.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2uecnjuia.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2pzxxfyhx.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2orlthcso.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2lggynevx.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2plodtufc.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2hkuabvpf.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2pmisofqz.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2ugnctxzj.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2sncqplrt.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2gxlfsjxr.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2odsmdlrw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2xkbrcnfo.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2rmiojzmb.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2qndpyjbt.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2frvnadqf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2vrtjmjry.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2igunzedy.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2vsxymedf.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2sqafqyav.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2auqqgwok.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2wtweoyjo.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2cbtaltvr.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2cafnjgzk.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2knmaolug.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2qhywkqba.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2xrypywqj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2nzibkhtv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2yrnprvuj.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2newlosvy.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vkhyxuce.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2qnbcjuuj.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2hgnjptus.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2iohxclgi.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2laambwrr.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2vcpnlmkv.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2nhgpnjwr.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2hsjomzrv.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2qlialxci.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2uxojmflf.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2mhenzjwr.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2zointpxn.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2uocuqkuw.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2gjvvmfak.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2xcpvsshe.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2vzdazgbv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2titvyzxx.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2hifgnwum.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2ybyptjbs.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2mkllgqgi.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2xqpamuoi.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2tospxrlg.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2cmfygnev.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2ztadgonn.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2wepnobvr.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2ppxwzeth.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2dppiujaz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2wzexporg.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2iefzimsn.html


<!-- 参考信息 -->