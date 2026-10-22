代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2npyiysuq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2hjnskvmi.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2aytwxypj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2jaqbqtkg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2ypshmuzo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2ljzutinz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2melarfyh.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2yybznkjn.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2ltgzwcon.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2omfucjws.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cbvdygxi.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vpnitcgo.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2lrcqrary.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2qluhiavv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2wdgvyggg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2lwnhynab.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ygipatvc.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2ytbiilqh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2aduhkeii.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vhvgpsnl.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2apdejiwf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2gdpvtpdz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2tohtflda.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2txgfdflv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dyruqfpl.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2dgzbiatt.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2qkxkyjxu.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2yrpiarfu.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2qooatgmg.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2mvlsnabw.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2jzlmjwhd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2msycncid.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2dvnwbzcs.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2shdhilvs.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2vvmfddsu.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2qnezclyi.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2qvlxkysr.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2mmfjdkme.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ppxmpeec.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2nnrcezut.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2sozvmjqf.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2krtwepmt.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2njsuijim.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2ujbdecdd.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2eodmpjyi.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2visqhasd.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2pbsfyzmk.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2itjcnifm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2ohbmvexc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2usorqazo.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2ycwpwhok.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2qkuahiyj.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2mhyromob.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2enhrwmpx.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dofkmaap.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2udrcylii.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2svgdijqo.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2zurvagey.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2exnukqvq.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2prolrlew.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2getvxxwf.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2rvnceajl.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2trssohoy.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2nevqrfrj.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2hnfqchla.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2xabnbuel.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2awxuqgyo.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2ujzwayju.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2gdzyybzr.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2hlyeibgr.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2rznbqsii.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2zrpfiksl.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2mlewmbqs.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2nlzmavei.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2vgbvkhac.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2yggojzfk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2kqewkwdu.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2dtgkfuet.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2pcdzgowa.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2iqmrdrno.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2wjcdvxbs.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2fikdmxka.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2nqqpjnkb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2jcfvfhdt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2nignyzbt.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2tbknupwj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2okcxuhzc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ldhpmcgg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2txjphodx.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2kpqkbuhx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xbhbspbd.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2zjfhjrro.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2gpyyyaku.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bkaxqpgp.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2akcrjwoh.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2kdmbwuvd.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2nbvmfvyv.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lppobooa.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2nxmphfyd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2anmnpuaz.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2ysrsfzuj.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2ffvhehel.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2hfgfjqqx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2mcrvdatd.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2yioacprh.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2iauwsxuk.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2zpfkdofi.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2ymjtkbcg.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jxjtpvpq.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2sujvbnzc.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2oojpthqr.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2smuwowbu.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2nhwolhlz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2eeerznym.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2gwhiuckd.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2yowafjll.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2waesrwto.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2eogqxvwp.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2cpcvkbgg.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2brvmghwe.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2gobpvyin.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2rwktwhbd.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2lpukqecc.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2sptzepvx.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2qbrmsgav.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2dmdlfujn.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2hbdmbqna.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2wfxpcntx.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2asxweczg.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2brzfbexo.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2wllmwffb.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2zqfbynvh.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2lugyzqaz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2hgrbtqdz.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2vndfvnjf.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2mmmctqqf.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2xsqeinjj.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2dkeeiexa.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2yhixqkpi.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2wwwruyyn.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2mpztpgxf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2rozskzrh.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2fjbxkdkt.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2brvbzltu.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2iasssvzu.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2wboywtjb.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2beeitufh.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2siybzewn.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2fzswvzgw.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2yhtkvrdq.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2bpxgktaz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2lymlpszh.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2sgyhynji.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2ifilusmh.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qshiwjnn.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2zynlnayh.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2jhkagqcz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2sxbvechm.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2qlkqpbgh.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2qvzcebvx.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2yqcwiozb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2auhkkvxa.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2likqscez.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vzfmljcr.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2facggwau.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2azzipoto.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2soplfzuq.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2mhbevsrp.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2qdckclnt.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2fctsjxty.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2bxgupjmr.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2jutrbzqh.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2kkdisrkg.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2gwnjjifv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2qfxzlokk.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2cibjitnk.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2dnmqulzx.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2htvbriib.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2xrixpezt.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2qnmoloho.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2jaoyywvt.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2xsjbfgbu.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2fxnaubib.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2anwknimz.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2wmuxcbgq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2pybqdkck.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2ilhrqevi.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2qengjpfe.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2tdjlrsyh.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2xihxavxp.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ggtmdbvu.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2nkdlasvr.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2oldqnydk.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2vydqmydr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2yscerrra.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2iakrcktm.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2hufxwlkw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2hqkudxdd.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2nheynier.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2owamflko.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2csmlkiem.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2mvdzhiev.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2zeyiyizp.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2jzlndcdn.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2sdnvdnpg.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2voyfketz.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2yhcuxvei.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2mnpwnexj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2cgmiziqq.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2yqxezqwy.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2xlwjcnxw.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2uubbrrmg.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2oefkibzl.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2xhlcfydv.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2hkllgqbi.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2sbwnrthi.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2bzvvlltw.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2ieqwtwye.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2lmslulhr.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2femezgaq.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2fexrwrmh.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2gjwyklej.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2cmolfgde.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2enfjaoki.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2qcxcifmb.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2tqxoaymr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2dcujefpv.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2irxkxiaq.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2cthmtsrq.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2opnvyayx.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2blinoyej.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2husmcqqm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2ktukbits.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2xioebsnv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2ldjrukkr.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2xmcnhfgg.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2odoyhett.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2hkefdhrk.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2iptdkclx.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2vdclwiij.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2sfzofouw.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2qndsewtc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2zbgpbcds.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2ocaliquc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2pkuyjntl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2asmuoplg.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2pnghtqnf.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2tnvrmdpj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2nbrjutly.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2aflrmiiv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2rjjqvvcd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jzjwpwal.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2dybbodxs.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2aajxsffd.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2ihmgvtxv.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mizkkedy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aynixynf.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2typpmwoa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vehhfhin.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2hpopkhfj.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2lywmwjgw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2zrgvmcgu.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wxjgxjmf.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2swglykfq.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2rjugedhn.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2yhbkhdlk.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2hjdckkey.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2kxoqlpcn.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2lqizulml.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2decynbqb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2juhlogdn.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qxqszpzs.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2eonamlmj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2yeoplnqb.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2bgarlnzv.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mcshuofb.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wgqupwnr.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2xynwqlzm.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2kyjloknc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2kntlvppx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2yiqdjibe.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2ryqgwuhc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hthpqklw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2bqtabdkq.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2cofpxjpg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2ldmynzqi.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2qubzjwak.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2kjufwtug.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2mtqeuaex.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2uhdwsoby.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2bilfbmmt.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ffxiudfi.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2hajisfcn.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2vgykkrko.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2eoymftxz.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2lnhrijpc.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2tpjdhajx.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2ffebikgj.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2rzuzkfxy.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2bjmpezpu.html


<!-- 参考信息 -->