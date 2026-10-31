代发 wailian999

PHP:  get_object_vars($obj);
来源：http://ty.muxihuayi.cn

JS:   Object.entries(obj)
来源：http://zy.hahajie.cn

TS:   Object.entries(obj)
来源：http://lp.yuexingan06.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ap.huanxung.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://eo.szsharing.cn

Ruby: obj.instance_variables
来源：http://be.521024.cn

C#:   // 用反射或 System.Text.Json
来源：http://pq.shtwfgs.cn

================================================================================
来源：http://kn.shxzukj.cn

H. 异常与错误处理
来源：http://if.gzmigu.cn

================================================================================
来源：http://xu.colortex.cn

[H01] try / catch 基础
来源：http://xo.huixinmuqiang.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fu.521024.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tu.shxzukj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pi.jianghongdianzi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bp.colortex.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pa.yuexingan06.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://bp.nicolike.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wu.asd995.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pj.shxzukj.cn

[H02] finally / ensure 收尾
来源：http://xp.521024.cn

Py:   try: f()⏎finally: cleanup()
来源：http://dv.asd995.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://zv.haigaiapp.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ce.hnjuh.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ts.yuntaijiaju.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ow.yuexingan06.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zt.hnjuh.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ab.521024.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://zc.bookmarksfly.cn

[H03] 主动抛出异常
来源：http://xy.hahajie.cn

Py:   raise ValueError("错误信息")
来源：http://ad.huanxung.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xw.521024.cn

JS:   throw new Error("错误信息");
来源：http://tx.jctech888.com.cn

TS:   throw new Error("错误信息");
来源：http://ke.yuexingan06.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ep.yuexingan06.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sa.huixiangedu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://zt.shxzskj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://jo.jianghongdianzi.cn

[H04] 自定义异常类型
来源：http://oq.9csxet.cn

Py:   class MyError(Exception): pass
来源：http://bw.szxytkj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://jg.bookmarksfly.cn

JS:   class MyError extends Error {}
来源：http://bv.lnxyls.cn

TS:   class MyError extends Error {}
来源：http://du.jianghongdianzi.cn

Java: class MyException extends RuntimeException {}
来源：http://yc.colortex.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vv.9csxet.cn

Ruby: class MyError < StandardError; end
来源：http://oh.shxzukj.cn

C#:   class MyException : Exception {}
来源：http://vt.newstarts.cn

[H05] 捕获特定类型
来源：http://fr.shtwfgs.cn

Py:   except ValueError as e:
来源：http://un.szsharing.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pt.521024.cn

JS:   if (e instanceof TypeError) {}
来源：http://gg.chemitech.net.cn

TS:   if (e instanceof TypeError) {}
来源：http://pp.muxihuayi.cn

Java: catch (IOException | SQLException e) {}
来源：http://kr.panjiajie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ze.szxytkj.cn

Ruby: rescue ArgumentError => e
来源：http://gx.nszjky.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ym.wgjwhj.cn

[H06] 可选值 / 空值安全访问
来源：http://sz.muxihuayi.cn

Py:   value = d.get("k") or default
来源：http://dy.shtwfgs.cn

PHP:  $v = $d["k"] ?? null;
来源：http://fb.yuexingan06.cn

JS:   obj?.a?.b;  d ?? default
来源：http://kt.yuntaijiaju.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ve.haigaiapp.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wv.haigaiapp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://iw.lnxyls.cn

Ruby: d&.dig(:a, :b)
来源：http://zy.hnjuh.cn

C#:   obj?.A?.B ?? default
来源：http://rd.wgjwhj.cn

[H07] 断言
来源：http://ce.hnjuh.cn

Py:   assert x > 0, "必须为正"
来源：http://sy.huixinmuqiang.cn

PHP:  assert($x > 0);
来源：http://je.newstarts.cn

JS:   console.assert(x > 0);
来源：http://us.huixinmuqiang.cn

TS:   console.assert(x > 0);
来源：http://nm.yuntaijiaju.cn

Java: assert x > 0 : "必须为正";
来源：http://lb.huixiangedu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yc.panjiajie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xl.nszjky.cn

C#:   Debug.Assert(x > 0);
来源：http://fs.nicolike.cn

[H08] 获取错误信息与堆栈
来源：http://fd.jianghongdianzi.cn

Py:   str(e);  traceback.format_exc()
来源：http://ni.szxytkj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ku.huixiangedu.cn

JS:   e.message;  e.stack
来源：http://iv.bjjhwx.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ot.yuntaijiaju.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://mw.jianghongdianzi.cn

Go:   err.Error()
来源：http://rb.shxzukj.cn

Ruby: e.message;  e.backtrace
来源：http://dt.hnjuh.cn

C#:   e.Message;  e.StackTrace
来源：http://lo.haigaiapp.cn

[H09] 带错误码的异常
来源：http://gk.asd995.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ce.yuntaijiaju.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://zx.haigaiapp.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ox.bjjhwx.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ac.huixinmuqiang.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://in.shxzukj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://un.haigaiapp.cn

Ruby: raise MyError.new("fail", 500)
来源：http://fw.huixiangedu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://da.huanxung.cn

[H10] 资源自动释放
来源：http://qx.yuexingan06.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zl.yuexingan06.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kh.colortex.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://we.lnxyls.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nw.hahajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://yd.panjiajie.cn

Go:   defer f.Close()
来源：http://yw.haigaiapp.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hu.haigaiapp.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tn.jctech888.com.cn

================================================================================
来源：http://bi.shxzukj.cn

I. 正则表达式
来源：http://ta.wgjwhj.cn

================================================================================
来源：http://kq.521024.cn

[I01] 判断是否匹配
来源：http://iz.panjiajie.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ih.shtwfgs.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xl.shxzukj.cn

JS:   /\d+/.test(s)
来源：http://zv.jctech888.com.cn

TS:   /\d+/.test(s)
来源：http://id.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jo.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qv.newstarts.cn

Ruby: s.match?(/\d+/)
来源：http://pf.shtwfgs.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nv.yuntaijiaju.cn

[I02] 提取所有匹配
来源：http://eu.shtwfgs.cn

Py:   re.findall(r"\d+", s)
来源：http://gq.haigaiapp.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://oi.yuntaijiaju.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zd.shxzukj.cn

TS:   s.match(/\d+/g)
来源：http://zc.nszjky.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ai.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://im.szxytkj.cn

Ruby: s.scan(/\d+/)
来源：http://rp.jianghongdianzi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://db.huanxung.cn

[I03] 提取捕获分组
来源：http://vz.jctech888.com.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zv.gzmigu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nl.9csxet.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wt.gzmigu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zq.huixinmuqiang.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dp.newstarts.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ig.shxzukj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://uw.hnjuh.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://al.yuexingan06.cn

[I04] 正则替换
来源：http://hh.shtwfgs.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ge.jctech888.com.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gi.newstarts.cn

JS:   s.replace(/\d+/g, "#")
来源：http://fo.panjiajie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ou.lnxyls.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rh.colortex.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ic.newstarts.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ed.bookmarksfly.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://es.shtwfgs.cn

[I05] 按正则拆分
来源：http://mh.jctech888.com.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ik.gzmigu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rq.yuexingan06.cn

JS:   s.split(/\s*,\s*/)
来源：http://qo.shxzskj.cn

TS:   s.split(/\s*,\s*/)
来源：http://it.nszjky.cn

Java: s.split("\\s*,\\s*")
来源：http://wt.muxihuayi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vq.nicolike.cn

Ruby: s.split(/\s*,\s*/)
来源：http://pw.huixinmuqiang.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jx.lnxyls.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kr.jianghongdianzi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tv.9csxet.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pg.hnjuh.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nt.yuexingan06.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xi.haigaiapp.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fr.shxzukj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jp.chemitech.net.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ji.szxytkj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cu.hnjuh.cn

[I07] 忽略大小写与多行模式
来源：http://zb.colortex.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hm.gzmigu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uj.yuexingan06.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://uh.521024.cn

TS:   /error/gim
来源：http://er.huixiangedu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jk.yuexingan06.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xw.bookmarksfly.cn

Ruby: s.scan(/error/i)
来源：http://vr.hahajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rq.shtwfgs.cn

[I08] 贪婪与非贪婪匹配
来源：http://rx.hahajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://iq.yuexingan06.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lo.haigaiapp.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://le.shxzukj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rl.shxzskj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xf.shxzskj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sg.jctech888.com.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://er.bjjhwx.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mx.muxihuayi.cn

================================================================================
来源：http://pt.colortex.cn

J. 日期与时间
来源：http://ly.shtwfgs.cn

================================================================================
来源：http://bk.9csxet.cn

[J01] 获取当前时间
来源：http://pa.521024.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zi.huixiangedu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ia.bjjhwx.cn

JS:   new Date();  Date.now()
来源：http://lh.yuntaijiaju.cn

TS:   new Date();  Date.now()
来源：http://ig.huanxung.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://hc.jianghongdianzi.cn

Go:   time.Now()
来源：http://em.shxzskj.cn

Ruby: Time.now
来源：http://do.hahajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zs.colortex.cn

[J02] 格式化输出
来源：http://ke.chemitech.net.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vx.shtwfgs.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://je.jctech888.com.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ub.yuexingan06.cn

TS:   d.toISOString()
来源：http://qa.yuexingan06.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ui.szxytkj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xw.nicolike.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://si.huanxung.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ew.huixinmuqiang.cn

[J03] 字符串解析为日期
来源：http://gz.gzmigu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lu.hahajie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hh.nszjky.cn

JS:   new Date("2024-01-02")
来源：http://xf.newstarts.cn

TS:   new Date("2024-01-02")
来源：http://rd.huixiangedu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://sj.hnjuh.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pg.gzmigu.cn

Ruby: Date.parse("2024-01-02")
来源：http://di.shxzukj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ap.haigaiapp.cn

[J04] 时间戳与日期互转
来源：http://gw.huixiangedu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nu.hnjuh.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qj.wgjwhj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://me.nicolike.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://oh.szxytkj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kj.huixiangedu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://co.yuexingan06.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ub.muxihuayi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cy.shxzukj.cn

[J05] 时间加减（加 7 天）
来源：http://to.shtwfgs.cn

Py:   now + timedelta(days=7)
来源：http://eh.huixiangedu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://zd.huanxung.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://io.lnxyls.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gb.wgjwhj.cn

Java: LocalDate.now().plusDays(7)
来源：http://vy.jianghongdianzi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gz.muxihuayi.cn

Ruby: Time.now + 7 * 86400
来源：http://tl.yuntaijiaju.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ra.shtwfgs.cn

[J06] 计算两时间之差
来源：http://ue.jctech888.com.cn

Py:   (end - start).total_seconds()
来源：http://nj.9csxet.cn

PHP:  $end->diff($start)->days;
来源：http://rs.yuexingan06.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dd.shtwfgs.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cf.asd995.cn

Java: Duration.between(start, end).toSeconds()
来源：http://dv.muxihuayi.cn

Go:   end.Sub(start).Hours()
来源：http://fb.huixiangedu.cn

Ruby: end - start                 # 返回秒数
来源：http://ro.gzmigu.cn

C#:   (end - start).TotalSeconds
来源：http://xu.shtwfgs.cn

[J07] 比较两个日期
来源：http://pt.hahajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://ev.nszjky.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://et.jctech888.com.cn

JS:   d1.getTime() < d2.getTime()
来源：http://io.jianghongdianzi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ql.bookmarksfly.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://li.jctech888.com.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://oc.muxihuayi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ql.huanxung.cn

C#:   d1 < d2;  d1 == d2
来源：http://sf.shxzukj.cn

[J08] 提取年月日与星期
来源：http://ez.shtwfgs.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://og.wgjwhj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yb.szsharing.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://eo.huixiangedu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fo.szsharing.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fy.521024.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ti.jianghongdianzi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fm.szxytkj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://we.nszjky.cn

[J09] 时区处理
来源：http://sc.bookmarksfly.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mr.bookmarksfly.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xj.huixiangedu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gn.hnjuh.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nl.gzmigu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wf.yuntaijiaju.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ii.szxytkj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://zh.yuexingan06.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yy.wgjwhj.cn

[J10] 取今天 / 本月第一天
来源：http://kw.yuexingan06.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ow.hahajie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mn.yuntaijiaju.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mq.bookmarksfly.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hk.shtwfgs.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wp.huixiangedu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rj.szsharing.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xe.9csxet.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ce.nicolike.cn

================================================================================
来源：http://ps.wgjwhj.cn

K. JSON 与序列化
来源：http://sc.szxytkj.cn

================================================================================
来源：http://do.jianghongdianzi.cn

[K01] 对象转 JSON 字符串
来源：http://nf.asd995.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://et.wgjwhj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://et.jianghongdianzi.cn

JS:   JSON.stringify(obj)
来源：http://co.muxihuayi.cn

TS:   JSON.stringify(obj)
来源：http://xm.newstarts.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nf.chemitech.net.cn

Go:   json.Marshal(obj)
来源：http://jj.wgjwhj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ug.shxzskj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vn.muxihuayi.cn

[K02] JSON 字符串转对象
来源：http://ei.muxihuayi.cn

Py:   json.loads(s)
来源：http://pd.shtwfgs.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://st.lnxyls.cn

JS:   JSON.parse(s)
来源：http://qq.huixinmuqiang.cn

TS:   JSON.parse(s)
来源：http://cq.jianghongdianzi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ge.shxzukj.cn

Go:   json.Unmarshal(data, &v)
来源：http://xp.huanxung.cn

Ruby: JSON.parse(s)
来源：http://hj.hnjuh.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ee.wgjwhj.cn

[K03] JSON 美化输出（带缩进）
来源：http://yi.bjjhwx.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dv.chemitech.net.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bl.huixiangedu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ig.huixinmuqiang.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ei.9csxet.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jv.haigaiapp.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xe.gzmigu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://as.lnxyls.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pe.nicolike.cn

[K04] 读取 JSON 文件
来源：http://eb.jianghongdianzi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tt.shxzukj.cn


<!-- 参考信息 -->