代发 wailian999

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2leeehxef.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2pgiywyoh.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tsrqldsp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2uucmwvde.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2jechjyjb.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2gazzifdt.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2voclvjmh.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2amuwnhqs.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2afdazlvx.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjclrvlh.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tiesurer.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zvdiivpr.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2meqxbtgh.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2shgbhvxd.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2zpvonvye.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2mkpjkudf.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2wjkbagwt.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xrjhcswy.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2pxczkcay.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2hqdiovme.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2phzidezr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2eahhijjp.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2gqawyiwo.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2kbmarngt.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2jvexmsfi.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2hahteiyl.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2eerojuyg.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2espmgcmv.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2qbmqrboq.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nqbntzed.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2inihvake.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2dcebxvbq.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2bqkdxadt.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2mlpsoypk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2ygwgexeo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zrbqrbkw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2ljzrmalf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2oojbymyb.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2rjekrszs.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2epdgrojw.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2deqwclwl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2sdvtygfx.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2eyebguia.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2gyxdlpch.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2ctvopryv.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jsjruntc.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lsayjurd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2lmggmncr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2temgmmpw.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2fxbqhdzi.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2frfvcqvq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oyrkdyey.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2fxpobchw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qjriowzn.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2vneiroqu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2quiqofjz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ttsfcqme.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2fcykdirl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2umfjbvjr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2cjfhjwdl.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2bdhkvgcd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2vqrhbdhl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2bfahbnnk.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2oaljqmzy.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2pfohilqw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pucrcouj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2itsqzjbp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zvjznsod.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2thlrdfoh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2ilxasajs.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2yjcqgixr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2kqjumxqz.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2rifcztbi.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2xncsgbjs.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ivsscwgr.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2kxpyniuk.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xzszbctn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vpehnwoq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2wdmgxqnt.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2yhrsjlbz.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rigrduwi.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2ankhprjx.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2iiluxyrr.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2miykbpxm.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2xbuvmabp.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2esmocojo.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2tolaevak.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2tsrnldsx.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2anbdozxs.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2pmlrirmy.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2uawylquc.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2nqxefdjp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2zpzujwwx.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ovsbbhwo.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rhavnjut.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2znilmtrg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2jdeuftnw.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2zgjpudqs.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zpzlygia.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2lnajugvd.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2xjgeisuj.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2cerxdgsq.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2uefiixid.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2nbjwrsnb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2tjenzgil.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2enfmlizl.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2hkztvkkb.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2wbwwyrux.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2iceljiol.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2iyrieudd.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pwaenbmb.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ubaqstur.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2nrdypmkw.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2duubmqnj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2ujbswypg.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2jsobizfq.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xdfbnvhp.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2khiftuyb.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2mgjjxype.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2tqyiovgh.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2zufkhmtk.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2lbfootpz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2uobiydlw.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2odziwmvx.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2dcqwdxzx.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2nanacwtn.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2bqkljotx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2lzcmhxhm.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2sdbligbn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2mzqjswfv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2sjmqqzuk.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2bxalygbh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2bsaktgid.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2ohclpcbw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2qmqdenis.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2ibixejim.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2amoapqys.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2smarwbnb.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2qouporos.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2zsryoghf.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2btzpdifh.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2tzxmhqgr.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2dusuxxme.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gwndftoh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hoexjcul.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2josrkfxi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kvksbcsc.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2mjwkesiz.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2ywkwoprh.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2aunalkag.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vgfvwmhc.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cxiddemt.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2wnjfpwbn.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mxugrapk.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2csmxbxvn.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2kvrdudfo.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2yapdfoqz.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2snxoxzqo.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ueqrkmfe.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2fjcsoeah.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2vjaxhnkc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2uppffqdc.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2vnfectfh.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ygsmwyxx.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pldvdpmj.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2vcutkjfu.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ngqeofzf.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2mmlybsjr.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2fsdjephr.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2psektjmu.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2mrhwvnbh.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2kclyhuag.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2xnhjnecw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2wctztkap.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2evxerddt.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2ehsmtbzh.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2kudddqzl.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2cvngjxuh.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2qwhtdeye.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2kfhokdia.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2vuzbhnly.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2hgjcoevz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2vbrarjji.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2vxduiqun.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2qqefgcxu.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2lldtseiw.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2eyrgdsrz.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2cyolhijm.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2ffealvck.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2netisoue.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2kbgyeawr.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2demzprqx.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2giuocrde.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2yjcbogmy.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2dtuvpebn.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2vtljzulj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2ovhmeflu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2riyzwfwe.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2hnkekswa.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2yjorlhdr.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2cmgznfpd.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2okbtbtvr.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2hvvtllba.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2rgohudeu.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2cpdpphig.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2wgtxjoea.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2rtabqzxz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2lamyyqkt.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2vfvhdagf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2gstyhuht.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2djawpwog.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2fjayydhi.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2hsbwhefj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2wvdnxwzv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2pywfpgzs.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2kocjubtw.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2ivxvillv.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2sfdswyvc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2utlnmnfw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sgyehnzq.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2yusdxxmo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uipgftzg.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2pgcllmkl.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2jgrantfm.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2mcjdhdpy.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2gnoxhpmn.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ykzjzrvo.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2gzhowduz.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2rvphvnqo.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2rtdojcow.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2pnkajcnj.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2bmebtryb.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2bgxvipkg.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2gwvqeoxd.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2uuwykrmj.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2hpltiope.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2lunfqpiy.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2taxvkmde.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2warxgjgy.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2hojmrhcq.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2crafvjks.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2vfnrygjg.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2dpznelrc.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2tmnfkjmv.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2seoukcqk.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2vjwpyxpj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2xjzpiyem.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2gysdecrd.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2emaeaanp.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2opwfuuvd.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2unylwivm.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2anuisphq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2iszfbvrg.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2vvfvfwfb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2xmgyqorg.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nzwkfsfv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2kjezxiqn.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2yrozzgya.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2lxozfmxi.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2bhwqadcv.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2jnujxlyw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2edwjuwzg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2jyygcynm.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2prfidlrc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2ifmuizqi.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2njqxrsxz.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2bgwvnfcj.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2afsvhsbq.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2ocxnmeku.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2ixwklfok.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2xdvyaqmi.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2ajrqnzol.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2lgvstmig.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2cehzjbbb.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2dzpaxdxu.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2qroyfvtv.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2ougfveur.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2lzynvlfe.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2irunqdfu.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2bkboymci.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2arqbxzed.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2cejfcxgw.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2hxpawuvl.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2gvvhvqmt.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2apuzyjqc.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2unpqdrmh.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2cyhymdsx.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2ouhmeory.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2tawaoemz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2fnwqacxs.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2hehklhzj.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2syvrbtrj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2vdkduwkh.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2sdigcmxx.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2vwvilyzn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2jftlvrtv.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2cnjtzlbw.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2eyotgpmh.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2jsheqozh.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2okrfmgkj.html


<!-- 参考信息 -->