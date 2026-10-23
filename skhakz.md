代发 wailian999

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3zvwxqvaz.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3gqgmtilc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3lktdmovl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uvxjofhv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3ldybxcdl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tlawittl.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3qumaqdtd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3ftdrogjt.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3hsyuguzl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3uqoqvwjp.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3tyjhawvy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3zfxtzkmx.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3ilnemgcd.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3pewmexfs.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3noiktcip.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3dqsjzwko.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3iwzpnxql.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3zgmqztxz.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3pbhgjipc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mloimyxu.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3bfbnjlwm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kouwzkpr.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3ppbzaohg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3cyahsdsb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3ataiaugg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ssaoucqy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3vfaxphvw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3mpfjgvvk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3daqvqvqf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3jfphecub.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3rznnwefe.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3mowvglon.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3bsnygmwi.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fkijfwks.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dlrwmzea.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wtdbuqrn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ldglaluf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3dflaambm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3mdvglugf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uwwfzznx.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3uygfxyvb.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3zruplkjl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3cnbmordl.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rostpgoi.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3enigaznw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3pzzjgxaj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3utxofhjq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3oxprxdjm.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3nlaaoiel.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3giewwthv.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3plprxtrm.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3yfnlfiyf.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3nrxnkiav.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3lhmerpig.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3utecjvvt.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3iljtowxn.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3zfsrqedi.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3gvtrxsgb.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3ehqmyqzv.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3zqxhnyqk.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3lnzpvucr.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3rqdouauw.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pjtkeenl.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3ujgosupc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3yuvdmfix.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3yjbtdype.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3izvlegof.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3olvqbofa.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3kqmfizpk.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3lotpuwnm.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3hxktcfkl.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3kecdlpqu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3ttaxgqls.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3myhzimep.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3mlpxbcqu.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3qqwamwlq.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3cmxgenml.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3ajxtudfo.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3dunakgmo.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3yuvmowse.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mejttamy.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3uopljtmq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3wxdbyzyj.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3bkzxwlph.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3loqjsmin.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3nylrxmic.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3gngwmafh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3oxbatcoa.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3llrcrsng.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3fwtaxuou.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3esfajdjs.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3aqlqrdvw.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3zgxvcbzi.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3etujxkuk.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3tlgaunql.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3ddzggloa.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3yuggsuai.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3xsdkurop.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3rnwrnmgv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3tshemwxc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3rhgqyubp.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3qymqlwru.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3sjgrnfhy.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3zfmvzolg.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3grhsdgst.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3ivrtexqm.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3lenxuivl.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3bntanvyr.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3nmntzwmz.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3vuijfare.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3lvchcazq.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jlxzxgdq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ioaqgkga.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wbmemcgg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wftuxlsx.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3xaqqiyae.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3czidmctf.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pfdhrbvw.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3qxbxnsjk.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vmgouwlq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3uvgcnjft.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3edznfwgh.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3kpsqzqnz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3tagfggub.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3kbofpfdl.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3gkrsrlip.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3evtnxcxp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3dlfyhyqy.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3qfjlgofw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3vewxfknk.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ywkrnbht.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3yzqehqef.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mautumlm.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3gvhwurri.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nkhzvqik.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3qicfslxg.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3btdwencv.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3xzqhlfzc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3qdwampdo.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3hjfoafko.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3wxufsmiv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3jjujrdoj.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3fmdigabd.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3gylujmrf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3nwwpaasg.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3jmwinkqt.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3lkdiqsdd.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3fzppzkzw.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3lwbvtloc.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3nycolfiy.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3hnwvccwp.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3exnyhpwz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3iaopgloy.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3aeyjjjda.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3vslakooi.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3ewwcatma.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3tvkexwhj.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3jsjibojx.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3dugjlidc.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3svriwhfr.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3oimspxxo.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3zuaexkvm.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3ynglkohq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3lwawlqzc.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3cqdgybgk.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3hokiffex.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3knnolwsg.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3myxpvxsc.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3ukzhbdrd.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3waxtwvvx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3qvclzmad.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3ucmamhlf.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3urxvfgir.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3wsbmmtar.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3dmzicdbg.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3iotkumbe.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3fibszpux.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3ewkalryd.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3ysvvoetu.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3wmwotwdb.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3rjutymkx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3qsvramlg.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3wrlskzvs.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3beiytqzy.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3gmcnznwi.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3wjhwfgba.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3qtfiwebr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zateznsl.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3chhqkmpe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3phseunfl.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3kuvwralu.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3wnhcpyew.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3gvwountp.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3mwlurjmn.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3yacicdom.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3lsxhehvh.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3oaimaioq.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3byymycru.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3iurorwft.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3mfgpuzyi.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3vgsckhau.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3jtygopgq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3dohwjukp.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3dmscingu.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3mnhagaqv.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3gclfyfam.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3ltqfkgsy.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3waudkvoi.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3swopnpku.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3vsrwqukp.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3cgkqlvcz.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3vtlsgoru.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3hyjyizth.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3qzhopaxn.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3uhpqlxdh.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3odfnuqmm.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3hdpyvgcx.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3jzguxynm.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3tppignrq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3dinckcwe.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3nelzzpur.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3berabcpi.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3dnkawbon.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uejzzwcm.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3fbvenxvo.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3njnrncbd.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3effccblt.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3xdxxukqs.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3jqvcujai.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3epjvxqtl.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3ptiwdslx.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3tdkkvrfu.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3upjbsusw.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3coydndhx.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3fvhpgpzx.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3edxdsqxq.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3dylqrupt.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3xtnvvmtc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3ygpoegbj.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3vzodfdcw.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3vqxuooho.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3wsjiefdn.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3ibwjoegk.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3htsfsyzl.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3bbqczivq.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3oqhjqvxi.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3dvdncfxe.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3widvhkyg.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3eqliafpa.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3jlxhcpri.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3zvujrkwo.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3tafptvuw.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3uuplrgte.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3vbxfzvoi.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3nxrrmcnd.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3ahbmeohl.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3ermwmrhb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3lejaeqan.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3gddcswub.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3yduokadv.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3vtfcnrwt.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3ttuihebo.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3cikyqrsd.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3izfiwfhn.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3hbnvguvm.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3kjitzajw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3xxeafcjb.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3gtbjjruh.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3zseekcif.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3fvphruak.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3hwnwnltg.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3ktwhvufd.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3jfcfzdyk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3ieinhnua.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3fhpmccnu.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ceewzoge.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bvhqpepz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3dgqvrjed.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3xbhweffj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xuedjaai.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pnlwoihe.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3ppmnthfd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rpsitiww.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uwjzxeaf.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3nkrdserb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3egyhmlso.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tfurythk.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3wrvkmtcn.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3qfiwfpfc.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3lchguswl.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3jxuioigt.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3vfzylyuq.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3yhjtirnf.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3iqaebfot.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3lybpzvgp.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xwkjupss.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eemjsmpq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3tfounwne.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3stjonrkf.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gutgkbcz.html


<!-- 参考信息 -->