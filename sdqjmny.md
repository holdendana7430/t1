代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://vr.newstarts.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gp.haigaiapp.cn

[G16] 对象转数组 / 字典
来源：http://fr.szsharing.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://le.gzmigu.cn

PHP:  get_object_vars($obj);
来源：http://mk.huixinmuqiang.cn

JS:   Object.entries(obj)
来源：http://xm.jianghongdianzi.cn

TS:   Object.entries(obj)
来源：http://uq.huanxung.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bq.9csxet.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://yp.jianghongdianzi.cn

Ruby: obj.instance_variables
来源：http://um.haigaiapp.cn

C#:   // 用反射或 System.Text.Json
来源：http://ge.hahajie.cn

================================================================================
来源：http://zk.haigaiapp.cn

H. 异常与错误处理
来源：http://or.newstarts.cn

================================================================================
来源：http://la.huanxung.cn

[H01] try / catch 基础
来源：http://ns.huixinmuqiang.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yn.haigaiapp.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gy.9csxet.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xy.colortex.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://da.nicolike.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gp.muxihuayi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vh.haigaiapp.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://oy.jctech888.com.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nn.nszjky.cn

[H02] finally / ensure 收尾
来源：http://fo.shtwfgs.cn

Py:   try: f()⏎finally: cleanup()
来源：http://il.asd995.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ah.newstarts.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ec.bookmarksfly.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://tq.szxytkj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://qm.lnxyls.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zw.bjjhwx.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ah.hahajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ll.chemitech.net.cn

[H03] 主动抛出异常
来源：http://nx.521024.cn

Py:   raise ValueError("错误信息")
来源：http://ni.hnjuh.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cx.muxihuayi.cn

JS:   throw new Error("错误信息");
来源：http://bo.huixiangedu.cn

TS:   throw new Error("错误信息");
来源：http://hk.yuexingan06.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://mh.huixiangedu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ql.521024.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://cd.panjiajie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://xe.huixiangedu.cn

[H04] 自定义异常类型
来源：http://nc.jianghongdianzi.cn

Py:   class MyError(Exception): pass
来源：http://pv.hahajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://bq.huixiangedu.cn

JS:   class MyError extends Error {}
来源：http://mg.shtwfgs.cn

TS:   class MyError extends Error {}
来源：http://fp.newstarts.cn

Java: class MyException extends RuntimeException {}
来源：http://uh.huanxung.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mf.muxihuayi.cn

Ruby: class MyError < StandardError; end
来源：http://or.lnxyls.cn

C#:   class MyException : Exception {}
来源：http://ju.nicolike.cn

[H05] 捕获特定类型
来源：http://jh.nszjky.cn

Py:   except ValueError as e:
来源：http://ct.yuntaijiaju.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fi.shxzukj.cn

JS:   if (e instanceof TypeError) {}
来源：http://tf.521024.cn

TS:   if (e instanceof TypeError) {}
来源：http://wz.bjjhwx.cn

Java: catch (IOException | SQLException e) {}
来源：http://eo.hnjuh.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ze.colortex.cn

Ruby: rescue ArgumentError => e
来源：http://vv.wgjwhj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pc.wgjwhj.cn

[H06] 可选值 / 空值安全访问
来源：http://mx.jctech888.com.cn

Py:   value = d.get("k") or default
来源：http://wp.shxzskj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ws.shtwfgs.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ek.yuexingan06.cn

TS:   obj?.a?.b;  d ?? default
来源：http://cg.huixinmuqiang.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ex.huanxung.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://vn.asd995.cn

Ruby: d&.dig(:a, :b)
来源：http://nz.jianghongdianzi.cn

C#:   obj?.A?.B ?? default
来源：http://jx.shxzskj.cn

[H07] 断言
来源：http://rv.jianghongdianzi.cn

Py:   assert x > 0, "必须为正"
来源：http://tf.shxzskj.cn

PHP:  assert($x > 0);
来源：http://gv.yuntaijiaju.cn

JS:   console.assert(x > 0);
来源：http://ly.haigaiapp.cn

TS:   console.assert(x > 0);
来源：http://au.jctech888.com.cn

Java: assert x > 0 : "必须为正";
来源：http://nm.colortex.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ej.shxzskj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://pw.muxihuayi.cn

C#:   Debug.Assert(x > 0);
来源：http://mu.huanxung.cn

[H08] 获取错误信息与堆栈
来源：http://lv.521024.cn

Py:   str(e);  traceback.format_exc()
来源：http://ru.9csxet.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zp.hnjuh.cn

JS:   e.message;  e.stack
来源：http://ax.gzmigu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ue.nszjky.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ub.521024.cn

Go:   err.Error()
来源：http://wr.huanxung.cn

Ruby: e.message;  e.backtrace
来源：http://jo.nicolike.cn

C#:   e.Message;  e.StackTrace
来源：http://ff.nszjky.cn

[H09] 带错误码的异常
来源：http://gy.521024.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hb.muxihuayi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ee.nicolike.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://iy.521024.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gl.huanxung.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gl.521024.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ty.gzmigu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ba.9csxet.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://xj.shxzskj.cn

[H10] 资源自动释放
来源：http://qa.bookmarksfly.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://gn.newstarts.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kk.hahajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mt.nicolike.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sw.yuntaijiaju.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pt.gzmigu.cn

Go:   defer f.Close()
来源：http://fp.hahajie.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://iw.shxzskj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xq.asd995.cn

================================================================================
来源：http://vc.szxytkj.cn

I. 正则表达式
来源：http://xq.szsharing.cn

================================================================================
来源：http://lt.lnxyls.cn

[I01] 判断是否匹配
来源：http://sv.shxzukj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wi.szsharing.cn

PHP:  preg_match('/\d+/', $s);
来源：http://lp.yuexingan06.cn

JS:   /\d+/.test(s)
来源：http://th.bjjhwx.cn

TS:   /\d+/.test(s)
来源：http://ps.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ot.szxytkj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zz.shxzskj.cn

Ruby: s.match?(/\d+/)
来源：http://an.haigaiapp.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ue.jctech888.com.cn

[I02] 提取所有匹配
来源：http://jg.shtwfgs.cn

Py:   re.findall(r"\d+", s)
来源：http://jg.nszjky.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dj.newstarts.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jp.9csxet.cn

TS:   s.match(/\d+/g)
来源：http://md.hahajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wk.jctech888.com.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ye.colortex.cn

Ruby: s.scan(/\d+/)
来源：http://se.521024.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jx.bookmarksfly.cn

[I03] 提取捕获分组
来源：http://mq.newstarts.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pm.muxihuayi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ae.newstarts.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nw.521024.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fb.colortex.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fo.hnjuh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://if.huixiangedu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cq.shxzskj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://iz.nszjky.cn

[I04] 正则替换
来源：http://kf.yuexingan06.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://fb.szxytkj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hc.huixiangedu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://us.asd995.cn

TS:   s.replace(/\d+/g, "#")
来源：http://uc.yuntaijiaju.cn

Java: s.replaceAll("\\d+", "#")
来源：http://nt.newstarts.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://lh.shxzskj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://av.asd995.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vv.muxihuayi.cn

[I05] 按正则拆分
来源：http://rc.yuntaijiaju.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://rh.shxzskj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://im.gzmigu.cn

JS:   s.split(/\s*,\s*/)
来源：http://wm.nicolike.cn

TS:   s.split(/\s*,\s*/)
来源：http://uc.shxzukj.cn

Java: s.split("\\s*,\\s*")
来源：http://bb.yuntaijiaju.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://he.huanxung.cn

Ruby: s.split(/\s*,\s*/)
来源：http://if.gzmigu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ir.muxihuayi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hf.hahajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lr.9csxet.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wl.521024.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tc.bookmarksfly.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ig.nszjky.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wd.shxzukj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jy.nszjky.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://md.chemitech.net.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uf.gzmigu.cn

[I07] 忽略大小写与多行模式
来源：http://zp.haigaiapp.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wz.muxihuayi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dt.huixinmuqiang.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nk.yuntaijiaju.cn

TS:   /error/gim
来源：http://zi.jianghongdianzi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xv.nicolike.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tj.bjjhwx.cn

Ruby: s.scan(/error/i)
来源：http://yp.bjjhwx.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yg.yuexingan06.cn

[I08] 贪婪与非贪婪匹配
来源：http://fd.muxihuayi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ft.9csxet.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zy.hahajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rr.newstarts.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://it.shxzskj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://gu.lnxyls.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pd.yuntaijiaju.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://eg.szxytkj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fa.nszjky.cn

================================================================================
来源：http://pi.jianghongdianzi.cn

J. 日期与时间
来源：http://og.newstarts.cn

================================================================================
来源：http://lw.9csxet.cn

[J01] 获取当前时间
来源：http://cm.colortex.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://as.haigaiapp.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ps.shxzskj.cn

JS:   new Date();  Date.now()
来源：http://wb.newstarts.cn

TS:   new Date();  Date.now()
来源：http://qd.muxihuayi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://id.panjiajie.cn

Go:   time.Now()
来源：http://cp.hahajie.cn

Ruby: Time.now
来源：http://qs.gzmigu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ib.colortex.cn

[J02] 格式化输出
来源：http://hy.szxytkj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gx.huixinmuqiang.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yb.shxzskj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://er.nicolike.cn

TS:   d.toISOString()
来源：http://gd.asd995.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bf.nszjky.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://di.newstarts.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ra.jianghongdianzi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rr.wgjwhj.cn

[J03] 字符串解析为日期
来源：http://nd.huanxung.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ue.gzmigu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nl.asd995.cn

JS:   new Date("2024-01-02")
来源：http://cz.hahajie.cn

TS:   new Date("2024-01-02")
来源：http://bd.jianghongdianzi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mu.shxzukj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://us.panjiajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://on.lnxyls.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://je.jctech888.com.cn

[J04] 时间戳与日期互转
来源：http://ko.chemitech.net.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kn.gzmigu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ay.9csxet.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://no.wgjwhj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://hr.newstarts.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gf.colortex.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tp.lnxyls.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qb.lnxyls.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://oq.haigaiapp.cn

[J05] 时间加减（加 7 天）
来源：http://rq.9csxet.cn

Py:   now + timedelta(days=7)
来源：http://qi.lnxyls.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://pw.hahajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ah.muxihuayi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mm.hnjuh.cn

Java: LocalDate.now().plusDays(7)
来源：http://fc.shxzukj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zg.huanxung.cn

Ruby: Time.now + 7 * 86400
来源：http://jk.lnxyls.cn

C#:   DateTime.Now.AddDays(7)
来源：http://dh.bookmarksfly.cn

[J06] 计算两时间之差
来源：http://tf.colortex.cn

Py:   (end - start).total_seconds()
来源：http://qx.wgjwhj.cn

PHP:  $end->diff($start)->days;
来源：http://li.shxzukj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pl.nszjky.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rv.hahajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://tk.shxzskj.cn

Go:   end.Sub(start).Hours()
来源：http://wv.muxihuayi.cn

Ruby: end - start                 # 返回秒数
来源：http://vv.szxytkj.cn

C#:   (end - start).TotalSeconds
来源：http://ic.huixinmuqiang.cn

[J07] 比较两个日期
来源：http://oy.chemitech.net.cn

Py:   d1 < d2;  d1 == d2
来源：http://dx.bjjhwx.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ti.huixinmuqiang.cn

JS:   d1.getTime() < d2.getTime()
来源：http://eu.colortex.cn

TS:   d1.getTime() < d2.getTime()
来源：http://id.yuexingan06.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qy.shtwfgs.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://og.yuexingan06.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wg.szsharing.cn

C#:   d1 < d2;  d1 == d2
来源：http://my.haigaiapp.cn

[J08] 提取年月日与星期
来源：http://kw.huanxung.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ih.gzmigu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qi.szsharing.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mp.asd995.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://db.jctech888.com.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dk.nicolike.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xy.szsharing.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xm.9csxet.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ed.gzmigu.cn

[J09] 时区处理
来源：http://ah.shxzukj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://by.lnxyls.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wa.gzmigu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jq.colortex.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eb.muxihuayi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://af.chemitech.net.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lo.colortex.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://sg.asd995.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bx.521024.cn

[J10] 取今天 / 本月第一天
来源：http://vn.jianghongdianzi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jj.bookmarksfly.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bm.9csxet.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uo.chemitech.net.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ec.huixinmuqiang.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jx.yuexingan06.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rm.shtwfgs.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fi.yuntaijiaju.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ep.asd995.cn

================================================================================
来源：http://lu.huanxung.cn

K. JSON 与序列化
来源：http://dq.huanxung.cn

================================================================================
来源：http://ch.nicolike.cn

[K01] 对象转 JSON 字符串
来源：http://ot.newstarts.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zo.521024.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bf.jianghongdianzi.cn

JS:   JSON.stringify(obj)
来源：http://ic.bjjhwx.cn

TS:   JSON.stringify(obj)
来源：http://rz.bookmarksfly.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bd.521024.cn

Go:   json.Marshal(obj)
来源：http://sc.hahajie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://cb.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://cu.huixinmuqiang.cn

[K02] JSON 字符串转对象
来源：http://pv.asd995.cn

Py:   json.loads(s)
来源：http://pi.yuexingan06.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ka.bookmarksfly.cn

JS:   JSON.parse(s)
来源：http://di.9csxet.cn

TS:   JSON.parse(s)
来源：http://rn.shtwfgs.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ov.szxytkj.cn

Go:   json.Unmarshal(data, &v)
来源：http://lo.gzmigu.cn

Ruby: JSON.parse(s)
来源：http://yf.panjiajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gz.gzmigu.cn

[K03] JSON 美化输出（带缩进）
来源：http://vv.yuntaijiaju.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ue.yuexingan06.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zh.nszjky.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://cw.yuexingan06.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://we.shtwfgs.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gi.colortex.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tz.huanxung.cn


<!-- 参考信息 -->