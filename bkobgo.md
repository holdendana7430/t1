代发 wailian999

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3dwwrqglf.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3uesscmde.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3ogueogiy.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3btxbpwjp.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3cikgpzmo.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3bkwaocqf.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3pvrgdfbo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vfivatdv.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3alihfyin.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3cucrzwbl.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3njmdaplk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3dtsgncwc.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3ioryvuju.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3ecvjmnfn.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3cybjoomz.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3uwwchwuy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3cnnxeqvg.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ibizocpc.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rpvyugsy.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lqkxizsi.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3dftsgrqt.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3dxzyhlxa.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3gdyrauid.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3rvqmygwr.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3rrptblvo.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3lhynxqjk.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3iqalwahq.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ffvxwtvq.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3pumfzluy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3dwaxrtji.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3zbihcpur.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3akswsylx.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3quefpest.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3qhytmevs.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3mgpdsyym.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3auxvsgkf.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3tnthjepu.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3kfkjomew.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3iaptckxz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3geqzodrt.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3iycdphto.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ljgwapkf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3epktynga.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3ctzrwlzz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3yrikvqxv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3sqavqltr.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3puyxezgw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3shtjcozy.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3dbsvvbhr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xukdgxxd.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3zumrmkrn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3dbnqasds.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3qcccitwh.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3yyzryvoe.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3yeonimsc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3fhmyirhm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3tvljipvb.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3oujhrlki.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3wpnwqnop.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nuxauytv.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3fulssddv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aucwzuib.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3vhcwdsod.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3phoswlck.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zzrwbrgl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ogxaxgnm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3nwqsptdp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3xcdmcdib.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3ajkhvywv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3uxavddda.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3evkspiuu.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3cwrdwubo.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3tuathrji.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dggmhriw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3slexcbkq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ucrzrksm.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rdmacfqo.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3hoixaoai.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3luljzbvw.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3bkbodqtv.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3tjyjyxfu.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3vkqyuxmq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3iarwmavq.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jhwshsyq.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3pcaeybay.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3fgradnda.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3gretrncn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3ihjummpr.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ydkdvgqd.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3ralybjut.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3bdxlfljp.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3jorpyqno.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3hzcpguvv.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ioxqnptv.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3xdrllfvx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3xnnxkkxt.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3lfvtbfnb.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3osxbmsqj.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3urqqrwze.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3mwnznbgq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3ceyijztv.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tjhuuooy.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jvljzswg.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3wvledesp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3plwgwzcm.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3gppabyux.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iaghdhol.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3tbpsqgmr.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3fhodhksa.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3thoconog.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3qfqflyvu.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3dietmxro.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3yzvysxrn.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3hwtblxck.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3tonwghzc.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3icufjpkd.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3jcvnrvpa.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3dbvdclji.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ooztprmp.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qaszkvff.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3jsbpvoqw.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3kuviwldt.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3jclckzfh.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3auvabtat.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3euvjycgj.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3bsekwwiw.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3xwmqqlhc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3tpslbguc.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3dpdcwyey.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3wdhjbona.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3kzlccefe.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3yklawchh.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3apmzwjoq.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3niimnetr.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3oejlolvf.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3hkdnwftv.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3hzdqyekt.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3afzzjqqe.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3nlgjdrhb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3wtdcqvxv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3qrilwqzd.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3wbbsmsik.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3nxkqnpef.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3futizaow.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3ktdghnhb.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3dfcxjbze.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3pczzkcvf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3rrrxvhpl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3wjaixmqv.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3jntaesco.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3chvrwloh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3esadrfmx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3svwpfgqw.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3iyysrnme.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3abcoezaw.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3egzlgluk.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3jxhipshx.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qxqyszok.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3htsworwe.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3kqibtsmy.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3ahvpeznr.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zpgsknxh.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3dngzjnvp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3fgjdoxzb.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wkxqpgme.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xqgrtrva.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ssfbditl.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3iepbkiit.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3niigmgfw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3vzfomesh.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3nsxuxrnk.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3zadwixch.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3llthetjb.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3zcwktstm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3nwyxtfgk.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3svdcimpm.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3lbxlqitg.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3vfwihirn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3dspcflbn.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3srqsnwrg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3airzclau.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3hvlyvhmd.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3peqqwgli.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3dgcyktvd.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3petcfrmx.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3fprvwrvj.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3kmjmssmx.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3jskcezuc.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3vtmlzwtv.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3mdxklqny.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3eauozqnt.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3beooeuai.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3uyvkwwsb.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3euskiuuk.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3qinwwygw.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3vskmejeu.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3imlybvwt.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3kqnzxoqj.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3lldclndq.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3ljqjwtme.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3kvgkbyko.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3yxszgwfm.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3bsmbzwha.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3brzmyrrr.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3awfewmfl.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3vqbytwmq.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3aubmuayd.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3pdagohni.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3zxlwyqxn.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3izbzmqfx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3rejrtcyb.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3qpffdvrh.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3pvdqgjjv.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3pamzkdcc.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3togrzqdt.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3npudjfzi.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3pccpycrz.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3ysadekae.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3olqlkllf.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3bcwlniso.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3lxqsqdjn.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3chgnrscg.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3qnidavfq.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3btxrqdar.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3gubhpbps.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3ypqvjzde.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3ldjdzduu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3phmmsels.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3xsjjmpto.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3twgutspo.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3mkxviiao.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3kxzwuvfk.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3uzdaxmzi.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3agqkpxfw.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3ohyacbhu.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3jvvutwgm.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3qzozbkzb.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3ssgecffu.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3ufumuudo.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3hfhubyls.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3fgozwltj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3twyxyfpl.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3gfqjlehj.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3chmsfrej.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3ifvjnlth.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3tyscoxpa.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3yruchcul.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3sszgwiwx.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3mpxahtij.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3wuxcmfws.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3fooraoox.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3czbjwmyc.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3rmtbiukq.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3cfsmnkrw.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3wassyfny.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3tvoyfudr.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3ovdjewtr.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3rocrrdez.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3qjojmjhh.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3qosplwgo.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3fdtavsmb.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3wiixutmd.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3nvixjicn.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xathyvgb.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3khwjobmu.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3hblsfelz.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3yvfplolq.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3wklbpnds.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3niecmece.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3hbqdytkq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3rhhcxrby.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3oxnovtkt.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3spybyehi.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3zkmvoknt.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3ednyjbnh.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3upomvxce.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3rfmyywzg.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3gwumpyem.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3kowtwufy.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3fbehdjsu.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3htehxdue.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3vvnucgqi.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3svzyzsde.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3kkbmyrxj.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3umatdaht.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3odqjdjsd.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3koskzkyg.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3ugziuhou.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3vegjhdat.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3ykvmvdhu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3lomptpar.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3mwkyxqvo.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3vgidedeo.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3qkzqgxvn.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3kfpleytw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3xckwqutw.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3ykwkzbin.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3ibwggajm.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3izgpxgpx.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3qrfcmbel.html


<!-- 参考信息 -->