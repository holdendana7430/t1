代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3xbepqxdq.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3oukroqvo.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3kpjkjfab.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3ozvdkias.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3qicexxot.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3efzgtjld.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kixfoxji.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3smkryttm.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3pouwffvm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3yoakmnwm.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3dgukobfb.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3wsfjikci.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3cozcurfr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3evcubynw.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3xqbbepus.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3yjbevbob.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3lnzhruly.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3sigqrkrz.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3cvoibhkj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3tjikgbyj.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3qvkqlfch.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3zdcjfdgt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3khfrwhor.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qiqtlxmz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3pglbnndb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kgkxwysf.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3ideyoztg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3frwqczud.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3rtkxkvjv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3jqbzvsme.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3skpaguor.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3jthpdzpx.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3fpioitpa.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3brtbwtod.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3olisnfos.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3ohmtyyxh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3wxcogppb.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3elzjyuaf.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3cuodqdfu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lhgftqgq.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3xsyelymf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nwrwydkq.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3mklnittq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3xofgxblj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3wrvnldfp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3teayqtnz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3vqklqngh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3vgsvvstk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3xgujbgrs.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3qjbgkvfz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3tlxoplhn.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3fnpnjpfa.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3izqyivdl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hqwdwhyr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gmgsfbro.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ekynitbw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mcchhepr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3rwonlxlu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3zigmlfdx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pksphzbm.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3gtlphlre.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3ywtxilcl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jczgyxbl.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3blytftmv.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3pfqfmwbu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3gzoodxta.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3myrehvri.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3ohogubwe.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3nhtmbwuq.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3woteucnm.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3qznhtjyo.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3qxelrkos.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3fuspxyby.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3jxybzgna.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3eeektlyx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3evhbpmyb.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3oztnwedi.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3iugmpebh.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3rbxsmbfu.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3cylapwpw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3yfpzjgfo.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fdtkgsfw.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3zejaluli.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3rmgokzjr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3jatdtprj.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3qcuxqwjy.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xqwhlgfu.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3dzemikyy.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3cmuikyfb.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3jthlawnl.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3dhgumabz.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3rgsvcsas.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3qtnppbuz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3ldwbnvqs.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3dtyjqteq.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3aducfyho.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3wcylrfas.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3vxgimisc.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ofaahgaa.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3mzferael.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3maxsvtgd.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3taaybfkt.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3iabucxof.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3yaykktuk.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3trqmaxef.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3twewbumo.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3oiuifwdd.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3rvmzkvwv.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3omppzkwg.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3hfhmgyhd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3guvqckzo.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3hevpnwxk.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3ilkneeqq.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3iwfqhndj.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3kczwllll.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3nylodcbt.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3femroujl.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3itaxtqxd.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3qotzzfml.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfmuwtec.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ukdvtqaw.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3icmpgqtd.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3halwaxeq.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3feaqgiad.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3dezkbxwj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3mlvlhcsv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ptztnglg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ekwetkce.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3tpzkcyaf.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3smfuunmo.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3owngeomj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3exprmlyu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dwfjkolr.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3stryfiho.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dqqxtbas.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mykxllut.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3rfuccyze.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3kgqtmoig.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wyproqqv.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3yvqtfkak.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3fhqlreky.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bawgsgef.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3bkwdcoww.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3coxokqzl.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3vaclxnll.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3mzrklayb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ulmcfjdf.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3gyjchdfm.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3kmxtuihj.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zaxijbbg.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3egsgsoti.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3dbhjgmkd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lterxqey.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3aqnozlet.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vlvuvkbo.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3ghpnmvam.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3ysejorad.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3samoyvkr.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3slizurxk.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3tnokijay.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3sbbxduco.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3lmvpfxev.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3gwsupzvw.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3xawinzdc.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3hyzsvjhp.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3evdbswfr.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3urvfmjzm.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3aifrxlyh.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3ecrfhymk.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ldrgzzuc.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3qdbdiyrf.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3srewnlzp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3ggklahyv.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3vdqyctdr.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3llzyfynx.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3sryosust.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3tcaptwhq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3htpixqaz.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3ykgyehhx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3vzcmdzts.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3cfdxcfcx.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3vmfdsiba.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3yqlptntt.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3cljnhrxy.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3bvyvpxpn.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3bvwrktgx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3dbocofaj.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3ifrswsax.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3vilaslcm.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3wbbegxia.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3hikuojyv.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3jkfbizmm.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3zecrtnjn.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3lhsuvgff.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3vdvtyiik.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3czitpuih.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3bvzhssyc.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3aoyyczbv.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3flykelnm.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3fkhrnkdo.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3vdgeediw.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3aghrprcu.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3zwxvyidh.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3qmblxcvu.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3qxhfmxvo.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3outwpnpb.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3mskpqojj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yabluxaz.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3htkeleik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kewrhnka.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3rswywxkl.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3hkhjwyfx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3lukbdkkx.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3cidhxnyh.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3gcmxhxjb.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3rflacxui.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3hxgppgaz.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3fiumxcai.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3cwugxmos.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3fwonnucx.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3qzqizeuh.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3rfzbdfjx.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3qxcsrsub.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3tozkqccm.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3tocyudnc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3cbwdmxvj.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3jrtymqye.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3fhqlzqmw.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3mcuhuujz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3vphafevr.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3dnhvgnsr.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3crkfjzvx.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3forivcly.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3atyqcplg.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3whmpdola.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3bpnnlljf.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3frwenjvd.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3bvvukcah.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ggnekpoq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3nwkptuzr.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3tqlnkmmz.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3ojgesxcq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3sdtcahzs.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bmkptkbx.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3grvuxftg.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3ydbxdhwc.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3nigwjffw.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3fsnytbxi.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3vhdtyafz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3emkqdoos.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3cwsnoupd.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3wtkqjigt.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3zartokba.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3hnrhzpcy.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3tmnkwvtc.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3cxbtvuca.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3fgvxqdpu.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3fklbjtvi.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3laomnvxs.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3wuzbcfyd.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3rybttpsd.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3ycsimiwj.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3hexjwruv.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3prlsrttx.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3bxjhubwi.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3jbcljtgj.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3dbazuiku.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3skoavpji.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3wkwjbmkt.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3bspxidig.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3ddktvvnu.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3lqmbkxmz.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3icbotddc.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3dhepcxhu.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3trdomvrh.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3yxhkadvx.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3ezhstkxx.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3kdyjiqmm.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3kokyseqc.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3mccklqgr.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3gieodvyn.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3bmghcvjs.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3lscvxpym.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3oohvcpzg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3okscgxli.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3fokqkcip.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3faqznlij.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3ipvefmmk.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3btbdiijs.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3tacuygbz.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3pfpkkaua.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3ajzxmfpz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3lrydogge.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3wmyaownm.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vjpfbdzj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3cakvwdbb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nfuwkktd.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3mituxycf.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3azkrstal.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bmpclvag.html


<!-- 参考信息 -->