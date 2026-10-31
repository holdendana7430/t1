代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://vc.yuntaijiaju.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://md.wgjwhj.cn

[G16] 对象转数组 / 字典
来源：http://pd.haigaiapp.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://st.yuntaijiaju.cn

PHP:  get_object_vars($obj);
来源：http://qx.hahajie.cn

JS:   Object.entries(obj)
来源：http://cb.huixiangedu.cn

TS:   Object.entries(obj)
来源：http://kp.colortex.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qh.shxzukj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ey.szsharing.cn

Ruby: obj.instance_variables
来源：http://zk.hnjuh.cn

C#:   // 用反射或 System.Text.Json
来源：http://cs.szxytkj.cn

================================================================================
来源：http://aq.521024.cn

H. 异常与错误处理
来源：http://mp.shxzukj.cn

================================================================================
来源：http://ga.521024.cn

[H01] try / catch 基础
来源：http://li.haigaiapp.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hl.nicolike.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ze.nicolike.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tm.huanxung.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qk.hnjuh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://da.yuntaijiaju.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vs.szsharing.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ug.9csxet.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ic.shxzukj.cn

[H02] finally / ensure 收尾
来源：http://ts.newstarts.cn

Py:   try: f()⏎finally: cleanup()
来源：http://jj.haigaiapp.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://pa.bjjhwx.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://qa.shtwfgs.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://cm.bjjhwx.cn

Java: try { f(); } finally { cleanup(); }
来源：http://gi.szxytkj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://or.9csxet.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://jp.shxzskj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://iv.nszjky.cn

[H03] 主动抛出异常
来源：http://co.shtwfgs.cn

Py:   raise ValueError("错误信息")
来源：http://gd.haigaiapp.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dl.chemitech.net.cn

JS:   throw new Error("错误信息");
来源：http://se.nszjky.cn

TS:   throw new Error("错误信息");
来源：http://ru.colortex.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://hc.asd995.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qi.nicolike.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ru.yuexingan06.cn

C#:   throw new ArgumentException("错误信息");
来源：http://fg.newstarts.cn

[H04] 自定义异常类型
来源：http://wv.yuntaijiaju.cn

Py:   class MyError(Exception): pass
来源：http://ms.shxzukj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://vd.jianghongdianzi.cn

JS:   class MyError extends Error {}
来源：http://ye.huanxung.cn

TS:   class MyError extends Error {}
来源：http://kf.asd995.cn

Java: class MyException extends RuntimeException {}
来源：http://rr.haigaiapp.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://er.bjjhwx.cn

Ruby: class MyError < StandardError; end
来源：http://im.lnxyls.cn

C#:   class MyException : Exception {}
来源：http://fe.colortex.cn

[H05] 捕获特定类型
来源：http://ta.jianghongdianzi.cn

Py:   except ValueError as e:
来源：http://mm.shtwfgs.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rd.nicolike.cn

JS:   if (e instanceof TypeError) {}
来源：http://jw.huixinmuqiang.cn

TS:   if (e instanceof TypeError) {}
来源：http://jn.hahajie.cn

Java: catch (IOException | SQLException e) {}
来源：http://tm.bjjhwx.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://on.nszjky.cn

Ruby: rescue ArgumentError => e
来源：http://vb.chemitech.net.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bd.hnjuh.cn

[H06] 可选值 / 空值安全访问
来源：http://sv.yuntaijiaju.cn

Py:   value = d.get("k") or default
来源：http://fa.bjjhwx.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rm.lnxyls.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ls.jctech888.com.cn

TS:   obj?.a?.b;  d ?? default
来源：http://wa.bookmarksfly.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://up.szsharing.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ft.9csxet.cn

Ruby: d&.dig(:a, :b)
来源：http://yn.hahajie.cn

C#:   obj?.A?.B ?? default
来源：http://ul.yuntaijiaju.cn

[H07] 断言
来源：http://sd.chemitech.net.cn

Py:   assert x > 0, "必须为正"
来源：http://il.szsharing.cn

PHP:  assert($x > 0);
来源：http://qj.jctech888.com.cn

JS:   console.assert(x > 0);
来源：http://qt.shxzukj.cn

TS:   console.assert(x > 0);
来源：http://eq.haigaiapp.cn

Java: assert x > 0 : "必须为正";
来源：http://xk.colortex.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://am.szsharing.cn

Ruby: raise "必须为正" unless x > 0
来源：http://kd.wgjwhj.cn

C#:   Debug.Assert(x > 0);
来源：http://hf.szxytkj.cn

[H08] 获取错误信息与堆栈
来源：http://sk.huixiangedu.cn

Py:   str(e);  traceback.format_exc()
来源：http://bc.nicolike.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kf.nszjky.cn

JS:   e.message;  e.stack
来源：http://id.shxzskj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://hm.huixiangedu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://xw.hnjuh.cn

Go:   err.Error()
来源：http://sn.shxzskj.cn

Ruby: e.message;  e.backtrace
来源：http://cs.szsharing.cn

C#:   e.Message;  e.StackTrace
来源：http://zv.jianghongdianzi.cn

[H09] 带错误码的异常
来源：http://xa.bjjhwx.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://es.asd995.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://dx.huanxung.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://es.haigaiapp.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dm.shxzskj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tu.colortex.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vh.shxzukj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://es.521024.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://fn.huanxung.cn

[H10] 资源自动释放
来源：http://em.szxytkj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://rx.yuexingan06.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://he.newstarts.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ij.panjiajie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ad.jctech888.com.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ro.shtwfgs.cn

Go:   defer f.Close()
来源：http://sk.hahajie.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hr.shxzukj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wj.shxzskj.cn

================================================================================
来源：http://bx.yuexingan06.cn

I. 正则表达式
来源：http://da.muxihuayi.cn

================================================================================
来源：http://jn.huixinmuqiang.cn

[I01] 判断是否匹配
来源：http://rj.colortex.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mb.shxzskj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://nk.haigaiapp.cn

JS:   /\d+/.test(s)
来源：http://pr.hahajie.cn

TS:   /\d+/.test(s)
来源：http://nv.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://as.jctech888.com.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tw.hnjuh.cn

Ruby: s.match?(/\d+/)
来源：http://xy.gzmigu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ku.gzmigu.cn

[I02] 提取所有匹配
来源：http://nt.colortex.cn

Py:   re.findall(r"\d+", s)
来源：http://jl.huixinmuqiang.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ih.panjiajie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ym.newstarts.cn

TS:   s.match(/\d+/g)
来源：http://av.hnjuh.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wd.huixinmuqiang.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xk.huixiangedu.cn

Ruby: s.scan(/\d+/)
来源：http://vk.wgjwhj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bq.bjjhwx.cn

[I03] 提取捕获分组
来源：http://aw.chemitech.net.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rm.szsharing.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ga.szsharing.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://du.bookmarksfly.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kh.colortex.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://op.muxihuayi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://iy.yuntaijiaju.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ar.nszjky.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bi.lnxyls.cn

[I04] 正则替换
来源：http://zk.bookmarksfly.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://sk.hahajie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ha.nicolike.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ad.gzmigu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://pu.chemitech.net.cn

Java: s.replaceAll("\\d+", "#")
来源：http://pk.jctech888.com.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://fq.hnjuh.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://uc.gzmigu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qw.haigaiapp.cn

[I05] 按正则拆分
来源：http://ff.haigaiapp.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ax.bookmarksfly.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://sl.jianghongdianzi.cn

JS:   s.split(/\s*,\s*/)
来源：http://em.huixiangedu.cn

TS:   s.split(/\s*,\s*/)
来源：http://ov.muxihuayi.cn

Java: s.split("\\s*,\\s*")
来源：http://yf.shxzskj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://aa.nszjky.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bk.wgjwhj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://od.newstarts.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ag.szxytkj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mf.szsharing.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jz.chemitech.net.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dj.yuexingan06.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sv.haigaiapp.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yk.shxzukj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tk.asd995.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jy.muxihuayi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ju.gzmigu.cn

[I07] 忽略大小写与多行模式
来源：http://zb.hnjuh.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zu.hnjuh.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lk.panjiajie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ri.yuntaijiaju.cn

TS:   /error/gim
来源：http://ga.colortex.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ob.shxzskj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ej.gzmigu.cn

Ruby: s.scan(/error/i)
来源：http://pb.hnjuh.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sc.shtwfgs.cn

[I08] 贪婪与非贪婪匹配
来源：http://qj.huixiangedu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tp.hnjuh.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pl.shxzskj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://we.yuntaijiaju.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hm.shxzukj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://tp.yuntaijiaju.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lm.521024.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ds.jctech888.com.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qw.gzmigu.cn

================================================================================
来源：http://zj.9csxet.cn

J. 日期与时间
来源：http://ky.szsharing.cn

================================================================================
来源：http://pa.huanxung.cn

[J01] 获取当前时间
来源：http://fu.newstarts.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://pj.gzmigu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fx.huixinmuqiang.cn

JS:   new Date();  Date.now()
来源：http://ht.huanxung.cn

TS:   new Date();  Date.now()
来源：http://gk.lnxyls.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vl.nicolike.cn

Go:   time.Now()
来源：http://yr.muxihuayi.cn

Ruby: Time.now
来源：http://jk.nszjky.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lx.yuntaijiaju.cn

[J02] 格式化输出
来源：http://mp.wgjwhj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yb.shxzskj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jr.shxzskj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ti.shtwfgs.cn

TS:   d.toISOString()
来源：http://lr.huixinmuqiang.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://is.yuntaijiaju.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lj.huixinmuqiang.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ye.bjjhwx.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mg.shtwfgs.cn

[J03] 字符串解析为日期
来源：http://th.shxzukj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ws.colortex.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uw.bookmarksfly.cn

JS:   new Date("2024-01-02")
来源：http://hh.521024.cn

TS:   new Date("2024-01-02")
来源：http://wl.lnxyls.cn

Java: LocalDate.parse("2024-01-02")
来源：http://bo.panjiajie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bp.lnxyls.cn

Ruby: Date.parse("2024-01-02")
来源：http://tk.huanxung.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nu.newstarts.cn

[J04] 时间戳与日期互转
来源：http://ry.huanxung.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://md.shtwfgs.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://og.asd995.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://am.muxihuayi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://iz.9csxet.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://iu.muxihuayi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bh.panjiajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://en.nszjky.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vy.shtwfgs.cn

[J05] 时间加减（加 7 天）
来源：http://om.9csxet.cn

Py:   now + timedelta(days=7)
来源：http://af.hnjuh.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vj.hnjuh.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ie.hnjuh.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hn.9csxet.cn

Java: LocalDate.now().plusDays(7)
来源：http://lm.haigaiapp.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ek.jianghongdianzi.cn

Ruby: Time.now + 7 * 86400
来源：http://zg.muxihuayi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://le.lnxyls.cn

[J06] 计算两时间之差
来源：http://mv.jctech888.com.cn

Py:   (end - start).total_seconds()
来源：http://fj.jctech888.com.cn

PHP:  $end->diff($start)->days;
来源：http://xp.shxzukj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ti.bookmarksfly.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cb.shtwfgs.cn

Java: Duration.between(start, end).toSeconds()
来源：http://oa.colortex.cn

Go:   end.Sub(start).Hours()
来源：http://ko.colortex.cn

Ruby: end - start                 # 返回秒数
来源：http://nb.yuexingan06.cn

C#:   (end - start).TotalSeconds
来源：http://as.jianghongdianzi.cn

[J07] 比较两个日期
来源：http://qi.nszjky.cn

Py:   d1 < d2;  d1 == d2
来源：http://sl.gzmigu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://at.jianghongdianzi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://rh.muxihuayi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://zh.huixinmuqiang.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qk.jctech888.com.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cu.shxzskj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://py.521024.cn

C#:   d1 < d2;  d1 == d2
来源：http://uc.jianghongdianzi.cn

[J08] 提取年月日与星期
来源：http://qr.9csxet.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wv.nszjky.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cn.lnxyls.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ui.huixiangedu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cd.szsharing.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nx.bookmarksfly.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tb.jctech888.com.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wv.shtwfgs.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://em.panjiajie.cn

[J09] 时区处理
来源：http://fg.colortex.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://eh.huixinmuqiang.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pe.yuexingan06.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lx.yuexingan06.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mf.hahajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://il.yuntaijiaju.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gl.jianghongdianzi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://jo.asd995.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://np.panjiajie.cn

[J10] 取今天 / 本月第一天
来源：http://hx.muxihuayi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://eu.521024.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yz.colortex.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xh.bookmarksfly.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wy.newstarts.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vc.wgjwhj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qo.lnxyls.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vn.haigaiapp.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rd.gzmigu.cn

================================================================================
来源：http://pp.lnxyls.cn

K. JSON 与序列化
来源：http://su.nicolike.cn

================================================================================
来源：http://db.gzmigu.cn

[K01] 对象转 JSON 字符串
来源：http://dp.huixinmuqiang.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pr.nicolike.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yx.bookmarksfly.cn

JS:   JSON.stringify(obj)
来源：http://dw.bookmarksfly.cn

TS:   JSON.stringify(obj)
来源：http://zz.szsharing.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xi.shxzskj.cn

Go:   json.Marshal(obj)
来源：http://wc.shxzukj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://oo.asd995.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://bc.bjjhwx.cn

[K02] JSON 字符串转对象
来源：http://eo.bookmarksfly.cn

Py:   json.loads(s)
来源：http://pu.asd995.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ql.lnxyls.cn

JS:   JSON.parse(s)
来源：http://sf.shtwfgs.cn

TS:   JSON.parse(s)
来源：http://rc.asd995.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ol.newstarts.cn

Go:   json.Unmarshal(data, &v)
来源：http://cy.muxihuayi.cn

Ruby: JSON.parse(s)
来源：http://vy.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://no.gzmigu.cn

[K03] JSON 美化输出（带缩进）
来源：http://kv.hnjuh.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ke.hnjuh.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ps.szxytkj.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://tr.wgjwhj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fm.9csxet.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ll.shtwfgs.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tr.gzmigu.cn


<!-- 参考信息 -->