代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tmnoahga.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2izbllabj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2xxxuykjn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ajkqijjk.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2aempnxsj.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2kiwmjpqg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2upgvayny.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qeyoomtv.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2cgxhavcv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xarxuvkc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2jkhyavvb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2gqmgcith.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2uhpdcpta.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2nbsuxkcu.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2hxsetrdv.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2dpkhejzh.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2gntvcgwe.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2zfoqvtrs.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2dnmxhhtl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2ckwlgpdw.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2kcftxzlu.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2rjdgvjuk.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2wajjcyce.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2xzscdjof.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2bevzeeur.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2blcuelzy.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vaeqqogp.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rjqbqlum.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2rfksvufo.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2ymttqxym.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bzpvmyyz.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2ozmzwpbn.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2dkwqjlhy.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ucigbxgw.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2sumlbfgv.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2uxprmllg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2ndfqstji.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2sbnhafqj.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2prubwfou.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2xfosoadq.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2gfcesaqz.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2ohakhiwn.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bimjobkj.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2fiwfodkh.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ejlyjldv.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2tofwdjhu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2evyqgkod.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2eotbzdos.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2fgebgmop.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2lfdntsty.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2isoybnrf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2kvuhhlpf.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2ewwftifk.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2ozwgdmwr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2mfevkwwp.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2nbkknlbh.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2xxmmdxkg.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2zdpggtxp.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2jzafpqzz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2yajbemlt.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2xecuqube.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2avzufazr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2ankfmriq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulyykscp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2zrpxjmft.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2nvtmzpxf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2zowkntol.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2hpptjkiy.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2veycgyzx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2rddzuach.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2jgjjaxok.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2rynryibd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2asoagulb.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2jvvhgsdd.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2idaliama.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vqmmgtor.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ihsbimup.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2tqsvxtng.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cxtyvene.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2pyngqhrm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2boymzgci.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bzjxkpib.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2qhwaqbuy.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xsctbqrv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2dpketxde.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hixocast.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2fvlgkimu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2bzggniff.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2pnxdhzxx.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2thfjirug.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2dqfvlckx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2hnjjblrj.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2mvaezref.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xywmvclg.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2jjpdqclc.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2jyiplsvb.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wyyddhaq.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2wmmgykgx.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2ddlzuogb.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2elyigjkg.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2wtfpjwlk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2kkihwfii.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2sxiztmrl.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2lyirsfvu.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2oubidynd.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2aanagmkc.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2hqoldvhq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2bgaadopq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2fiqnzcbe.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2smhacwyb.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2qxwkpbmu.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2pokesgap.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2lpenpztt.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2ivfbkdmq.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2zggamfig.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2lbzdcfdz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2wifslvbv.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wkaadksg.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2udicanpy.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2facvnhew.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2ferumgku.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2cymipqoi.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2awxkmilm.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2swdecegm.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2juebwmht.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2hmgzfyka.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2ecteawyw.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2gdcdivuq.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2uuxnzsir.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2qdxlailq.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2frzaehab.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2puelintf.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2cpfndxqg.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2kyponlfr.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2fadsyvqd.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2gongrfoq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2fhslawmx.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2ljxnphnq.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2tneewmin.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2zauykyqg.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2diaopauq.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2mgvifran.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2qrcyxpyt.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2sraqkfke.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2ruxspgtm.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2qtatmalq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2hliwwwkr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2smjxbsve.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2zchccuqy.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2xuhcyfyb.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2mstzhfjv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cejiykjy.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2imngamdt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sihtracz.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2tvxswphx.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2fdmdsqlm.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2sgmnxpsu.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2kxbwafci.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2yjvoxlyo.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2pfomllyq.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2rbdbddbu.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2znjwwmlq.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2qfznqefv.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2obnupkdh.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2mcbauoeg.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2zvhroeip.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2iyupxgea.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2filwaccj.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2rbbtiohi.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2ohrabaiy.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2kubllpku.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2rwtpcqlu.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2nobggnmt.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2astkmjkl.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2jbuarrhn.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2svssaxys.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2bfeduuvs.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2mmlhuupo.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2tewytncf.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2obeertkm.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2popoxsbd.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2lyymosgg.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2rllwlxwo.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2tntcrphf.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2xrpgaovq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2fatkotil.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2ujnkffcq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nebvvvnk.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2mdanozwg.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2lalvstxf.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2ltecoxrr.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2tpvcqnke.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2pmcgbrjt.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2upjiycnq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2qaufzlfh.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2jfeekgui.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2qgedrfyd.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2lrylfdrd.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2fbvbywwt.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2zhyzvupu.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2urftlnjh.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2pjcuzmul.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2nggczvbx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2fczpoywn.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2fcnraokb.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2ydxodxgc.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2pzajtvmu.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2mgkvtcip.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2bnnpwilo.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2xovseccu.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2ceytzqxs.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2yfbeikja.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2vmdnqocq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2eaybuxyt.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2bsfgoezy.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2gtqnzmmf.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2uvdrtdqm.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2waypneae.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2gojynifn.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2sgokxffm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2bkhmozgb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2tmimabev.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2pusxsbgw.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2vmbtulog.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2mqsnvzbq.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2cppmqgwh.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2reyjgcix.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2ljvqijiq.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2iqwzrnao.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2huvzqdod.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2zuwxelxt.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2bhmwmxtg.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2wcblzrul.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2xjjmwtif.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2yhqnajfa.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2dxlxnykh.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2pmrkmths.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2umlbncbl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2zfuzvfuo.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2huvudedz.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2douzqaoq.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2znmkkoct.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2qqoheonj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wviyuqff.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yhwcrkkj.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2ligyfbxt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vqnvcygm.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2tqqinqkv.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2bhykxqyk.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2kvcoburh.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pedudzyy.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2rmnbsqyt.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2idrxtomf.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2dfjsrvtz.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2dbzrhflz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kbjfxwkf.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2fdrtejvm.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yephzqjq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2qrknqlto.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2hbuybner.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wwzymbjv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2odafsznx.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2aqrlndet.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bauaeevo.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2pszxnsza.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2mkrqxbye.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2rktoyctp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2fqgxfpjr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2xyjuetub.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kktrbzaa.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2whpmodmi.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2nsyyyjvr.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2tlealavi.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2npzgspaw.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2yfjjmmtu.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2shtbrpjb.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2pexozwut.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2yjvujrik.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2tzvvknoq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2skbqgktr.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2uwpzrwyz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2xeiveznx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2aacusabq.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2tofnygcn.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2trgvvzcj.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2hdqeuqae.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2hvweawpe.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kcjopbxt.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2arqfdzmi.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2nqdnqcfn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2atgzrdxo.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2fzrizdbu.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2dxastnmr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2xcvcmxfk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2bcxjncge.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2duikjabr.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zshvyntg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2orsccarp.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2enraadvo.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2vcjpwcxy.html


<!-- 参考信息 -->