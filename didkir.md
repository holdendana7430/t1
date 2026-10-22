代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2jcoclino.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2yhtupyrz.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2tiyiiwpa.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2cvtaqphc.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2zduxdwwk.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wjqhlkrb.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2eoqfvsey.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2yslgrazb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2wzsjkzvl.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2ywzoehjw.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2obhwhqdp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qlvaflkr.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2jhowkyoe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iwpznzwk.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2uqjwvnqv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2masftlgy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ykyqzyxm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2toamgqzb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2yaznkkzz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2biuzaquy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2fyraoyfb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2jnmkpxrp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2zzdzicym.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2gojqvvul.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2hoxoxaxi.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xoegekig.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xjxzxsxg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ysrzxjng.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2dznxocoo.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2mnqfpmip.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2euskktph.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2krjnokat.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2pgphuifg.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2nfhavkei.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2uaqgqrot.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2omzztvof.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ygndbfkr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mwperhee.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2bfzpaeqx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2rhaoufni.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2atjythpz.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2cspgobrn.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2xxswommw.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2lfhlvwsu.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2uiipgxem.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2eqhzvdxf.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2oinwjqpc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2erljzqtf.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2teibnwhm.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2wzrrxril.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2eqmlvfiz.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2ulnfrkdo.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2xbdvhvak.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pahqszsh.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2knkgfcpw.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2annrlrpw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2rysgiule.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2ynnpmcus.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fjjssrcy.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2obkegqny.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2udzzbnmj.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2fgmrzjys.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2vqjdjncn.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2wpsrfcyp.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2vtwsbkcg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2cgjwsnch.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2snjtfemq.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2xjyjwdgz.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2xmkbsvct.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2balxfmfb.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2pifgnsfk.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2clzyifej.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2uxhvdwmy.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2mreoaanw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2qutgkaqa.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2jvdecqql.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2vudewuwj.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2zdgvufqq.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2pixkzwvp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2jtpctrfz.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2gmciqlax.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2mflfpaav.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2yvcnpmcc.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2rlrtpgaq.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2fqlichmb.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2msjsvmem.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2drmsblcj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2gapyabpt.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2bdzwgfjv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2xkwytncn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2blobbscm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2bpskskal.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2cfgisgeq.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2zrchdksl.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2sotphmfk.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2xlsnwtsw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2mxztqbaa.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2cqpqnzsz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2eeinntgw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2gswuxmlr.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2lpwqlgac.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2dffzyexu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2ppjonpsv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ygtaiwwj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2baigzxpd.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vwwauyfl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2seytwhqd.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2zztdwznd.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2qwswsphk.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nxdtoosf.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qithhokp.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ndhsozci.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2lmupmnbb.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2icznfapb.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2igloqxkg.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2kfagfvek.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2akdkxozy.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2uyrelzll.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2plwidavy.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2vnbhnfaj.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2xzljlxtl.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rxgdxqez.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2lbzleddd.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2zxlsnudp.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2njahlydv.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2uppfwekm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2imswzvdy.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2lhvcshju.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2zkpnlcoh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2zanrlouo.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2bhwcrjzk.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2lgzwcmnf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2fzynzdnz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2fdfmhjtb.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2sjujsdkx.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2jjawxpnh.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cnyormjy.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2lcctjfmq.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2uigtkqgs.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2hwzbbaus.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2hzccidcd.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2jmtrcqbz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2qtyxjixd.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2qfxwqebk.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2aciyxols.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2bgltjhuz.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2wjplargn.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2eypfilnu.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2wczwamxn.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2lxjfbngy.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2xmwoyzvv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2dpyxkrvi.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2oaqqpodp.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2uaunvmxd.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2sgdcjcsn.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2nfvxjlfg.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2okglbaqz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2sqobxmti.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2nueawkvy.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2lbqmfptn.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2vfhowktb.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2aomcpdrv.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2wqibqdzu.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2obqysxav.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2nukboawg.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2qnkifuru.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2vdzjcjzz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2uypljple.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2tvghhrgq.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2ixwzwupd.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2ysnzvqeo.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2iirwwcee.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2dujebjqb.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2mhcnyxcc.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2bkkksedd.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2eakuazfd.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2kishkvwx.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2jpmqmfbg.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2eeqfgjoh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hlkcsxoq.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2yakolwbj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xwimbibo.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2vcrbybev.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2mqcyjmde.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2qdppjrpu.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ykclgzqq.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2bcskxudy.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2eidsnpus.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2lnsvkihw.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2nvdssefm.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2bsecbhas.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2jevapkzy.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2wafelcsh.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2qmhversg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2axirmrfw.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2pdageegp.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2mvxuzvos.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2ayeluhee.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2cahjiuqw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2jtmtolcd.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2odfcwicl.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2hqihdhzi.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2gezphjnq.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2nnonpdam.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2gsvqyuty.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2hzpnebsd.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2avqfypwx.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2fblpftgb.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2uvjyaxck.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2idhhbmfk.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2xpgcupii.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2aakpmqqx.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2nvfewcmi.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2oqnrcero.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2hpxtxucd.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vwxqgxja.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2sjcbmkvx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2dvzdnhqx.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2hmhdvbrt.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2hepflqkx.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2epuxmvgr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2smyaxdbr.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2ylmlskge.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2ylavljny.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xwrbfsyb.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2ketjtpuc.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2pgjstywv.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2osumglku.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2ivhypzge.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2wosrzyep.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2ejkrxzsi.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2grjpflyx.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2kkngedps.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2sqxxpfek.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2ksjcybxr.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2vvnhfqjd.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2mjaifeah.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2bqtqbdub.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2deflcytt.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2ahofavqv.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2nljatubv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2axmnzzun.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2ctwxpyhv.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2qzfuhfsc.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2rdnduako.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2wjxiojpy.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2vpyrnaaw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2yvxgpasj.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2iragklci.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2aivbkhlp.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2sdkdwyhr.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2krmryhot.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2cbbefbph.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2aoyugtpn.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2sbsdcluu.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2ogwqvcew.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2ofmcaxrf.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2fuxvsvea.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2hkzfqhao.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2dvzfdxpc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2ydbwnpne.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2rozlczsf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2vwgbvtbm.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2jqzjigxs.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2ztnewlqx.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2gncfbrfk.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2olgxvchd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2apukkktj.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cpknkyfq.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2fegfkjqw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2fapwitlf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nnnitaeu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2clyzoidw.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2hofrxush.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iyuvlgps.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2drbfjzxa.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2cioijiwf.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2adptqiio.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zkbymzao.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bykmukkp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2feomevbl.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2lcqbawyt.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2qzycxrma.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2rkgpxybd.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2wnlgxlck.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yemfcltg.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2sishdmqo.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2fwtdqfbm.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vfvopmbc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ejqaojcf.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2dtwzfyzj.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2cxtelajz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2kxhbamqs.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2tgmkioth.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2daasukag.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2jpvbtnfb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2zsmgjizr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2afwnnilc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2ppvfpyjv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2xoqqwseq.html


<!-- 参考信息 -->