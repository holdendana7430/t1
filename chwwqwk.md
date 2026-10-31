代发 wailian999

PHP:  get_object_vars($obj);
来源：http://bv.huixiangedu.cn

JS:   Object.entries(obj)
来源：http://ax.newstarts.cn

TS:   Object.entries(obj)
来源：http://qz.szsharing.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hj.shtwfgs.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://if.szxytkj.cn

Ruby: obj.instance_variables
来源：http://zr.haigaiapp.cn

C#:   // 用反射或 System.Text.Json
来源：http://ib.szsharing.cn

================================================================================
来源：http://he.wgjwhj.cn

H. 异常与错误处理
来源：http://qj.gzmigu.cn

================================================================================
来源：http://hs.nicolike.cn

[H01] try / catch 基础
来源：http://hr.nszjky.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fr.hnjuh.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://es.chemitech.net.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ht.asd995.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://he.szxytkj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kv.huixiangedu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ny.wgjwhj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ps.bookmarksfly.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xg.shtwfgs.cn

[H02] finally / ensure 收尾
来源：http://co.chemitech.net.cn

Py:   try: f()⏎finally: cleanup()
来源：http://di.huanxung.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://kk.newstarts.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://rl.newstarts.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://za.bjjhwx.cn

Java: try { f(); } finally { cleanup(); }
来源：http://bb.huixiangedu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://sl.gzmigu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://lf.hnjuh.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://yt.szxytkj.cn

[H03] 主动抛出异常
来源：http://to.hnjuh.cn

Py:   raise ValueError("错误信息")
来源：http://ij.jctech888.com.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fb.jianghongdianzi.cn

JS:   throw new Error("错误信息");
来源：http://fs.muxihuayi.cn

TS:   throw new Error("错误信息");
来源：http://zt.haigaiapp.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://bb.muxihuayi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ao.szsharing.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://uy.haigaiapp.cn

C#:   throw new ArgumentException("错误信息");
来源：http://rf.huanxung.cn

[H04] 自定义异常类型
来源：http://sd.bookmarksfly.cn

Py:   class MyError(Exception): pass
来源：http://os.yuntaijiaju.cn

PHP:  class MyError extends RuntimeException {}
来源：http://eg.521024.cn

JS:   class MyError extends Error {}
来源：http://bl.szsharing.cn

TS:   class MyError extends Error {}
来源：http://fx.shxzskj.cn

Java: class MyException extends RuntimeException {}
来源：http://ay.nicolike.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fn.gzmigu.cn

Ruby: class MyError < StandardError; end
来源：http://rn.yuntaijiaju.cn

C#:   class MyException : Exception {}
来源：http://zj.chemitech.net.cn

[H05] 捕获特定类型
来源：http://qo.hahajie.cn

Py:   except ValueError as e:
来源：http://qb.newstarts.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nm.szsharing.cn

JS:   if (e instanceof TypeError) {}
来源：http://ee.hahajie.cn

TS:   if (e instanceof TypeError) {}
来源：http://qz.shxzukj.cn

Java: catch (IOException | SQLException e) {}
来源：http://lo.lnxyls.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://aq.haigaiapp.cn

Ruby: rescue ArgumentError => e
来源：http://va.521024.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jl.shxzukj.cn

[H06] 可选值 / 空值安全访问
来源：http://fo.newstarts.cn

Py:   value = d.get("k") or default
来源：http://ra.gzmigu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://fk.muxihuayi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://sj.shxzskj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://pc.nicolike.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ji.wgjwhj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://vj.yuntaijiaju.cn

Ruby: d&.dig(:a, :b)
来源：http://ob.huixinmuqiang.cn

C#:   obj?.A?.B ?? default
来源：http://dx.yuntaijiaju.cn

[H07] 断言
来源：http://pe.521024.cn

Py:   assert x > 0, "必须为正"
来源：http://lu.shxzskj.cn

PHP:  assert($x > 0);
来源：http://aa.colortex.cn

JS:   console.assert(x > 0);
来源：http://og.521024.cn

TS:   console.assert(x > 0);
来源：http://rf.hnjuh.cn

Java: assert x > 0 : "必须为正";
来源：http://jo.muxihuayi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zr.wgjwhj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vx.jianghongdianzi.cn

C#:   Debug.Assert(x > 0);
来源：http://ru.shxzskj.cn

[H08] 获取错误信息与堆栈
来源：http://to.szsharing.cn

Py:   str(e);  traceback.format_exc()
来源：http://ow.jianghongdianzi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vl.shxzskj.cn

JS:   e.message;  e.stack
来源：http://pg.newstarts.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ek.521024.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://fz.newstarts.cn

Go:   err.Error()
来源：http://vh.chemitech.net.cn

Ruby: e.message;  e.backtrace
来源：http://ec.hahajie.cn

C#:   e.Message;  e.StackTrace
来源：http://gr.yuexingan06.cn

[H09] 带错误码的异常
来源：http://ie.yuexingan06.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cr.colortex.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://hq.huixiangedu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kx.muxihuayi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cb.hnjuh.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ha.hahajie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nl.hahajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://df.wgjwhj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://oo.colortex.cn

[H10] 资源自动释放
来源：http://ii.colortex.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vr.hahajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://iq.shxzukj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dz.wgjwhj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://se.hnjuh.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ff.hnjuh.cn

Go:   defer f.Close()
来源：http://kq.lnxyls.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://sn.521024.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://je.huixiangedu.cn

================================================================================
来源：http://zv.huixiangedu.cn

I. 正则表达式
来源：http://bc.lnxyls.cn

================================================================================
来源：http://at.haigaiapp.cn

[I01] 判断是否匹配
来源：http://is.szsharing.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://al.nicolike.cn

PHP:  preg_match('/\d+/', $s);
来源：http://nz.jianghongdianzi.cn

JS:   /\d+/.test(s)
来源：http://iu.bjjhwx.cn

TS:   /\d+/.test(s)
来源：http://sg.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fj.newstarts.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hu.nicolike.cn

Ruby: s.match?(/\d+/)
来源：http://vu.asd995.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hs.yuntaijiaju.cn

[I02] 提取所有匹配
来源：http://al.szxytkj.cn

Py:   re.findall(r"\d+", s)
来源：http://ag.shtwfgs.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fl.huixinmuqiang.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ei.hahajie.cn

TS:   s.match(/\d+/g)
来源：http://ao.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zx.huixinmuqiang.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://uv.jianghongdianzi.cn

Ruby: s.scan(/\d+/)
来源：http://ls.hnjuh.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ld.szxytkj.cn

[I03] 提取捕获分组
来源：http://ec.nszjky.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ez.hahajie.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xj.haigaiapp.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mj.lnxyls.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zv.shtwfgs.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lc.hahajie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wv.szxytkj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hw.muxihuayi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mt.chemitech.net.cn

[I04] 正则替换
来源：http://mr.yuntaijiaju.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://il.shtwfgs.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://op.newstarts.cn

JS:   s.replace(/\d+/g, "#")
来源：http://kc.hahajie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://tm.colortex.cn

Java: s.replaceAll("\\d+", "#")
来源：http://no.chemitech.net.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://oa.shxzskj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://mj.haigaiapp.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gm.hnjuh.cn

[I05] 按正则拆分
来源：http://ta.hnjuh.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hm.lnxyls.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fg.szxytkj.cn

JS:   s.split(/\s*,\s*/)
来源：http://ch.shxzskj.cn

TS:   s.split(/\s*,\s*/)
来源：http://as.521024.cn

Java: s.split("\\s*,\\s*")
来源：http://cr.szsharing.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ks.colortex.cn

Ruby: s.split(/\s*,\s*/)
来源：http://af.yuntaijiaju.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mj.shtwfgs.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://no.huanxung.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ai.yuexingan06.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gp.haigaiapp.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gx.szsharing.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lw.muxihuayi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bs.colortex.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qq.newstarts.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hj.nicolike.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xn.521024.cn

[I07] 忽略大小写与多行模式
来源：http://sa.shxzukj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ju.yuntaijiaju.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hk.shtwfgs.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://en.shxzskj.cn

TS:   /error/gim
来源：http://ef.muxihuayi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gl.muxihuayi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dz.panjiajie.cn

Ruby: s.scan(/error/i)
来源：http://mz.nicolike.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jj.asd995.cn

[I08] 贪婪与非贪婪匹配
来源：http://qt.asd995.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mo.szxytkj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mc.huixinmuqiang.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ga.nicolike.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fp.colortex.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://gd.panjiajie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hq.asd995.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nj.szxytkj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lm.haigaiapp.cn

================================================================================
来源：http://io.szxytkj.cn

J. 日期与时间
来源：http://aq.muxihuayi.cn

================================================================================
来源：http://fx.szxytkj.cn

[J01] 获取当前时间
来源：http://so.yuexingan06.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vf.hnjuh.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xs.chemitech.net.cn

JS:   new Date();  Date.now()
来源：http://sk.lnxyls.cn

TS:   new Date();  Date.now()
来源：http://en.lnxyls.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://iy.hahajie.cn

Go:   time.Now()
来源：http://ud.szsharing.cn

Ruby: Time.now
来源：http://le.huanxung.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ra.hahajie.cn

[J02] 格式化输出
来源：http://eb.521024.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gm.jctech888.com.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xa.szsharing.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sr.huanxung.cn

TS:   d.toISOString()
来源：http://zr.gzmigu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ev.haigaiapp.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ub.bjjhwx.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rh.huixiangedu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kz.521024.cn

[J03] 字符串解析为日期
来源：http://on.yuexingan06.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kc.yuntaijiaju.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bf.hnjuh.cn

JS:   new Date("2024-01-02")
来源：http://td.shxzukj.cn

TS:   new Date("2024-01-02")
来源：http://wg.haigaiapp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ar.hnjuh.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cc.9csxet.cn

Ruby: Date.parse("2024-01-02")
来源：http://oj.jctech888.com.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nh.huixinmuqiang.cn

[J04] 时间戳与日期互转
来源：http://ea.szsharing.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jy.szxytkj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hx.haigaiapp.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sk.szxytkj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://vb.muxihuayi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qq.szxytkj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tx.shxzukj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qt.shxzskj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dg.nicolike.cn

[J05] 时间加减（加 7 天）
来源：http://bp.521024.cn

Py:   now + timedelta(days=7)
来源：http://pt.huanxung.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ja.szxytkj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://go.panjiajie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gr.yuntaijiaju.cn

Java: LocalDate.now().plusDays(7)
来源：http://ro.yuntaijiaju.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ez.jctech888.com.cn

Ruby: Time.now + 7 * 86400
来源：http://gq.haigaiapp.cn

C#:   DateTime.Now.AddDays(7)
来源：http://wt.szsharing.cn

[J06] 计算两时间之差
来源：http://oz.hahajie.cn

Py:   (end - start).total_seconds()
来源：http://zn.521024.cn

PHP:  $end->diff($start)->days;
来源：http://dd.hnjuh.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nw.9csxet.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ta.huixiangedu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://eq.panjiajie.cn

Go:   end.Sub(start).Hours()
来源：http://dc.szxytkj.cn

Ruby: end - start                 # 返回秒数
来源：http://ji.hahajie.cn

C#:   (end - start).TotalSeconds
来源：http://ke.yuexingan06.cn

[J07] 比较两个日期
来源：http://sp.hnjuh.cn

Py:   d1 < d2;  d1 == d2
来源：http://un.asd995.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ow.9csxet.cn

JS:   d1.getTime() < d2.getTime()
来源：http://rz.521024.cn

TS:   d1.getTime() < d2.getTime()
来源：http://hx.panjiajie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://me.bjjhwx.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://id.bjjhwx.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qv.haigaiapp.cn

C#:   d1 < d2;  d1 == d2
来源：http://yx.muxihuayi.cn

[J08] 提取年月日与星期
来源：http://uo.huanxung.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qe.asd995.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vi.hnjuh.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dz.szxytkj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qk.hahajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pv.shxzskj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pj.yuntaijiaju.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://la.panjiajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jn.nicolike.cn

[J09] 时区处理
来源：http://rz.yuexingan06.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lo.huanxung.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sp.shxzukj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uh.shxzukj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vo.hahajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bb.hahajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://um.9csxet.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://nr.bookmarksfly.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kr.shxzukj.cn

[J10] 取今天 / 本月第一天
来源：http://na.bjjhwx.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://km.colortex.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ye.huixinmuqiang.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zs.bookmarksfly.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tz.asd995.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jh.hnjuh.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://du.nszjky.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gf.9csxet.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://uw.yuexingan06.cn

================================================================================
来源：http://ps.yuexingan06.cn

K. JSON 与序列化
来源：http://td.muxihuayi.cn

================================================================================
来源：http://jz.bjjhwx.cn

[K01] 对象转 JSON 字符串
来源：http://uf.9csxet.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://uf.panjiajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rw.huanxung.cn

JS:   JSON.stringify(obj)
来源：http://bz.muxihuayi.cn

TS:   JSON.stringify(obj)
来源：http://ge.haigaiapp.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://br.muxihuayi.cn

Go:   json.Marshal(obj)
来源：http://vv.bjjhwx.cn

Ruby: obj.to_json                                     // require "json"
来源：http://wc.newstarts.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://oh.jianghongdianzi.cn

[K02] JSON 字符串转对象
来源：http://zf.jianghongdianzi.cn

Py:   json.loads(s)
来源：http://ni.bookmarksfly.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ma.huixinmuqiang.cn

JS:   JSON.parse(s)
来源：http://ct.huanxung.cn

TS:   JSON.parse(s)
来源：http://yx.shxzskj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xo.huixinmuqiang.cn

Go:   json.Unmarshal(data, &v)
来源：http://cv.asd995.cn

Ruby: JSON.parse(s)
来源：http://lc.muxihuayi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dj.gzmigu.cn

[K03] JSON 美化输出（带缩进）
来源：http://qm.hahajie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dx.huixiangedu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ou.huanxung.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://bd.wgjwhj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://jt.hahajie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://li.wgjwhj.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dh.yuntaijiaju.cn

Ruby: JSON.pretty_generate(obj)
来源：http://bo.colortex.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ki.hnjuh.cn

[K04] 读取 JSON 文件
来源：http://ah.jianghongdianzi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yz.haigaiapp.cn


<!-- 参考信息 -->