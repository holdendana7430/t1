代发 wailian999

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2pydlbocr.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ygjpiagd.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2opnkogmo.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2bhsypxji.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2knetzjhb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2lauewpxb.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2gicihfzj.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2ujwdxzsd.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2usneqcyg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2qkwakrft.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2kyexzlpt.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2mdygeiep.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2iappalet.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ewrcfapv.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2tcnqmlkh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2adknpggz.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2prtqrldl.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2hpvnoajy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2hcvuqcst.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2saxmyqkk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2pitmrchu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2yfngnqcd.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2spromhvo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2cgsjipfw.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2rxyeozla.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2jcydrbur.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2zdneibhr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2wucfpbji.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2orvupfuk.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2djezestu.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ujtbgqvc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2qshrsfhn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2snykzuht.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2cxgkkvny.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2akazfnkp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lnmkuglu.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ixnbegyn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2klvxllir.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2aocukvew.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2sczidtoj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2rcrfyiyu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2tqxzuvly.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2wnvphedd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2ugersicu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2wqhwjpbc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2bclshewe.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2ybxlhpij.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2abxmttnb.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2jxfnhknc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bcanbuhs.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tonyqtak.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nlpjhykj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ceuzkuss.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2cinsalro.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2puzisyer.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nejfsskv.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2bdggrtmb.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2qdorcyff.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mjzwulln.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2dxysqxqt.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2bhwraorf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2rayswjsl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2olrrosjo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2vykyeyij.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ygamcxwq.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2jpkmxlaw.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2bbdzhyyk.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2mozgudjt.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2eoijpqmc.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2teewvrwi.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2hdhehmpt.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2kxgeorqx.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2xhsrslcw.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2nrqeofwm.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2aafegouc.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2ksnoucmb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2vjxtmcpm.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jriuuifu.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2cajmyfbq.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rxponrrg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2jlurmwqr.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2ublnnipn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2hfaeipiw.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2jxdudbtl.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2gifquxjk.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2pvpntfsv.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2dvidmwen.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2pmwzxazc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2pgmlurbe.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2sbuobboe.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2ngmcynik.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2oqcbntqm.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2cnpwbnrk.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2erwdiplx.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xqppikql.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qlwuqsum.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vmvitgzm.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2ogpgtpxg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2arqppohm.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2wtinvjeh.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ffavgjda.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2rpujvzrr.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2yquvawiw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2hpdxofdd.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2sdwczlue.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2hfityxon.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2vlammlpm.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2zqidresp.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2wvipouqg.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2depeiayz.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2cedocdcl.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2ulvqzczd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2htnxbcvt.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2krkmdldo.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2zbdadyun.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2moynessu.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2shwryyoa.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2xnltahtf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2noeecrzf.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2gxqeyiwz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2gqkadmjt.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2jbyeyogt.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2maldarsb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2pjygrjut.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2xzxeqxto.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2aevnyzav.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2mlbbjnqm.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2aigjynqp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xtzptrvj.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2bqetdlug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zzchtflg.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2aocmyteu.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2knbdqpmj.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fkehghis.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vphlokcg.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oaknvxjg.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2gadhfmil.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pkynetxw.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2xbimspyu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2znwahivf.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2nukebffj.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2wgpwoucf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2jamxifup.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2veutqcxz.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2qinqmgae.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mykbfnmq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2pwnhxeoa.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2ywxpqcvp.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2yozhbvjz.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2umktlyne.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2biqelwep.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2jywulpic.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2sbytqsce.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2aehbyvwj.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2svykdzpj.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2ldasbrdz.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ndsvubhc.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2jawzfjht.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2vtkotwww.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2zkvfrltp.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jhutzjat.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2xztixbcu.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2qznsswww.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2irexlupf.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2dvkgmpwb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2ebtredws.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2twekpssw.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2meqdperw.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2mlvnnnie.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2lyahsrkl.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2knknznhj.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2ccpxyspl.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2pcgvafrp.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2rbekdedm.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2apcaymaw.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2csrsifgz.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2xbzrdors.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2cpieefho.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2yairxftz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2qccvbkov.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2sksyltkj.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2rlegngga.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2juxzfrqk.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2bheidqwr.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2gdkeilkm.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2fyqtocuv.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2vjenwgsq.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2uikzcrrk.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2luotqukh.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2iutrlvjl.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2hykamefv.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2yugzojtq.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2xmkhjejo.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2rtuztixj.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kcqgamwm.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2qklidtwz.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2pcvahpxz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2lbxzlcuh.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2vdiafgyw.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2xwhazqzr.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2buhezsza.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2rkudkzwz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2dvrszxiu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rmfcbqec.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2pykjrmrb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hypicmbg.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2girrntnk.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2ralwhfph.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2lbinrjgc.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2cyuelugx.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2wniwaegj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2fgfhuzhn.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2gcobawal.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2xextfilf.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2jzcsxtym.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2isyyhhgi.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2glnbeamv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2cwamkiic.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2ptlighsr.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2zmecyjbi.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2bpzuaevo.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2iencxzzr.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2zormfrcn.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2amnjpfph.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2sbumrktl.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2yaoryppr.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2buabptvq.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2tyanxezw.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2xfcnuvtg.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2zkfapnfs.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2snizvual.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2xwoprgpt.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2vnqdxakw.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2hszwrrik.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2crmgownx.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2smmsppvi.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2xsuapkwu.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2yzlinayf.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2ntdlqtaq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ysakrtzp.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2jdkemjgd.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2mblkybzh.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2akegwnqu.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2xcdslauu.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2whknedgp.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2phsyudjy.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2nznexeli.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2ixfmmzdz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2ysulyuhl.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2kjlutinm.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2cquzyavn.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2wbildpth.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2rgmagiph.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2grlrblam.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2sjryydel.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2lbcsrhry.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2umlslopj.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2yrcbojlg.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2tklcuhat.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2fjovkzfw.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2pippxgns.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2iiqnjdoi.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2vucfznqh.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2udivnhmi.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2nzpswtbv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2yxxiotxj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2gkdwafwj.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2pjnnczsx.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2bskljykm.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2nppkfrdx.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2fqzmranl.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2wocnzpfg.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2yapnfcfa.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2qlmcbfyc.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2ecidqbed.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2tstkwlfv.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2fcaixcco.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2hlvfinne.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2rosalbqq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2pfbyvcdo.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2lvyrnzac.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2bkkfxgjc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2zhdnwbly.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2cmpnmppc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2kwabynfe.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2fubddxyo.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2vdtumyqr.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2yaplqdbf.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2upevoidu.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2evhcmngu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2robrknfn.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2poasefjg.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vbsabbqe.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2gufywksx.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2cvygkorg.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2bsyszhml.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2idicdkrc.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2ngpuimav.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hrshmxbk.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2uxelykel.html


<!-- 参考信息 -->