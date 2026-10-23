代发 wailian999

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3wxyueghm.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3jtphyaky.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lpdgugkg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3hsopvfzy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3mgfuqxzz.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3hffaufjp.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3grauznqa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ajqslrbw.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3lcvylbmh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xixvzaaq.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3dntzkyfd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3bzkgpkfv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3afzalrrl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3oadcyywr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3hksvxgzq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3wteliayx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3wludzksb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3gelnkovq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3vevfhotp.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3fmluswmf.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3dyiokusd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3bsgjfhwg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ryrdugzo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qojvkpit.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rkdzxteu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3qmlriclh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3isgsauqk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hztqxmpe.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3tuqhkmln.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3zxqhttay.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3zefbxxbp.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vzgtgvpd.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3febnkbrn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3labufpac.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3oojpllud.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3rjbuehws.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3pksnpnxf.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3pqpgkygd.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3rlcdzwdu.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3edoogpne.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3dxvvqxls.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3qomccccm.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3mzdehehh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3lkdhvdha.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3dpsypera.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3pyaguzph.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3memfhfzu.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3hcqxxcrx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3nkxklsbz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3prsnmvcp.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3mxonqbzr.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fpqjzeja.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3bwuzkwmm.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3bnnnbgkc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ndkrqmae.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3vsgmabrl.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3tcasffyh.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3cbhkbovr.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3yfefopal.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3tbbbonrw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3vxayghbh.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3dzcbdzld.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3uhssjqrs.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3bosdbvsv.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3bobvgsiz.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3ljvkcdyz.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ysopfash.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fuicgoia.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xfkbudss.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3eoqweocy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3hmzowkwn.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3mzmabphb.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3xilzsubt.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3fqztjycw.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3pukflztx.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3tszcudoe.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3fgsndlub.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ithjjjsr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3kityeerg.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3evdthacq.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3knybzotu.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3dhqssvsy.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3mchuislu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3hqrhrpmg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3kbryhvco.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3vonbactw.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3qrrfwaae.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3ipmhlqor.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3zcysvyae.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3xjiipyax.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3gxtcsuyj.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3oqedpoon.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3umknyukq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3weqgpbjp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3zptlirsx.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ziocezhr.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3tixkbifj.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3pojhdyhf.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3qqkdqzej.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3czmoxmfi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ilpkyicf.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3nmobjmjy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jprklfnz.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3xmenhtkf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3koavslgx.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ynzwwybu.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jpaxsnmq.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dgiuvgpw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3baqdtqvx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3zwwjiqrj.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3yzpmauyc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3urrxymzf.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tubypghl.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3tfpmihql.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3ddbfopgt.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3mkrvujvs.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3lkqhmusz.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mkbqsagk.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3fuxpqfjf.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3caslulpb.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mkxpxyqp.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3hqiubgwc.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cyhtzvsj.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3zxfwjnlf.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3moahlqbm.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3iewsujgv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3nmromech.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3htvjvrwx.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3xpfxeglc.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3mkoxhobx.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3dbijfsav.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3tirohogr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3wfwjxeqc.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3fwgctzjg.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3vntuquty.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3aqyfxiyd.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3yrevtqed.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3gltwcnwc.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3mdqedkup.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3yjmmlpmh.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3nvsewaqr.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3onctadnt.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3vdsclvry.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3ywwyuplr.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3qacgncay.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3mctbimky.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3snwwntwd.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3zgjsefkq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3xfqqyrqt.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3bbwvozuc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3webspiba.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3vsdxwwss.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3kjcvnuxj.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3hjkxljgd.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3yunbjekj.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3kesbgary.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3pgivpyiv.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3hijqbtdw.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3xzxqqhsy.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3uxdbycvo.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3uojdiwso.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3gvrnsojb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3zrqkfsiq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3eyjxkwul.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3gwqdbiyw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3azcqohxe.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wrpbxxyj.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3jkmgpths.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3njhmfuzt.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3rzxqnuik.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3vwktfaln.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3obgmmyrf.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3loxqlpqu.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3pzssxngb.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3lxztkfai.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3loqdzfxa.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3prybyyhm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3efetfqne.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3termemud.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3jhdanvqx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3vdnmennn.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3efubapjh.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3whwrxyrj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3ctdrfjmb.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3wpimoqnr.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3nywiodgb.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3dlnqkspz.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3seujoorg.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3sjiywhbw.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3ijtbpgod.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3khjqafaz.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3ehttzcmd.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3grxtfpmb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3zhhcdymi.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3mvpbyuzy.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3abqxrnet.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3tezqkkkq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3migqtrmn.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3wvppiuvo.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3mtmteuri.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3cdmelfwr.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3cqyihbto.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3oevhamtr.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3kegqjotz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3qsaemtce.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3edfxjdjm.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3lewqeueo.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3xhmqdgsm.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3ldukedei.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3uptpcorw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3wgibknis.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3puahmgiw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ljaaoooa.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3kptejkyi.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3vazixahi.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3vgoznuve.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3ifkkzdxj.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3jczivxow.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3uvqotgen.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3ibxybfbv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3ozbcnmqy.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3lxxqskhb.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3lxkasxtx.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3llunehyz.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3nuenompr.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3uosuwmuu.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3wapttibe.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3zpkemhhb.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3eoiewpht.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3fcstigsz.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3yepyzgtw.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3uukbpefh.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3fikrnxok.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3izevvjtc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3dsyorsud.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3qaqcibza.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3uqtdvgsr.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3dabgtbiq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3oppupyyu.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3bjnqrlrs.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3sclliptq.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3jpjwkjyw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3cpapxlkj.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3dldbbzsy.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3etmddsdt.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3tihatonl.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3bfyvbnzb.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3idikxfmz.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3rbcfjjpn.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3bddpxfmv.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3qfpermxm.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3figyhdvi.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3lgvkjqno.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3gufkvsmv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3kqjkpcae.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3ioyhnbwt.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3ovtistrs.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3zqzdzhei.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3pjugboek.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3lkiieadm.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3gvisqzsq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3nfuvgykh.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ortemruq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3sfsebrtm.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3mdkjfmat.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3sgtvzciv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3wtbuplnn.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qclzzjoy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ebhigyms.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3vnzhrexl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dqhfgbsz.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3dkmlflkx.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3zqzfzjzt.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3tygehqpj.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bcivekym.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3ojwltyxv.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3ntpxpgtw.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nwhpwzdw.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3dpoctuam.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3rhkkyjlf.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3cynifqso.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3rlrlvdua.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3fzyyfcri.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rotwujlu.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hewcblnv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ewhrudzg.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3vnnyynzu.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ijabnshw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nwedraai.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3grhnazlp.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3tcdosifv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3lsyptpml.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nbpfnswe.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3wndzifvd.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3wjejhgbg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3iqqzxtdd.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3lyxbefcf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3tqkzieqv.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3zzjwgkmp.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3okqdwtcu.html


<!-- 参考信息 -->