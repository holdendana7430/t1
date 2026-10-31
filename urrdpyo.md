代发 wailian999

H. 异常与错误处理
来源：http://dk.wgjwhj.cn

================================================================================
来源：http://pq.wgjwhj.cn

[H01] try / catch 基础
来源：http://bc.szsharing.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pn.nicolike.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tn.shxzukj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ts.wgjwhj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ip.9csxet.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://to.521024.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cu.newstarts.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jr.muxihuayi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lq.muxihuayi.cn

[H02] finally / ensure 收尾
来源：http://ve.szsharing.cn

Py:   try: f()⏎finally: cleanup()
来源：http://vi.9csxet.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://wu.szsharing.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://va.bookmarksfly.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://sr.yuntaijiaju.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ya.hnjuh.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://gw.bookmarksfly.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://av.huanxung.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ab.huixinmuqiang.cn

[H03] 主动抛出异常
来源：http://zv.asd995.cn

Py:   raise ValueError("错误信息")
来源：http://jl.newstarts.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bo.yuexingan06.cn

JS:   throw new Error("错误信息");
来源：http://rn.haigaiapp.cn

TS:   throw new Error("错误信息");
来源：http://va.yuntaijiaju.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://rs.9csxet.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fm.hahajie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ae.huixiangedu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://qp.jctech888.com.cn

[H04] 自定义异常类型
来源：http://ue.nicolike.cn

Py:   class MyError(Exception): pass
来源：http://zf.shxzskj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://oq.szsharing.cn

JS:   class MyError extends Error {}
来源：http://do.colortex.cn

TS:   class MyError extends Error {}
来源：http://ri.yuntaijiaju.cn

Java: class MyException extends RuntimeException {}
来源：http://qm.muxihuayi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bt.lnxyls.cn

Ruby: class MyError < StandardError; end
来源：http://tj.asd995.cn

C#:   class MyException : Exception {}
来源：http://ep.bjjhwx.cn

[H05] 捕获特定类型
来源：http://sm.huixinmuqiang.cn

Py:   except ValueError as e:
来源：http://lv.szsharing.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ys.9csxet.cn

JS:   if (e instanceof TypeError) {}
来源：http://it.hahajie.cn

TS:   if (e instanceof TypeError) {}
来源：http://nd.bookmarksfly.cn

Java: catch (IOException | SQLException e) {}
来源：http://yx.gzmigu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xv.huixiangedu.cn

Ruby: rescue ArgumentError => e
来源：http://an.newstarts.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nz.nszjky.cn

[H06] 可选值 / 空值安全访问
来源：http://ok.jianghongdianzi.cn

Py:   value = d.get("k") or default
来源：http://zj.huixinmuqiang.cn

PHP:  $v = $d["k"] ?? null;
来源：http://zo.gzmigu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://fw.9csxet.cn

TS:   obj?.a?.b;  d ?? default
来源：http://at.shxzukj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cf.hahajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ho.521024.cn

Ruby: d&.dig(:a, :b)
来源：http://oi.shxzukj.cn

C#:   obj?.A?.B ?? default
来源：http://fy.colortex.cn

[H07] 断言
来源：http://lu.yuntaijiaju.cn

Py:   assert x > 0, "必须为正"
来源：http://rx.hahajie.cn

PHP:  assert($x > 0);
来源：http://ad.wgjwhj.cn

JS:   console.assert(x > 0);
来源：http://aa.jctech888.com.cn

TS:   console.assert(x > 0);
来源：http://sv.colortex.cn

Java: assert x > 0 : "必须为正";
来源：http://zj.nicolike.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jf.colortex.cn

Ruby: raise "必须为正" unless x > 0
来源：http://kc.colortex.cn

C#:   Debug.Assert(x > 0);
来源：http://py.hnjuh.cn

[H08] 获取错误信息与堆栈
来源：http://tk.szsharing.cn

Py:   str(e);  traceback.format_exc()
来源：http://su.yuntaijiaju.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yu.shtwfgs.cn

JS:   e.message;  e.stack
来源：http://wd.jianghongdianzi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pk.jianghongdianzi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://dw.hahajie.cn

Go:   err.Error()
来源：http://ht.panjiajie.cn

Ruby: e.message;  e.backtrace
来源：http://fw.colortex.cn

C#:   e.Message;  e.StackTrace
来源：http://qd.haigaiapp.cn

[H09] 带错误码的异常
来源：http://bd.szxytkj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://sq.asd995.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://yo.521024.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rf.hnjuh.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ql.haigaiapp.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ms.asd995.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dt.hahajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jj.szsharing.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://mv.shtwfgs.cn

[H10] 资源自动释放
来源：http://vf.bookmarksfly.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://gy.jctech888.com.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hf.yuexingan06.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lu.bjjhwx.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ff.newstarts.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dj.muxihuayi.cn

Go:   defer f.Close()
来源：http://vc.bjjhwx.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ph.hnjuh.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fw.szxytkj.cn

================================================================================
来源：http://ym.yuntaijiaju.cn

I. 正则表达式
来源：http://wc.hnjuh.cn

================================================================================
来源：http://cy.yuntaijiaju.cn

[I01] 判断是否匹配
来源：http://bi.lnxyls.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zn.gzmigu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://mw.haigaiapp.cn

JS:   /\d+/.test(s)
来源：http://em.huixinmuqiang.cn

TS:   /\d+/.test(s)
来源：http://bh.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ya.nicolike.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dw.wgjwhj.cn

Ruby: s.match?(/\d+/)
来源：http://rk.9csxet.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xq.jctech888.com.cn

[I02] 提取所有匹配
来源：http://vc.hnjuh.cn

Py:   re.findall(r"\d+", s)
来源：http://mn.bjjhwx.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xb.yuexingan06.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qe.bookmarksfly.cn

TS:   s.match(/\d+/g)
来源：http://sr.asd995.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kc.shxzskj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://uf.nszjky.cn

Ruby: s.scan(/\d+/)
来源：http://tn.nszjky.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mx.9csxet.cn

[I03] 提取捕获分组
来源：http://tu.hnjuh.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jr.huanxung.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hh.521024.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ls.bookmarksfly.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ym.chemitech.net.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nx.shxzukj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xw.9csxet.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zy.szxytkj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rj.hnjuh.cn

[I04] 正则替换
来源：http://tc.521024.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://de.hahajie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yu.panjiajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://wq.yuexingan06.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ct.jianghongdianzi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://gm.bookmarksfly.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ek.colortex.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://zo.colortex.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ls.szsharing.cn

[I05] 按正则拆分
来源：http://zo.jctech888.com.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://el.shxzskj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pn.nicolike.cn

JS:   s.split(/\s*,\s*/)
来源：http://nt.nszjky.cn

TS:   s.split(/\s*,\s*/)
来源：http://nv.shxzukj.cn

Java: s.split("\\s*,\\s*")
来源：http://mn.yuexingan06.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ik.nicolike.cn

Ruby: s.split(/\s*,\s*/)
来源：http://to.szxytkj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qv.chemitech.net.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qv.panjiajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ur.muxihuayi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hn.shxzukj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tn.9csxet.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ma.9csxet.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mi.colortex.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kb.huixiangedu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sv.hnjuh.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pe.shxzukj.cn

[I07] 忽略大小写与多行模式
来源：http://ga.jctech888.com.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://me.shxzukj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fq.muxihuayi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wc.huanxung.cn

TS:   /error/gim
来源：http://az.chemitech.net.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qg.huixiangedu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ro.szsharing.cn

Ruby: s.scan(/error/i)
来源：http://yn.gzmigu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fh.newstarts.cn

[I08] 贪婪与非贪婪匹配
来源：http://ph.panjiajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jh.bjjhwx.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://iz.yuexingan06.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zn.yuexingan06.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ej.521024.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zl.huanxung.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yh.newstarts.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dd.huixiangedu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sw.hnjuh.cn

================================================================================
来源：http://sw.huanxung.cn

J. 日期与时间
来源：http://zh.9csxet.cn

================================================================================
来源：http://ry.bjjhwx.cn

[J01] 获取当前时间
来源：http://th.jianghongdianzi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://tg.huixinmuqiang.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pk.huixinmuqiang.cn

JS:   new Date();  Date.now()
来源：http://rc.hnjuh.cn

TS:   new Date();  Date.now()
来源：http://yl.newstarts.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fx.shxzukj.cn

Go:   time.Now()
来源：http://ti.nicolike.cn

Ruby: Time.now
来源：http://vv.szxytkj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jx.newstarts.cn

[J02] 格式化输出
来源：http://yy.lnxyls.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gf.huanxung.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ri.panjiajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sv.lnxyls.cn

TS:   d.toISOString()
来源：http://qb.chemitech.net.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ar.hahajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rx.jianghongdianzi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qz.colortex.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rs.muxihuayi.cn

[J03] 字符串解析为日期
来源：http://lp.jctech888.com.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ms.asd995.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dv.szsharing.cn

JS:   new Date("2024-01-02")
来源：http://of.huanxung.cn

TS:   new Date("2024-01-02")
来源：http://lu.bjjhwx.cn

Java: LocalDate.parse("2024-01-02")
来源：http://kn.bjjhwx.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hf.wgjwhj.cn

Ruby: Date.parse("2024-01-02")
来源：http://ee.muxihuayi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wo.yuntaijiaju.cn

[J04] 时间戳与日期互转
来源：http://yt.szxytkj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://or.szxytkj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uh.haigaiapp.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kc.chemitech.net.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://yy.lnxyls.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yj.huixinmuqiang.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xq.wgjwhj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ez.panjiajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ze.shxzukj.cn

[J05] 时间加减（加 7 天）
来源：http://dn.shxzukj.cn

Py:   now + timedelta(days=7)
来源：http://lj.shtwfgs.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://nc.szsharing.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nt.gzmigu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wi.shtwfgs.cn

Java: LocalDate.now().plusDays(7)
来源：http://ps.szsharing.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zr.yuntaijiaju.cn

Ruby: Time.now + 7 * 86400
来源：http://vt.nszjky.cn

C#:   DateTime.Now.AddDays(7)
来源：http://zm.9csxet.cn

[J06] 计算两时间之差
来源：http://tu.521024.cn

Py:   (end - start).total_seconds()
来源：http://lk.lnxyls.cn

PHP:  $end->diff($start)->days;
来源：http://wa.nicolike.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://br.huanxung.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://uj.huanxung.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ar.shxzukj.cn

Go:   end.Sub(start).Hours()
来源：http://hq.hnjuh.cn

Ruby: end - start                 # 返回秒数
来源：http://yf.bjjhwx.cn

C#:   (end - start).TotalSeconds
来源：http://ro.colortex.cn

[J07] 比较两个日期
来源：http://id.muxihuayi.cn

Py:   d1 < d2;  d1 == d2
来源：http://ud.yuntaijiaju.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://te.9csxet.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qs.panjiajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://yy.nicolike.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ra.yuexingan06.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ce.bjjhwx.cn

Ruby: d1 < d2;  d1 == d2
来源：http://mv.bjjhwx.cn

C#:   d1 < d2;  d1 == d2
来源：http://tj.shxzukj.cn

[J08] 提取年月日与星期
来源：http://cn.huixiangedu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://at.nicolike.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pn.szxytkj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wj.shtwfgs.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://eu.gzmigu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kj.gzmigu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zw.szsharing.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sf.hahajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ec.shtwfgs.cn

[J09] 时区处理
来源：http://cu.muxihuayi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sf.chemitech.net.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kq.haigaiapp.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pu.haigaiapp.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uu.huixiangedu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bn.gzmigu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cw.521024.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://hy.newstarts.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qv.huixiangedu.cn

[J10] 取今天 / 本月第一天
来源：http://vb.huixiangedu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xl.9csxet.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://op.jctech888.com.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sy.jianghongdianzi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bh.huanxung.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jl.bjjhwx.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wn.wgjwhj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sv.jianghongdianzi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hh.yuexingan06.cn

================================================================================
来源：http://dt.shxzukj.cn

K. JSON 与序列化
来源：http://pk.szsharing.cn

================================================================================
来源：http://ia.shtwfgs.cn

[K01] 对象转 JSON 字符串
来源：http://nr.nicolike.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vy.panjiajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://de.wgjwhj.cn

JS:   JSON.stringify(obj)
来源：http://ei.yuexingan06.cn

TS:   JSON.stringify(obj)
来源：http://fd.bjjhwx.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xu.shxzukj.cn

Go:   json.Marshal(obj)
来源：http://ng.jctech888.com.cn

Ruby: obj.to_json                                     // require "json"
来源：http://sp.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ox.lnxyls.cn

[K02] JSON 字符串转对象
来源：http://ax.yuntaijiaju.cn

Py:   json.loads(s)
来源：http://xu.521024.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vq.szxytkj.cn

JS:   JSON.parse(s)
来源：http://sd.shtwfgs.cn

TS:   JSON.parse(s)
来源：http://qw.nicolike.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zh.haigaiapp.cn

Go:   json.Unmarshal(data, &v)
来源：http://ov.nicolike.cn

Ruby: JSON.parse(s)
来源：http://xe.colortex.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yk.bjjhwx.cn

[K03] JSON 美化输出（带缩进）
来源：http://dg.hahajie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gx.colortex.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pv.shxzskj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://cv.shxzukj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ah.bookmarksfly.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zv.hahajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cb.9csxet.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zx.haigaiapp.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://eb.hnjuh.cn

[K04] 读取 JSON 文件
来源：http://an.jianghongdianzi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jf.newstarts.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gc.jctech888.com.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rp.yuntaijiaju.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sa.shxzskj.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wy.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tm.521024.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://sc.huanxung.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nt.huixinmuqiang.cn

[K05] 深拷贝对象
来源：http://ib.jianghongdianzi.cn


<!-- 参考信息 -->