代发 wailian999

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibofphgk.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3vhcqctpy.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iejmstps.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3wojqoygw.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3poxrumsb.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3jnecosbw.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dydxmuxb.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3sfwvgkix.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3crbhhmlm.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nvnxqvew.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3lkbsukyh.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bgiczygk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3dgzigsgf.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3zsgeqnxw.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3viwnuaie.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3fsvfvlde.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3mudqwwwe.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vmtbmyne.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3jrnfwehm.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3cjzmospc.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ncfsflch.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3unjbbdfc.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3dvbuedfv.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3bebiwecx.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3sypzjetd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3remwyuav.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3imdngmep.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3kpczdrmo.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3zoubwxpd.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3tzldyajh.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3eellrtyf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3ssogrrqp.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3nkkknqyy.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3eeywvzdr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3cpqdyujb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3inqqsgax.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3yytrtgdk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3smhxungp.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3znqeroew.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3tiywqaxz.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3kfezyewm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3xzlegebl.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3xcdmxqog.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3dkcxtros.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3etfogyjq.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3euydsbra.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3zdftjmri.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3onbwqwni.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3hhwefwvq.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3zbzjzrjb.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3mzxyafdq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eifejgcy.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3vvaqosgg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3seinsliw.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3vkjoedbn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3eprzhsix.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jdipdyad.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3wgvijspj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3votfwcid.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3vtemiojk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3yfctlkfp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3trcptulp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3lvwkndui.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3qbbyhczf.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3xnxirjoh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3amdksdea.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vzrvoami.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3gjtbsacl.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tofpuhty.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3bwjlnwyx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3ceonrfee.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vgpqsqqq.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ymeciqaz.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3xxstscnj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3kmjzckqf.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ntmjsblf.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3zlmvvjzj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3iohwhgzx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3clpuavpj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3fyfganjy.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rgbiyluq.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3pcxqmeac.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ndlrflto.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3oovekyhd.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3ihbwqsyp.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3odfszmdt.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3mgoihvzd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3onxkwtna.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3vcllbuon.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3ijisowve.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3jaydopbj.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3mhxlskic.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3upiktpmf.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ncssacid.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3foyzmuli.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gsfgdwwx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3qxbbhnla.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3esemyoiw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xchmkeam.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3qjlajeaw.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3ziopslvk.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3lefcxcdx.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3nhvntkzi.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3jliyjdob.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3yglqvwvh.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3wvywlpqk.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3qhnuujsi.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3elfrqtyv.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3ecrxxfix.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3bmkezkzq.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3auftxnet.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3zegsiqkn.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3xdgceclk.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3zunhipmr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3uxkxqbsf.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3oqdgtqoa.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3qhxelsta.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3hcusfawy.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3mcfrvxck.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3esksleyc.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3glhqolnm.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3cexluecd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3ghhtjtvb.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3ipcaintq.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3hcgjvcwg.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3gmxfvdil.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3hymugmhu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3prozalgx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3yehcctdm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3cpzjtkbc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3iuoaexyi.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3dylkqgqa.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3jacepwea.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3efxcbzip.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3isogmqrl.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3dzstslwp.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3dcsisifz.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3etbqemju.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3wxlybycs.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3uddbsaqp.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3aksivtiv.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3jauasdkj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3fcjjjots.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3slckeram.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nhewfwqo.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3svuujghv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dwunetcs.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ydiamhws.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3kvrunbrk.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3aihznxze.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3ankjftxz.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3hvnqvaft.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3pcpjpuck.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3aiqitnja.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3ivpqnjmh.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3fqquxche.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3vgphvpqf.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3hzqidhvt.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3xxnbjvwl.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3lilamucf.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3riquaphh.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kabfybry.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3znrjvacs.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3egdgrxkw.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3watfxlmg.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3vnzmczpk.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3esixvlzk.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3thhqhvys.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3zjrdswui.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3arpxsgvj.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3vufumyjf.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3kjljgopo.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3xwisyrkn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3cloylmjk.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3zsvsicne.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3dpfftefd.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3thhzkaqn.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3ttwhzfqw.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3mgdutbdv.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3eeicuueb.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3lqbptgyn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3tupiyspr.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3jlgxtagf.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3pgndklcn.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3mambwypi.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xdhftsge.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3upxzjgmu.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3lievzfjk.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3wjgixkid.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3xaqokpti.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3bujrmvpp.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3kcggoyey.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3epkvvumv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3ziryuyqy.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3ijcbzddk.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3gdcavbgm.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3xmqkpfpu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3ieszzvgx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3lnhnwhzz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3suxytpny.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3cjeuauaw.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3ajltlxzm.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3miynyatn.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3wmssvzdv.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3gpjajbnv.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3ydfvjdir.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3ksxccnmp.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3glabwkdi.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3iptodpjv.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3cfpdimrq.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ogngfvye.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3hvchiblf.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3tuglzqoo.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3khlltxxi.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3ldyvxzmt.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3kqvirvnv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3tyyfqqsw.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3carosicb.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3fbvhiceu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dufrmzbp.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3vytkdjpp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rmslgzkp.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3ybtxlnsx.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3rsqqdmef.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3jbmcnbtl.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3tovmluob.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3kjcyndhj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3estoduve.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3bjpbuihw.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3gjkawxyz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3sxqcjlov.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3rjicwrld.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3woiswggl.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3lqqrotvu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3xggpmxre.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3gqoodbmt.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3cgvoesim.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3txorvcyh.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3sdztqgep.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3khwjtxqb.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3swnukbzg.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3cuyumfio.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3ridylouu.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3sxxsttae.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3xhryucsc.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ltynuohg.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3jnyzqbzg.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3zrwrgqpc.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3oyqwrtix.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3kqnbzjjj.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ndloovlf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3htgrswwj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3dkafpwmj.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3pkvqzxcm.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3cfryxbyn.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3zsnkgstz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3crrteaha.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3kyfdibcc.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3oynnggrc.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3uprmdvnu.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3hutavnzk.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3hyafpoxx.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3frpgugfg.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3ddmskqse.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3yrhmqxsa.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3gqpywtsa.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3bmouabty.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3agvoronj.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3rxkkciai.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3myfwodli.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3xwbrrpse.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3melcturq.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3nbejvadh.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3fetmztld.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3mqadudhg.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3wdawfkfr.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3gorybwey.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3xekwrfjq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3qufhobxj.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3vtxodhep.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3dztajibj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3swpvfwpg.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3mwzsrvnw.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3guyfohvw.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3uahisjkx.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3awlyudjq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3ncngrxro.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3mpoeblxu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3oqvsoplv.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3gcgxcquz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3mmtgnoys.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3zfokdghf.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3jaspwtrc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3efvidsne.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3tpfsqppw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3viqpbomi.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3nkxhbyia.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3niwvamlz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3pltybhxl.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3pkiowolj.html


<!-- 参考信息 -->