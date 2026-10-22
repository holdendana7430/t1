代发 wailian999

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2qdlwuadt.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2zcutjldx.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2bzsnwrwy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2gjtzhtuy.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2qtrdankp.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2vlqhbkkn.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pohdfsvp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2uqrghsfa.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2dvzrvbve.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2hipyjwxz.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2dyuezrqe.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2uyyxivss.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qcjjvsur.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qjkrpoeo.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2poozcfbx.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ueajigoj.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2lmofeqnk.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ibijiuap.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2zgpercxr.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2vdwnlyuu.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2rrfabziy.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2oododunt.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2cduvmnbk.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qshgsksg.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2dqhqfnix.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2dlcdolur.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2bglaoazg.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2axmrormy.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2tzzilpdu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2gbqiovns.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2ujplhlez.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2jnpvxrxn.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2xcotkonk.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aspphrjn.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2oueotbxn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2mgxkqpek.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2ohqqrsqy.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2rbrmputk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2gvtofyqx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2macypxqk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2tticjlqm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2izqbsaid.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2ncydmtcs.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2pploazuh.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2yuilzrij.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2umhniwok.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2aytyedcb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2qownevmo.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2rdulhfrq.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2incjgkbd.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ebejqcrk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2aynopchp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2ttuolczz.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2fnptjgsj.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2rjudhaar.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jvyfedsk.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2zgwnglch.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vdcvsbdz.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2ezgjkhki.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2ftzttyew.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2kervkkbk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2drbseitf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2qbjzavtl.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2gpuuqsmi.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2xnpxvqpc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2xiofewhc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2lztyxkap.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2zgvludgz.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2etjpnrhv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yngsxael.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dkobciai.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2yssbpwnh.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2hxmngzcm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2xdygwjhi.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2dimiqoxa.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kvlohvxg.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2agvatiom.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2sdcexzta.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mvjxbtob.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dakzjktt.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ivwpsqfu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mmnrnidy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2pdkevggf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2pnzphgfa.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ygkdqzvq.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2wsieatvt.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2aoxelbva.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2lfjshthb.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2muzvrgcz.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2cjrxcwfq.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2wjbvqhza.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2umqwcppe.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2lklkgesu.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2aflbwzuo.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2jaewmalp.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2uawfudvk.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2mkbqecmj.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2itbfjwho.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2gbamqwmu.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ewijefgj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2xfzuzyzu.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2merehsdt.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nfwkslxm.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2dgxzxsqw.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2qvoxqzvp.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2tccegden.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2jpdgtwjr.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2kihihltl.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2muookztc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2lwmbmtmd.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2ccbxltev.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2llqmlneg.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2wkljdjrh.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2ejmnokki.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cieecxok.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2weqibpxm.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ugrbxpfp.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2vhvkrlmv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2kngomemv.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2nfllcjdl.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ebhcjhxi.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2zzxmjttw.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2jntkcyvc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2oaryrrck.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2ggkushon.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2wljhbyfk.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2vyeffwxv.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2bquvqrcv.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2smyknlpb.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2jfnzelvg.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2vlkzjvha.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2nxeulqqp.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2nifzixmr.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2unzkbiey.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2zpsxexlh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2paqkadbr.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2aqbckvnl.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2okrlxfrd.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2otlegsli.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2mlkburhb.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2tefnjyus.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2mzazmdqj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2pwzlnjrd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ligzjimy.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2llvdfaso.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2vzsnqarj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2kxsetydg.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lkkotomf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eyflenjh.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2zhxxnkfy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2srmtylln.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2xusvspzn.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2nmonakuv.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hgdueowi.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2zrfikqgt.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2usrlsoow.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2xzemrdcg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gcwewrdo.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2bbtkrkvb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2glbsrqvv.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2whnucykj.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2clqewjeg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2etdlatos.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2redgfpxn.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2jnplaxue.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2osqrsszp.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2zfdqzebh.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2ceufordm.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bctvomgf.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2moaupfgu.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2cjaladnp.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2whiqnymw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2rvygirjo.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2lzkmkkry.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2vtfckhql.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2vukzdxah.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ikiwhcci.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2qqtyawiq.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2angwckkf.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2wwnpaict.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kzdwcloc.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2hpkuaspq.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2gbmteduj.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2cdfboguu.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2wtoaggyo.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2rwwhlhfz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2cfffcbgg.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2nzjpxinz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2ehuunhvg.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pcknfifk.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2pvqesdbk.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2xvkccozu.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2izugnlng.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2uzwfhypi.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2ylsdzvzh.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2cpzprygh.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2ejwqwzbq.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2sncxrawl.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2yphjhlzq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2hwzuwnvd.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2hpskzryd.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2ebreeuor.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2ymrsgxhk.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2gzcwdirj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2knyvbnfx.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2owkcmpus.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2cxeqvwhg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2bsdbwktq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2gogdbree.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2yxvmsjfo.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2ibmwfonm.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2cddvmkzd.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2aahqrjjd.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2azfdlwre.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dweaiolo.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2jywixtsu.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2gummktsn.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2wcmegtzs.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2evhtrlqh.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2yxqxobnt.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2lldjpwnp.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2kbjiqsyb.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2chtedmpe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qzksyeeq.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2arzlyhng.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2evgjmsqf.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2ifclgpzk.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2sffupaew.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2ejaguuwe.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2qkaqqkiv.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2nfkwscrn.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2eixgqtdt.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2gqvcbqnd.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2uausdcxa.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2iepaqyyw.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ofpdabqv.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2mcqpfjyz.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2wotcwval.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2olllbboa.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2wkllkndj.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2jwggiakd.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2igqhaamw.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2bpwkwewc.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2gzsrnjsa.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2yxfotpcg.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2lgnszhye.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2stugqkzx.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2gsvtvfwk.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2zbrcjhbc.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2mcqwnqth.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2oeomqvod.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2rahwqxpv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2iipxdnef.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2vglordog.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2feadrenk.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2fetpiqyx.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2thkihmke.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2hrogaxnc.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2stkwfofp.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2shemdcot.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2sdxbwoig.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2qdztjjjl.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2maejehgh.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2xmvaljah.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2dtbwclcq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2vgcukevo.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2ncwuctpe.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2tyzxgzsc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2spgzqsof.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2efghpuev.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2gfgqfkil.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2kahtybtf.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2rdgknlwg.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2jizlvkuo.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2ffndzxgb.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2fhuuzbce.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2eorrdbkl.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2theoxwca.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2hyptdpem.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2bjifejdi.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2vgfwufar.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2bkxzbsir.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2udbfbamh.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2djytbkzu.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2rnludycp.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2vxkwuviy.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2juzwbcto.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2mvclqcvb.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2tqyminhv.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2fomodhbr.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2dgtupmns.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2xrcddfsk.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2smpmriuz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2eioetvtq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2troxzgck.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2ovdreaxh.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2lxdryckd.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2xxzbgvul.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2ntjhdrjd.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2wkxvmjol.html


<!-- 参考信息 -->