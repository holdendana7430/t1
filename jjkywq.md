代发 wailian999

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3smqhggfd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3fnmeoztl.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3acruupyg.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3nexqzwbn.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3xgtbgmgc.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3qvmjvppd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3bnraqtlh.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3honcqzsv.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3vptbovsg.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3zxxzjxgr.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3sinfyeso.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hprmcqun.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3creqjffv.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xboflfvg.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vlqboxnz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3wduzbfbl.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3qtnujvri.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3jsvukgqh.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ehdwjgvy.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ybzfmcrv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ewrsuqdm.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bljpceeg.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jpefatan.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pkbhsqnk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3zgfxozcc.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3nzczpenw.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3bnefkgzc.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3teoikntz.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3scftnrbv.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ipsjsfij.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3lfqnvfir.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vfgveukl.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zkxzpccz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3xzjskurz.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3hsqlyoln.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3noqfcxwj.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3gslngozq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3wyjyrhoy.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3cfdwdxrf.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3hcfvnfjn.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3tlmkbglo.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pydpweeh.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3kiznkizq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3qkuxjkac.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3lwclqimt.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vpykhvql.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ncumuhda.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3obgebrzy.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3muplkjpg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3myypqebc.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3tdlkhkcd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3lvnwxdic.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3qqzwmqxq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3gmyzdkys.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3ieuzpwrp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3fqqmnlyy.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3mhcwhwfi.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3okszhqjj.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rjxfjgyc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3bfvtqxaw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3qdvusgus.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3domcaplw.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3aqwswgry.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nbeotgrn.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3vawypljz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lcmlcdiy.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3yecnfqov.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3xmddzyie.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3xjtcfuxd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3zqzwgolm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3vllmczfv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3nczzqhmo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3ximystxh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3jbcmwocg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3pehbuopc.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3zpvoldvm.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3skfyhxkg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3eyzeifvq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mhxvvgwm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tqqmpnly.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ktnzokas.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3vumriezw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3qxpunpfy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zwukhmmg.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ahvvhbgn.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3nkjqikdi.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jxyolxtv.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qfxhhink.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xgvxebue.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bmhwiibe.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3isigmsha.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3pvworhhb.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3twrcylfc.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3mrhkqfdm.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3cygoxfwl.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3pbiywfqw.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3lqpotegr.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3clbqjpow.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3dnodxfqa.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3dolvcqsw.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3zrkomakh.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3aozdqoqj.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3bmmgbgfm.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3wreqfqdn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3bocelhoc.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3odxeqkcu.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xavowsqz.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wmuxloyb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3bymghlfc.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3nyooxlij.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xfsmraps.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3zkoqjrrs.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3zwsjpeqk.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3dvuyodcy.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3zwytqkpo.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3fjcvzcfr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3ccquzwhr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3yeqlkjzj.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3gzlktiaq.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3bmdtbwxy.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3osozeeqw.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3asthzgeq.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hxbedrnm.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3okmumkud.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ogdwfhin.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3udgmtsjj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3hdkkszth.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3cdohpfzm.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3wmtasitl.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3ptoabxmk.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3gojzwosg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3pmgsjpce.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3vfmkjodq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ojlamonr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3hgthgemd.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3kntmhglv.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3onobinqg.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3tizeehfm.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3cdwshbei.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3shsqtlom.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3ipruebll.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3pnhsbetg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3cpcbojvo.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3qdndkloe.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3szbaeiqb.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3xmzhdvmo.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3amfqmhqn.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3gvwaqnbv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3wyyunjwe.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3rqbpizll.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3xyfaejet.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3qqgwrczy.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3trjnbvwv.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3arltggmp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3vzdkyobr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3whwofgdy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xfrhroxk.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3yjpiqihl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3adghserx.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3orhidqqm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3rxnpodzo.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3frjgxkyo.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3zonmfpwd.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3ffrjmwgf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3szqjxnvq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3obtaqhyq.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3dxazhxtz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3uyeonrro.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zgwtxqjr.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3rlthdbln.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3vjetfnhb.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3fyjlnodc.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3gmsgxdsq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3ufoajdcq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3gphfrglk.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3dwlqomcs.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qkqrmmce.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3qvkmwrau.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3okiowdek.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3ygxalxdo.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ywamfqze.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3cnqefims.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3aihiabah.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3rractwjg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3bksjgunl.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3gepkolax.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3wujrttzo.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3nnxilehg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3eufxgxzc.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3fyijmfmk.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3jdaovocn.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3blezolxz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3lvqzeuxf.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3imxrzhut.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3rbtgzufi.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3fuxutwpk.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3teebsduh.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3rhugwmhn.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3etwbjzuq.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3ovupddwv.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3tylehylr.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3yrqskxnj.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3kzcaskgh.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3bhydvebq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3nacbgirf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3ndqrrsyp.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3mujedkcb.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3ekxhczuf.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3cowdkkvp.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3tdjomjhe.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3edvvxugq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3gnsigtne.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3jynvqkjw.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3fecqvtky.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3dwbgkyki.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3ipvtzcgy.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3jozzalxv.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3ifiqggki.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3ohwuzhqg.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3aqwmvfxc.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3cctqvaya.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3qiwdstyp.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zsavhgki.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3anodxcyd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3aeunwfck.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3ywoyugcm.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3cagwntgp.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3qykbnoih.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3inqkcdzu.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3llttkkgw.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3thqmghjp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3curpvumi.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3ihfhrkko.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ahoajssr.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3jesaufks.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3rtducezv.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3hpiyivju.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3krwlukas.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3mlmascyz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3nkiacpay.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3qbpwxvqp.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3lyfsuvsf.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3azdpapny.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3hykdvvxr.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3ssjuwgqy.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3phdfipzl.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3xfrfxwhf.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3rrhodbej.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3zysdifob.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3vouavynw.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3pdgblfpn.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3azvpvkdd.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3xcmyipzs.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3atgkplbz.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3mwyeoqqp.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3zloglvqs.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3mgiuuaet.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3fkioqjbj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3tvylmzfi.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3qprwntfz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3jarvanfa.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3golfnxgf.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ssenphat.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3vmmjbthh.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3yaxadxco.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3icrncspw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3faeeolhz.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3qaadcntx.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3orzvkrey.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3mgoabfud.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3yhxgzshk.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3ketahhjb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3gtpjkcff.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3skartrjr.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3rhtuskjm.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3aeainntg.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qxztjyct.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3leaqbhcc.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3phsndugz.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3akfzxqpn.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3rfqgzkjf.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3ujyopvvv.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3jtrynhma.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3vrzlabpz.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3bqbucyjk.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3jtuavlmm.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3tybmiplg.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3rktbhcnp.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3zozribbr.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3zbjloied.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3bkvugyrw.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3qinjvplp.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3cbzlxstv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3lupmufod.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3blbfzxvw.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ttyrabhd.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3nkcxgetu.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3fadlmuiw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3pvcjwbcq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3pcmhdcgx.html


<!-- 参考信息 -->