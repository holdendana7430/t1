代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3zuuruhkj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3lgmatuwk.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3mljsrige.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3zwkuvqzu.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3ctgrshab.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kzmwzofn.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3ylaanygv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3iwmizzrp.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3khmtbdei.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cygqtoxt.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3rtpenwui.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3hmfobyji.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3uxkwxbki.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3seutrupx.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3wnxtzjnt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ohybhjun.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ydrprmid.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rjzxgebq.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3wbmmhbaq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3yuihqzmb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3zmcuhvmd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3dywnztxa.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3qzaxhqij.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3jemrfpaq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3cbtdcyca.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3nzdmhwzw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3thwdyxtr.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3xptdrxze.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3xppuehpv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qpsbxrwo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cctuxmin.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zdmlgrxf.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3rxdsnazi.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3wsyoyhto.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3rzhtwacx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3giywbxxi.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3jmyxfuyz.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3msznypdb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ofjcsvcu.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3kwwrykhm.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3slibplcv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wdjppnjo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3iemlvonk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3osagejif.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3gbnnwpny.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3pymfhkpg.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3gyrizzvc.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3mmdcmisb.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3iktuaelh.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3jpoqevbu.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ggpqpnna.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3zbcrtngh.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3vofnfmsm.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3cscbasth.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3ptsoohpe.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3iyxdmbcn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3gdfcmmlu.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3taatygna.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cbigpiqj.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ltioxsqo.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3tuvkeytr.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3mtsbdckd.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3erhzqaph.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3madtmhwl.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3zfoktpvm.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3xqrwgpto.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3bmmxzicz.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3rlxbsfrb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3bfapzetf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3luncomwl.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3gjzbruoy.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3yurzoele.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3adscperr.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3fjgijglw.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3woiizotc.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3bcqzjkdr.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3eruxdvot.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3jimymums.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3aevxsnqy.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3uldfqgoq.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3odrbnafj.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3zbwdywok.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3dsvyljfm.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3lirnamql.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3cfjscdru.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3jnyilbpt.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3deqmbzda.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3uuciwiuk.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3slyvkyou.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3qgyzothv.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3hoarfmgg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3jpvkjpka.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3zducynej.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3beggwmig.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3sazadutb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3vvspgnim.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3rbdwywcu.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3zookthds.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3viccxwju.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3rjmnmleb.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3edocxafo.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3vthzqtmf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3jtbwovjx.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3xmvpyjhp.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3neidslvj.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3cvyyzmno.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3ybsygygu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3shfnioiy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bthudfpa.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3norzlqio.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xpqnxvyz.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3nbznmiql.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3eaibmfxs.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dnivbwrj.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wpngwyml.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3acobgvtv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3krnufclu.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3oyypmczi.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3kwabwykg.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3rjpfnqpr.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3qwpzmozw.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3phewunpd.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3vjecrbwx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3ummtihqu.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3mrkizqag.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ftzycymu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3rxcpfkqv.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3ujjrdgsv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xfmanebi.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3vpxbfavc.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xowgwluy.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3hnabdpfj.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3kwawmhso.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3okoacsho.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3zxncgink.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3bzjdclzi.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3emptewro.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3ihewpbef.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3ojjanabc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3yjuwhpyg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3meuumtgs.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3kysuzrxj.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3gwxtxwdy.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3atqrmbhn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3opaibzxb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3cgelvpui.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3kadebnaz.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3yzoiskwn.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3cnmtahao.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3hxqfznho.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3ruhdlyuf.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3gdddxjio.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3meluvpwh.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3hpdmtsva.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3zgarsrin.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3wuxsqcll.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3rnfzmbkl.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3yjtjwfyi.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3quauhiuc.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3atodwrsl.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3hjovsifc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3eaybeyhw.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3dyxaqdey.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3xsajsqoh.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3sffslitj.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3fqhobjai.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3aptshngc.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3biulbyxy.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3imesrbpn.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3iblpjwdz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3dckapoti.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3mbnejadj.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3jkxcpakz.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3boysgemd.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3ojsfbxct.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3unysyjjl.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3zyekjjvy.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3dhfzpjdc.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3mtybrdgn.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3fydgxvkm.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3slqjjihx.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3hkdyrahg.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3owsjwriz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rvuhqqac.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3eimdjiht.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lfpcmjxg.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3mcwsiqqq.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3eqcaitpm.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3uvhwfxhf.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3vudchhwh.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3rtjqmeen.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3ujedvdgu.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3vuybgakz.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3kpkfhgtb.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3uzmndttf.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3qcdelavk.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3pyxrfjax.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3olcnfpzz.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3hpkwfyqn.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3eelcwvlm.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3poyuwkfm.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3mdanqzbb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3htvraiei.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3uqzppefo.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3zidtuiah.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3sdklzojl.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3qvlamjuc.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3xmjbjqng.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ialhcful.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3vhbbduke.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3pddkrgsb.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ruwsvrnw.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3oqamukos.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3wgurfncj.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3bqirztiz.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3ywngvjrl.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3zpjsaeji.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3ekvbuqrl.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3dbichaqk.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ptnmskzn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3dvpmempp.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3maobntau.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3plqyxatk.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3kesuxety.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3gztdoxcj.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3qeqjfqbq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3tqbncwhm.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3bfpjqwqt.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3dgowahvl.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3qarklyme.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3llwuueqb.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3wjpfhtfm.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3ionzyzno.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3zvybtloe.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3grbjliiv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3gyvlpaoy.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3xecifuiv.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3welpdnvq.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3wsrfcnfv.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3qkuztlhr.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3spgkfqpl.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3kyajnfup.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3kirhectk.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3gopkewsa.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3uhxebpnw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3kuckyqez.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3xihsdlis.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3zbmsxvfp.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3fklxbdow.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3dkadpsxh.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3yczcakxc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3sceysgjn.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3kxvactpz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3dkrikxza.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3gexngywf.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3gqsxmjhe.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3yrnjhrjy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3slbwteuu.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3rsbcnzjs.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3otiblvma.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3zglhaiyq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3utyrjyvs.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3pagijkdo.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3gszbktpu.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3jaasesek.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3fkodxssz.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3uquqbfkg.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3peutccyr.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3emcoxsmu.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3rfvhgqil.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3nywqlrna.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kvackjfh.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3orwyyona.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3fowqtqnv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3rbkmruuq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3ozaoaizo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3njcmdzun.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3tqrqibaw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kaksdcki.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zpmbdytt.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3yppaomyh.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3lujsjhcy.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3slrmpvly.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nfiixmib.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3sqzocbrq.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3rzdkofsh.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3tzrpfjam.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3trkivzxo.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3naugpsgi.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fwsqlwlk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3corzgfvd.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bxgkqzie.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kgwmhujq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3jhatulxf.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3ebgkqrmk.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3xnyfjetx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3cthhepvf.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3himfdhvm.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3ggavkebo.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ilxsgyug.html


<!-- 参考信息 -->