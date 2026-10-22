代发 wailian999

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ujitvrpf.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2pdtryero.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2hewsdsht.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2tfrxhuux.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2bttccqns.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2ofuocirr.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2uoqwxrab.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2tkmifiyj.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ycqpfcqq.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2fufzqrtg.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mqscvieh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2xqyukkfk.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2ziewxykn.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2zeldlhsf.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2doqdstlh.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2qsruehkg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2sevlmyue.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tuzlmcdf.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vwoclddx.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vpoheszs.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2pgdkfwlp.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2xkndlbwp.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2saxybfeh.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2kmxusofc.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2zoqbyhuw.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2lboyvvhr.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zazaujok.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xjnnqupv.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2egyqkiml.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2oeqqmypp.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2dyvbdbfx.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2ncthtsbq.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2jymqnjrb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2vubnsrio.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2hzargqqu.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2znspzpvu.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2rfnbuzfq.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oareanrj.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2stdkcclp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2ldqoxawm.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2msvpukak.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2eaphnsjs.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2opofzcrs.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2heiyplup.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2jurawqun.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2acrxpgmi.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2gackbdyj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2irlqsmtx.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2mjdjvveq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dbjxatis.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2nyfyjohg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2xbyrziek.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2gsydvuvm.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pkhbwatx.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2uupdiniz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2eghaaxhl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2softxkli.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2fodmwfrf.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2slhkqdri.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kvpukoqd.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2bxstbfkw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wbaicmeb.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2gleojuew.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2wocydhsd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pzimajmg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2wtssazzj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2spqeyhto.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2epuwghut.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2thmzrvnk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2mrixlnrl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2nhacbnsi.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2etiogiyq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2kjdzgpsw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xhorkgow.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pelmglnp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vzagfsis.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tkjovulz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2pjbgmses.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2nbtwbxfl.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2upluyqqf.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2omjqgczv.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2yohucohl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ypjwjpid.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zzlykgda.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2znbrejki.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qpewmkux.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2tyomfbcs.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2qlgacbaf.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vvihldrx.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2gokfsyxt.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2tykzgyys.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2wochkkjr.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2vdpakmho.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ryomqzfz.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2amabboig.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2jyomcfff.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2uunixkwl.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2sgzxlidv.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2cgpqdrdm.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2iqitxzqq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2fzmhgsnj.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2xshsvznt.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bjfeghkh.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2foljmzcn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2dbymwhgt.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2ybxqnqpg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2llecybtw.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2ooiklczd.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2ftggngdf.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2zycewfmi.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2kghhwhfl.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2qesvwlfv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2thuegiqe.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2lvqlaqpf.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2hezvgdbt.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2wndvzizj.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2mifyzwwn.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2xcdumovm.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2legnxuvf.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2nieoowyq.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2utppqvni.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2zcuvqvyp.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2roeqbgpi.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2czddnxdh.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2sdxshvph.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2cgvpvgft.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2paytivps.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2dzlgodiq.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2kfpgoorj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2hwfsutjx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2utlplxif.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2sgtryiof.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2qorulxnx.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2etevkswe.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2mjdnlzwo.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2antnxdjj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2igqsjksy.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2msgqgkca.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2evqckadg.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2cupqtqat.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2iapzrcgo.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2jtvfkiuv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2rolxlfqg.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2lhrfaimf.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2cazqytcy.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2goicirjq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2zmsrigfl.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2wubjrygf.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2kudungrl.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2upqjjbxe.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2fsamqror.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mpymnjyi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uuaashsq.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2dygzsciw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gbvmvahp.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tkgdvjtt.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2jtjdzore.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yxmjapdp.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nkkkrcje.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2aunbjwcv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2rgrowioo.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2xfqmnapv.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2uddzampg.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2fkgcxnkg.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2frpcfvdv.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2msopxbwh.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2rlyswlne.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2vkdlqpce.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2hejcvwah.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xoptglbm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2wzrrmqus.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2lsuhmqjc.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hmtdedov.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2ylazxhuv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ltkslapc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ejqrxtaa.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2laeeevqd.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2vslaopwj.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2jsoqwohu.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2tbvgnpzp.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2iwwsiigv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2hsvefiov.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2ygusforz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ydroeplw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2wzyfhhxn.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ahulclbm.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2xwsoizgu.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2xcjujhzu.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ptgzbmmk.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ubjbbmtr.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ludfaffc.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2btffxnnz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2gquangsf.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jxjthhuc.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2kuuadfme.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2ntrsgiif.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2zfgmdbkb.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2dyzuhlgk.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2dwnecsgp.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2rnseongg.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2syeeyhnd.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2trrahjlv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2vdzeikzw.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2gyyoarqp.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2tgjssogp.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2gxelwmkn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2ecwzkcqg.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2anqjveve.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2bswfcima.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2yaqrdkxc.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2zlarlxef.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2inazfqqd.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2otckdnhk.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2ngjbriox.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2aczxammx.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2dnhrjluv.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2fpnhjhuc.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2nvnxlgpg.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2uwzokgda.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2epsqsvdo.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2fqqzmjbg.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2bypkrqxz.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2kgekhvdl.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2aansrusk.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2gnykbdri.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2wvnzqvdl.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2fonwxwvu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sjkykskz.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2wgmiuyuc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rtuefxct.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2dpubrjna.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2dkkzvqik.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2qgxcgekm.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2gumvpito.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2ozcaldli.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2wrfuxqrj.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2mnetkqkq.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2qbymhhfj.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2ureajzin.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2urxvepdl.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2kxexcjjf.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2orfyyizm.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2tfdmfbib.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2rdasmomx.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2mkgsjagd.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2yppjvbxg.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2aqulvdvl.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2jflagevf.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2rlbkkgti.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2cfzqmpmv.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2nnbxfdhh.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2qtpxczyu.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2sgkfkryq.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2sdecreui.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2nxcxewsa.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2wssoykve.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2nurvzmrz.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2xzrtalaz.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2pddjkngq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2jyowpies.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2zmodgkcw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2vqfuygmv.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2gysftxdh.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2obstcgnq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2jjtzqzxk.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2eniumuym.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2mdpaipgu.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2kdojjwza.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2rojzugok.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2jtsqmrif.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2iipdxykr.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2nrelexnw.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2lzifikhr.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2pxrcqxct.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2jlrfagbz.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2ptlqoztz.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2ywynuejs.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2ajdwaequ.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2zmmxbcud.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2ymimlpiw.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2skntlzvf.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2odabjgfh.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2zmzqezrl.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2gtjbzlmj.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2xwydyhha.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2hfphjnbx.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2bnmnxxhn.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2kxfeujid.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2foijpood.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2keblunov.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2xgabhqzp.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2mcwkdaan.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2jbuxwpir.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2xrexiiqy.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2zpmznfvi.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2rgogdflq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2rdmjlsos.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2eirclybh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2kjcnmafo.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2eoouzmgf.html


<!-- 参考信息 -->