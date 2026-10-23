代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3nmzkcpco.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3fktxmsbx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3ytwzzaiu.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3loxezuts.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xmouoekh.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3hwlysasx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3gkvdflqg.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3isyaafay.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3rvifguwy.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3vzgwsvmn.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3evfmdyqi.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3fkpuxkpj.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3jzxhuqan.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3iiavlovk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3gdxkzmec.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3jltvjhvc.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3evdnddrw.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3ephdoqrc.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3ldxxwhby.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwyjoqup.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nlkcdqef.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tkndyjso.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wfqyiqfw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3mjgzppcg.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3stddxbgg.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3bkptjhat.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mnasoxto.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3kxrwxzfm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rzodenpt.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdkazema.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3srultnny.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zfcifnvi.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3xdbukyvi.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ovisrbbq.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3xlrkgnjr.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3sxefyfrl.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3ivdkzywd.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3yurukzvp.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3cdsnlbnv.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3thvsjikb.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3arylcfqo.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3yccnczzx.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3hapxkcvk.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3kuallaiy.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3knruvuia.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3dslerptg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3rkbpcugq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3bjpjlprk.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3jminhfqu.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3dgklwgyy.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3vqpfvljs.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3ppncmlgh.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3toeglmep.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3tddvwkvz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3cephsodl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3udestdze.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3zxyzehsm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3yztjhmmz.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3pjikmyuu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3nciptgiw.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3hjlymeru.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3yrlvdlnk.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3woojpugh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3dwkvxzsq.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3wrzmgaln.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3aeyexvmo.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ztyqjnjj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3nfgxiuyf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3jszrmvvq.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3ihcgtksn.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3qvgnkjxj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ksywxwcx.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3xppxqkug.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qvumrmuf.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3sageilsb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3jsaebave.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3gwdmixso.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3rlfkbycf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3jgqqnfub.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3xzdtcary.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3pokhwmky.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3ojqsvgpz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3jxsrngaj.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3vnxsrvwx.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3hdqwzujt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zodykqfg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dybrpqqn.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kiojyhgh.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xkynsxul.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3yjbymfqc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3agerdsgf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3akskktpq.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3bkojtaeg.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3rrplqrhk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jimbvrnt.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jcityiow.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3libktvls.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qssizshk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3mienrjka.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3wcpwpgcl.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3slscuuur.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3dybkfavg.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3mtspggzm.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3pojehedd.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3obgthkag.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3bsxzamhm.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3hgasuyyx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3byyfosad.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3ghmaqbvn.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3ckloxddf.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3qbrmdifc.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3fsdruise.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3emobaoer.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gqttogge.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jnwztvcj.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3hysuwyfw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3noljuqvm.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3busxjvwf.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hlidjthr.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3gzwqodqm.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3afkukpno.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3eazymskw.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3unztregu.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3pffrfbvy.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3akicvhqi.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3rnxmxryw.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3jgtlwcuh.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3pcnzomhm.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3pppxhptb.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3tkfivnez.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3elefkxvj.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3shofhcbr.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gujmeeas.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3qqrswqos.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3gdnqagho.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3cistxyuz.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wzzidgel.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3cwqyxsis.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3fdoqqlkd.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3vowssoma.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3mmpibmka.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3tapslpge.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3hbvmopxz.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3fsnuyxbb.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3ijxrbtyx.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3ryjwogsn.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3hvyvjoxx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3adfotbhq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3jdqzuwlz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3lkdprgej.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3wcjiymrm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3otbvyikf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3yqrczdfy.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3tbpwyooq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3qjatunhg.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3fugeblqu.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3xfryrnjs.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3reysrqyj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3opypfgsa.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ewfogmjb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3xgekqjjr.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3wgjewubm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3zkdnzmpg.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3flyeriop.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wnyltspg.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3hqixwkgk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jfcfqhhv.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3uthogpjw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3jrjonmqq.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kykkjhfk.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3zqitassc.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3phqlgupf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3rslcljoy.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3auyzqcft.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3seimirxd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3dtupxweh.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3rmfvcgyb.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3wlrzsbdc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3ilpkiwpw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3twhvvhic.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3yopkqrxb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3tknxgtrb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ukunjiny.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3gsjbueno.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lhbnrtop.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3tzgrgrim.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3iydajqrq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3vpzxxbgw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3midyjbsw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ijmzcbar.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3lndafujp.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3fyjgkxqc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3xhceydfa.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3ncwcvgos.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3grtrdozz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3sgtihwtf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fcldxgfp.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3kvkivzxw.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3lbzupelw.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3ccfxydka.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ziptyfey.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3susvzvyj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3apyxdmbj.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3gfolfcrx.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3lrvbhgod.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3syvxkbqq.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3ahkhhlhz.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3btgadjiq.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3dszduiyk.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3numamhst.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3bdlrxqsc.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3bmojlufw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3vwjybbac.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3cffjkeet.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3gcidtdxn.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3vrjhbixu.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3gdhizmwv.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3mvqneyqs.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3tyjanyqt.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3cmsszdjw.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3uijukkxa.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3dlwrcwbv.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3lcrzduhr.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3qilvvsqi.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3xsoolsen.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3ntclhmcx.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3nshctmfz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3zcyczsfe.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3qiuujwjj.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3fsnkxgfi.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3kslrmupi.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3bwsglebg.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3vddandbr.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3lrzkfgvj.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3krbqomow.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3yafxyplq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3dnvseqiq.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3alwgvuiz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3ppwafsxx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vgltutlr.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3dyuhyoiv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ykmlhham.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3igwdonsv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3ownisxwb.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3wgypjyxn.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3gwosaasy.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3znuawyoq.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3rktgofwi.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3pgcgevbj.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3wyfjcbym.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3tycdgscm.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3thpckmdm.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3gegaozzv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3yxatyrqu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3daekxtpj.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3onhgjkog.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3ilzbgyis.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3vqygynxv.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3gvnvyhmi.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3pukdhepx.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3ssbmylhk.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3etsxmbee.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3uffhhdjg.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3xyrlfupg.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3psbtulpz.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ehitvqyj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3qxpxnoyw.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3klsoqilq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3zrsdahvy.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3nkymswgr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3sdszhkuf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3supfjgib.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3ijwhztxc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3lfaycoax.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3kcuikbuc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3opwfwhdn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3kadhygkz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3epppcbua.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3udjslsib.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3xpzwzyka.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3fdritgmf.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3wyrpeiek.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3ghtpzdxz.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3ktosvoiv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3yrdqhckl.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3ivpeqmjf.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3aqlxhmez.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3oqfqfkoj.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3jlwdqllg.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3oblxdreo.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3sksubpfe.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3agliqqhl.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3unvbqwzh.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3axjpnaua.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3jjuzhxqq.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3wdknklya.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3qejlvqts.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3hjdysufw.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3upcwffni.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3kffzdjiu.html


<!-- 参考信息 -->