代发 wailian999

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kgvjzrfd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2stalfeox.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2sgivohlu.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wkfjztxi.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2hjcbvxai.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2pvvdkgsv.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2awdjozqx.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2bnyuctwz.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2htcwxzua.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2fwxizfpo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2yjiircij.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xedfqlqu.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2sezhsday.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2kejkwlfk.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2hnfpmpes.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2csplvnfu.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydhdinsi.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vxkivief.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nneaqnnk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2tynppmwy.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2wemiolrl.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2nnhslynv.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2qsffnxrd.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2rqquflys.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tfyzevmu.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2reggfhbv.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aokohyal.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xilppvpr.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2qhuqqftk.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2wjyfigqo.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ttpoykxr.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2oroxaost.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2yzycqeth.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2aqrxrlyy.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2fvgnfrxs.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2irohlfum.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2nsaxlrbk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2gkhqnsbn.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2zjahwgit.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2daeomjcg.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2ulmxmutb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2ualdvnno.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2tzwnclbo.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2bbmalkwf.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2myxzbodc.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2idikonmp.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2wycasvzc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2ssjmnkvk.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2hqxkryyx.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2vcjdjmvb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2omaivesb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2lyvzxusb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2fqkiwjcs.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2tsvumvyz.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2uvgcvxly.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2kogntyhw.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2qntmqdco.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pwfjtoof.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2pymmlewt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2yqhqmxre.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2vzydkyqy.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bhkwjnvc.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2irvcxgop.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2fydfzfxh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2zrrejhfc.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2vihjdabq.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2qmbmcyex.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nwsugcbv.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2qqfjcgki.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gpxxwnjr.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2gyzgbrip.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2wizlranc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fxgvzmhb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ekkkvrvx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2mkqqyonw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2tzeahjnz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2tzugswst.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2vikfwrjq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2yswiwlnk.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2tskfpxtv.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2jggcyzmh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2frgyamys.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jsrbgqps.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mqfwhmay.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nsyswmil.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2brhugzsb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2iqjxivwh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fmiukzle.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2jrhypslt.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2quvxtujd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jstlkual.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xjvfikly.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ibdjludy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2juqaqedd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2hobwuinx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2kvpvkdgv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2nyuqewpa.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2jrpgfele.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2dkfnhoep.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2mourkarq.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2gztiwrrj.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ajnqfaun.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2pswgemql.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2lkqtefql.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2votesuhx.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2jbjamqte.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2ebnivkpo.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2lgievoxi.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2ugqenvhb.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2clchdgwf.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2sazxfsjw.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2djltaomq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2efteyrhi.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2oaatxwek.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2zabzscby.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2qulfxfqn.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2jhwdtrje.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2vjyalhrv.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2kejcffph.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2pewmxwqe.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2mlolkbxw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2heqfoyxg.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2ldynlfly.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2luvlbovg.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2svedfklc.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2xkeqfcdn.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ykkoseay.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2acosbqsp.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2diumhrqx.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2stehikkg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2jmbxfasd.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2zkkehsxz.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xalzcuws.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2wlgxocxd.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2xqnnxyyt.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2kenmfguw.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2rbinkrst.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2kprahedy.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2xybbnamf.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2bvbaqnrn.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2pbckcivj.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2ebrkdduw.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2uyzfyjio.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2hqksvhxs.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2fjdjeliy.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2wwugqchl.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2sicjdrfg.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2flhcvclv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2fyxggwbj.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2mrsufsan.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2qpmdzizy.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2yyyexwkr.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2ujcanmfz.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2bmmxwzuj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2mdedvfkf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2bdthvcgg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2oeiulaie.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2percbwvl.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2wqvynecn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bwjrnjqz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ummrorte.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2fabyjcjj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ssigixrw.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ilzgkxss.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2scbcjwbs.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2oicyhwrf.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2uwhqwksh.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2itknczml.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2mqymwkhb.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2wqpkxqms.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2divjtqry.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2bzqeqwqe.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2pjdpklwx.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2ckvadzxb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2qawnebkq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2rzihliph.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2ctqigree.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2vbqawqhc.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2kkjpzina.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2frquxdwn.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wcrizpeb.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2nggovcax.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2iuuxnkhk.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2vpijqqaz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2nanjhgoc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ntgnlynx.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2qkijlrhj.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2jaiwupav.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2tqxmbpfu.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2jsoevdlj.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2tkmuxbne.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2bdeslfmq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2cxirpgfo.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2wqtnehge.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2jcapmzlm.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2pvydrfcd.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2tedvwdyu.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2gxbttscm.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2eobvakhz.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2hqghcrow.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2gaencwil.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2tjcxhfsw.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2sjcllxnk.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2maebuofx.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2rryiagxh.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2zvtbtmiw.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2ypmejbts.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2jytbkvju.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2casjmfwy.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2xghjjnuq.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2rociukmw.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2cxlvpitz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2wuajstyb.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2vcaoqydm.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2xttlxwwo.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2pxavudzs.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2zbjbctlk.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2ghvdjkod.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2qfemawtf.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2hizgemcr.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2klbumvsp.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2vygizrnf.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2msbaeclj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2pakwetbu.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2ojsdujlv.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2dtgywuib.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2rzpybyqy.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2pxbijkbz.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2tyntikpo.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2omxgqihi.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2vokgptak.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2vjtqqrsn.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2ohlhsvst.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2qeuipexu.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2oilywjyc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hlowbmkp.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2gkungafe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cssgfzes.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2cgyewpyi.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2yabcaqvh.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2bpmogcjw.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2rezuyccn.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2esrczkqp.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2uehyaihg.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2mfkojwgy.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2dpgyvpip.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2wfiugcia.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2vetjnjtt.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2ffcgxjez.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2tvwlbrwd.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2wcpmgeju.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2wkxqgbid.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2jrvrfalr.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2zmwckerh.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2ginwcdlx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2sckadksn.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2gebombjr.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2wdmthsah.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2lfrwzmfz.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2xylnctrn.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2qlrjfglq.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2drcutmzy.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2wmjatdww.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2iwcwjphp.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2fzaiudcm.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2ddkydpzq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2vfxsvayx.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2olmmvzag.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2uqbrlxeo.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2oqlfvvjl.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2tbmkkoxr.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2qldqwobo.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2tuxezefv.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2zwfxbdxi.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2wuyakleh.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2tltjafou.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2ipcolsmo.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2moczzfof.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2ehgzampn.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2jbemitvf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jkfccdfd.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2yxjjxlrt.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2xohjgdwh.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2qnqrjuns.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2pdlyspdn.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2ddqostch.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2pbdvtmhw.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2vofkkusk.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2tbndvhas.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2hslpmilw.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2djsiktyo.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2gfxuohbx.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2zutjgqho.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2petvyytb.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2fqvkavyq.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2sfmaffzq.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2vjleajrh.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2unfbhtql.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2niwwknet.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2eqbqiwoq.html


<!-- 参考信息 -->