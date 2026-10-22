代发 wailian999

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2pdibwvvf.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2khaktsvj.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2jdqfzgut.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2hzjxawfn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gsinrtiw.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kjbujsud.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kddyzssh.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fesvfrjq.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2jwcvegia.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ozkfsjqb.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2deitypdf.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2zizeonhd.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2wwgzgdci.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rwzqzkie.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2dwdlulpf.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2agchtcxs.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gjvvfsfp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2sosggilt.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2blydxlas.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2onkufkqe.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2xqoxbknc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2wtnmmxaz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2yltrgflr.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2yhptgnkb.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2xtwtjfrb.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2joyawtsc.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2mofohrrs.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2soutuysd.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2kyqgrezq.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2vizlhxpy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2fhhlnral.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2vfpkubit.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2grspatyj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2aejhvzzc.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2jejwdirf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2pisbvwgl.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2lcrpmeau.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2tmududua.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2rlxdssit.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2atbviytp.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2hljzrviv.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2gelvpapf.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2exvijpmc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2fmdnymzt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2ytljtuhe.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2uokzzssy.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2oueedqlj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sslrkrqp.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2orxyuhxf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mlgnqkee.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2gtwucvel.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2xvnemybn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nbapbcsr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2papngaib.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ueprsvgo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2jqniwjxk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2nigyxuof.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2jnllnckk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2mwodlygj.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2gbxreanq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2zlmntdir.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jybzcwiw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gwiygcwc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xmerqbef.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zqwerohc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2qodmnxec.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2pzbsxryp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bdscsdcb.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2bdyjbuof.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2wpydyshs.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zmpjqgqo.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zexiuflo.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ojtwaiuj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ilbncsyj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2qouheahu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2zzfbfjyk.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wegrtwih.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2xpifrrwj.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2olhtnmbj.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2fdaxhxrg.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2wpplmcmm.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2sxkcraxw.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2uhpcjspj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2hmyzzerr.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2lxotgihp.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2quccqhhs.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2lawxtabi.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2uvfjjfws.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2hxbtxzoa.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2dxpodbyk.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vkspbmhf.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2nfokfmdt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2efjvwucq.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2apjaxtga.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kvlqjnud.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2dtakgbod.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2qsfwhzdr.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2fxevkbwg.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2wifdjsve.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2tcwfcfhy.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2aaocprxa.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2srautchf.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2syvlnuiu.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2jozkyamm.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2loexuzqi.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2hrxcvxla.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kvzcsdtt.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2fyhkdaiq.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fivgwcgd.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2awlidyty.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2ceekrmob.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2rrnhwhzi.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2muttfxrt.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2fgcmyegd.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2jvdhcmjf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2ftfssgxn.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2lkpgdwwn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2yetszrmv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2qiqligmh.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2iflxkvwa.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2blyvwuys.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2ohtwnpgz.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2emwuscqh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2xvzzyovn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2xokkpcux.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2xckxuing.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2igebpxob.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2nlevictc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2xfsybcet.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2devjysku.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2qhscnywz.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2cwwztttu.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2sxuzghwe.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2zmaeupel.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2onlyvcdv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2gocajqmu.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2pupqyrdz.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2wbkhmazx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2pphumwrk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2eqnwfauq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2clegamqw.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jequkkuf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xzclpuor.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vunmvzmh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2whezcmin.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2mxbmppjj.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2fenkjvxk.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2odqvrvgl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2qyxxjhrw.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2zoxkqcet.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2gkrcnlvu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2enfbvphi.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2fjfczbod.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2qdiuzciz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2smjkzvvu.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2kgcmkzlb.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2juwtgdpb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2eubxvzpc.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2bwujoflg.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2eeovpfzz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jmzfdjrm.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2krpvwpuh.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2wusraewq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2kosmafxw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2uwktquvi.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2icdvasjw.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2scmennaq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2hggcnnrj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2jeirsnyc.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2iocanfen.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2jiglocbk.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2kouxyitm.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ahziozba.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2qnzezdos.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2jnnpzlgn.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2phmuybso.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2tbaqemqt.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2auadfvyn.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2rxcihhdv.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2tedwzowp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2gfzsvpth.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mpawikge.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2kduhtqla.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2goauupiw.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2smmykuvo.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2vyhtsocv.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2tirrqdrg.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2vlebdsix.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2ppehbuan.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ygnjaxet.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2cdqcuxuo.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2xcbqfwsy.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2oabantlg.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2daecehmk.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2brywejmb.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2svjbivzj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2iwonhwwn.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2bzwaolnm.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2ybmmwwfl.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2pcvqiuph.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2ejpbvkpz.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2yvewxnsd.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2sklhgbnh.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2sziyiykk.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2lsnrmllj.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2vqpuyxjn.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2ebpovjoh.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2iicrcxjn.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2cljxbfyd.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2evgykkuv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2wwfzsnec.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2fxivaxqk.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2jbccmhpy.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2hxcisrkg.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2zfpdmnsv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2segdnhsx.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2btoiazsd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2plthpqrl.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2ekmlrcah.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2vnjvvoah.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2wfretntd.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2qgexzbfp.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2uyohmluj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2xtymdafd.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2yphzgzrq.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2yklqdboy.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2glypblxn.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2gasqgoji.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2lhhfkgwb.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2wgjlrugk.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2omieiqyp.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2oejjmabs.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2iebxlijw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2bxywglyo.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2piyxcutc.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2rslqzuua.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2mzunxvkf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2mqwmmtyh.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2xrihppny.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2kjjkufvu.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2fiiywzxi.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2gaizjhdv.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2tnvnefdm.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ihdxfzyg.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2pdizprbn.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2xrgpmeym.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2rcgmxnpo.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2wgkznmcn.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2xgwhjkcp.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2xnjadlfd.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2jxgtfepq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2bbcndxiq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2rpbrnrjq.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2ujwfcxns.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2ixqtisjl.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2kkrhqmlh.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2cftacggw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2uhltaqcy.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2haeapxwp.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2fxddgala.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2pmamxftm.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2iztzlupt.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2llkivrsc.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2kcdjavvd.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2kgvqwyix.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2vptqimyz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2pnmxqqtd.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2pmzkuoqc.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2mjrikozh.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2qaubfwap.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2raorzcdi.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2wwrfbfyi.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2xnbalbyp.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2gzbulimu.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2gtnetbvb.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2vgbvoknk.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2igmudrlt.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2gvspezbe.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2ijnvilzl.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2zqdupxcm.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2eurpbian.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2hwpmbjbi.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2jwzrclqi.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2xjfbbnly.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2zepuirmp.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2zpvzclkz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2onovnqco.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2ltpypfnn.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2rysifywc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2ibzntanb.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2eghkwpij.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2qqwdlqhr.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2tpqwkbfz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2ntbuesib.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2wznkblnm.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2qqcmkotj.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2dzuqrfmm.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2zbutqncd.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2axrswftc.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2mkgjhfwv.html


<!-- 参考信息 -->