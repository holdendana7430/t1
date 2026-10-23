代发 wailian999

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3rxbnyebl.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lmryclgp.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gjohabhl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3ewquyakq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3colbfpnv.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3kvaqnjip.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3doylydbr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bgefkyea.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3nwnowoiy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3meraryip.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3fwcjlhbp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3nuajfbnr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3fksgstfb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3cdhmheak.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3rlhtuhfp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3zkxcztxs.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3jzlchtbm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3jhcwmwsh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3wqadcbnx.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3ostunrez.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3wfthvdzo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ftkuhxay.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3givngsww.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ofwlplwk.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3cqcgptus.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3fvfjaueg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3rtkhyblx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gdfmpren.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3xmxulpoo.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3adpmltcz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3nkpqnakt.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rxriwpix.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xiypbatc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3bdvrpsqm.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3ymnwyopi.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3uebmndsw.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mwsxevrb.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3myvslgcq.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ocuixxbt.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3crhumncv.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3pvgoaysy.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3sjfwtbns.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3vinxdzvp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3wbdiaiuu.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3dovsynyj.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3teaejowp.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3vxqvcwtx.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3kgbsurgj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3yqywgzyo.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wsvnpzdj.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jexgqzto.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3rzaowqno.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3yqwbymtb.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3xscnscuc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kozmdvkp.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3pwotbuet.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3lfuvuaho.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3szgiwayb.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3cklqcrlg.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3djsdonjk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3snowhnhm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3hyakltox.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3kdaeibcv.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3hpwbeckr.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3kgjzocct.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3rpbjaioy.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3vhbhvath.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3eiuthjtk.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3radbrhxt.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3rkcuvypg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3ufbkrxkz.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3ctffzgpc.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3nsuvpykp.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3fxkwzyht.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3iaxutuhg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3sujsmkjw.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3nfzwzmzk.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3amygrzeb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3yddtqykr.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3howzrtyh.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3gssbgfde.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3gqnudluj.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3rztegijz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3swmmskoq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3jbvnxcua.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3nopoatrl.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3jdyvllad.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3onejwnks.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3ppspkljc.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3ozfvjtbi.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3tuhilwcl.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3fcijtded.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3erpbqeid.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3nwofvsqv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3scamtkdc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3cwhpjjcw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3lnzjjolh.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3wuhjqddd.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3bsaquzkb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ruhesjbi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dfgfgrgv.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3bqizbfmo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yadtpyxa.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3ofpgjzvc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3nprjtihw.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3qpkytyjv.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3ohsqvmnc.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3fcmjgfqe.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3bywexagd.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3nttlofww.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3kfytqbxa.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3eyicdnuy.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3ygvxagwb.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ezppbwwv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3dfaduztg.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3qfwjxoer.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3zapdjhyp.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3crepadfe.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3ptccjflb.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3hznwlukg.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vlauhyqt.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3jyyqogka.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rxidadkd.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3tfuojroa.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3toathigd.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3crvewzta.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3gydybcll.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3uglduvcf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3oeqxravf.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3dbcovrux.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3odcgksbl.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ncahgnkg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zoqnzbfl.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3nfusokeo.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3rbaztmad.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3urrjnbyo.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3zaxmriwb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3thoebfjw.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3orropldh.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3upgvxpjz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3lngkuids.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rpphytbn.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3nviojuqg.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3mjaxusor.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3kmqlxzkx.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3keabohvv.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3niusadwz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3orzswwgu.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3metsugwp.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3idlusmmm.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3motjwdlc.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3kiefqipf.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3ijiaouqh.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3fkhlxmtj.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3wcuhgoqj.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3fdmowshw.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3hlqmmqpa.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3npfvfypx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3wlngycoy.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3huefdvda.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3ogbjeymv.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3dvryozqy.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3aqwcxafv.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3giuhedvb.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3zrfhvntf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3kflorjpl.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mztkmegp.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3wwbedfcq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3aisiviyv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3fgvlujpo.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3zoctzbjq.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3ganxayte.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3ewegzycy.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3hnpibvtc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3yzxdiazn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jkrywlic.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3tthzhbwr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lniyvfoe.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3nrcntpvn.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3cwgaqjaj.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3nhnmzhet.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3bsujbtmc.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3acrgjprw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3dqcndfdu.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3yxaayzdk.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3tvvicwjn.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3nxsjrcrn.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3qfvfgqsu.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3vhfckzaf.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3nsyhvybx.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3dvyvoxww.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3dcwnppdm.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3xbgvangc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3yakuyrtn.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3ovnneqhb.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3gfamdhpm.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3vbqpnsss.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3xvnzjjbv.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3hrcylhrg.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3dwlawdwf.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3mwjrmfrr.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3mlptxfut.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3mzjkenug.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3fmaumbyv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3kupfvkze.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3thadaxau.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3puiwuuvo.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3rsomoeql.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3lqurkegi.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3phqmpgyl.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3kvmsjafl.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lzcmofrw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3nhvxdqzj.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3pjlxqxbm.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3nzruajqw.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3orlfuzdb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3giofbnmp.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3iwxsmgeu.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3uauciobn.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3gnwgkbce.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3izahxiik.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3fxbyvnks.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3jyghpymp.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3rzyplfav.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3ktpdanwu.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3enmfrhor.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3qvgvmfvz.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3ongzyawc.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3cdmcqwmo.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3fctkxzbp.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3ippqydts.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3epbapcqg.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3edjclkow.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3iedkemrv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3utrvoqlj.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3steychoq.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3cidrwsam.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3uexsmxge.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3otwocqgw.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ntvcabal.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3qrotznyp.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3xnnbkqki.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3hflwrxmh.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3lpvlldun.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3faqdhago.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3etageuks.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3bjkgdppd.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3qqyftspv.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3pjvuozzz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3ityzfplb.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3bbwvusii.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3xwdpfbvs.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3kznfvzhw.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3ouyfiysw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3vihpuciv.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3jkzqtalw.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3dcjrnofj.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3gtljfmuk.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3qaleajvz.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3ijhhumnl.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3mrydrbwi.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3gtuncttg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3pmatpscd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3iaqrytlz.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rgdgdcmk.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3ayyexzox.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3sftizpta.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3katmathm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cvcpfbok.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3dbzvjaip.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vqqjcqqz.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3ofymvowo.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3rqqytekl.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ogzhyvfp.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zmnmaavs.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wpgimfrc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3nbyxrmwk.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fxulhluw.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3hvjmmuvc.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zowufcbs.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3xcmjfbkt.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jmfwakzc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3qhgiqppr.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zluohqza.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wrkctqpv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3qybqioey.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3nlesepno.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3fpzsjhrl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tycyjsic.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3lvtwoetg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3efpsaoej.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3rwwrrkxp.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3yveldjje.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ziphwmgv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nzahpvgo.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3mvedrkxl.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3svixwefa.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3pcdzfrom.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3nvmojgil.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3vpjwbice.html


<!-- 参考信息 -->