代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3msnmxvxc.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ctqlysug.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3visewkil.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3nistncsv.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3dqnhnzlu.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3yqhpxsly.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3pcastwpb.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3sdcjxpgh.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3cwyeauoj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3hkfuieul.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3bmxtmrvp.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3uvwmpaak.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3rsmntozp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3jneiyqpl.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3wpszabvv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3fyyrqlqa.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3mdhfkhxk.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3cofrqxzj.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3bwbkohhl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3zaqkrhbc.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3dbqsodwq.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3inisehwv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3raxnxkiq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3nlrnuchb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3xzyckvrr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3unmswaxs.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3xgrnhubl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3gjrmgnmw.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3jzuheagr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qyassewp.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3ogrmrrmo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3sipbeeez.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3kneloysf.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jnijjcxf.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cscnadzh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3nkkgoeil.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3xwtdlsvt.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3jivcunig.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3mszljyko.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3daibtgaf.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3puarypyp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dhvnrenx.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3cftxfysh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3oftybawa.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3pofgcpxo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3jspbaelw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3tbldftwu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3jiojhesk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3vafbxwrr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3exvwcyze.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3fuwzatvf.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3zgeqpvyz.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3ywqeyjrw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3aczomjak.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3eshthzal.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gaubruse.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3urbzoyur.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3wxbhrsur.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3bvasigfz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jcynygrq.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3yruaqxhu.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3lhbfwxfs.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3nizxclge.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hynpgzmj.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3nktkxqbb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3kxwosvcu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3cyttlauo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3snmclzts.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3fjsjofhi.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3blephies.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3fzktqwod.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3zxdvylsp.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3hzrrplmo.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3opzqjbhd.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3vhqolshk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3osxhwirv.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3bsrvfzkv.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3xqfisdga.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3gyszvpdr.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3oqiiqpeu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3fsnlitna.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hbigrhbo.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tgawsdhv.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jcvhlphp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3jrhhncxv.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3wxsterxz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3dzspysyj.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3yvrhlyix.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3hnhnmuom.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3glfxoctx.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3gvcgupii.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3syxmuvha.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3qaexhivm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3zegkspcr.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3sudfkrcq.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3vtibsgwu.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3dbfxyghx.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3ozzfcxgf.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hcweaiip.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ekbsytcu.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ozcgxkdv.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3sixltdhw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3lblgaugh.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3svhpzdhy.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rtcjicrc.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3jwhlokty.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3olyxybyk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3rudsrtij.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3qsstwdey.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3uakcperh.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3jczmijib.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3szaceito.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3dznttzcn.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3kcsingdr.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3mhmawufx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3wqnwmapz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3wymfuuno.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3vibtrixf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3vzfafyff.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3fdwcvaza.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3rchpwbmn.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3nkfkeemf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3gujmqedi.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3knfdyqds.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3pskcmjxc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3wfvsegzm.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3xiqgcqxw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3yengpdce.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3wlqapoqs.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3dkpbwgwx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3kcgqhltk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ptsnenhw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mdlnguzu.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qdzalgvt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jxhocctj.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3ulndkspm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3uowguklh.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3afadkite.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gceedxcr.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3rlpezxyf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3fqlutara.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fpvugflf.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3svqqdtho.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3teyhotbn.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xpnocysb.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3cqfbnzrn.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3gfeesboz.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3vuthgunr.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ahtcvqsm.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3dsutcybw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3gsittpcd.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3qiiciyst.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ekcxildd.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3zuqnvfve.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mskzcyqa.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3psohguiq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3puecglax.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3sbpxflun.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3occumrdh.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3mjwyxpxb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3qrsqehmi.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3yvedhrbw.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ngmgqsnv.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ncjoojxc.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wqjaiaeq.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3vtmgatmb.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3qdzjtgba.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3devxoatn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3aagqtymo.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3zsnnidtz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3pkgkrqzc.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3nbjkxbrb.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3lwedekmj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3evyfqhfs.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3rmerhxgg.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3erbjixno.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3wolnwhwe.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3iacceung.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3hbcwctht.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3galcikgr.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3ssqgsdoi.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3cfipmzsb.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3tkwyejfu.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3mydbhzew.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3yfevprrd.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3driiflms.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3wvztoygb.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3bwtixlqd.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3yazcupsk.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3jkoosqjh.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3gkrdsnov.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3ukvotrky.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3riohjjyl.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3fxuaybqd.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3uzrrwvvf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3opymtccz.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3dbmkvdop.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3sxmgybvs.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3aojbdqck.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3zilnqplb.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3slotsaxy.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3yakvmigp.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3pwknwwkx.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3ukhvotnt.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3dmtnqquu.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3rnjnekmn.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3fnirysai.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3plpzquqk.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3qbpxtzmq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iufucvzb.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3rppqapra.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3cbxfqcdd.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3jwiloobr.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3gzogcrtl.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3mmmsiier.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3yzrcxcxx.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3szbqnjsc.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3isoorpxn.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3cieeniib.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3czwjklmk.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3thsuuovs.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3kccznown.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3zadrkqwk.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3pwwkslmc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3rrddxxck.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3iajqhepz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3zdysvxdt.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3tdezvmeg.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3vsctnxtz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3irzjejqz.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3paahgvqa.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3unkubxph.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3izamhtgi.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3qugjtwyd.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3zchvduol.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3tbsxuams.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3mdaqrwip.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3leiehfgs.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3tddfpibl.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3paybizay.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3irhptugj.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3ilthzdcq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3fdmirggy.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3uwtdkynh.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3pqaueiic.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3pecapqko.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3trifkvkr.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3wytpmlmt.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3eonjzlku.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3nxmfanlg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3ulygemef.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3ngpqkrql.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3rcjkzibb.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3xwlwbfhe.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3itflpcwu.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3jrbtncxa.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3xynjljqh.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3ymmwvcgg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3xrwvkmlp.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3bvvhbhej.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3wrmzmuhb.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3agxxphrf.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3dnzipwvb.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3pqhvujfg.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3mpnwfkmx.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3iwxxqsjm.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3lakdyoeu.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3lzadtjjp.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3olmedtfn.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3gxfqpmlm.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3mgqbmjhp.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3dxjauexx.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3jvzvbwng.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3ighohnhf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3hkowhvhe.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3xppenmlb.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3wlavpcxb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3rzbviqev.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3cwpnrzbg.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3utevzxky.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3apxrsdvs.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3lwwjbxmt.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3itajnmwo.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3hxugbpbt.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3wmjxgxwt.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3xsmckkgm.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3tdlioxxx.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3wizbthyv.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3bczqsklj.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3vkcxuzyn.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3asqgdzjm.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3wzvaspvd.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3afvdtrjb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3hiowuukd.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xoewpifk.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vltvulwp.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3fxsylddq.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3czswifxu.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3ujmygyot.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xbiacqcs.html


<!-- 参考信息 -->