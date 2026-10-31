代发 wailian999

PHP:  get_object_vars($obj);
来源：http://yw.hnjuh.cn

JS:   Object.entries(obj)
来源：http://sq.nszjky.cn

TS:   Object.entries(obj)
来源：http://hi.newstarts.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ft.jianghongdianzi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://mi.hahajie.cn

Ruby: obj.instance_variables
来源：http://fz.nicolike.cn

C#:   // 用反射或 System.Text.Json
来源：http://jr.lnxyls.cn

================================================================================
来源：http://oc.lnxyls.cn

H. 异常与错误处理
来源：http://kb.newstarts.cn

================================================================================
来源：http://uo.shxzukj.cn

[H01] try / catch 基础
来源：http://hg.gzmigu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yw.haigaiapp.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yh.nszjky.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bf.nszjky.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rg.hnjuh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mb.yuntaijiaju.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sb.chemitech.net.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ec.shxzukj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vn.bjjhwx.cn

[H02] finally / ensure 收尾
来源：http://do.hnjuh.cn

Py:   try: f()⏎finally: cleanup()
来源：http://nj.shxzskj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://la.yuntaijiaju.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://cj.colortex.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qh.shtwfgs.cn

Java: try { f(); } finally { cleanup(); }
来源：http://kc.shxzskj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://do.szsharing.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://jl.yuntaijiaju.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://in.muxihuayi.cn

[H03] 主动抛出异常
来源：http://vq.9csxet.cn

Py:   raise ValueError("错误信息")
来源：http://mp.huixiangedu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yl.jctech888.com.cn

JS:   throw new Error("错误信息");
来源：http://fi.lnxyls.cn

TS:   throw new Error("错误信息");
来源：http://yk.nicolike.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://kl.521024.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fb.hnjuh.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://yi.bjjhwx.cn

C#:   throw new ArgumentException("错误信息");
来源：http://yt.muxihuayi.cn

[H04] 自定义异常类型
来源：http://ai.jianghongdianzi.cn

Py:   class MyError(Exception): pass
来源：http://yd.jianghongdianzi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://so.shtwfgs.cn

JS:   class MyError extends Error {}
来源：http://pz.asd995.cn

TS:   class MyError extends Error {}
来源：http://cf.9csxet.cn

Java: class MyException extends RuntimeException {}
来源：http://xd.szsharing.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qi.gzmigu.cn

Ruby: class MyError < StandardError; end
来源：http://es.huixiangedu.cn

C#:   class MyException : Exception {}
来源：http://dn.szsharing.cn

[H05] 捕获特定类型
来源：http://og.chemitech.net.cn

Py:   except ValueError as e:
来源：http://sy.szsharing.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ap.shxzukj.cn

JS:   if (e instanceof TypeError) {}
来源：http://rw.yuntaijiaju.cn

TS:   if (e instanceof TypeError) {}
来源：http://qy.szxytkj.cn

Java: catch (IOException | SQLException e) {}
来源：http://df.huixinmuqiang.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ew.shxzukj.cn

Ruby: rescue ArgumentError => e
来源：http://mc.jianghongdianzi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bg.bookmarksfly.cn

[H06] 可选值 / 空值安全访问
来源：http://fm.wgjwhj.cn

Py:   value = d.get("k") or default
来源：http://mi.bookmarksfly.cn

PHP:  $v = $d["k"] ?? null;
来源：http://nt.bjjhwx.cn

JS:   obj?.a?.b;  d ?? default
来源：http://xn.yuntaijiaju.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ht.huanxung.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ss.hahajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ne.lnxyls.cn

Ruby: d&.dig(:a, :b)
来源：http://ci.bjjhwx.cn

C#:   obj?.A?.B ?? default
来源：http://ty.hahajie.cn

[H07] 断言
来源：http://qt.nicolike.cn

Py:   assert x > 0, "必须为正"
来源：http://aw.nicolike.cn

PHP:  assert($x > 0);
来源：http://yf.shxzskj.cn

JS:   console.assert(x > 0);
来源：http://lt.jctech888.com.cn

TS:   console.assert(x > 0);
来源：http://db.shxzukj.cn

Java: assert x > 0 : "必须为正";
来源：http://un.lnxyls.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sv.hnjuh.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ih.wgjwhj.cn

C#:   Debug.Assert(x > 0);
来源：http://jk.chemitech.net.cn

[H08] 获取错误信息与堆栈
来源：http://sa.bookmarksfly.cn

Py:   str(e);  traceback.format_exc()
来源：http://yg.wgjwhj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xk.521024.cn

JS:   e.message;  e.stack
来源：http://vp.bookmarksfly.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://og.yuntaijiaju.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://fq.panjiajie.cn

Go:   err.Error()
来源：http://pc.jianghongdianzi.cn

Ruby: e.message;  e.backtrace
来源：http://rr.bookmarksfly.cn

C#:   e.Message;  e.StackTrace
来源：http://ey.nszjky.cn

[H09] 带错误码的异常
来源：http://sv.yuntaijiaju.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yh.huixiangedu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://fa.muxihuayi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wn.nicolike.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yd.yuexingan06.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tv.huanxung.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gv.nszjky.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ec.yuntaijiaju.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://dz.huixiangedu.cn

[H10] 资源自动释放
来源：http://lm.hahajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ec.521024.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gf.huixinmuqiang.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ar.szsharing.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bw.hnjuh.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qh.lnxyls.cn

Go:   defer f.Close()
来源：http://il.nicolike.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rc.szsharing.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://oz.asd995.cn

================================================================================
来源：http://jn.szsharing.cn

I. 正则表达式
来源：http://cd.yuntaijiaju.cn

================================================================================
来源：http://iv.wgjwhj.cn

[I01] 判断是否匹配
来源：http://so.521024.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wm.newstarts.cn

PHP:  preg_match('/\d+/', $s);
来源：http://dk.haigaiapp.cn

JS:   /\d+/.test(s)
来源：http://uh.yuntaijiaju.cn

TS:   /\d+/.test(s)
来源：http://fz.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jv.yuexingan06.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cs.nszjky.cn

Ruby: s.match?(/\d+/)
来源：http://kd.wgjwhj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hy.colortex.cn

[I02] 提取所有匹配
来源：http://qc.nszjky.cn

Py:   re.findall(r"\d+", s)
来源：http://pp.521024.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ef.hnjuh.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zk.shxzskj.cn

TS:   s.match(/\d+/g)
来源：http://pe.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ys.9csxet.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zt.shxzukj.cn

Ruby: s.scan(/\d+/)
来源：http://oh.asd995.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://to.yuexingan06.cn

[I03] 提取捕获分组
来源：http://kl.yuexingan06.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mr.shxzukj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vr.shxzukj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://uh.bookmarksfly.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fh.asd995.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gz.yuexingan06.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fr.colortex.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://el.gzmigu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ck.huixiangedu.cn

[I04] 正则替换
来源：http://cf.haigaiapp.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://io.jianghongdianzi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gl.huixinmuqiang.cn

JS:   s.replace(/\d+/g, "#")
来源：http://rr.asd995.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ls.nicolike.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ra.nszjky.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://cu.nicolike.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://kj.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ci.yuexingan06.cn

[I05] 按正则拆分
来源：http://ie.nicolike.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://nz.yuntaijiaju.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nw.wgjwhj.cn

JS:   s.split(/\s*,\s*/)
来源：http://bp.521024.cn

TS:   s.split(/\s*,\s*/)
来源：http://yp.panjiajie.cn

Java: s.split("\\s*,\\s*")
来源：http://cy.9csxet.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cc.chemitech.net.cn

Ruby: s.split(/\s*,\s*/)
来源：http://gm.haigaiapp.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qf.nicolike.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yn.521024.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://td.9csxet.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vv.colortex.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://db.colortex.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qg.yuexingan06.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fj.yuntaijiaju.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xu.colortex.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vl.shtwfgs.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zo.gzmigu.cn

[I07] 忽略大小写与多行模式
来源：http://aq.shxzukj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bu.szsharing.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cr.haigaiapp.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cz.shxzukj.cn

TS:   /error/gim
来源：http://lm.jctech888.com.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ph.shxzskj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dv.colortex.cn

Ruby: s.scan(/error/i)
来源：http://mf.panjiajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mi.huixinmuqiang.cn

[I08] 贪婪与非贪婪匹配
来源：http://ad.nicolike.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zt.jctech888.com.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jn.yuexingan06.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ho.hahajie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wm.szsharing.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://cg.shxzukj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kj.yuntaijiaju.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://no.wgjwhj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ux.hahajie.cn

================================================================================
来源：http://qt.newstarts.cn

J. 日期与时间
来源：http://ic.panjiajie.cn

================================================================================
来源：http://dr.hnjuh.cn

[J01] 获取当前时间
来源：http://df.shxzskj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ze.haigaiapp.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ln.hnjuh.cn

JS:   new Date();  Date.now()
来源：http://ht.yuntaijiaju.cn

TS:   new Date();  Date.now()
来源：http://ex.hnjuh.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://lk.wgjwhj.cn

Go:   time.Now()
来源：http://tm.shtwfgs.cn

Ruby: Time.now
来源：http://io.yuexingan06.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nw.haigaiapp.cn

[J02] 格式化输出
来源：http://rg.521024.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://al.nszjky.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qm.colortex.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nx.huixinmuqiang.cn

TS:   d.toISOString()
来源：http://wg.gzmigu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gc.szxytkj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ny.szsharing.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zg.newstarts.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tx.nszjky.cn

[J03] 字符串解析为日期
来源：http://pw.gzmigu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sa.nicolike.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://db.newstarts.cn

JS:   new Date("2024-01-02")
来源：http://vx.haigaiapp.cn

TS:   new Date("2024-01-02")
来源：http://fw.yuntaijiaju.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ya.nszjky.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yo.521024.cn

Ruby: Date.parse("2024-01-02")
来源：http://nb.colortex.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uh.nicolike.cn

[J04] 时间戳与日期互转
来源：http://xr.bookmarksfly.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rg.gzmigu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://eg.yuexingan06.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dq.shxzskj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://nf.szsharing.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xk.521024.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hr.wgjwhj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xe.bjjhwx.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yq.nszjky.cn

[J05] 时间加减（加 7 天）
来源：http://my.panjiajie.cn

Py:   now + timedelta(days=7)
来源：http://ln.jctech888.com.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://qa.huixiangedu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://au.panjiajie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zn.yuexingan06.cn

Java: LocalDate.now().plusDays(7)
来源：http://zr.chemitech.net.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://us.yuexingan06.cn

Ruby: Time.now + 7 * 86400
来源：http://fw.9csxet.cn

C#:   DateTime.Now.AddDays(7)
来源：http://so.bjjhwx.cn

[J06] 计算两时间之差
来源：http://ek.szxytkj.cn

Py:   (end - start).total_seconds()
来源：http://po.nszjky.cn

PHP:  $end->diff($start)->days;
来源：http://kh.szsharing.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rv.yuexingan06.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ct.colortex.cn

Java: Duration.between(start, end).toSeconds()
来源：http://tw.bjjhwx.cn

Go:   end.Sub(start).Hours()
来源：http://wi.bjjhwx.cn

Ruby: end - start                 # 返回秒数
来源：http://vm.newstarts.cn

C#:   (end - start).TotalSeconds
来源：http://qf.nicolike.cn

[J07] 比较两个日期
来源：http://mz.szxytkj.cn

Py:   d1 < d2;  d1 == d2
来源：http://ge.muxihuayi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ne.wgjwhj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qy.yuntaijiaju.cn

TS:   d1.getTime() < d2.getTime()
来源：http://vq.huanxung.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dg.gzmigu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://iy.szsharing.cn

Ruby: d1 < d2;  d1 == d2
来源：http://tn.jianghongdianzi.cn

C#:   d1 < d2;  d1 == d2
来源：http://ew.wgjwhj.cn

[J08] 提取年月日与星期
来源：http://ob.jctech888.com.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zs.lnxyls.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qh.nicolike.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ou.szsharing.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mu.shtwfgs.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cm.jianghongdianzi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://en.hnjuh.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ba.shxzukj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pv.szsharing.cn

[J09] 时区处理
来源：http://jw.newstarts.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vh.newstarts.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gc.bjjhwx.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gm.colortex.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sq.hnjuh.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kl.huixiangedu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sj.jctech888.com.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://rv.9csxet.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ll.shxzukj.cn

[J10] 取今天 / 本月第一天
来源：http://zw.haigaiapp.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://il.521024.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ey.nszjky.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hd.jianghongdianzi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rb.lnxyls.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ey.nszjky.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ql.muxihuayi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ir.gzmigu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ap.9csxet.cn

================================================================================
来源：http://si.hahajie.cn

K. JSON 与序列化
来源：http://gm.shxzukj.cn

================================================================================
来源：http://sr.shtwfgs.cn

[K01] 对象转 JSON 字符串
来源：http://vn.bookmarksfly.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cn.hnjuh.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ua.colortex.cn

JS:   JSON.stringify(obj)
来源：http://qw.9csxet.cn

TS:   JSON.stringify(obj)
来源：http://bb.huanxung.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://av.szsharing.cn

Go:   json.Marshal(obj)
来源：http://zq.muxihuayi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://dw.huixinmuqiang.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://yo.shxzukj.cn

[K02] JSON 字符串转对象
来源：http://ug.521024.cn

Py:   json.loads(s)
来源：http://sp.huixiangedu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qg.9csxet.cn

JS:   JSON.parse(s)
来源：http://ib.yuexingan06.cn

TS:   JSON.parse(s)
来源：http://ih.huixiangedu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fc.huixinmuqiang.cn

Go:   json.Unmarshal(data, &v)
来源：http://sj.jctech888.com.cn

Ruby: JSON.parse(s)
来源：http://vt.yuntaijiaju.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zi.jianghongdianzi.cn

[K03] JSON 美化输出（带缩进）
来源：http://tk.huixiangedu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jv.jianghongdianzi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mg.colortex.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://nd.colortex.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://mt.shxzskj.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fl.yuntaijiaju.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sk.shxzukj.cn

Ruby: JSON.pretty_generate(obj)
来源：http://si.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ik.jianghongdianzi.cn

[K04] 读取 JSON 文件
来源：http://at.521024.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hq.nicolike.cn


<!-- 参考信息 -->