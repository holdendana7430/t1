代发 wailian999

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ekddpltx.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3houoicki.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3kgvqdjac.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3zgregkzh.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3pcibkmlp.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3hxnoapsv.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3xfyvcsij.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3vkzdffcq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3xxlwqupv.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lnhrranc.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pxonlrtd.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3avuoedkj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3wccxhvju.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3hcyrxrgz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3ubdokesx.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3jifohnrp.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3xesdiwis.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3xnqwseyi.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3hkshsrej.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3mxnslnbt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3qdykedcf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3aojajzru.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3ugtwpbqf.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3surwypki.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3bbhkflen.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3bocqnhqe.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3zudgsdln.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3warvrqew.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bhkqzzum.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3kcmfsaru.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3wdnbsqpz.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3ltbvbjhm.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3kbqznivl.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3kcqjmqek.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3rifqmoyt.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3daqxczlq.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3rdcusncl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3gimvojll.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3fdneccei.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3wwlxfkic.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3xvyagkdc.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3lmyoaicy.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3gkfaencs.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3odqwoutt.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3ispgvqzc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3vkyurpcn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3aukfhlak.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3kafdfdqw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3emkcyrej.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3pzlvvgrh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3jisuaeub.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3rijhrmrc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3iyfciebk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3liheeazh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3ymwgoqds.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3uwkhqscb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3bvxuusyv.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3ewrdvwgp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3rfoswuju.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ztmqeyhj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gqlgcsml.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3ykvstxmx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hsqtkcgn.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3sqlbionv.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3wgiokjuy.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3dzbvhdiv.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3gxzmypvo.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hgtlesnb.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3sqwyhyqg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3zcfkdjrg.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3rsksenwj.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3qrdojvmz.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3yferpemi.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3iyhlcnuw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3bwctbzok.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3lfnausfg.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3tdpspisd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3odggbvpj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3bujlwynx.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3yulytmdq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zjiyxkkn.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3hwgfxmsd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3irhhdzpi.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3ulfgrksw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3ozofnngp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3xijevmww.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3dptrhhis.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3ehvilvzf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3tykxodiu.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3rvndawsk.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3zplrvuwu.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3qnzeurvq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3odvjwoag.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3euxxtycm.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3eikcfmyu.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3iybrguic.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3fcmgctvv.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3wgxecvrq.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3brrrousr.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3ecilymsa.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3ntifyrli.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3sluqqevc.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3rxshljtc.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3tnwkdnex.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3eowwxbum.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3bvljlaft.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3sxpiaflf.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3ceodfmrt.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3lfgwlydr.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3cfmmyafc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3sfrejrkd.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3qbtdivbz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3ktlvepxl.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3nbbckuct.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3roksfypj.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3iensfutz.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3nznwxlzr.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3awaxxvyj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3hqbdnesv.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3axbxxppx.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3lhgdfjpn.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3nidaufve.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3lqfizhev.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3sowwjbez.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3wfoohrcc.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3cdhwyqmf.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3diegydbe.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3beaepzkr.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3itzjbqgb.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3iwfprhnw.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3xckhkrkr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3rwdgwaon.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3drsldugx.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3xbvbnpkx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3ypezmiex.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ouvxohfd.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3yohcafol.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nwkoeekn.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3xaibfyrk.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3zpzepskn.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3oyzxxgby.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3fdkuzjof.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3tbajzxsv.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3yjwpurfy.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3igkfdxjm.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3tfbikqkk.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3djiqynle.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3uwdxlcdm.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3grrlkoci.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3roahyryt.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3nncthmnx.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3ewknpdwy.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3mpfbgeyq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3szhgrhpv.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3nuelawax.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3mdfqxzoe.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3yafkwkio.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3cstrhups.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3ggycvxuc.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3qdfwfauf.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3mkhyepeq.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3onjrohjy.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3xneusnmj.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3quivilny.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3ftwfckpz.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3lvjmawnj.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3xvonmeqd.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3banzkgrd.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3ovgocjjm.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3btrupszi.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3bfbiuswk.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yokjiyua.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3bpgvigoj.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ztaddsqy.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3yhxkzoko.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3nkrtvohl.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3pmrwmdmd.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3kkvhdygb.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3qbnzqnqg.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3yzkkohsf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3tggwnczv.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3qlvyoqvl.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3hdeoqifv.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3hcvvvsxl.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3tpuzoopx.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3hivxrpqb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3spdiwsfk.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3alpbqdyx.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3tzqihljs.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3lbmaxfwq.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3djkwemyp.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3dfshqacl.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3ubyumvdk.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3kcfvvcck.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3bqtfnlzb.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3dsvxnjst.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3bpqqkspx.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3lsznmxsq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3zfcphdfq.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3iywovzkk.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3bceiokjg.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3jzboklkc.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3xyrwejef.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3tpshczod.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3clpzfhnj.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3iotgbmyh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3ooihcacj.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3imybsivn.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3gmcinxps.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3zdkaykga.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3odloehpq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3rllhuttz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3rhlfhkdi.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3xmfkwbqz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3mqyirrzc.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3dskusbdo.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3htypongd.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3xvpumvoa.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3rsvkmtog.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3xeiikvrw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3hlvoagla.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3mcfridcv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vlturykf.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3bqawxjzc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3cdokslwj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3xkweoigg.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3nvnnkivo.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3rkcxnbtx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mkkpxptn.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3onlovhhw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jpiwvbkf.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wnsuchwf.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3tkumpgap.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3nrmirwxm.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3pmvjjxzz.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ylqvuffo.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3hwdoysow.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3aoixkscz.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3nmwwbcgj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3obiuxwuu.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3wxeheheh.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3cjvpuaqh.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3ciuoxexz.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lmkminle.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oujhryqq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3jkpruclu.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3dtqrotal.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tncgxoce.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pwluadbb.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3vkuptesp.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3fjacwqfa.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3vikhatll.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ulagneai.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vssdkhhf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3ytozriel.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3trmapwza.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3offenukq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3ilynedbf.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3dfmziipp.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3ibgmniph.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3ghuzhitw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3edenmfrm.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3yxmsydpo.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3lmdzorhg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3xthfgoif.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3aypxwyok.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3dweyqpyu.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3klymxhzh.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3qzccfgxm.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3ktvydneb.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uyflrddp.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bvtwfxwd.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3sgxvgxoe.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3alabnelc.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ilqczwmd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3fkjafpzb.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3bdhzjsvh.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3rtrkjtoa.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3mpafwtum.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3smqlpdjz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3nggkitcc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3omnysybu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3aboctfrl.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3kawjsypn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3rwbmmrvc.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3zhqjhsoh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3kqmhwlfx.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3powzwjgv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3mdgoxnkk.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xuthlhlm.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3aroexojo.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3jdvjvese.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3vroyjseu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3hildnfwn.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3svclglfv.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3evgzqtzk.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3sjvyxoib.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3niwdkajg.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3zpvzhdzk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3rlmboyzg.html


<!-- 参考信息 -->