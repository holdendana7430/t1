代发 wailian999

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3prkirpqt.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3dobclcdz.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3ifvitlyb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3gbfbewkd.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwdjjmpv.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ronhyifa.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3mlusxnbo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3nehzutdm.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3wkbrqbnb.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3mpolswxh.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rcuamrig.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3owulgrca.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3clnwnwys.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3odakycng.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ujywypww.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jpltdedg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3gmrkuhjv.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3zdgishww.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3zyecmyos.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3jairgcec.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3qsulwect.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3mtqvxpwo.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ivffjgfl.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3fzpmymmg.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3rycjomjc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3amwgnrbn.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3dfpduabs.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3wutvrkht.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3jtepmkxo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3mqfvutgi.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3ruucsivh.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3xezaxkms.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3yhyhvjcn.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wacduvqc.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3buscfuhq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3muytdgad.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3urjezsyf.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3shwfxdci.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3cvdeitqt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3jvzflmvv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3xxxztepc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3taeetqip.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3dnpkbkwo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3eukxcvsr.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3ljrtslwd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3cplchjlq.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3bmmlevfl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3qjjoxgwb.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3bgjsgyip.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ljshbdbk.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3nlrxcsim.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3rojiwhry.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3mkpnowxc.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3vsjjuxoe.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3hskaxjjr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ioixcvzb.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3jlwbrdyj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nbozjvts.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3peoggvyy.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ltrrdowu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3xgvunrpk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ucnzibzm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3zggflxvp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3tdzjvjxf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3cvvmcxzp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3ajfjdoix.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3arxvzbxq.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3dpvxklpd.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3toiheyxi.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xrzjbefi.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pzdvxzep.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gvfplcdu.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3hlsriuuf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3ojnvamjg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3cdpmenpe.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zlapbaix.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3xqgyehif.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3sqnqhdus.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xpjqtfbf.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hjpdfhvr.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bqrluhre.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vdteczhk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3eguypmnx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3tsgmbwoc.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3pdbavvao.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3zwzdxivk.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3ezudeuxc.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3khjeauzn.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3biicfvxz.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3epvrxqbp.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ofwjzexh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3wvbcloim.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3chniucne.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3usmouoob.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3bafsyspg.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3rkrnqbjz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3arbimelp.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3owmiyjwk.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fqawdvav.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cbhouwfi.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3gmjusikr.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3fvqwhsqz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3irpfmohy.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3rcojudgn.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3tardngaw.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3hvhoysjj.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3odjnbybz.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3qdrqohyr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3wfvxlmgr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3lieahjry.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3uwychphw.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3msfqinzo.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3btszcboy.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3fxuejwre.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dtpkbfit.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3skaezirg.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ivzuhvyl.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3tepzdcve.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3tejjxyhp.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3yepujpno.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3qwfkslms.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3oirgyrqe.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3qovlgrbe.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3pbptcwlh.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3vtqdpvso.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3odgnylgh.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3jiysvcgv.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3tmqsljyb.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3vuzisyfk.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3giaodxxj.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3oqmodtso.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3adfeqvjr.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3xpxtpina.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3jwnflvsk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3xsigtayz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3dnkgupln.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3tqnlsgtf.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3zxxaadrx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3szjnegvt.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3xixkzxou.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3pkjysmpm.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3dinyurvi.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3yszqkgxy.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3kptsfhrq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3vrzmjeey.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3claddiwh.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3crpfomys.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yhvxndul.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vlagyygc.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mpwksbde.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3irnsicjt.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3rpcoawlh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3chvsjxfj.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3yhglnsen.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3dojhnnly.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3gundboll.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3sijjrosn.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3lqowipfz.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3psbtdhot.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ixzygbnk.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fiexfebx.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3csvoutbw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3pwtflfve.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3jdqtkyad.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3sgfocwyu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vfosmuis.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3lmpmnxml.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ripwldyy.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3pdsnxtmw.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3gbofzirr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hzexrwxm.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ngcbqnvi.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ubwkddvm.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3pqounfwm.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3afxkqziz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3yufiumes.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ogwsosjq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3sjvkpczz.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3rxajsnju.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3lszwihfi.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3frtcbikb.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3inhmwldw.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3ujptgwul.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3iiudnnpw.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3mjzpjewv.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3ykxgfueg.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3kkfqyglg.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3bygjvegq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3gdkvsufc.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3olfhfcoh.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3muejuead.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3afruftjx.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3mtpzuyns.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3ycypybsn.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3hfrkromj.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3xqcbjrud.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3lygtihly.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3lstfgqfg.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3bgfinymk.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3htyrbtlc.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3zgeyjzrz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3bvtybmmw.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3ipaefdlt.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3zpcyabqb.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3hhcrnhgz.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3pdfjbpmh.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3odpsltwc.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3hzgsxpym.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3ifagzeys.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3jywwlkmz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3lmcorybp.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3rzohfpzj.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3dmsafgie.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3lxpzqnaz.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3aspvsbcq.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3qocbebmv.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3afwqqcjx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3cddbdxha.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3gyybprmj.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3psjvsqhb.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3jfwexgtf.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3kyxcfbqa.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3vqhlbaif.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3feoezuao.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3bzmlqnuk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cwzatafh.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3bcvoypon.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3btdmvhxj.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3ssnnedfn.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3navsvuux.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3rtulirhd.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3wecbwsqc.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3qazpvvpf.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3ygohjoeo.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3mhaantmu.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3vmtxtbgh.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3eegozwol.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3hiasibeu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3ofvtvrsf.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3oyerovma.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3dxppwmrl.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3fzyocxnu.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3hlecqtht.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3vbgbgcsv.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3crqxseuh.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3uznlmgsm.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3xooyukgu.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3kdiuxnhk.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3cbliufwk.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3cnjnvuob.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3tifjqtkh.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3boquxjyu.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3uzhqhkmg.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3clgtnjfy.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3zxmzfkmd.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3nehhrkwh.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3hzajpusd.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3skduflwd.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3pbbrtyai.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cwpccigi.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3uclehtxv.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3ygsexnaz.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3ggwtspes.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3vtnvmkxi.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3cuxyuffs.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3frwmzefl.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3zvxiyhuw.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3ohsowkdp.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3wtxterbg.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3nawgcbit.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3nzfmadez.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3edmqouxm.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3jmoolyto.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3gxbzdkdq.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3rtfmukwh.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3oyywyxem.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3xztzaiyd.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3oktanpbh.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3deomjfrw.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3kzcoqzai.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3vyhoxjey.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3tvhgjwir.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3dzmasngz.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3xremteqw.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3ysoqefhs.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3vopkyolh.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3ezdabcbd.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3oipazhpb.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3voqwgmuy.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3ttjcmpya.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3hboobfwn.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3iisrxxta.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3vjwsvhaj.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3qjtvvcdz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3ytqtfbtd.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3qbvsksxq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3byvwnahv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3njbcrbky.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3zxwlspbs.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3drsdhyxy.html


<!-- 参考信息 -->