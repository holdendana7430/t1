代发 wailian999

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3gqomsiiq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3sgaiqldn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3tdvspfum.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pmzlpxhd.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3rpnsfubn.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3tgbuebok.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vmxacfte.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3anjvzors.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3mnvcrzjr.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3nbqqbcjg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3zayufawv.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3hqdlkouo.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3gaadzjfz.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3xslhcgnz.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3ekokqrhx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3flzhfoez.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jccoyfqf.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3zrqgvftl.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iibgsxgj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3lyingatw.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3pinfqhyi.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3sdrblsqd.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pxmziuer.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3tjuyqdkn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wxrlxbhf.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qzvudqiq.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zzfmtssc.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qoucgdmm.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3lnxlruwa.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3qbknieuf.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ntqtzspn.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3pbtawyjj.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3bvnsfiww.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ygsflcba.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gkhsoxvv.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3lsdpgmpe.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3awgcsqlg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3ptirpabb.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3shnrxrek.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3ddnalpgs.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3kbdeaksm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3lmqmwjnw.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3ztsfnkzi.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3skpozbvq.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3djkyqhbj.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3crjdqwzo.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3viyfojnu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3tzjploqb.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3ivacrfkl.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3losiurty.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3peezzkjd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3fdkivztw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3hwzcwhju.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3zubhayuk.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3hvsqyccq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3effnvmit.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3frxtczpc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vjnbavzw.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3gzjifnbl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3krxgvcqw.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3sqjsidbx.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ygbzkyzg.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ytkldjgs.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3xcyeoanh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3eurppknu.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3iwahkrez.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3icpwbefg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uexfvftw.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3yoagiyyz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hqqjaqza.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3bbhaboiy.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3yuxosbth.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3kamtalml.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3blnulnkm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3zvifkypl.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3fhbtwmeo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3wllqmfnj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3yvtszxir.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3fnazevyt.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3oomhutdr.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3psnzlwfa.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dvzckfow.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xqroetcn.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xahzrcuf.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zriophdj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3jyqkrrcp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3kztxxqrk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xevkdyrp.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3rizxetcp.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3vexwvdbp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3zhotzofp.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3mcdbuoke.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qzwietdx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rlzdwfxj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3bktahizc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3yemurktt.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xmdamqfc.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3pdntuczp.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3saqlmink.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ybnnspzz.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3abugxmjm.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3xdleaweq.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3hhhmdoxk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3xrqaupvl.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3oemxavgc.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3wmhdoigr.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3ujnxhite.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3amygecqm.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3ddczwjls.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3llbpzgbv.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3wkadzede.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kslqhmcr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3xnxksruy.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3crtnbrpf.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lugsbbuo.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3hqfvevgr.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3gjgwwurx.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ajjogwov.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3jnfyvjnv.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3dgkrpakx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3qhnkaeed.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3wywqbgev.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3zjlnippi.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3apyyswms.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3hwlroxlq.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3lnmnhnmu.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ysbipzxj.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3eqrwrnde.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3dhbsxlnt.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3zsmkossl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3biscbuof.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3ynvnekkj.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3dklrxvnt.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3vtheevhp.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3rmgvwcnq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3iigwuica.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3texdbkjt.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3fedwsryy.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3gznjceca.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3oxfwwdgg.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3ilttgoql.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3zossqenw.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3olwsbvzl.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3ognjdjzy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3fpaqrjyz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3flmuzlxe.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3ubcjfyzl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3sspxshwd.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3ttwbiuzr.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3uhrdydhi.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3vidiefyd.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3uwvagzxk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3xtpqvwhr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3uijbugec.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3rjylyzcn.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3znylfxul.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3vsgeiwfk.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3hansdvkw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3medpzhbe.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lbyffgby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pgeqrouy.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3yizqjory.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vnlwcrdb.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3cxiuxgnk.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3uvqckycw.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3hxhbfwdj.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rddleblv.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3dqdljiya.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3yuasuluk.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3zdxnnrld.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3blvjmrmn.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3jtuioioi.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3foviztez.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3fuwaioci.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3gktrkkja.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3tvvrsjzr.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3uhbmkdom.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xujnvlba.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3jiohoror.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3nbbmvoay.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3msieafee.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3ngzfmygb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uiqriqcx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ppqcejga.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3bkdzhzcr.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3pjubbgve.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3hjscfmhi.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3txgoikwe.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3alsobgpc.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3tluiwxkn.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3dzcrglzj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3bxzshhdd.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fazcpocr.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3tsivwrud.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3xajdqhvq.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3xmkudvbe.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3pwfhvjck.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3uubphtac.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3mcvwiuro.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3vosnroqs.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3pfappwxy.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3oriuhisb.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3hicahpvc.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3vwwyplcn.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3ohaonyvj.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3iuivkyou.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3nhxibhta.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3lccbgsyu.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3cxymaagc.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3vaacszaj.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3scmizmtx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3pxbgijmb.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3cmuffouc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3igjtsafa.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3vgmbafqe.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3cprxutwr.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3sjlrvmyh.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3ngakdbtx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3duolicly.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3kfohybpo.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3qypqztmw.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3ftdzhvom.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3lyajmxuj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3sbrkcgcy.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3iwzmoiqp.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3gngnogsc.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3sjuveivl.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3izttloub.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3lgdrwpgx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ptyopvuf.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3cthndyyl.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3xzduaeew.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3eqpecxue.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3jatyxmbi.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3lfnjdtyv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yptwsbcr.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3afallkwg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uheqyzoz.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3mntljoes.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3hwkodgjs.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3wzeourrh.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3wwhieuot.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3dmrrhfdz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3eupothgw.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3qemimvxs.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3nbbiwzob.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3hxyqajfm.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3mxhdbmuf.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3ftwfohhv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3xowxfdcn.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3upfwugnf.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3fbntjlhh.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3hclpzvst.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3tximspbx.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3gycrnwjt.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3xgsfmytb.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3nnphjkxb.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3iwvkanys.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3ootrfdxy.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3yzlhvigr.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3hmqgliph.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3dhhqebjf.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3vwlhhblv.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3lfeqctmj.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3eqwszokv.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3vwrrcxvr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3wmxlwest.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3iaygyvam.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3ptkovvzd.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3leriwtsp.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3vvgwohko.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3cvklkcnj.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3dgsnvysv.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3anpyxzbu.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3apdnmfgo.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3sjlzjnjx.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3jpumvify.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3ohmuzauk.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3vlecocju.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3opnotroj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3wbdfepnk.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3ezegefbo.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3cpbxeeso.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3vrqpejhb.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3vjnloeio.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3onsptlrs.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3kivvxdns.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3eijwragr.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3spvanjnq.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3ijbkxrey.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3koavshpm.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3zpregcuz.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3zjrqkxit.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3faupbdap.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3anwxyyvf.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3iujyheic.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3jndeamxn.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3dygmpgqi.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3odgxdihv.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3rtfxudso.html


<!-- 参考信息 -->