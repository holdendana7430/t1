代发 wailian999

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3izyyncmv.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3lvpskndc.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3oioqugyl.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3pfvnejxs.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3tsnsdhyi.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3zyxenoko.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3mbrhjdgq.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ebixpcms.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3tqbzxqqo.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3gpbbscku.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3ngqqytdo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3gzcuzqtv.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ipcllyvu.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vwcrjsee.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3abffgzli.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3yozmxrkw.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3jakrrofl.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3mbokqylq.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3svzyfgzy.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3tkvxrezz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3chqrgsvt.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3wxqpsfgf.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nheivlfs.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vodsyhwl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3fasiqrzx.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3pighpszm.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3sgjsnkzj.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3oorguacm.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3qqirybyg.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3yvwdduel.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3mktlzqaf.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3foggbtsn.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3uiyattyo.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3pnacackz.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3fpgxdaun.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3gmxmgzef.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3qnbmtjxl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3gqdaihsu.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3ykspbddy.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3ccqmcwyk.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3hxuhahxo.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3orlnbhxg.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3gmoaunmm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3yeqkgfpu.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3haqdvomu.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3pudvqtdk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3bnketowx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwzyvayh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3buomwzpx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3sdqemmqc.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3vkmxbivu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3frcpjupq.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3zonbmeaw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ugqlothj.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3dwwefbsc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3yolubudz.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3wvnfgpat.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3kmsbbwtm.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3udrwfcea.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3phguvsxt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3lrudsegb.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3chbzxsoo.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3nmcnubeu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xedahcgl.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3hjytyoun.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3enwifmfg.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3avjgcmwv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3hllqdrjg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ywlyjwjw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3yfluvnaf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3lephhtgp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3dardpbzy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3tdvlcgpk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3qxdexwcz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3sgqupbef.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3irzpezui.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3dauhkrnw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3eomggyon.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3onxeizjp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ucsibeis.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xvkvizpb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3hwbgkirt.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3tpsvjwjt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3pjftcqfc.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3xgrxgrff.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3qdfnjlje.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rtdvjrrc.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3yqdoqgyj.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ogximwvd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ugxqfdip.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3wxepwvlp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3qvhrixoe.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3pykciymn.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3smmsfqja.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3tqozghnj.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ifirxfgf.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3iouoedmm.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3wuulhqlf.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3rcxitdku.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3evldffvz.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3godonycc.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3bakbwejc.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3jgmcxcpz.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3nsebsuoo.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3ogmpspoa.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3reofyocn.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hcssouic.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3gisoyfkq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3zzfelitb.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3ujywddqq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3tkkrqlae.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3cdjbtrhu.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3gssjupok.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3mvuselgk.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3hlhzlmxs.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3fkjypoqg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3wkujfpbs.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3xjfatpxh.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3agedlofa.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3ddfuuknk.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3fcrjfnin.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3rfhmxrzp.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3gescutvl.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3hwxmvzbo.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3akyrobim.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3ulrktmym.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3pxlbtxxu.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3zxbxerya.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fzqtbgwz.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3wkiabean.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3moahnxjx.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3gyidnkmm.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3acjxxqco.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3jxggerez.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3bexewxwv.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3phmwjfsp.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3acshqrpu.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3ufkfdlny.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3xzwefsip.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3jexliedv.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3ptrjgivz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3kuzkvgxy.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3fbosbvtg.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmevbhxb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3vrikbhqy.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3secwumdk.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3xzescxke.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3zhmzafbg.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3jlvjosas.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3kllurmdu.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3dvxkktho.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3vijnsxyr.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3zvoaqtbq.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3uovcblsj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3loeyuhic.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tfxvsbqt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jubsnpuj.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3plouacas.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vgqsethk.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gkbmumbb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3hnobmelw.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xsxaipdc.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oqtqyejj.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uellaoxe.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3tagxjkwy.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fjpetyfz.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3obuqbnix.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3gnkqtyza.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3yitwulji.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3jqyzgyfu.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3fwtdmffe.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3grvhdzld.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3gnapobmo.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mpifghgg.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3qwpzdfcm.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3vulbkobt.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3myfemegq.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3cfkffhtb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3nyqudtoq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3dmtyscwl.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3xwguzeji.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3goagerbp.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3lnhfppdv.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3ntwkoxou.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3rweadjxj.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3ifvrhmhh.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3ruimairp.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3qdltbmfg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3dfccnmjz.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3syyvafgh.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3ejmocfwq.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3dvcimhcw.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3lzulnqog.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3zbmwwfcw.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3nnuefkvv.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3blukivtm.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3dshinrwz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3zupeklci.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3fjxllydh.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3ohabdpxu.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3oxzckpkk.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3aejseouh.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3rrzmerdc.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3socgqoph.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3egxjxgtc.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3zgprhhiy.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3idiwksew.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3pciytghi.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3lareemhf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3hpditykk.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3grladmob.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3avwejizn.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3lsewopan.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3cuongssz.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3omlilvgv.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3lyhovknf.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3sqeeeapi.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3ovjggiea.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3hupirnys.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3chslpgsx.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3pefabett.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3osipzdie.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bnrnsglh.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3ypsmxrgk.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3yycrkxgv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3nlqdvwps.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3wpqgjwya.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3gtikybvn.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3whdgnjfx.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3dzelkupw.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3hmvuzbzr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vecdidwr.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3svjsjuui.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oqfrvxzr.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3vqoqwrku.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3nfweufyr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3gvxuoycc.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3uazityim.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3wjriodds.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3artweyll.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3wpfyeewd.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3eowlhoau.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3tzgcfflq.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3uywlrfjl.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3wydczbsp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3nnjcpgai.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3lleuwngn.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3onctbdic.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3jzgeqlki.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3fibbnuhb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3ixrognfr.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3mnrwgipo.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3ljjilrdq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3wbaqgqxd.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3pedgsgex.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3bpnlpixw.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3qgfgjlqx.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ptknpfpy.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3lxposfsm.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3dsefmbkk.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3qlrcyjrw.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3zhthfdkx.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ulfkrmqm.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3plllmbfs.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3dourwweo.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3fqsrbrwx.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3pahjifez.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rvlyelwf.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3jskuntgi.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3izhcqqyo.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3xpikinoi.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3ddmblnlt.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3ghqlxfqj.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3udmqoohr.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3pppwfund.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3zcttityl.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3wygdygll.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3jvmgnhqr.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3avpavwvd.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3oixjxkkv.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3yumwpguy.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3mcjicvge.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3twqjqpnt.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3volaqtet.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3giqcfeba.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3qivmxvct.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3uomdfifx.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3iypjezoj.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3uyublbhd.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3uevcgasu.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3xxollrpz.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3tdccfzzv.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3cyicgtoi.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3farvlhnh.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3bjuwpnqy.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3tsvofsqg.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3bngwcsok.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3nsgdiczu.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3mvtmgvwk.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3gzmalulq.html


<!-- 参考信息 -->