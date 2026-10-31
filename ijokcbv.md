代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://qd.lnxyls.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vs.szsharing.cn

[G16] 对象转数组 / 字典
来源：http://hg.chemitech.net.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dp.jianghongdianzi.cn

PHP:  get_object_vars($obj);
来源：http://wz.jianghongdianzi.cn

JS:   Object.entries(obj)
来源：http://co.yuexingan06.cn

TS:   Object.entries(obj)
来源：http://bf.nicolike.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fo.gzmigu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://wr.shxzskj.cn

Ruby: obj.instance_variables
来源：http://pg.colortex.cn

C#:   // 用反射或 System.Text.Json
来源：http://kz.yuexingan06.cn

================================================================================
来源：http://pf.hahajie.cn

H. 异常与错误处理
来源：http://zp.shxzskj.cn

================================================================================
来源：http://ek.yuexingan06.cn

[H01] try / catch 基础
来源：http://zw.bookmarksfly.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qn.yuexingan06.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ns.newstarts.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ap.szxytkj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fm.szxytkj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://il.huanxung.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://di.bjjhwx.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xa.newstarts.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ea.colortex.cn

[H02] finally / ensure 收尾
来源：http://jx.gzmigu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ne.lnxyls.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://in.huanxung.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hk.huixinmuqiang.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://yt.yuntaijiaju.cn

Java: try { f(); } finally { cleanup(); }
来源：http://cs.hahajie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ed.szxytkj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wa.shxzskj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://po.muxihuayi.cn

[H03] 主动抛出异常
来源：http://nw.asd995.cn

Py:   raise ValueError("错误信息")
来源：http://ga.chemitech.net.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ew.muxihuayi.cn

JS:   throw new Error("错误信息");
来源：http://kb.jctech888.com.cn

TS:   throw new Error("错误信息");
来源：http://rq.colortex.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://oz.shxzukj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mk.colortex.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ze.nicolike.cn

C#:   throw new ArgumentException("错误信息");
来源：http://sl.nszjky.cn

[H04] 自定义异常类型
来源：http://gb.huanxung.cn

Py:   class MyError(Exception): pass
来源：http://hr.nicolike.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ms.bjjhwx.cn

JS:   class MyError extends Error {}
来源：http://ge.panjiajie.cn

TS:   class MyError extends Error {}
来源：http://zh.newstarts.cn

Java: class MyException extends RuntimeException {}
来源：http://ap.nszjky.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yw.bjjhwx.cn

Ruby: class MyError < StandardError; end
来源：http://ki.lnxyls.cn

C#:   class MyException : Exception {}
来源：http://im.gzmigu.cn

[H05] 捕获特定类型
来源：http://ks.bjjhwx.cn

Py:   except ValueError as e:
来源：http://kz.yuntaijiaju.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yw.newstarts.cn

JS:   if (e instanceof TypeError) {}
来源：http://hv.shxzukj.cn

TS:   if (e instanceof TypeError) {}
来源：http://yz.yuexingan06.cn

Java: catch (IOException | SQLException e) {}
来源：http://eu.jianghongdianzi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ms.huixiangedu.cn

Ruby: rescue ArgumentError => e
来源：http://md.shxzukj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bi.lnxyls.cn

[H06] 可选值 / 空值安全访问
来源：http://oy.9csxet.cn

Py:   value = d.get("k") or default
来源：http://ty.yuexingan06.cn

PHP:  $v = $d["k"] ?? null;
来源：http://pu.hahajie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://zn.lnxyls.cn

TS:   obj?.a?.b;  d ?? default
来源：http://av.jctech888.com.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tz.shxzukj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://md.yuexingan06.cn

Ruby: d&.dig(:a, :b)
来源：http://hu.yuexingan06.cn

C#:   obj?.A?.B ?? default
来源：http://ew.lnxyls.cn

[H07] 断言
来源：http://of.jctech888.com.cn

Py:   assert x > 0, "必须为正"
来源：http://bg.huanxung.cn

PHP:  assert($x > 0);
来源：http://rw.shtwfgs.cn

JS:   console.assert(x > 0);
来源：http://mi.szxytkj.cn

TS:   console.assert(x > 0);
来源：http://kw.lnxyls.cn

Java: assert x > 0 : "必须为正";
来源：http://xw.haigaiapp.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vs.newstarts.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ai.colortex.cn

C#:   Debug.Assert(x > 0);
来源：http://fz.szxytkj.cn

[H08] 获取错误信息与堆栈
来源：http://zl.huixiangedu.cn

Py:   str(e);  traceback.format_exc()
来源：http://xx.newstarts.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qh.bjjhwx.cn

JS:   e.message;  e.stack
来源：http://mt.shxzukj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://tg.panjiajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://qf.521024.cn

Go:   err.Error()
来源：http://tv.jctech888.com.cn

Ruby: e.message;  e.backtrace
来源：http://in.haigaiapp.cn

C#:   e.Message;  e.StackTrace
来源：http://at.hahajie.cn

[H09] 带错误码的异常
来源：http://uq.muxihuayi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cg.lnxyls.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://lr.szxytkj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vv.wgjwhj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rl.szxytkj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mc.yuexingan06.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kj.9csxet.cn

Ruby: raise MyError.new("fail", 500)
来源：http://bl.szsharing.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://gc.panjiajie.cn

[H10] 资源自动释放
来源：http://us.newstarts.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ft.nszjky.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cn.haigaiapp.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ro.yuntaijiaju.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://if.muxihuayi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jw.huixinmuqiang.cn

Go:   defer f.Close()
来源：http://wj.521024.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://af.newstarts.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bv.nszjky.cn

================================================================================
来源：http://ka.jianghongdianzi.cn

I. 正则表达式
来源：http://iv.yuexingan06.cn

================================================================================
来源：http://et.9csxet.cn

[I01] 判断是否匹配
来源：http://sv.bookmarksfly.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zd.gzmigu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fq.521024.cn

JS:   /\d+/.test(s)
来源：http://hc.bookmarksfly.cn

TS:   /\d+/.test(s)
来源：http://sc.jctech888.com.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zu.wgjwhj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mk.newstarts.cn

Ruby: s.match?(/\d+/)
来源：http://sq.panjiajie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lg.muxihuayi.cn

[I02] 提取所有匹配
来源：http://vp.bookmarksfly.cn

Py:   re.findall(r"\d+", s)
来源：http://bv.shxzskj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://iu.panjiajie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qq.jctech888.com.cn

TS:   s.match(/\d+/g)
来源：http://ms.nszjky.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qm.panjiajie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rz.panjiajie.cn

Ruby: s.scan(/\d+/)
来源：http://qu.huixiangedu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ty.shxzukj.cn

[I03] 提取捕获分组
来源：http://co.yuntaijiaju.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zu.shxzskj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bm.yuexingan06.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://oy.chemitech.net.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bj.hnjuh.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rq.huixiangedu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dv.colortex.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rt.szxytkj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kq.lnxyls.cn

[I04] 正则替换
来源：http://sr.asd995.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://if.jctech888.com.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ji.jctech888.com.cn

JS:   s.replace(/\d+/g, "#")
来源：http://tv.wgjwhj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://lk.newstarts.cn

Java: s.replaceAll("\\d+", "#")
来源：http://se.nicolike.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://zz.gzmigu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ke.asd995.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gm.yuexingan06.cn

[I05] 按正则拆分
来源：http://vk.nszjky.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://sg.szxytkj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bq.nicolike.cn

JS:   s.split(/\s*,\s*/)
来源：http://nd.hnjuh.cn

TS:   s.split(/\s*,\s*/)
来源：http://yt.colortex.cn

Java: s.split("\\s*,\\s*")
来源：http://nv.panjiajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://li.yuntaijiaju.cn

Ruby: s.split(/\s*,\s*/)
来源：http://rt.haigaiapp.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xy.lnxyls.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vk.gzmigu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xv.yuntaijiaju.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bg.9csxet.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hc.asd995.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yn.haigaiapp.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://or.jianghongdianzi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cz.lnxyls.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pi.huanxung.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lw.shxzskj.cn

[I07] 忽略大小写与多行模式
来源：http://nk.521024.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ij.muxihuayi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dk.colortex.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://oe.bjjhwx.cn

TS:   /error/gim
来源：http://ac.nicolike.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ae.hahajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jv.bookmarksfly.cn

Ruby: s.scan(/error/i)
来源：http://zk.hnjuh.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zy.chemitech.net.cn

[I08] 贪婪与非贪婪匹配
来源：http://bv.muxihuayi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://uu.szxytkj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vf.hahajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bk.hahajie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ep.colortex.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ow.haigaiapp.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ln.muxihuayi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ws.jctech888.com.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fs.szxytkj.cn

================================================================================
来源：http://xg.haigaiapp.cn

J. 日期与时间
来源：http://ew.newstarts.cn

================================================================================
来源：http://ej.gzmigu.cn

[J01] 获取当前时间
来源：http://qa.colortex.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wf.jianghongdianzi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nx.hnjuh.cn

JS:   new Date();  Date.now()
来源：http://tp.huixiangedu.cn

TS:   new Date();  Date.now()
来源：http://or.panjiajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ru.hahajie.cn

Go:   time.Now()
来源：http://ap.jianghongdianzi.cn

Ruby: Time.now
来源：http://gf.shxzskj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://py.yuexingan06.cn

[J02] 格式化输出
来源：http://rm.hnjuh.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hm.gzmigu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fu.haigaiapp.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gi.9csxet.cn

TS:   d.toISOString()
来源：http://pn.521024.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xm.bookmarksfly.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ch.bookmarksfly.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fa.shxzskj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ll.gzmigu.cn

[J03] 字符串解析为日期
来源：http://um.muxihuayi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hg.nszjky.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ca.colortex.cn

JS:   new Date("2024-01-02")
来源：http://wc.hahajie.cn

TS:   new Date("2024-01-02")
来源：http://lq.szsharing.cn

Java: LocalDate.parse("2024-01-02")
来源：http://rh.bjjhwx.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kp.huixiangedu.cn

Ruby: Date.parse("2024-01-02")
来源：http://ry.chemitech.net.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://js.huanxung.cn

[J04] 时间戳与日期互转
来源：http://nw.shxzskj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lm.9csxet.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lw.muxihuayi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bx.huixiangedu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ux.colortex.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mj.bjjhwx.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ic.huixinmuqiang.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cf.nicolike.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yw.jianghongdianzi.cn

[J05] 时间加减（加 7 天）
来源：http://rg.lnxyls.cn

Py:   now + timedelta(days=7)
来源：http://tr.hnjuh.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xz.lnxyls.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dw.521024.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xs.newstarts.cn

Java: LocalDate.now().plusDays(7)
来源：http://gk.hnjuh.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://oi.shxzskj.cn

Ruby: Time.now + 7 * 86400
来源：http://qb.huanxung.cn

C#:   DateTime.Now.AddDays(7)
来源：http://tk.szxytkj.cn

[J06] 计算两时间之差
来源：http://wf.haigaiapp.cn

Py:   (end - start).total_seconds()
来源：http://oo.hnjuh.cn

PHP:  $end->diff($start)->days;
来源：http://to.9csxet.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ct.hnjuh.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yn.nszjky.cn

Java: Duration.between(start, end).toSeconds()
来源：http://is.huanxung.cn

Go:   end.Sub(start).Hours()
来源：http://lg.newstarts.cn

Ruby: end - start                 # 返回秒数
来源：http://qh.9csxet.cn

C#:   (end - start).TotalSeconds
来源：http://ns.nszjky.cn

[J07] 比较两个日期
来源：http://ld.panjiajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://ya.wgjwhj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://uz.gzmigu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xy.nszjky.cn

TS:   d1.getTime() < d2.getTime()
来源：http://pr.shxzskj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://sk.hahajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zi.lnxyls.cn

Ruby: d1 < d2;  d1 == d2
来源：http://tj.yuntaijiaju.cn

C#:   d1 < d2;  d1 == d2
来源：http://ag.nicolike.cn

[J08] 提取年月日与星期
来源：http://ld.hahajie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://uo.haigaiapp.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ba.haigaiapp.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xr.lnxyls.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yc.nszjky.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tm.haigaiapp.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tj.szxytkj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sd.colortex.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vk.jctech888.com.cn

[J09] 时区处理
来源：http://pb.hnjuh.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://by.szxytkj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rv.newstarts.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://is.bjjhwx.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vb.huixiangedu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kd.nszjky.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://va.szsharing.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cb.wgjwhj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kh.bjjhwx.cn

[J10] 取今天 / 本月第一天
来源：http://ge.shxzukj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ks.nicolike.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://np.jctech888.com.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wa.shxzukj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wo.bjjhwx.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kl.huixiangedu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mm.chemitech.net.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qw.colortex.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bf.bjjhwx.cn

================================================================================
来源：http://vp.newstarts.cn

K. JSON 与序列化
来源：http://ge.shxzukj.cn

================================================================================
来源：http://tn.gzmigu.cn

[K01] 对象转 JSON 字符串
来源：http://pb.521024.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ee.szsharing.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wy.szxytkj.cn

JS:   JSON.stringify(obj)
来源：http://ic.chemitech.net.cn

TS:   JSON.stringify(obj)
来源：http://bl.newstarts.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://de.nicolike.cn

Go:   json.Marshal(obj)
来源：http://qh.bjjhwx.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ye.newstarts.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ru.9csxet.cn

[K02] JSON 字符串转对象
来源：http://uf.jctech888.com.cn

Py:   json.loads(s)
来源：http://wa.huixinmuqiang.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ha.haigaiapp.cn

JS:   JSON.parse(s)
来源：http://qj.nszjky.cn

TS:   JSON.parse(s)
来源：http://pd.szsharing.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yc.nszjky.cn

Go:   json.Unmarshal(data, &v)
来源：http://eu.521024.cn

Ruby: JSON.parse(s)
来源：http://mz.szsharing.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tf.shtwfgs.cn

[K03] JSON 美化输出（带缩进）
来源：http://li.huixinmuqiang.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://um.nicolike.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://el.huixiangedu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://yj.newstarts.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vb.huixinmuqiang.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ga.shtwfgs.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hs.jianghongdianzi.cn


<!-- 参考信息 -->