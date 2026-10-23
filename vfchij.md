代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3momyyuor.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3wkfephvm.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3picutqac.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3icjfdaig.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3kbndujbj.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ymfykskz.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3oczlzkst.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vrxyzlvk.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3suzcluao.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3cnmozphn.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3ufjftram.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3etvehdkh.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3zqcdwfql.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3vamybkqh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3metftfyb.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3nnyucvgg.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3cuyjzhvr.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3ybpldnha.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3uwftgopx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3qmrdhsyx.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3wrqdtgcw.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3evhrolef.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3genwsefd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vloiupcw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3lmmpfetn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3wsctgrxc.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3nuqkncbq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3mggmajuu.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3rkfjqryf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ggdrtywv.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3goodkzgd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3rerawrhi.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3svjdfvuo.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3acsqzcna.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dqbaslnp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3sqtnfzms.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3ibfpcktx.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3gduiaqes.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3biczxmjy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zbjprdgn.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3gqvdwmhp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kggddypm.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3hlnpotpk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3igpyatut.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3qtsmvjtw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ytogousi.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3rooxhiry.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3rmzbedak.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3gplbdoye.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3dfnaqfuk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3eqwdloiv.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3lkizxplo.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3xgciavzo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zcoilxns.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kfoesdye.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vujnmsxl.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tgdwltyl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3izvjvysr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3ahpigghx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3yijxfnff.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3qbubkswz.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3churddas.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ksfyafme.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3seiwuggc.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3lfrzsnhk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3aicmlgav.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3vtutstlp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3gxaokkst.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3akolfagj.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3shzqykow.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ihdfkuqc.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3lcuzmcng.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3vuukhvhf.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3eotgqbpw.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3nktwiawc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3xmvkfgri.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3slqhmyyo.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3kbcfjbaq.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3nrqcsymg.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3djntxtzc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3nqhikkqv.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3achcumsm.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bzcyxdsb.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3olsxplcl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3ievhctdq.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3eafdxdto.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jbxfljck.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3pffwfddf.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3ggfymbez.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3anwxonhy.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3udbnzpnt.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ttlxltqc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3ctlqvehl.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3tzdpzohw.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3ocaeytit.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3yvxwmbmc.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3kxlldmqw.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3aybzszkr.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3wbzcsfei.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3hkifnpea.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jyyvartv.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3uguivktj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3qehkdmre.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3nflaflhy.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fjtfehbi.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3aojlxtgh.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3ztiyavjf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3kcagqyze.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3itadrfev.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3yawqaedf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3vftvpmuh.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3ifrbhhyl.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3ggkedhco.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3mpxzuxjc.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3culqknpq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3yyqjczbu.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3udjtueil.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3pdzhmvlk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3bjduvfie.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3tgghqygp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3weifvlvo.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3hoxnirgq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3nnywuole.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3uypbyzih.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3biopjjgi.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3dhxffztm.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3tsvcsnog.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3afeydozl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3iqzrzjqs.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3tqmhgtcd.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3znhfgeuj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pwamcvsi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3znmjfxew.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zfwhhaly.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3snxcypps.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3eaylqmfd.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3ehhflbxo.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bkmhoqwx.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3nfsypslh.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zfkvilai.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3eluettva.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gwxoehae.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3rolhbxwr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3smtffblk.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3yxqtxjre.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3abvgydhj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3jibinbof.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3gycrgpfk.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3isrdrhsx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3afiylmsy.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3gydkfxki.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3kbjatvqi.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jqrqtddi.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3zaluixqv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3twhptbow.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3idhqdhyb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3snlqdnay.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3fmkwzkfh.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3jlxuorwi.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3iciupuss.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3fmmseksq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3cxufqqbu.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3lhfixfmv.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3uykcxfhx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3uyquhowl.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3ltpziowh.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3tmcrbnaq.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3wlydehuv.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3hevmeunx.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3xbvkdhmb.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3orufaijq.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3opaukmud.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3sjtduvbp.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3mdzeejrd.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3jqcytzxj.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3eygbkfyc.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3jmgqmwsx.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3wwjjklnh.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3vluezand.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3narinicc.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3hmkrlgsp.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3byvesaod.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3puuuyzyp.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3apzrftdu.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3tccqjpyg.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3gzeagcwb.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3mceifxwl.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3epwxgdbx.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3cvlhbaej.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3njmohjru.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3tvnoextw.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3lfdmtair.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3tdpybkbt.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3trttahyt.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3ygiegstn.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3lnuvtzrr.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3mfcriayr.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3vstjlvex.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qnzjzzds.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3njhbabjd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3sehqtlzi.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3dmqsznpq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3wmhbwbee.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3nyhfonxi.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3rxuyougi.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3nfcoplqf.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3nsbjanmx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hcvrgyjz.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3oprvrlka.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pmoyvlqs.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3asdgwcsb.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3pjtyxlyj.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3rxibxliv.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3iivftgxi.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3hkdrvuxz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3xhytrqdj.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3rcqijxdx.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3lcpbsotw.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3jdzhjxxg.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3buqzovtb.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3oycywvdv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3jlmtwgye.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3drafgazs.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3rcwpnjqa.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3yodiwxbz.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3vmlfacyu.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3fbwemlvp.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3lsaqluul.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3yzqedweo.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3idfnzgxu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3jbdvjayy.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3gjiwhrja.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3aimkgtxz.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3tnegkeyp.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3zxqypaom.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3kmnohhgq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3plykrvoc.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3grueopez.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3yppoftzn.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3syxjbgmo.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3prkwapkk.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3rymgivvd.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3gzklpmbm.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3eqqequyu.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3mhrprsnc.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3ddwdiqob.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3slofxcqq.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3wnndqvvg.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3qlaoehrh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3gajsmxqt.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3viqqvoit.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3eskcwxmx.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3iltgplhv.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3iddmogxf.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3zjjhmisk.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3psnbngyt.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3xuhucxpp.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3gzjceyjp.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3bnyypyhu.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3eznehgeg.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3declfqic.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3bpbzliwx.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3ggrqfrga.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3gdbsjdxk.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3zzbpnhgc.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3xrqsyxfu.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3ylbcwzhj.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3lamkklig.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3xxlbpnux.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3cdknmusz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3tifjvglk.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3owstcryk.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3spzpzpyz.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3yzxaovfz.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3zekjnfny.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3ldkmgzwo.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3jvycrrpa.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3ddvthmdb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3nykexzav.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3zjtymfln.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3qzsmioip.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3mhkmzlfg.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3doobpfbq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3ageictoc.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3eyxqmgof.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3aprenkzz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3yfrgrwnz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3wbyqttpt.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3jlvoxbdj.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3umbispnk.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3zdfqclhz.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3jbjfzrbk.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3rmrojwkc.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3hlbdsktw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3vwcegbcd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3mlaahbmb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3twiltclh.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3awvfqjdp.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3woqawifj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hnidvnhm.html


<!-- 参考信息 -->