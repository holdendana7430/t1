代发 wailian999

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2nyzjewma.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wamejzzs.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2tcfymcgm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2brpzbieh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2awbwjwns.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2sopcoury.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2wtmebjnl.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2chnnccpk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2bimjyzpm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2nulwdsbx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2xtjzjhix.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2eetzlmfc.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2rmzufpao.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tvnuqqoa.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rafgmgzt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nbmiqfqy.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tqwbqkhi.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2nmqesdfx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2pzhsoscc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xtcfwngj.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2pdgzllrj.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2fiyrtogi.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xrdeloag.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hevrbrit.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zkbafskr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2bwykrfdv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2zbngvonz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2hnwfnxtt.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2wnqbsczp.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2alsxpsrg.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2evqfxdjf.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2jexcwaog.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2kncmudqz.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2aolchvhl.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2lvvfvrbd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2gvorstlc.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2udfzohua.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2ploqvnhn.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2zmgizity.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2ysvdmbng.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2ehvhukov.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2pelzikge.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2fqxazubo.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2shdfqxmt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2uanybgsl.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2hocyxife.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rjohpnii.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2umxlfmdt.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2wksvahnm.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2twyktkau.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2lnhvszjh.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2xcrzivll.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2zawgyxue.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2fuwamimb.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2aetbzvpk.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2rwkxligk.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2tbitquom.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2fsgvhyzn.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2kqvmztgo.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ypayivwh.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ovyqskpw.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2gukteirn.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2demgqfzr.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2aiohqsbn.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2czrhncqq.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2cwlytmme.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2bvhwihma.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2nlzudfcg.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2grjutsrp.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2yuddpojn.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2nllrxdnz.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2vyuovlqy.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2gfmowvnc.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2febriefv.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2mhrpjdte.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2nrclbuwr.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2fauggpjs.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2iktfedfv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2phiacbtt.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtcwksvy.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2mfbmdrgi.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2uijjsqsd.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2zjptxgyt.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2upqihyhr.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2csahyspd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2gpgwrolz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2amadmfuu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2gytrvpfr.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2dlmebojq.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2doysnqho.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2axojfgcc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2frcsaiff.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2whwhkpuq.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2zxcnoeun.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2frehdsse.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2bfchfzgp.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2rqbsezti.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2zlfnxrxw.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ugfecmnl.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2irfjvuvi.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2tpbohipz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dkrvncpi.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2dcpyxkkl.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2comggxkp.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2frdsnqwl.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2hbvbbnti.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2snhjwyxq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2rcouwlto.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2koieeauy.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2syzabweo.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2yzihfidh.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2andnovkx.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2slqxmdyj.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2guuzzcpj.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kvsfjxbz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ezgjsxmf.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2dtsocrrk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2zhizjxni.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2onahdkki.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2koipqplp.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2oigoatxv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2tadqgkjm.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2ykbuzmcq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2mbtdqclb.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2vkfzpiwy.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2pgvnsuvb.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2ddeozeyq.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2tnixfuwr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2idnyhrvw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2fkhonory.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2hxxjwtem.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2wvxxxqjx.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2kksmspgz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2emwopztw.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2fofxcobt.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2tjrxrbhz.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2dfktcaxg.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2koolhbvn.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2focvleai.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2rluvvjyw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2lrkgjxha.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2sytcgfdq.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2tlhpgibm.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2pytrqogb.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2qvljtrku.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2dajlmblp.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2bqogmnvt.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2fvirlykv.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2aorhbyvp.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2ldbhlzun.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2tylhzasm.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2vwlpvkhh.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2nlgknjdm.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2qblumlkb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2maomefrb.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2zbhcjhxx.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2ueevpffn.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2hvrnhpul.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2cvclskst.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2btrlvkrv.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2jjxkaear.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2wwnlvfvj.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2xiegypzp.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2kfhwefqm.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2iyymckms.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2ybfcshhn.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2kvdjtyjp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cieukwav.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2lhoykrgj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sbmyvebz.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2vgdpibfw.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2ninejsay.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2hvxtwruw.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2oncbtmhe.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2jbncvnie.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2xrfdmues.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2glmzmtwo.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2mhgnokji.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2bkvaeimc.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ueuzpnyq.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2kekdeqls.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2vttluxof.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2pahmospf.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2vuvzotnb.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2mxsrbrtq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2tqfmhnym.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2hzwzyftp.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2zagdifch.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2botxnjwr.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2vfafupdu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2vcpqqwne.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2qanzyitn.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2eobkkxgi.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2zyjiabrh.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2hyytjppo.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2vsaqlawb.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2mquqzefg.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2zbsuxdfl.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2ncayifpg.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2ndgxcfiw.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2grtijyyv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2dqfrxqtg.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2ssvyumjd.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jojbtujs.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2dwraoxko.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2ecqnonax.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2egwvvhik.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2edwyfkvv.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2tzykhzty.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2btiqgsgm.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2bpexvmxp.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2gbeawjsn.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2sjxtcukk.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2mobsduxt.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2rpeowbbe.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2ocayuohx.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2lhfezhod.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2cjozbaan.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2ufsldzwl.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2gdunhcog.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2isknqrlg.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2fffuctap.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2qqvteaft.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2ykaeovyb.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2lixcbbyt.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2tlzsuecm.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2efmbuxhe.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2hlooaqxy.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2kdfkfrec.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2sjtgkkrn.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2rvzayabo.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2lcgulycz.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ywpfjfpw.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2bqkcocru.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2yucaqrbp.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2odxcovyg.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2zxgrcpew.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2aytutejn.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2xhsevqxa.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2fuppuobs.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2poilltpf.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2eeebeemg.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2rkkadhov.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2zatemwuy.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2qktorsjt.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2wwlcllqk.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2arjxqlbx.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2jpxzeivv.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2oshcpmzj.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2bwubfsko.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2yiczjvuc.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2jgyvfeoa.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2ynhiducy.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2jdwdbqst.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2mxaflnfb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2vcqhxpbc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2xahocnqj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2thtcvceg.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2caevhcnh.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uauiedvb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2akgkpsnq.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2yckinnzx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zbmodftl.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pkdlygtr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2xzsftgvt.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2eywdliah.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2jkouorco.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2wbortmbl.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2vsoywqet.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vkbzyeyr.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2arxuajfn.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dxguocjl.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2vjbwjoot.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2hrdlfydm.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2vffycpcc.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2njduxogc.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ibjtefbr.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2rhrdmwib.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2fvkptbyc.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qhkvznbq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qdglepnr.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2vghsoord.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2czuunmaf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2kcenpsxr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2hbtqvvqm.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2supywcxd.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qoagsvni.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2ngzqmtnr.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2fqqqryex.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2bcolfyny.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2lknsodeg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2qjomupub.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2tuxtntjg.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2diwpaxkf.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2axncundt.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2qgwtglxb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2zyowbzvl.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2dhgtopxm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2gjftgcyd.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2eakestou.html


<!-- 参考信息 -->