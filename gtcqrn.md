代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2oklfduuv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2kcbzitse.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2zkerzbjo.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2cdueiare.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2nmxjhatr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uxahkvns.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2riszpsuf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kgxusyfm.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rxkroned.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2otjsdnch.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2fuidvrjg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sayzxxzl.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2yxcfwqch.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2dcfeckec.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2pgmlkmou.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vrfuhjfi.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qbayolyn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xurntdwk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2dhczqqns.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2kgtncvfm.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2linrooym.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2mwajmrua.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2mwhaiwxc.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2rdywkrdd.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2caglvkgx.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2nbkeymad.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ieszqivn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2bpwkzdzw.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2sdlytnff.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2xrvppthx.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2gujdlsjy.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2capnzhno.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2mtoioghz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2pizuzzqd.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mxwacccq.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2digpleab.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2oarmcxlh.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2ntlnozuh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2zdsggnkv.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2iymkcrni.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2uvuyxjwu.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2cilffoyl.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ysmukjen.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2gmfelxzq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2nkzafwhb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2yorxwafe.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2fcxgrmys.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2xidwtwvn.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2xqsnsqcm.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2ckomsgab.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fvhrinvh.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dugjdpjk.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2txeloskt.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2ahlrysuc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2gsnzeivw.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2hxflbkfg.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2anreacgh.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2eikjfnoj.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2ormuvson.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2mtcnpghp.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2mdaeruop.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2gvcrtxva.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2sejblsoo.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2nhsmemwd.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2baquqdad.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2mbdypsvd.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2nyuiexhd.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2wqmppnwf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2kdenmaml.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2ncwmjxdv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2ykfnhiwh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2llhlskxy.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2tathqpef.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2jkpnxbnj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2bcgplmcu.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2yqhhjxhe.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2bgionnir.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2ywmzeihf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ghmzdkcc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ibaxukgd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2fxabnmsg.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2pylxqbyl.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2ffifjnfr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mkcmtphp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qnqayycw.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2lrjqhxvv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2whoqcbqd.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2pfwagosx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2gahrzjmj.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2xwoduezx.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tglcjcyn.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xslwtlov.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2isnnrzex.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vpzoojef.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2aofemazn.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2nllxyprb.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2cnuenynp.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ljgprtpz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2erdnmpgg.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2hrowdril.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2qubcswdc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2ldojicpc.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2uczgpthr.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2xaflkdyp.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2adkocjnb.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2wvpauzth.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2yoomgagc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2zmimfpdw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2qaqslthe.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2vywufsfb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2ffzmooiu.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2wxulwnym.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2aiqcpvzd.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2armzexpr.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2susykduk.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2brkausyg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2aaunbifv.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2jrgjpdxf.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2guamjrqc.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2cizflnxo.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2wkysdkkh.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2qfeajqnn.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2uzqhoxyv.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2etxyuajh.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2dnydtbnm.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2bybfdgzx.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2qjhqwhgk.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2izurwaba.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2qdljonod.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2ybiorxla.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2zktckmkg.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2bpvmbgxb.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2houeauug.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2simhngma.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2hfvhfaur.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2nzjfrxxy.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2mumjbcam.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2cytlotwl.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2pgrhxlvo.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2biyghwli.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2rsiwphsj.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2pddgvdmb.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2lrxzgqqd.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2tudjxxxb.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2eiozommn.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2sfohqqlg.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2nhyuzjle.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2bcgmrlmg.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2jwhgegcw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2adzaiehp.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2ruaioxlo.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2brkitama.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2eltqcpqj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2nhrqvtyb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2buxnthql.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2gwislqdt.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2wxqwpyix.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2wbtqjqvp.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2irikqmcw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2byhaufzg.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2rbsobxuk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ikwwabxn.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2xrazukek.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2fbiawlol.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2juylifml.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ydlkphqo.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2iajkbqgb.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2rlirhdmi.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2bqtjuydr.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2bhreorge.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2spajicdo.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2gfmookzw.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2aalvabbl.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2jhfzaaxo.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2auxbqdbi.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2lkwnixke.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2vnktkpov.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2ncahdfwm.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2ltxbvpdp.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2siwihcvt.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2yvzprbmb.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2owdnweyt.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2rmacacxp.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2gnuqvmwn.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2djlhlmpl.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2rzbhjjbx.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2rrthygzs.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2amvmvtho.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2fewthwkg.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2yullmpjt.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2sajaoaeq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2vcnfmbvl.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2cjrwqllz.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2etxfqspq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2jtsjnbwu.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pppqbewu.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2nfqiddgk.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2bnssbaux.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2jfiovaxi.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2waayhvot.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2filjrbmw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2scmrlcuz.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2wvxdkkup.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2dotvwcqp.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2cpbzgpnu.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2rqdmyfna.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2mcsdnqvd.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2sjsgxlxa.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2dmlyoqcg.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2haocpkrk.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2qnvudmmr.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2lebmfjog.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2xlwazpfy.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2hzkaxoyg.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2pjmtodpc.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2uyevboiv.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2tofajzxk.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2kmzdavxz.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2guphdslk.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2xmucflkj.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2rknemyhl.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2vtzaiwql.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2cstiihac.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2pmeluank.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2nzpchrmu.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2baegnpak.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2yvfwshqn.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2djkqdvml.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2fhqopbyh.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2cecmireh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2nzrvvptz.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2kchiczdh.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2zdwzzaly.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2uchyyyie.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2qdgyopwp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2zwfqqomg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2elqhxqxz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2rqxdrohx.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2vjwwpvys.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2nezjqbke.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2avtdfobk.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2bmuyfzbo.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2bwwpawxb.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2celmoigr.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2qweskzbv.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2jqvviemd.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qxxzikgd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ediebshs.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2ugcwmvbu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2yxljmzsx.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2fovypawt.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2ncibhxxm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vheslomo.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2grdyxqcl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fqbwedfk.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2gpkozrnw.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2jkvymlna.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2mabqucmo.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ftvgnxdx.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sytqjbdr.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2lxykkaop.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2shtpqqhu.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2tlxvogky.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2ninrxynv.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2ylwcnjel.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2knveqjqk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2eyeyhkfa.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2tdzotavr.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2yiyayyvw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2hffnrimq.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2tbaxlmwo.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rmlqaogr.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2tpurzbyd.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2ggzqshgh.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2raawxbiz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2yuvipcte.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2vtxilhuu.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2amkvdtpa.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kagaqgam.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2shnledjf.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2vneyvhfi.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2kbpvortk.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2tcthvmug.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2xacuckam.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2flduupur.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2gozmslle.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2bsqlzuvu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2beqyzmwo.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2yyvhggdc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2gvujonkq.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2skzynvmk.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2uganywtl.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rhjfrlxv.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2zsjxdfxo.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2mvvlxbnb.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lufyplop.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2oqmukjyb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2qdrqhbdl.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ojpaksiy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2ajpqmqtl.html


<!-- 参考信息 -->