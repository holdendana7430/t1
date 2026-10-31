代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://cv.szsharing.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fy.szxytkj.cn

[G16] 对象转数组 / 字典
来源：http://ev.asd995.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vv.jctech888.com.cn

PHP:  get_object_vars($obj);
来源：http://ig.bookmarksfly.cn

JS:   Object.entries(obj)
来源：http://hc.newstarts.cn

TS:   Object.entries(obj)
来源：http://ok.521024.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://uw.hahajie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://oy.szxytkj.cn

Ruby: obj.instance_variables
来源：http://in.newstarts.cn

C#:   // 用反射或 System.Text.Json
来源：http://gc.szxytkj.cn

================================================================================
来源：http://at.nicolike.cn

H. 异常与错误处理
来源：http://lo.yuntaijiaju.cn

================================================================================
来源：http://ti.muxihuayi.cn

[H01] try / catch 基础
来源：http://lb.shtwfgs.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dd.szsharing.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://up.shtwfgs.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kf.shxzskj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lj.gzmigu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ak.newstarts.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zh.szsharing.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vi.jctech888.com.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ft.chemitech.net.cn

[H02] finally / ensure 收尾
来源：http://nl.asd995.cn

Py:   try: f()⏎finally: cleanup()
来源：http://oo.haigaiapp.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xk.huixiangedu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://qr.shxzskj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://bh.shxzukj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://em.haigaiapp.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://rh.gzmigu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ua.nszjky.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://to.jianghongdianzi.cn

[H03] 主动抛出异常
来源：http://tp.lnxyls.cn

Py:   raise ValueError("错误信息")
来源：http://ee.panjiajie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kl.lnxyls.cn

JS:   throw new Error("错误信息");
来源：http://rn.yuntaijiaju.cn

TS:   throw new Error("错误信息");
来源：http://md.huixinmuqiang.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://lf.szxytkj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ut.colortex.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://kf.szsharing.cn

C#:   throw new ArgumentException("错误信息");
来源：http://bs.muxihuayi.cn

[H04] 自定义异常类型
来源：http://ni.szsharing.cn

Py:   class MyError(Exception): pass
来源：http://jj.colortex.cn

PHP:  class MyError extends RuntimeException {}
来源：http://sj.jctech888.com.cn

JS:   class MyError extends Error {}
来源：http://co.hahajie.cn

TS:   class MyError extends Error {}
来源：http://am.shxzskj.cn

Java: class MyException extends RuntimeException {}
来源：http://lg.wgjwhj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zd.bookmarksfly.cn

Ruby: class MyError < StandardError; end
来源：http://hy.bookmarksfly.cn

C#:   class MyException : Exception {}
来源：http://ro.huixiangedu.cn

[H05] 捕获特定类型
来源：http://la.jianghongdianzi.cn

Py:   except ValueError as e:
来源：http://fl.nszjky.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tb.huixiangedu.cn

JS:   if (e instanceof TypeError) {}
来源：http://uq.chemitech.net.cn

TS:   if (e instanceof TypeError) {}
来源：http://ay.hahajie.cn

Java: catch (IOException | SQLException e) {}
来源：http://mv.colortex.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gg.chemitech.net.cn

Ruby: rescue ArgumentError => e
来源：http://ay.shtwfgs.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ww.shxzukj.cn

[H06] 可选值 / 空值安全访问
来源：http://up.chemitech.net.cn

Py:   value = d.get("k") or default
来源：http://va.chemitech.net.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kw.nicolike.cn

JS:   obj?.a?.b;  d ?? default
来源：http://kf.hahajie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://fb.shxzskj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xa.szxytkj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://no.bjjhwx.cn

Ruby: d&.dig(:a, :b)
来源：http://dz.shxzukj.cn

C#:   obj?.A?.B ?? default
来源：http://dm.521024.cn

[H07] 断言
来源：http://jz.bookmarksfly.cn

Py:   assert x > 0, "必须为正"
来源：http://ui.panjiajie.cn

PHP:  assert($x > 0);
来源：http://xx.huanxung.cn

JS:   console.assert(x > 0);
来源：http://zh.bookmarksfly.cn

TS:   console.assert(x > 0);
来源：http://es.yuntaijiaju.cn

Java: assert x > 0 : "必须为正";
来源：http://wk.newstarts.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tq.panjiajie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://hq.yuexingan06.cn

C#:   Debug.Assert(x > 0);
来源：http://az.wgjwhj.cn

[H08] 获取错误信息与堆栈
来源：http://qy.nicolike.cn

Py:   str(e);  traceback.format_exc()
来源：http://wt.gzmigu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pr.bookmarksfly.cn

JS:   e.message;  e.stack
来源：http://gi.yuntaijiaju.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://gj.huixiangedu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://vp.jctech888.com.cn

Go:   err.Error()
来源：http://uq.colortex.cn

Ruby: e.message;  e.backtrace
来源：http://tf.shxzskj.cn

C#:   e.Message;  e.StackTrace
来源：http://gg.huixinmuqiang.cn

[H09] 带错误码的异常
来源：http://ge.huanxung.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ft.nszjky.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://br.hnjuh.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lw.huixiangedu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yc.haigaiapp.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xm.shtwfgs.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qr.colortex.cn

Ruby: raise MyError.new("fail", 500)
来源：http://va.nszjky.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://xd.muxihuayi.cn

[H10] 资源自动释放
来源：http://ol.szxytkj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://it.wgjwhj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qh.colortex.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lr.bookmarksfly.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xh.gzmigu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gd.szsharing.cn

Go:   defer f.Close()
来源：http://yw.shtwfgs.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://sv.521024.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cu.hnjuh.cn

================================================================================
来源：http://yn.huixiangedu.cn

I. 正则表达式
来源：http://il.panjiajie.cn

================================================================================
来源：http://kt.newstarts.cn

[I01] 判断是否匹配
来源：http://mp.szxytkj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cm.wgjwhj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://og.haigaiapp.cn

JS:   /\d+/.test(s)
来源：http://so.newstarts.cn

TS:   /\d+/.test(s)
来源：http://hu.shtwfgs.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gx.hahajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://me.newstarts.cn

Ruby: s.match?(/\d+/)
来源：http://ab.521024.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lc.muxihuayi.cn

[I02] 提取所有匹配
来源：http://rn.huanxung.cn

Py:   re.findall(r"\d+", s)
来源：http://lb.wgjwhj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fs.jctech888.com.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vf.hahajie.cn

TS:   s.match(/\d+/g)
来源：http://ak.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bo.szsharing.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mg.szsharing.cn

Ruby: s.scan(/\d+/)
来源：http://zg.yuntaijiaju.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bf.shxzukj.cn

[I03] 提取捕获分组
来源：http://gz.szxytkj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mp.colortex.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sf.wgjwhj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yb.gzmigu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sm.szsharing.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gj.chemitech.net.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sy.shxzskj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gm.yuntaijiaju.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nb.panjiajie.cn

[I04] 正则替换
来源：http://wz.asd995.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://kj.haigaiapp.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sk.shxzskj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://tm.huixinmuqiang.cn

TS:   s.replace(/\d+/g, "#")
来源：http://sg.hnjuh.cn

Java: s.replaceAll("\\d+", "#")
来源：http://od.huixinmuqiang.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://hw.lnxyls.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://kg.9csxet.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://sf.huanxung.cn

[I05] 按正则拆分
来源：http://fa.jianghongdianzi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://xv.newstarts.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uy.asd995.cn

JS:   s.split(/\s*,\s*/)
来源：http://ns.asd995.cn

TS:   s.split(/\s*,\s*/)
来源：http://ev.szxytkj.cn

Java: s.split("\\s*,\\s*")
来源：http://is.bjjhwx.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://io.szsharing.cn

Ruby: s.split(/\s*,\s*/)
来源：http://un.521024.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://er.chemitech.net.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rh.szsharing.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gv.yuexingan06.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ph.colortex.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lt.lnxyls.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nq.jctech888.com.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sc.haigaiapp.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jo.hahajie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://te.nszjky.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nj.asd995.cn

[I07] 忽略大小写与多行模式
来源：http://bl.bjjhwx.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bj.haigaiapp.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qh.lnxyls.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ej.shtwfgs.cn

TS:   /error/gim
来源：http://zz.asd995.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xa.nszjky.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pp.nicolike.cn

Ruby: s.scan(/error/i)
来源：http://ta.gzmigu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zk.521024.cn

[I08] 贪婪与非贪婪匹配
来源：http://yo.9csxet.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rh.shtwfgs.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fu.huanxung.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wo.9csxet.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mg.shxzukj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://px.huixiangedu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pr.9csxet.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://md.bjjhwx.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mf.shtwfgs.cn

================================================================================
来源：http://lq.colortex.cn

J. 日期与时间
来源：http://qm.panjiajie.cn

================================================================================
来源：http://sw.shxzskj.cn

[J01] 获取当前时间
来源：http://jb.colortex.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://dw.shxzukj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jx.521024.cn

JS:   new Date();  Date.now()
来源：http://ur.bjjhwx.cn

TS:   new Date();  Date.now()
来源：http://tv.9csxet.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://xa.9csxet.cn

Go:   time.Now()
来源：http://ih.wgjwhj.cn

Ruby: Time.now
来源：http://ca.hnjuh.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jt.jianghongdianzi.cn

[J02] 格式化输出
来源：http://bh.yuntaijiaju.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yw.shxzskj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xe.lnxyls.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tb.nicolike.cn

TS:   d.toISOString()
来源：http://sm.521024.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wk.shxzukj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rn.nicolike.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rw.bookmarksfly.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wh.wgjwhj.cn

[J03] 字符串解析为日期
来源：http://xr.chemitech.net.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xo.haigaiapp.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gy.shtwfgs.cn

JS:   new Date("2024-01-02")
来源：http://cn.huixiangedu.cn

TS:   new Date("2024-01-02")
来源：http://lu.nszjky.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ki.panjiajie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gt.haigaiapp.cn

Ruby: Date.parse("2024-01-02")
来源：http://db.hahajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://av.nicolike.cn

[J04] 时间戳与日期互转
来源：http://da.bookmarksfly.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mw.chemitech.net.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://je.panjiajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hc.hahajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://mo.521024.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zz.lnxyls.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hr.wgjwhj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uc.shtwfgs.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://de.chemitech.net.cn

[J05] 时间加减（加 7 天）
来源：http://mq.panjiajie.cn

Py:   now + timedelta(days=7)
来源：http://oy.9csxet.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://yd.jctech888.com.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://of.yuexingan06.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gb.shxzskj.cn

Java: LocalDate.now().plusDays(7)
来源：http://kk.muxihuayi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cz.nicolike.cn

Ruby: Time.now + 7 * 86400
来源：http://hr.yuexingan06.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jw.hahajie.cn

[J06] 计算两时间之差
来源：http://cs.nicolike.cn

Py:   (end - start).total_seconds()
来源：http://ax.yuexingan06.cn

PHP:  $end->diff($start)->days;
来源：http://ls.wgjwhj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mj.asd995.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://po.9csxet.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bn.bookmarksfly.cn

Go:   end.Sub(start).Hours()
来源：http://pi.chemitech.net.cn

Ruby: end - start                 # 返回秒数
来源：http://ra.hnjuh.cn

C#:   (end - start).TotalSeconds
来源：http://ta.colortex.cn

[J07] 比较两个日期
来源：http://bu.chemitech.net.cn

Py:   d1 < d2;  d1 == d2
来源：http://ql.bookmarksfly.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://he.huixiangedu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://pm.wgjwhj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://zd.gzmigu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mm.bjjhwx.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hg.nicolike.cn

Ruby: d1 < d2;  d1 == d2
来源：http://nr.jctech888.com.cn

C#:   d1 < d2;  d1 == d2
来源：http://bb.huixiangedu.cn

[J08] 提取年月日与星期
来源：http://yk.yuexingan06.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vg.wgjwhj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kj.lnxyls.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jd.wgjwhj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ie.521024.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xj.yuexingan06.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ff.hahajie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qc.wgjwhj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://id.shxzukj.cn

[J09] 时区处理
来源：http://yh.521024.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lo.asd995.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cx.hnjuh.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tm.yuntaijiaju.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cs.szxytkj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lb.haigaiapp.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://se.shxzskj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qw.shtwfgs.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lu.hahajie.cn

[J10] 取今天 / 本月第一天
来源：http://ii.newstarts.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://hy.colortex.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qp.hnjuh.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wc.jctech888.com.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://oy.hahajie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nv.gzmigu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kb.jctech888.com.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://et.shxzskj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cl.521024.cn

================================================================================
来源：http://rs.colortex.cn

K. JSON 与序列化
来源：http://dr.nicolike.cn

================================================================================
来源：http://ba.panjiajie.cn

[K01] 对象转 JSON 字符串
来源：http://ux.jctech888.com.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fz.newstarts.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ua.lnxyls.cn

JS:   JSON.stringify(obj)
来源：http://lt.wgjwhj.cn

TS:   JSON.stringify(obj)
来源：http://nb.jianghongdianzi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xq.lnxyls.cn

Go:   json.Marshal(obj)
来源：http://jo.hnjuh.cn

Ruby: obj.to_json                                     // require "json"
来源：http://bp.huanxung.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://kr.hnjuh.cn

[K02] JSON 字符串转对象
来源：http://oo.wgjwhj.cn

Py:   json.loads(s)
来源：http://ro.newstarts.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vw.jianghongdianzi.cn

JS:   JSON.parse(s)
来源：http://fi.huixinmuqiang.cn

TS:   JSON.parse(s)
来源：http://yp.shxzskj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://uz.newstarts.cn

Go:   json.Unmarshal(data, &v)
来源：http://dv.huanxung.cn

Ruby: JSON.parse(s)
来源：http://yd.shxzskj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xu.gzmigu.cn

[K03] JSON 美化输出（带缩进）
来源：http://mj.huanxung.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lz.nszjky.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cu.colortex.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://sw.shxzskj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://re.yuexingan06.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xo.lnxyls.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vp.asd995.cn


<!-- 参考信息 -->