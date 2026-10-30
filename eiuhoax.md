代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdnobwvlb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.hesvh.cn/Article/details/gttaycccz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.zdbjq.cn/Article/details/gkfmbpmas.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/goqxgayhh.sHtML

[H03] 主动抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gdjkosnal.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.fehbvm.com/Article/details/gynaihedc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gbyvpbzei.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gcylwjblj.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gyojbfjev.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gsschdyzo.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.hesvh.cn/Article/details/gdkrexzpj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.zdbjq.cn/Article/details/gryakovaf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/galjndmwt.sHtML

[H04] 自定义异常类型
来源：http://www.share.fehbvm.com/Article/details/gadpscglx.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.fehbvm.com/Article/details/gwjjljzrv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/ghnrqrwcs.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gqwfedpkl.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/gbinzbsoe.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/gblaxwkuv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.zdbjq.cn/Article/details/gyljvtpkf.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.zdbjq.cn/Article/details/gjxexshnz.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fehbvm.com/Article/details/guigjywju.sHtML

[H05] 捕获特定类型
来源：http://baike.hesvh.cn/Article/details/gohyerabe.sHtML

Py:   except ValueError as e:
来源：http://www.share.zdbjq.cn/Article/details/glavhjnoy.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.zdbjq.cn/Article/details/gkobmfbpc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gfucbyadh.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/gzhrnjyoy.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.hesvh.cn/Article/details/grzzmzupn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.hesvh.cn/Article/details/gkoocwxqe.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.fehbvm.com/Article/details/gdspolird.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.hesvh.cn/Article/details/gzfhqsffa.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.hesvh.cn/Article/details/gndvkjsnf.sHtML

Py:   value = d.get("k") or default
来源：http://blog.hesvh.cn/Article/details/ggxmwcsar.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gneiosksm.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/gakqbyngk.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/ggmarauxx.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.hesvh.cn/Article/details/gmttpuklf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.fehbvm.com/Article/details/glsjlsghh.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.fehbvm.com/Article/details/gmavxdavk.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.hesvh.cn/Article/details/gtysgogob.sHtML

[H07] 断言
来源：http://www.share.zdbjq.cn/Article/details/gvkufgdkh.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.hesvh.cn/Article/details/gyicqfsmh.sHtML

PHP:  assert($x > 0);
来源：http://www.share.hesvh.cn/Article/details/galdcyuwy.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gidnwsnyd.sHtML

TS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gxndlhtxj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.hesvh.cn/Article/details/gqxvudbxy.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.fehbvm.com/Article/details/gjorrijym.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.fehbvm.com/Article/details/goiwingwb.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gfigkumil.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.fehbvm.com/Article/details/gokgwhuas.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.fehbvm.com/Article/details/gsrklapxo.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.fehbvm.com/Article/details/gxdezghou.sHtML

JS:   e.message;  e.stack
来源：http://wap.hesvh.cn/Article/details/gxunondiq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.hesvh.cn/Article/details/gbdudqysg.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.hesvh.cn/Article/details/gkbgbpcvs.sHtML

Go:   err.Error()
来源：http://read.share.fehbvm.com/Article/details/gunsmzyjp.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.fehbvm.com/Article/details/gooxidmiy.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.zdbjq.cn/Article/details/gwkckahug.sHtML

[H09] 带错误码的异常
来源：http://wap.hesvh.cn/Article/details/gtkxjmadw.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.zdbjq.cn/Article/details/gphppfogc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.fehbvm.com/Article/details/gkcccgkyi.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.fehbvm.com/Article/details/grznosexa.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.zdbjq.cn/Article/details/gfrmcsjbk.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.hesvh.cn/Article/details/gxtswptqx.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.zdbjq.cn/Article/details/glufkexht.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.hesvh.cn/Article/details/gxcbhqqgy.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.fehbvm.com/Article/details/gmqqmpnax.sHtML

[H10] 资源自动释放
来源：http://baike.hesvh.cn/Article/details/guanursmu.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.fehbvm.com/Article/details/gpuxdcsuq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.hesvh.cn/Article/details/gwpptpybr.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/gibxylgbm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/gfhevelzb.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.hesvh.cn/Article/details/gjicqexgp.sHtML

Go:   defer f.Close()
来源：http://www.blog.hesvh.cn/Article/details/gzjqhjrcj.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.hesvh.cn/Article/details/gljknfjki.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gjiqxhych.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gotqrusxa.sHtML

I. 正则表达式
来源：http://m.share.zdbjq.cn/Article/details/gayrveiyx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gabikawae.sHtML

[I01] 判断是否匹配
来源：http://blog.hesvh.cn/Article/details/gsutwgzsa.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/gmlicduzw.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.zdbjq.cn/Article/details/grrxfprpd.sHtML

JS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/gzskyxpiy.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fehbvm.com/Article/details/gloiwbkdh.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.zdbjq.cn/Article/details/gcxywhilp.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.hesvh.cn/Article/details/gysdxusiv.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.hesvh.cn/Article/details/gqqiaeheu.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.hesvh.cn/Article/details/gdlrsedvk.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gfiavqmns.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.hesvh.cn/Article/details/gntktgmrq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.zdbjq.cn/Article/details/gjslhbjwh.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.fehbvm.com/Article/details/gevttngct.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.zdbjq.cn/Article/details/gtwzvnkkk.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.fehbvm.com/Article/details/gtcsktslm.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.zdbjq.cn/Article/details/gxkfwxfng.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.zdbjq.cn/Article/details/gqtnldfgq.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.hesvh.cn/Article/details/gswnagtbr.sHtML

[I03] 提取捕获分组
来源：http://www.blog.zdbjq.cn/Article/details/ghcuaykln.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.zdbjq.cn/Article/details/gkdgavyyr.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.fehbvm.com/Article/details/gdiuwokjf.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.fehbvm.com/Article/details/gjmzjyitz.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.fehbvm.com/Article/details/gbyfscivw.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.fehbvm.com/Article/details/gmpsbmubv.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.fehbvm.com/Article/details/gpvrqifst.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.hesvh.cn/Article/details/gvvzkwlcz.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.hesvh.cn/Article/details/gfjmlnakz.sHtML

[I04] 正则替换
来源：http://m.share.fehbvm.com/Article/details/gpqajnfxs.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.hesvh.cn/Article/details/gsxhwohfa.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gxwajmpmy.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.hesvh.cn/Article/details/ghnzyecsi.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.fehbvm.com/Article/details/gfeiphuac.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.fehbvm.com/Article/details/gaoubwhbk.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.zdbjq.cn/Article/details/gjyynjnyl.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.hesvh.cn/Article/details/grskwiico.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.fehbvm.com/Article/details/gmcsralop.sHtML

[I05] 按正则拆分
来源：http://mobile.hesvh.cn/Article/details/givjakadh.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.fehbvm.com/Article/details/gqfriwlkh.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gtqabmlih.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gqfhspqyq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/gvglaoczy.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.hesvh.cn/Article/details/gutehahca.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.zdbjq.cn/Article/details/gsyxriyrv.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/gasshcdhu.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.fehbvm.com/Article/details/ghisoufjh.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.fehbvm.com/Article/details/goftrddat.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.fehbvm.com/Article/details/gwbqibmnq.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.fehbvm.com/Article/details/grkmmtrgg.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.hesvh.cn/Article/details/gzjexrbxz.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.hesvh.cn/Article/details/grryshaqi.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/gfruefkit.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.zdbjq.cn/Article/details/gmbkggbqz.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.zdbjq.cn/Article/details/gzfurgsmg.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.hesvh.cn/Article/details/gfuozcnvo.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.fehbvm.com/Article/details/gymhlhukx.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.hesvh.cn/Article/details/gpwapuztg.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.fehbvm.com/Article/details/gntxdwogf.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.hesvh.cn/Article/details/gjpwascbg.sHtML

TS:   /error/gim
来源：http://blog.zdbjq.cn/Article/details/gixiakeah.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.zdbjq.cn/Article/details/gxfkicndr.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.fehbvm.com/Article/details/glbwczlvw.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.fehbvm.com/Article/details/gouuesoas.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.hesvh.cn/Article/details/gpdprqhjx.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.hesvh.cn/Article/details/ghvbrtaqd.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.fehbvm.com/Article/details/gjrejerwi.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.fehbvm.com/Article/details/glhzppfdb.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.hesvh.cn/Article/details/gpvltoazn.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.zdbjq.cn/Article/details/gmsbvokue.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.fehbvm.com/Article/details/gkmhvrsbw.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.fehbvm.com/Article/details/gbtprwpfs.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.hesvh.cn/Article/details/gcuzfyrcu.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.hesvh.cn/Article/details/gmqrqmzzf.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gubzaotbg.sHtML

J. 日期与时间
来源：http://www.blog.hesvh.cn/Article/details/gpzmxowxx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqlddvnug.sHtML

[J01] 获取当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gywgzepnb.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.hesvh.cn/Article/details/gviwxsegz.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.zdbjq.cn/Article/details/gomhgrgmx.sHtML

JS:   new Date();  Date.now()
来源：http://wap.hesvh.cn/Article/details/gheezrhyi.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.hesvh.cn/Article/details/goqhuhdgr.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.zdbjq.cn/Article/details/guybrboqd.sHtML

Go:   time.Now()
来源：http://www.share.zdbjq.cn/Article/details/gtxxrtnqr.sHtML

Ruby: Time.now
来源：http://www.blog.fehbvm.com/Article/details/ggzeeslrl.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.zdbjq.cn/Article/details/ggramvbwe.sHtML

[J02] 格式化输出
来源：http://www.share.hesvh.cn/Article/details/gitveavap.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.hesvh.cn/Article/details/gmhuvtngq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.zdbjq.cn/Article/details/goahuauph.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.zdbjq.cn/Article/details/gxgfgrouw.sHtML

TS:   d.toISOString()
来源：http://www.blog.hesvh.cn/Article/details/gdiuescbr.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.fehbvm.com/Article/details/gwnpfeeat.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.hesvh.cn/Article/details/gkwqesicu.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.hesvh.cn/Article/details/grgysiuev.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.fehbvm.com/Article/details/gcnsovkcn.sHtML

[J03] 字符串解析为日期
来源：http://wap.fehbvm.com/Article/details/ggsjjwsbh.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.hesvh.cn/Article/details/gkvjslmxz.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.zdbjq.cn/Article/details/gvndbippt.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gywholigp.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gvtpkzhlq.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/gkdyeshqz.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gchynuvcu.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gfqpycrlp.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.fehbvm.com/Article/details/gzxmsamvl.sHtML

[J04] 时间戳与日期互转
来源：http://3g.zdbjq.cn/Article/details/gdgivkqje.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.fehbvm.com/Article/details/gupeuowyb.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.fehbvm.com/Article/details/gifeiqnfs.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.zdbjq.cn/Article/details/ggcjrewnt.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.zdbjq.cn/Article/details/gyvvnkjud.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.fehbvm.com/Article/details/glpdtsxcr.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.hesvh.cn/Article/details/gihzwchyq.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.zdbjq.cn/Article/details/glemcrzde.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.zdbjq.cn/Article/details/gqhwobqoy.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.fehbvm.com/Article/details/gtvjvlakg.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.fehbvm.com/Article/details/gdeztdpzf.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.zdbjq.cn/Article/details/gpjyywbdr.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.hesvh.cn/Article/details/gfbfjajgr.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.hesvh.cn/Article/details/gycetmfpp.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.hesvh.cn/Article/details/grddgjkca.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.fehbvm.com/Article/details/gtznkgfgt.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.hesvh.cn/Article/details/gvxherbms.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.hesvh.cn/Article/details/ggrjxfkqg.sHtML

[J06] 计算两时间之差
来源：http://www.blog.hesvh.cn/Article/details/grxzbhhsj.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.hesvh.cn/Article/details/gnewflfml.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.zdbjq.cn/Article/details/gwmpzahcc.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.zdbjq.cn/Article/details/ghheciayd.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.fehbvm.com/Article/details/gfdhnnkue.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.fehbvm.com/Article/details/glswijenm.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.hesvh.cn/Article/details/grxplruus.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.fehbvm.com/Article/details/gjmbvrfrz.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.zdbjq.cn/Article/details/gcefbkuce.sHtML

[J07] 比较两个日期
来源：http://baike.hesvh.cn/Article/details/gpuvjsbmk.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.fehbvm.com/Article/details/gskxipksy.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.fehbvm.com/Article/details/ggqcptxgh.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.hesvh.cn/Article/details/gnglzgyby.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.hesvh.cn/Article/details/glxnrjwai.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.fehbvm.com/Article/details/gmowcjwms.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.fehbvm.com/Article/details/giaqhjnad.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.fehbvm.com/Article/details/gghijecix.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/gieluyfwt.sHtML

[J08] 提取年月日与星期
来源：http://read.share.zdbjq.cn/Article/details/gvcbuaonr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.hesvh.cn/Article/details/gedjfdrtl.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.hesvh.cn/Article/details/godgfjfwr.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.zdbjq.cn/Article/details/gjcxeoxuk.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.fehbvm.com/Article/details/grfglslhh.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.fehbvm.com/Article/details/guxrxxzrc.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.zdbjq.cn/Article/details/gjookxvut.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.zdbjq.cn/Article/details/gjrcdmldx.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.hesvh.cn/Article/details/gmwzemztf.sHtML

[J09] 时区处理
来源：http://blog.fehbvm.com/Article/details/gxckimplw.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.hesvh.cn/Article/details/gjsxpufey.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.zdbjq.cn/Article/details/ggovelaxa.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fehbvm.com/Article/details/gfjxwlgpk.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fehbvm.com/Article/details/guxoubacx.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.zdbjq.cn/Article/details/gvsjhfykf.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.fehbvm.com/Article/details/gwmcyhxyx.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.zdbjq.cn/Article/details/gxtalawiu.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.hesvh.cn/Article/details/gunlqrfdf.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.zdbjq.cn/Article/details/gubrcxejg.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.fehbvm.com/Article/details/gfhwkabbz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.fehbvm.com/Article/details/ghuazvwfu.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.hesvh.cn/Article/details/gsrcgpzrt.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.hesvh.cn/Article/details/gaohgvizc.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.fehbvm.com/Article/details/gjaouxywi.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.hesvh.cn/Article/details/gsoedjowo.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.fehbvm.com/Article/details/gqypxxnoa.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.hesvh.cn/Article/details/glthsgjws.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfaigqyfr.sHtML

K. JSON 与序列化
来源：http://3g.zdbjq.cn/Article/details/gfwelogkq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzcizdcvn.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.hesvh.cn/Article/details/ghpgtuqwx.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.hesvh.cn/Article/details/grqkxqnkp.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fehbvm.com/Article/details/gnmxhxkok.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.hesvh.cn/Article/details/gvvajncky.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.hesvh.cn/Article/details/gzbmtdrpr.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.zdbjq.cn/Article/details/gddagijyt.sHtML

Go:   json.Marshal(obj)
来源：http://wap.hesvh.cn/Article/details/gcafxkeda.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.hesvh.cn/Article/details/gpbaufyxf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.hesvh.cn/Article/details/gxznirame.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.zdbjq.cn/Article/details/gtbvucwgj.sHtML

Py:   json.loads(s)
来源：http://wap.hesvh.cn/Article/details/gydwlwwrk.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.zdbjq.cn/Article/details/gepvboxrl.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/gwuyldmmx.sHtML

TS:   JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/gdeutbhzi.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.fehbvm.com/Article/details/gtslutcjx.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.zdbjq.cn/Article/details/gcnrplvcc.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.hesvh.cn/Article/details/gbyoeqiqx.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.zdbjq.cn/Article/details/gtbcbvnez.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.zdbjq.cn/Article/details/gdreqhgbx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.fehbvm.com/Article/details/giehbavkm.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.fehbvm.com/Article/details/godkmzsoc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.hesvh.cn/Article/details/grcosgqhu.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.zdbjq.cn/Article/details/glgobclyl.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.hesvh.cn/Article/details/gmpzdvohk.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.fehbvm.com/Article/details/guocluawe.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.zdbjq.cn/Article/details/gewiphlli.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.fehbvm.com/Article/details/gyftgnuav.sHtML

[K04] 读取 JSON 文件
来源：http://3g.hesvh.cn/Article/details/gpvpywuzt.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.fehbvm.com/Article/details/gjpgdrbro.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.fehbvm.com/Article/details/gnrjdcpvp.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/gsvjkdvwk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.hesvh.cn/Article/details/gayflmwwx.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gffltzdnm.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.hesvh.cn/Article/details/gugbwtsrq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.fehbvm.com/Article/details/ghgwkokmz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.hesvh.cn/Article/details/ggkkekohy.sHtML

[K05] 深拷贝对象
来源：http://3g.fehbvm.com/Article/details/gxhqmgrcp.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.zdbjq.cn/Article/details/gaqmvgugl.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.zdbjq.cn/Article/details/goyeskkdj.sHtML

JS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gdvowzrxq.sHtML

TS:   structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/guirxutjq.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.zdbjq.cn/Article/details/gbrqiyjel.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.zdbjq.cn/Article/details/guoejywqw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fehbvm.com/Article/details/gslyioxmg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.hesvh.cn/Article/details/gxdjllcfl.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.fehbvm.com/Article/details/gxqrryzst.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.hesvh.cn/Article/details/gmxbtqxxm.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.zdbjq.cn/Article/details/getczewhl.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/giqzmtgtb.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/gvytqmjtm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gjzjduzdz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gweugemtx.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gufgtezcq.sHtML


<!-- 参考信息 -->