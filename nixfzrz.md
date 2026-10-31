代发 wailian999

PHP:  get_object_vars($obj);
来源：http://hy.bjjhwx.cn

JS:   Object.entries(obj)
来源：http://fu.nszjky.cn

TS:   Object.entries(obj)
来源：http://zv.yuexingan06.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ga.yuexingan06.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://vm.gzmigu.cn

Ruby: obj.instance_variables
来源：http://ht.shtwfgs.cn

C#:   // 用反射或 System.Text.Json
来源：http://fz.9csxet.cn

================================================================================
来源：http://lj.szsharing.cn

H. 异常与错误处理
来源：http://yc.yuntaijiaju.cn

================================================================================
来源：http://sr.szsharing.cn

[H01] try / catch 基础
来源：http://ul.hnjuh.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ev.huixiangedu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xm.szsharing.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://uk.bjjhwx.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kq.9csxet.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qr.lnxyls.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fq.shxzskj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rd.newstarts.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qs.muxihuayi.cn

[H02] finally / ensure 收尾
来源：http://md.shtwfgs.cn

Py:   try: f()⏎finally: cleanup()
来源：http://eb.panjiajie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://el.jianghongdianzi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://eb.shxzskj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://kt.newstarts.cn

Java: try { f(); } finally { cleanup(); }
来源：http://fr.szxytkj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://pg.newstarts.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://yw.haigaiapp.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://cq.jianghongdianzi.cn

[H03] 主动抛出异常
来源：http://wn.shtwfgs.cn

Py:   raise ValueError("错误信息")
来源：http://gy.bjjhwx.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://za.jianghongdianzi.cn

JS:   throw new Error("错误信息");
来源：http://qk.lnxyls.cn

TS:   throw new Error("错误信息");
来源：http://wf.lnxyls.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://cc.521024.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bg.nszjky.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ci.huanxung.cn

C#:   throw new ArgumentException("错误信息");
来源：http://je.hnjuh.cn

[H04] 自定义异常类型
来源：http://uy.huixinmuqiang.cn

Py:   class MyError(Exception): pass
来源：http://pz.huanxung.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ay.shxzskj.cn

JS:   class MyError extends Error {}
来源：http://kp.shxzskj.cn

TS:   class MyError extends Error {}
来源：http://fc.lnxyls.cn

Java: class MyException extends RuntimeException {}
来源：http://aq.9csxet.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rl.nszjky.cn

Ruby: class MyError < StandardError; end
来源：http://up.hahajie.cn

C#:   class MyException : Exception {}
来源：http://jq.shtwfgs.cn

[H05] 捕获特定类型
来源：http://ts.szsharing.cn

Py:   except ValueError as e:
来源：http://ks.yuexingan06.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qh.bjjhwx.cn

JS:   if (e instanceof TypeError) {}
来源：http://et.huixinmuqiang.cn

TS:   if (e instanceof TypeError) {}
来源：http://su.wgjwhj.cn

Java: catch (IOException | SQLException e) {}
来源：http://ad.asd995.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ng.muxihuayi.cn

Ruby: rescue ArgumentError => e
来源：http://wv.nszjky.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bu.wgjwhj.cn

[H06] 可选值 / 空值安全访问
来源：http://pa.hnjuh.cn

Py:   value = d.get("k") or default
来源：http://ut.bookmarksfly.cn

PHP:  $v = $d["k"] ?? null;
来源：http://vb.bjjhwx.cn

JS:   obj?.a?.b;  d ?? default
来源：http://pq.hnjuh.cn

TS:   obj?.a?.b;  d ?? default
来源：http://kr.szsharing.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ri.bookmarksfly.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ql.wgjwhj.cn

Ruby: d&.dig(:a, :b)
来源：http://vu.chemitech.net.cn

C#:   obj?.A?.B ?? default
来源：http://po.bookmarksfly.cn

[H07] 断言
来源：http://fq.haigaiapp.cn

Py:   assert x > 0, "必须为正"
来源：http://vj.bookmarksfly.cn

PHP:  assert($x > 0);
来源：http://eu.bookmarksfly.cn

JS:   console.assert(x > 0);
来源：http://wu.chemitech.net.cn

TS:   console.assert(x > 0);
来源：http://hj.shxzskj.cn

Java: assert x > 0 : "必须为正";
来源：http://eg.lnxyls.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mw.asd995.cn

Ruby: raise "必须为正" unless x > 0
来源：http://gw.yuexingan06.cn

C#:   Debug.Assert(x > 0);
来源：http://ef.asd995.cn

[H08] 获取错误信息与堆栈
来源：http://mj.gzmigu.cn

Py:   str(e);  traceback.format_exc()
来源：http://zk.bookmarksfly.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kg.shtwfgs.cn

JS:   e.message;  e.stack
来源：http://wf.hahajie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://dp.colortex.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://xf.jctech888.com.cn

Go:   err.Error()
来源：http://ym.jctech888.com.cn

Ruby: e.message;  e.backtrace
来源：http://lu.gzmigu.cn

C#:   e.Message;  e.StackTrace
来源：http://gd.panjiajie.cn

[H09] 带错误码的异常
来源：http://lk.szsharing.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ur.wgjwhj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://wt.shtwfgs.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ll.huixiangedu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xu.muxihuayi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zb.jctech888.com.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hr.jctech888.com.cn

Ruby: raise MyError.new("fail", 500)
来源：http://gy.lnxyls.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://fc.bookmarksfly.cn

[H10] 资源自动释放
来源：http://kf.huanxung.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://hh.gzmigu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sk.shxzskj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bb.jctech888.com.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zz.bjjhwx.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xn.shtwfgs.cn

Go:   defer f.Close()
来源：http://co.lnxyls.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cv.yuntaijiaju.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sb.panjiajie.cn

================================================================================
来源：http://sq.yuntaijiaju.cn

I. 正则表达式
来源：http://mj.gzmigu.cn

================================================================================
来源：http://yp.shxzskj.cn

[I01] 判断是否匹配
来源：http://yt.shtwfgs.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yc.newstarts.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wy.asd995.cn

JS:   /\d+/.test(s)
来源：http://xb.szxytkj.cn

TS:   /\d+/.test(s)
来源：http://ss.hahajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bw.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mi.hnjuh.cn

Ruby: s.match?(/\d+/)
来源：http://fn.chemitech.net.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://en.gzmigu.cn

[I02] 提取所有匹配
来源：http://ia.chemitech.net.cn

Py:   re.findall(r"\d+", s)
来源：http://hs.jctech888.com.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bg.newstarts.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ig.9csxet.cn

TS:   s.match(/\d+/g)
来源：http://ki.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://df.szxytkj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://af.lnxyls.cn

Ruby: s.scan(/\d+/)
来源：http://fz.hahajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://br.huixinmuqiang.cn

[I03] 提取捕获分组
来源：http://bw.bjjhwx.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ev.szsharing.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gz.nszjky.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pf.nicolike.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sp.gzmigu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jh.gzmigu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ot.521024.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zn.colortex.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tp.newstarts.cn

[I04] 正则替换
来源：http://gy.bookmarksfly.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ga.yuntaijiaju.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dq.jctech888.com.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ap.haigaiapp.cn

TS:   s.replace(/\d+/g, "#")
来源：http://dp.521024.cn

Java: s.replaceAll("\\d+", "#")
来源：http://du.szsharing.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://gu.haigaiapp.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://nr.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jk.colortex.cn

[I05] 按正则拆分
来源：http://hc.nicolike.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://kw.lnxyls.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ho.huanxung.cn

JS:   s.split(/\s*,\s*/)
来源：http://rd.wgjwhj.cn

TS:   s.split(/\s*,\s*/)
来源：http://oc.huixiangedu.cn

Java: s.split("\\s*,\\s*")
来源：http://kk.yuexingan06.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ds.szxytkj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bb.wgjwhj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wa.521024.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://co.hnjuh.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bs.haigaiapp.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rj.nicolike.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://os.jianghongdianzi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ib.gzmigu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lf.panjiajie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://db.muxihuayi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cg.9csxet.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tu.hahajie.cn

[I07] 忽略大小写与多行模式
来源：http://nd.hnjuh.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://li.shxzskj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gb.nicolike.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ka.wgjwhj.cn

TS:   /error/gim
来源：http://na.lnxyls.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xi.lnxyls.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pn.521024.cn

Ruby: s.scan(/error/i)
来源：http://va.asd995.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://db.asd995.cn

[I08] 贪婪与非贪婪匹配
来源：http://xt.hahajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xg.huanxung.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fa.lnxyls.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dc.shxzskj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ev.9csxet.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://fw.shxzukj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://he.nicolike.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ld.lnxyls.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bf.shxzukj.cn

================================================================================
来源：http://tp.9csxet.cn

J. 日期与时间
来源：http://rf.shtwfgs.cn

================================================================================
来源：http://cp.huixinmuqiang.cn

[J01] 获取当前时间
来源：http://sq.newstarts.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ao.jianghongdianzi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qa.panjiajie.cn

JS:   new Date();  Date.now()
来源：http://bt.nicolike.cn

TS:   new Date();  Date.now()
来源：http://lp.chemitech.net.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://xf.colortex.cn

Go:   time.Now()
来源：http://dz.nicolike.cn

Ruby: Time.now
来源：http://ch.shxzskj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qb.bjjhwx.cn

[J02] 格式化输出
来源：http://te.nszjky.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pc.yuntaijiaju.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://oc.colortex.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kl.haigaiapp.cn

TS:   d.toISOString()
来源：http://wh.9csxet.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ru.jianghongdianzi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://at.asd995.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lq.panjiajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kj.huixiangedu.cn

[J03] 字符串解析为日期
来源：http://gy.gzmigu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wa.panjiajie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://iw.bjjhwx.cn

JS:   new Date("2024-01-02")
来源：http://rk.yuntaijiaju.cn

TS:   new Date("2024-01-02")
来源：http://ga.muxihuayi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mc.chemitech.net.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kc.chemitech.net.cn

Ruby: Date.parse("2024-01-02")
来源：http://ms.yuntaijiaju.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qf.jctech888.com.cn

[J04] 时间戳与日期互转
来源：http://od.shtwfgs.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qg.nszjky.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://az.muxihuayi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://oc.panjiajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://pv.bookmarksfly.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vx.newstarts.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dn.haigaiapp.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gg.9csxet.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://az.bjjhwx.cn

[J05] 时间加减（加 7 天）
来源：http://fd.panjiajie.cn

Py:   now + timedelta(days=7)
来源：http://ex.huixinmuqiang.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vv.huanxung.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yp.panjiajie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xx.panjiajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://tc.huixiangedu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ys.gzmigu.cn

Ruby: Time.now + 7 * 86400
来源：http://hl.shxzukj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://en.huixinmuqiang.cn

[J06] 计算两时间之差
来源：http://xi.shtwfgs.cn

Py:   (end - start).total_seconds()
来源：http://to.huanxung.cn

PHP:  $end->diff($start)->days;
来源：http://nh.yuexingan06.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fc.newstarts.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wa.nszjky.cn

Java: Duration.between(start, end).toSeconds()
来源：http://fn.shxzukj.cn

Go:   end.Sub(start).Hours()
来源：http://wa.hahajie.cn

Ruby: end - start                 # 返回秒数
来源：http://ru.bookmarksfly.cn

C#:   (end - start).TotalSeconds
来源：http://we.bookmarksfly.cn

[J07] 比较两个日期
来源：http://su.jctech888.com.cn

Py:   d1 < d2;  d1 == d2
来源：http://ou.newstarts.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ed.asd995.cn

JS:   d1.getTime() < d2.getTime()
来源：http://lt.jctech888.com.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xv.lnxyls.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dd.yuntaijiaju.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nm.hnjuh.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bv.yuexingan06.cn

C#:   d1 < d2;  d1 == d2
来源：http://nk.9csxet.cn

[J08] 提取年月日与星期
来源：http://pp.szsharing.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xw.nicolike.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rw.muxihuayi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qg.jctech888.com.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://iw.hnjuh.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ph.newstarts.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ki.jianghongdianzi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nt.gzmigu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ze.colortex.cn

[J09] 时区处理
来源：http://pk.shxzskj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ly.yuexingan06.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://oy.shxzukj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://in.asd995.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gv.panjiajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jm.muxihuayi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ks.colortex.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://tf.bookmarksfly.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://es.asd995.cn

[J10] 取今天 / 本月第一天
来源：http://ys.yuntaijiaju.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ko.huixinmuqiang.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://iq.panjiajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://el.huixiangedu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://da.jctech888.com.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vz.yuexingan06.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wx.9csxet.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://za.haigaiapp.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://av.nicolike.cn

================================================================================
来源：http://eg.haigaiapp.cn

K. JSON 与序列化
来源：http://id.yuexingan06.cn

================================================================================
来源：http://ys.szxytkj.cn

[K01] 对象转 JSON 字符串
来源：http://xy.gzmigu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qc.shxzukj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pm.colortex.cn

JS:   JSON.stringify(obj)
来源：http://ig.jctech888.com.cn

TS:   JSON.stringify(obj)
来源：http://lw.chemitech.net.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fr.lnxyls.cn

Go:   json.Marshal(obj)
来源：http://tk.jctech888.com.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ig.9csxet.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://du.shxzskj.cn

[K02] JSON 字符串转对象
来源：http://gv.panjiajie.cn

Py:   json.loads(s)
来源：http://pn.yuntaijiaju.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nf.nszjky.cn

JS:   JSON.parse(s)
来源：http://hh.szxytkj.cn

TS:   JSON.parse(s)
来源：http://ks.hnjuh.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://uw.521024.cn

Go:   json.Unmarshal(data, &v)
来源：http://tx.huanxung.cn

Ruby: JSON.parse(s)
来源：http://pd.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rw.gzmigu.cn

[K03] JSON 美化输出（带缩进）
来源：http://um.bjjhwx.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://iq.panjiajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zt.huanxung.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ps.gzmigu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://nd.wgjwhj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ca.szxytkj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gg.huixinmuqiang.cn

Ruby: JSON.pretty_generate(obj)
来源：http://yw.shtwfgs.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mh.jianghongdianzi.cn

[K04] 读取 JSON 文件
来源：http://qq.yuexingan06.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xw.newstarts.cn


<!-- 参考信息 -->