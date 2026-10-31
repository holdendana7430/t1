代发 wailian999

H. 异常与错误处理
来源：http://ux.hahajie.cn

================================================================================
来源：http://yn.colortex.cn

[H01] try / catch 基础
来源：http://bz.newstarts.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lu.jctech888.com.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://do.huixiangedu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jo.szxytkj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://my.colortex.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wy.chemitech.net.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jy.shxzskj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cw.jianghongdianzi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ze.haigaiapp.cn

[H02] finally / ensure 收尾
来源：http://hk.bookmarksfly.cn

Py:   try: f()⏎finally: cleanup()
来源：http://rb.bjjhwx.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://dz.yuntaijiaju.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://lv.jctech888.com.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qv.521024.cn

Java: try { f(); } finally { cleanup(); }
来源：http://mb.jctech888.com.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://km.9csxet.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://fk.gzmigu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://mp.huixiangedu.cn

[H03] 主动抛出异常
来源：http://qn.shxzskj.cn

Py:   raise ValueError("错误信息")
来源：http://fs.huixiangedu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gf.muxihuayi.cn

JS:   throw new Error("错误信息");
来源：http://mv.yuexingan06.cn

TS:   throw new Error("错误信息");
来源：http://cm.bookmarksfly.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ua.hnjuh.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fd.wgjwhj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://dr.yuntaijiaju.cn

C#:   throw new ArgumentException("错误信息");
来源：http://vk.wgjwhj.cn

[H04] 自定义异常类型
来源：http://eq.asd995.cn

Py:   class MyError(Exception): pass
来源：http://sv.haigaiapp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://by.chemitech.net.cn

JS:   class MyError extends Error {}
来源：http://hf.bjjhwx.cn

TS:   class MyError extends Error {}
来源：http://zl.bjjhwx.cn

Java: class MyException extends RuntimeException {}
来源：http://xe.lnxyls.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zb.yuntaijiaju.cn

Ruby: class MyError < StandardError; end
来源：http://or.hnjuh.cn

C#:   class MyException : Exception {}
来源：http://bl.hnjuh.cn

[H05] 捕获特定类型
来源：http://ti.shxzskj.cn

Py:   except ValueError as e:
来源：http://vj.yuntaijiaju.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wa.haigaiapp.cn

JS:   if (e instanceof TypeError) {}
来源：http://jx.gzmigu.cn

TS:   if (e instanceof TypeError) {}
来源：http://cc.hnjuh.cn

Java: catch (IOException | SQLException e) {}
来源：http://rp.jianghongdianzi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://oy.nicolike.cn

Ruby: rescue ArgumentError => e
来源：http://ci.yuntaijiaju.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hi.haigaiapp.cn

[H06] 可选值 / 空值安全访问
来源：http://ck.yuntaijiaju.cn

Py:   value = d.get("k") or default
来源：http://xt.asd995.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ri.hnjuh.cn

JS:   obj?.a?.b;  d ?? default
来源：http://av.hahajie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://my.jianghongdianzi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://uy.521024.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://na.yuexingan06.cn

Ruby: d&.dig(:a, :b)
来源：http://fi.szxytkj.cn

C#:   obj?.A?.B ?? default
来源：http://rz.wgjwhj.cn

[H07] 断言
来源：http://ji.hnjuh.cn

Py:   assert x > 0, "必须为正"
来源：http://pl.jctech888.com.cn

PHP:  assert($x > 0);
来源：http://xb.bjjhwx.cn

JS:   console.assert(x > 0);
来源：http://da.huixinmuqiang.cn

TS:   console.assert(x > 0);
来源：http://zc.gzmigu.cn

Java: assert x > 0 : "必须为正";
来源：http://us.hahajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ue.muxihuayi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://sc.newstarts.cn

C#:   Debug.Assert(x > 0);
来源：http://me.haigaiapp.cn

[H08] 获取错误信息与堆栈
来源：http://uk.szxytkj.cn

Py:   str(e);  traceback.format_exc()
来源：http://js.jianghongdianzi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ka.lnxyls.cn

JS:   e.message;  e.stack
来源：http://tn.521024.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://fo.nszjky.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ff.shxzukj.cn

Go:   err.Error()
来源：http://et.szsharing.cn

Ruby: e.message;  e.backtrace
来源：http://ji.newstarts.cn

C#:   e.Message;  e.StackTrace
来源：http://by.huixinmuqiang.cn

[H09] 带错误码的异常
来源：http://wt.gzmigu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bo.huixinmuqiang.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://fe.szxytkj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pz.gzmigu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vf.muxihuayi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hl.chemitech.net.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kh.muxihuayi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://sr.jianghongdianzi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://or.szxytkj.cn

[H10] 资源自动释放
来源：http://ui.colortex.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://sp.yuexingan06.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sb.szxytkj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pd.wgjwhj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://px.muxihuayi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://od.huanxung.cn

Go:   defer f.Close()
来源：http://gg.asd995.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ot.muxihuayi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://np.shxzukj.cn

================================================================================
来源：http://bc.shtwfgs.cn

I. 正则表达式
来源：http://uo.szxytkj.cn

================================================================================
来源：http://dx.szsharing.cn

[I01] 判断是否匹配
来源：http://hd.bjjhwx.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dp.jctech888.com.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ig.shxzskj.cn

JS:   /\d+/.test(s)
来源：http://hx.muxihuayi.cn

TS:   /\d+/.test(s)
来源：http://hp.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ls.colortex.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wr.lnxyls.cn

Ruby: s.match?(/\d+/)
来源：http://gv.colortex.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gn.lnxyls.cn

[I02] 提取所有匹配
来源：http://tf.bookmarksfly.cn

Py:   re.findall(r"\d+", s)
来源：http://ca.jctech888.com.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mp.yuexingan06.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wz.jctech888.com.cn

TS:   s.match(/\d+/g)
来源：http://mk.huixiangedu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ak.jianghongdianzi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pq.panjiajie.cn

Ruby: s.scan(/\d+/)
来源：http://jh.nszjky.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lk.gzmigu.cn

[I03] 提取捕获分组
来源：http://cf.haigaiapp.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://km.yuntaijiaju.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gy.asd995.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://di.nszjky.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vu.jianghongdianzi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://of.huixiangedu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hi.huixiangedu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fx.nicolike.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ta.huixinmuqiang.cn

[I04] 正则替换
来源：http://gj.asd995.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xa.nicolike.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://of.521024.cn

JS:   s.replace(/\d+/g, "#")
来源：http://np.huixiangedu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mt.hnjuh.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ow.szsharing.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xo.shxzukj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://yz.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ae.yuexingan06.cn

[I05] 按正则拆分
来源：http://js.shxzukj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://va.colortex.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://md.hahajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://es.huixinmuqiang.cn

TS:   s.split(/\s*,\s*/)
来源：http://lo.newstarts.cn

Java: s.split("\\s*,\\s*")
来源：http://gh.colortex.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lz.newstarts.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ls.jianghongdianzi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://uy.shxzskj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hy.chemitech.net.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zd.9csxet.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ek.521024.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://aj.szxytkj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cc.yuntaijiaju.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qv.huanxung.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wn.asd995.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vp.shxzskj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mq.shtwfgs.cn

[I07] 忽略大小写与多行模式
来源：http://dh.huixinmuqiang.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yl.yuexingan06.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tk.hahajie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://uu.jctech888.com.cn

TS:   /error/gim
来源：http://xo.shxzukj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://da.szsharing.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wa.yuntaijiaju.cn

Ruby: s.scan(/error/i)
来源：http://an.bjjhwx.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wo.hnjuh.cn

[I08] 贪婪与非贪婪匹配
来源：http://sg.shtwfgs.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pt.huanxung.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ne.huixiangedu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ym.panjiajie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ra.haigaiapp.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://qa.szsharing.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mr.hahajie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tn.yuntaijiaju.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lm.shxzukj.cn

================================================================================
来源：http://vq.asd995.cn

J. 日期与时间
来源：http://nf.bookmarksfly.cn

================================================================================
来源：http://qc.wgjwhj.cn

[J01] 获取当前时间
来源：http://pd.yuntaijiaju.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ra.huixiangedu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jh.521024.cn

JS:   new Date();  Date.now()
来源：http://ex.panjiajie.cn

TS:   new Date();  Date.now()
来源：http://qz.huixiangedu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://nw.wgjwhj.cn

Go:   time.Now()
来源：http://ya.hahajie.cn

Ruby: Time.now
来源：http://ph.jianghongdianzi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ar.jianghongdianzi.cn

[J02] 格式化输出
来源：http://nf.newstarts.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uy.hnjuh.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dt.huanxung.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mz.haigaiapp.cn

TS:   d.toISOString()
来源：http://hz.huanxung.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fe.gzmigu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ek.wgjwhj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jh.haigaiapp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kw.chemitech.net.cn

[J03] 字符串解析为日期
来源：http://ge.panjiajie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vl.muxihuayi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bu.huixinmuqiang.cn

JS:   new Date("2024-01-02")
来源：http://mm.bjjhwx.cn

TS:   new Date("2024-01-02")
来源：http://bt.nicolike.cn

Java: LocalDate.parse("2024-01-02")
来源：http://om.huixinmuqiang.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bi.yuntaijiaju.cn

Ruby: Date.parse("2024-01-02")
来源：http://tp.hnjuh.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yk.hnjuh.cn

[J04] 时间戳与日期互转
来源：http://gj.panjiajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lw.hnjuh.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dw.bookmarksfly.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ct.muxihuayi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://wx.lnxyls.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://au.wgjwhj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://av.wgjwhj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://co.colortex.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pc.shxzskj.cn

[J05] 时间加减（加 7 天）
来源：http://pe.muxihuayi.cn

Py:   now + timedelta(days=7)
来源：http://hm.szxytkj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ju.panjiajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://uh.haigaiapp.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uh.newstarts.cn

Java: LocalDate.now().plusDays(7)
来源：http://vq.colortex.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dx.521024.cn

Ruby: Time.now + 7 * 86400
来源：http://ji.bookmarksfly.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jd.szsharing.cn

[J06] 计算两时间之差
来源：http://xs.huixiangedu.cn

Py:   (end - start).total_seconds()
来源：http://lb.shxzskj.cn

PHP:  $end->diff($start)->days;
来源：http://ef.shtwfgs.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rt.newstarts.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fl.lnxyls.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ip.jctech888.com.cn

Go:   end.Sub(start).Hours()
来源：http://qg.panjiajie.cn

Ruby: end - start                 # 返回秒数
来源：http://bz.bjjhwx.cn

C#:   (end - start).TotalSeconds
来源：http://qy.colortex.cn

[J07] 比较两个日期
来源：http://jt.nszjky.cn

Py:   d1 < d2;  d1 == d2
来源：http://mk.jianghongdianzi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kc.muxihuayi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qd.jctech888.com.cn

TS:   d1.getTime() < d2.getTime()
来源：http://vp.szsharing.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mw.muxihuayi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hw.lnxyls.cn

Ruby: d1 < d2;  d1 == d2
来源：http://hk.wgjwhj.cn

C#:   d1 < d2;  d1 == d2
来源：http://if.hahajie.cn

[J08] 提取年月日与星期
来源：http://xz.haigaiapp.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://or.gzmigu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rc.lnxyls.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vi.lnxyls.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://aj.muxihuayi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ta.yuntaijiaju.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://es.shxzukj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ta.huixinmuqiang.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jq.521024.cn

[J09] 时区处理
来源：http://ye.jctech888.com.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ee.yuexingan06.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mh.shxzskj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ls.huixiangedu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qn.colortex.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ct.bookmarksfly.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hd.lnxyls.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://na.lnxyls.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ok.yuexingan06.cn

[J10] 取今天 / 本月第一天
来源：http://zv.huixinmuqiang.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://rk.shxzskj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ea.shxzskj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vv.shxzukj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://iv.shxzskj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ay.yuexingan06.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sl.nicolike.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lc.9csxet.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cs.muxihuayi.cn

================================================================================
来源：http://un.colortex.cn

K. JSON 与序列化
来源：http://ni.shxzukj.cn

================================================================================
来源：http://zu.haigaiapp.cn

[K01] 对象转 JSON 字符串
来源：http://rq.wgjwhj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kh.shtwfgs.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pp.yuntaijiaju.cn

JS:   JSON.stringify(obj)
来源：http://sv.wgjwhj.cn

TS:   JSON.stringify(obj)
来源：http://gh.hnjuh.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nz.gzmigu.cn

Go:   json.Marshal(obj)
来源：http://fx.hahajie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qw.huixiangedu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://uw.hahajie.cn

[K02] JSON 字符串转对象
来源：http://um.huixiangedu.cn

Py:   json.loads(s)
来源：http://te.hnjuh.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xw.bjjhwx.cn

JS:   JSON.parse(s)
来源：http://ao.521024.cn

TS:   JSON.parse(s)
来源：http://ga.yuntaijiaju.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kv.lnxyls.cn

Go:   json.Unmarshal(data, &v)
来源：http://kh.chemitech.net.cn

Ruby: JSON.parse(s)
来源：http://rw.huixinmuqiang.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fj.shxzukj.cn

[K03] JSON 美化输出（带缩进）
来源：http://hf.bjjhwx.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fy.wgjwhj.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jc.lnxyls.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fd.colortex.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://cc.nicolike.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ub.huanxung.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://oz.huanxung.cn

Ruby: JSON.pretty_generate(obj)
来源：http://hi.jianghongdianzi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ey.huanxung.cn

[K04] 读取 JSON 文件
来源：http://hq.newstarts.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uk.521024.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xx.asd995.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hj.hnjuh.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dg.gzmigu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tz.wgjwhj.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fi.yuntaijiaju.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wl.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rn.szsharing.cn

[K05] 深拷贝对象
来源：http://rc.huixiangedu.cn


<!-- 参考信息 -->