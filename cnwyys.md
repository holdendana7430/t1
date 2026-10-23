代发 wailian999

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3ztlmtmqs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vdukzcvk.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3ejdwjgko.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ocoxmumx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3swldgmtk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3tqfihirs.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3gbwvqihp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3qiczicob.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3efrehnya.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3gxghwpco.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3gkkepcvw.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3bbfamrog.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3epzmyurp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bpmavjvj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wdelwydc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3keycevlp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3rqxgefcn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3svzlgrlv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3wdgyxvwc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3rwpqwvqn.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3vdlqgbzd.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3wuzateht.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dlxzwbgf.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3azsuxrtd.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3kizeyezs.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ifkwksln.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3dfltbhyz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3ahtuvyvc.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3gankydno.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3nhsemmtq.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3xyhaaoxs.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ssbxwthm.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3akwmxyjj.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3hepidgmt.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ryxidtpi.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3ojxwibgc.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3eaxvvrcn.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3gdekxsae.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3nqlnaqlx.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3itnzcxkl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3mmqywrws.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3vsdosvmn.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3mewguqir.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zbhesbpj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3njdeecwv.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3sndnpkiy.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ynblrdvc.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3lziqpesx.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3qusjcmjy.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3kuuwnvni.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3pqcjhukl.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3bjhaakpz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3mqlvnmdt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3iacbakor.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3btnlwvth.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3unhszppp.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3enppmfmv.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3qhyhnskl.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wjdfuecc.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3vhheujzm.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3inpnlfod.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3fxcojmmh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3eucnjlgl.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3egmyjqtl.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zyinntyx.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3jujagfbj.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3rtabribs.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3qwaxahuo.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3vnsbjlbm.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3qwqmbqyu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3gpwmhslb.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3arrfehpp.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3akhckfiz.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3hpmcrgyn.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3ncepzjdn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3glmdlsas.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3xklkrzjh.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3gafwoslu.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3edlljmmq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3dhzskwkf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3uqsvjoue.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3xylpdowd.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3xmhyklms.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3butuwhbw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3vyabcjvc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3trkpomgl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ueilfgzk.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3spwrdwal.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3jkbynzoi.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3hobfijit.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3xqplwumf.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bmwfmepa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gqslsuxg.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mbaggwsz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dzapqcqm.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3yutcczed.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3kgtmfrly.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3asfozusi.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3orwqnohp.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3ennaekxz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3stvonirj.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mdreuhxf.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3ykhldvcz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3zosoedpu.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3yiwhfkry.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ugivpjiz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3cvdubviy.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3fzdqblob.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3iazncmlw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3bqktvnoo.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3gwxpjvjs.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3jftotjkd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3aqypudkh.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3aaphsowh.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vhqepnvp.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3macyhapg.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3xiqmwrzg.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3upyyyybz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3kbyheshv.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3posraxsz.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3nrjbuugu.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3khhxzdyd.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3xidbswxv.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3wrlagjih.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3szgktaxg.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3kuarwtij.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3smmrysmu.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3bixqxksx.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3hynxpmdm.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3okubwtgh.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3twyymhfx.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3qsnpydas.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3jmiaofkn.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fkucxizr.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3nhbxjzfw.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3grukvchb.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3glcqctuv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3cttqqksm.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3kcchllke.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3wvxlkprt.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3arjwssxc.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3wjriorfp.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3ehplxntz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3hihtstsr.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3hegeraae.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3rsvjqnig.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3zmgclneb.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3cgqagmrg.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3ttokjori.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3mjnbrozi.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3pkjtkrjn.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3dqouxguc.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3dtjpprdi.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3xqyuifio.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3psmbykbf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3jcdmopnl.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3vvqjuzsh.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3dvszyuss.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bxrfcmss.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3tnxrlukj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3idgevvps.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3orpdixsf.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3hzlemjyr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3ocqjxewl.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3dzqnkcfn.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3hbndxhjm.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3bvgsoxio.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3obrkdymc.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3xptiduoi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rmqbsfhe.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3pxhbixsk.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3laglsmef.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3cmulakgb.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3wccozchx.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3xxzqftkr.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3rjxusgun.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3zehirqdv.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3zspdmtia.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3fqlmltfx.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3cgvqwydz.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3igzvaxik.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3vipuyvsw.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3byumddvo.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3neuvowmv.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3lhxfchrz.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3wncoxbul.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3yoevmtme.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3exzdoigy.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3leyzihxk.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3jchgqxpz.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3lecjltlp.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3becwzujp.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3kwkzctyd.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ziiagplv.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ptposbyh.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3dbceyakk.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3fggeybwd.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3whizeczs.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3bkxstpos.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3dxhbeuei.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3hdgccbhy.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3edmqzsdg.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3qucjusbf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ehamccos.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3icanunoc.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3xkpxxguz.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3jnlncgli.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3afcrczcb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3gjhrbwdq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3mofhhtfy.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3gfxfumsp.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3oanjexyl.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3moxhjnee.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3wdqorqke.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3exxrohky.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3yjgeoyba.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3xsaudzdg.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3igwaemnc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3nuewirai.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3zyapmbkx.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3ecbpbjea.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3jwizmnad.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3oxkmcosc.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3hmgraeym.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3cdpqlfuh.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3cjjibaia.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3qugsfrof.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3hsmgvwtr.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3ijevxwii.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3vvgsnipu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3wupybytn.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ecpehjnk.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3whdbuiyo.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3qzaxfzrw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3lgmrgvdu.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3ynepdgye.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3xtoqvryl.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3cgqgqubp.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3asoagbkr.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3jqtrkpds.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3ijbgyuqf.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3ytvxivca.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3qevwurbo.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3dknvvksd.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3tarkmoeu.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3lkaxexoe.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3bugzvkpw.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3pbcytlnb.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3qfjafifg.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3ipxdkjhz.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3jxpiozxy.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3uxhyihvw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3puxsybqb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3rdlhspjj.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3jjgjxawc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3jnlcdgvy.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zgayirbi.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3lqvgzjek.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3pncnzqbd.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3yxorewdi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qwlybexm.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3boynwpwf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3apismrwp.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ufobocsk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3uivtxfgm.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3inqpfkhp.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yfhbrupw.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3nrpqtsrq.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3nudntcjo.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3xgwgfzjt.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3vzldzhff.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kiyywlhi.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3xmspgoma.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3odljnxcj.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3ttltmvfk.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iraboguu.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3wydsewfb.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3nldkmecm.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3ueqmuzks.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eyaecsee.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3ofmdfgvw.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3aixgkwbj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3jpboswlk.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3rhlpnxel.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3zfjwkfzg.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3xdzsggcz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bmoqhpka.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3qgaftvwm.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3gbolcnrc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3vzzztsqp.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3rxjbgssx.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3ijjacmra.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3iqgwilgp.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3djynkbzc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3eoblqttv.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3eaebbpnz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3lgljjamo.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3twmzkexw.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3eynsmoiy.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3vcyzlvkn.html


<!-- 参考信息 -->