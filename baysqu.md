代发 wailian999

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3moishcgu.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3revvtisl.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3oamhpisb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3howrwysy.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxsmnlxd.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3uhhgelil.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ouyiakkq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ckrfurud.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3thtfqgzu.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3okdoarop.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kymfwtae.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3govpxygl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3znibhtuc.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lsiijoaw.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ajffjbgt.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gjrewene.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3azfcrbkt.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ljuwcgew.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3jddhsyke.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3qaymhhto.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3pbqanijo.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hcyxzkhy.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3oimrebcn.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xdoowbkx.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3mppckvsm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3evvkqzcw.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3naxqwwzo.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3sdhwnlbj.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3clgauyss.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3wpmfzcbh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3moobfzrs.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3eguuzocr.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3kxalqbgs.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3dgqqtsew.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3fzuixwku.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3svvvlxwo.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3opkxmfum.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qicycpnw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3rphhucsi.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jfndkrpt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3hmjuapbl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lexatljl.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3zxqkwqao.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3fhjxusdj.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3ogddhtmx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3pohyymzg.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3inqnbvfe.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3awtnmkdu.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3ryrafhpq.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3esqjlvlr.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dpbupomz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3whknlyus.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3ugrzquok.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3debscfms.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3tqxphmkg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fyqybfoq.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3ystvjvmx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xfuhxntn.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3snbphrzc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3osluqcgp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3wobzzpme.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ufcvxcfn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3rfrworrx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3vdtujvnl.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3kymxsdeg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3inwqtfst.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3wtancmlq.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3nfzzljhu.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3mdwkwerm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3eylgfifh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kkdehulb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xlobetnl.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qgfsukto.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3koplimky.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3fpvrbxtv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zzshygvo.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ylacurof.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3dzqyfqnt.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ohckvrmv.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mlumdxbg.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3wojacmmg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bhfahzmi.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3ranipdue.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3dglhfygg.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3aincwuew.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3xuqvevbm.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3olzneysr.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3nomxftdc.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3dysgsdaz.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3jfmfuacy.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3zvbwgmuq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3ctjmlwzc.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3esutqubo.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3mficmoot.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3wrmfgdaz.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3hvwiklox.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3vcaoaygk.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uxrgmopx.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cuqmgwqg.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3pyoggvgm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3cfjtcfpb.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3dhyelcsm.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3mldfhsiz.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3ayycntga.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3ckfevuwy.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3cogmqukp.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3pnwkhmdj.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3wonvrhwj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3tyeqfazz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3tjmzkses.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3zncbfotw.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3ynimvwfx.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3cnxoowgo.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3wopnsohu.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3hhcdohjv.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3gpyaoqfa.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lcpppsej.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3zhipyngk.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3ufgscxbr.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3svmqmcev.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3jgrqughp.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3marfvqyq.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3izmizzvl.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3gioockqt.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3dxosbfda.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3lhtblnzr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3oupvohko.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3aepssdeg.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3bnggvwem.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3mfhsqjqf.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3rnuhvgcw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3bvludump.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3zvlwsxcy.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3nlstlcxs.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3ohareqta.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3pukegugt.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ojspolah.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3njnijrko.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3rpkrkyhn.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3yamtrsjl.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3nyfbmpji.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3ltmajvpe.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3ixxvbpwq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3udcdycaf.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3jnsficnv.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3xmuzvbxv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3jlsqybfb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kzfwyrtb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uezgpcyl.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3fxbaccuf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uufwzzrc.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3efzcmkqk.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3tdstxtcx.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3encrvrih.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3lrqpsnep.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3olgatboa.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3snglkjft.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lxdwbhou.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3tomgyyud.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3fdxgvlcs.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lccbldsd.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3sgxnjscd.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3chhilxzs.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3etobrxjc.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3zptqikkm.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ffqtknny.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ukszvdbb.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3jhhgtalv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zscxeaoc.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3pkpqxgqr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3oxpfqrnn.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3qrzpgypm.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3xgkctqvb.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3kqvvrfgi.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3yutsdxgl.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3nrflwryv.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3xmlclggr.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3xvsiktsx.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3vtyjsyyx.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3imtwvwwp.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nqnvllal.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3vapfkfcu.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3dscogygy.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3mtbtzxyb.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3qgzmgujd.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3colrdzli.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3pnnhhuib.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3quuuyhfg.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3hnodvmoc.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rciwyqbn.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3ivxjwvct.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3lriyzyfr.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3idwncbah.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3cvshrqmh.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3xedfbbbn.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3wfkbphju.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3mrhchqva.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3jlerfjua.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3ycsotjsr.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3fizjczrx.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3odjoyphq.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3vbqwohvd.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3nxpjmbbu.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3xollcnjj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3nxcmcswu.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3trzkaisr.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3oaqgtawj.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3ryfngsyc.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3gshdbups.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3eajslvlk.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3oymltkbi.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3olmhhirt.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3nhwzagou.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3njunjfqh.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bfweexfi.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3pfbjzcnq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3xjjztrbf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ojdevgpd.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3zjhtkbht.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3agczfaiw.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3pzjibuah.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3nhjmkfro.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3vlaaylpc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rwxplfhk.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3sixumyul.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kulabbyg.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3kuwlsico.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3ievyeyla.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3ulffovro.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3nikwxllx.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3dvffilnn.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3ihboiqby.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3zkonlwxu.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3bwmcmacz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3dsoiozxf.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3juhyqmoz.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3dtbqlfrw.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3haujckcs.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3dahzxpok.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3ggpuqihl.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3jjcfkpcq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3nkofaqti.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3jubgbxlq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3ghvhwyet.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3mcmjmror.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3kwxupfgo.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3vxjsktgh.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3vdhxnxyz.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3etmurjyc.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3gebqjkrp.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ktkdozpp.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3rysndyzw.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3rbbdjfih.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3tdkowaks.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3sxzwawzi.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3icfihehm.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3ikallsup.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3jpxagffq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3xhpdqani.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3qhmtouyp.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3rberfvql.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3zgjypbzv.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3paybocdl.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3nbdhsuya.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3ybmakfyz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3jywwwoeh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3fhwzsjvk.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3mellwuqm.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3kqwtixhe.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3kafssxcc.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3ngbwelzn.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3hknnwvgn.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3vkuuuqvp.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3hgrcolbv.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3impurrmg.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3bkklnoor.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3dobxlzry.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3qwalbhcc.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3zumsfpua.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3kewevram.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3eelebkil.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3okhzanol.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3dfhcczza.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3vfwpeoul.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3plduaoue.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3iczyiojm.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3pejipwxv.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3vuojgmdc.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3qblyermx.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3kakjrkfj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3irucqezq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3atpillgt.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3ytagbxep.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3wcuerhaq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3zbcsfwkf.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3oceddpfj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3wipalutq.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3eesngbxc.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3ggihzqed.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3sumtathc.html


<!-- 参考信息 -->