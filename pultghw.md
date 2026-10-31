代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://wu.bookmarksfly.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cu.huixinmuqiang.cn

[G16] 对象转数组 / 字典
来源：http://dv.szsharing.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pp.bookmarksfly.cn

PHP:  get_object_vars($obj);
来源：http://ow.lnxyls.cn

JS:   Object.entries(obj)
来源：http://as.panjiajie.cn

TS:   Object.entries(obj)
来源：http://xc.lnxyls.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cj.hahajie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://dx.bookmarksfly.cn

Ruby: obj.instance_variables
来源：http://xs.colortex.cn

C#:   // 用反射或 System.Text.Json
来源：http://gj.nszjky.cn

================================================================================
来源：http://rd.shtwfgs.cn

H. 异常与错误处理
来源：http://vp.hahajie.cn

================================================================================
来源：http://ug.huanxung.cn

[H01] try / catch 基础
来源：http://pc.jianghongdianzi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bk.yuntaijiaju.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ri.colortex.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://af.nicolike.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bt.hnjuh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xl.panjiajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vd.521024.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ba.9csxet.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lg.shtwfgs.cn

[H02] finally / ensure 收尾
来源：http://ym.bjjhwx.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ul.bookmarksfly.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://dz.shtwfgs.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ws.wgjwhj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://dr.nicolike.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ep.nicolike.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://jx.bookmarksfly.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://mg.newstarts.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://wo.asd995.cn

[H03] 主动抛出异常
来源：http://xa.chemitech.net.cn

Py:   raise ValueError("错误信息")
来源：http://if.jianghongdianzi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dv.szxytkj.cn

JS:   throw new Error("错误信息");
来源：http://vr.huixinmuqiang.cn

TS:   throw new Error("错误信息");
来源：http://um.nicolike.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ks.yuexingan06.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dk.szxytkj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wi.asd995.cn

C#:   throw new ArgumentException("错误信息");
来源：http://jj.shxzskj.cn

[H04] 自定义异常类型
来源：http://oh.huanxung.cn

Py:   class MyError(Exception): pass
来源：http://hr.hahajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://hi.huixinmuqiang.cn

JS:   class MyError extends Error {}
来源：http://hj.panjiajie.cn

TS:   class MyError extends Error {}
来源：http://xf.wgjwhj.cn

Java: class MyException extends RuntimeException {}
来源：http://ey.colortex.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hr.huanxung.cn

Ruby: class MyError < StandardError; end
来源：http://pi.panjiajie.cn

C#:   class MyException : Exception {}
来源：http://vq.newstarts.cn

[H05] 捕获特定类型
来源：http://rz.chemitech.net.cn

Py:   except ValueError as e:
来源：http://rj.huanxung.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zs.huanxung.cn

JS:   if (e instanceof TypeError) {}
来源：http://ob.bjjhwx.cn

TS:   if (e instanceof TypeError) {}
来源：http://ku.9csxet.cn

Java: catch (IOException | SQLException e) {}
来源：http://pw.hnjuh.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://io.chemitech.net.cn

Ruby: rescue ArgumentError => e
来源：http://dj.hnjuh.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bj.hnjuh.cn

[H06] 可选值 / 空值安全访问
来源：http://zu.bjjhwx.cn

Py:   value = d.get("k") or default
来源：http://fr.nicolike.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ka.colortex.cn

JS:   obj?.a?.b;  d ?? default
来源：http://dt.nicolike.cn

TS:   obj?.a?.b;  d ?? default
来源：http://hm.chemitech.net.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ks.shxzskj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://xu.nszjky.cn

Ruby: d&.dig(:a, :b)
来源：http://tj.hahajie.cn

C#:   obj?.A?.B ?? default
来源：http://jo.huanxung.cn

[H07] 断言
来源：http://ww.chemitech.net.cn

Py:   assert x > 0, "必须为正"
来源：http://jd.asd995.cn

PHP:  assert($x > 0);
来源：http://zp.shxzskj.cn

JS:   console.assert(x > 0);
来源：http://vf.asd995.cn

TS:   console.assert(x > 0);
来源：http://ed.hnjuh.cn

Java: assert x > 0 : "必须为正";
来源：http://kw.huixiangedu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sg.asd995.cn

Ruby: raise "必须为正" unless x > 0
来源：http://fn.hnjuh.cn

C#:   Debug.Assert(x > 0);
来源：http://uw.shxzukj.cn

[H08] 获取错误信息与堆栈
来源：http://be.newstarts.cn

Py:   str(e);  traceback.format_exc()
来源：http://cx.haigaiapp.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tz.huixiangedu.cn

JS:   e.message;  e.stack
来源：http://eo.huixinmuqiang.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://yd.shtwfgs.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://av.szxytkj.cn

Go:   err.Error()
来源：http://tu.szsharing.cn

Ruby: e.message;  e.backtrace
来源：http://kx.521024.cn

C#:   e.Message;  e.StackTrace
来源：http://rd.521024.cn

[H09] 带错误码的异常
来源：http://pf.huixinmuqiang.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mv.huixinmuqiang.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ax.szxytkj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yn.shxzukj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lm.huanxung.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mf.shxzukj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zk.lnxyls.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ci.bjjhwx.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://xi.bookmarksfly.cn

[H10] 资源自动释放
来源：http://rn.jianghongdianzi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lg.szxytkj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bm.szsharing.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://px.nicolike.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nv.nszjky.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wk.szsharing.cn

Go:   defer f.Close()
来源：http://ej.szsharing.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tz.panjiajie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zl.haigaiapp.cn

================================================================================
来源：http://ky.jctech888.com.cn

I. 正则表达式
来源：http://bq.9csxet.cn

================================================================================
来源：http://ju.hahajie.cn

[I01] 判断是否匹配
来源：http://cm.yuexingan06.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lm.wgjwhj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jt.shxzukj.cn

JS:   /\d+/.test(s)
来源：http://cp.szxytkj.cn

TS:   /\d+/.test(s)
来源：http://yt.muxihuayi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xe.muxihuayi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jz.huanxung.cn

Ruby: s.match?(/\d+/)
来源：http://xa.bookmarksfly.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fn.huanxung.cn

[I02] 提取所有匹配
来源：http://jx.huixinmuqiang.cn

Py:   re.findall(r"\d+", s)
来源：http://ll.huixiangedu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mc.bjjhwx.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qt.bookmarksfly.cn

TS:   s.match(/\d+/g)
来源：http://wl.huixiangedu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pb.huanxung.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rs.huanxung.cn

Ruby: s.scan(/\d+/)
来源：http://wy.nicolike.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://sr.nszjky.cn

[I03] 提取捕获分组
来源：http://qu.shxzukj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sz.asd995.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ec.nicolike.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kk.jianghongdianzi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bj.nszjky.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wg.huixinmuqiang.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sk.chemitech.net.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mh.521024.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://aa.huanxung.cn

[I04] 正则替换
来源：http://fp.bookmarksfly.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://vo.huixiangedu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tl.szxytkj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://kj.colortex.cn

TS:   s.replace(/\d+/g, "#")
来源：http://da.wgjwhj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ur.huixinmuqiang.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ar.gzmigu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://kz.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ab.nszjky.cn

[I05] 按正则拆分
来源：http://rq.jctech888.com.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://dh.huixiangedu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://my.huixiangedu.cn

JS:   s.split(/\s*,\s*/)
来源：http://gd.asd995.cn

TS:   s.split(/\s*,\s*/)
来源：http://qq.shtwfgs.cn

Java: s.split("\\s*,\\s*")
来源：http://cj.nszjky.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lq.huixinmuqiang.cn

Ruby: s.split(/\s*,\s*/)
来源：http://sh.hahajie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sr.wgjwhj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rp.szxytkj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nm.colortex.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ir.wgjwhj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://va.9csxet.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wm.9csxet.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fv.asd995.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://id.chemitech.net.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jx.nicolike.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hy.hnjuh.cn

[I07] 忽略大小写与多行模式
来源：http://kr.newstarts.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yb.lnxyls.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://po.nszjky.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dx.shxzukj.cn

TS:   /error/gim
来源：http://ei.colortex.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://og.huixinmuqiang.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://js.hnjuh.cn

Ruby: s.scan(/error/i)
来源：http://ar.bookmarksfly.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tt.nicolike.cn

[I08] 贪婪与非贪婪匹配
来源：http://ql.9csxet.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://go.huixiangedu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yd.9csxet.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gz.newstarts.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wf.wgjwhj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://th.chemitech.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jf.newstarts.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vr.lnxyls.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fp.lnxyls.cn

================================================================================
来源：http://jg.huanxung.cn

J. 日期与时间
来源：http://hs.nszjky.cn

================================================================================
来源：http://wq.yuexingan06.cn

[J01] 获取当前时间
来源：http://ry.wgjwhj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://og.shxzukj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://co.9csxet.cn

JS:   new Date();  Date.now()
来源：http://wr.shxzskj.cn

TS:   new Date();  Date.now()
来源：http://ik.muxihuayi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://xj.shxzukj.cn

Go:   time.Now()
来源：http://pc.colortex.cn

Ruby: Time.now
来源：http://kx.panjiajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ao.gzmigu.cn

[J02] 格式化输出
来源：http://nt.chemitech.net.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rw.hahajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ww.bookmarksfly.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hj.521024.cn

TS:   d.toISOString()
来源：http://lt.szsharing.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gx.haigaiapp.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zp.huixinmuqiang.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sk.shxzskj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xw.jctech888.com.cn

[J03] 字符串解析为日期
来源：http://ts.nicolike.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dw.hahajie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mi.521024.cn

JS:   new Date("2024-01-02")
来源：http://js.chemitech.net.cn

TS:   new Date("2024-01-02")
来源：http://sr.shxzskj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://kd.yuntaijiaju.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rv.521024.cn

Ruby: Date.parse("2024-01-02")
来源：http://kv.yuntaijiaju.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cs.shtwfgs.cn

[J04] 时间戳与日期互转
来源：http://tl.szxytkj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rw.jianghongdianzi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gz.colortex.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xg.9csxet.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://er.lnxyls.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zg.huixiangedu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kn.yuexingan06.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bf.hahajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lx.yuntaijiaju.cn

[J05] 时间加减（加 7 天）
来源：http://wi.yuexingan06.cn

Py:   now + timedelta(days=7)
来源：http://bt.521024.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://dg.nszjky.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://uf.shxzukj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nq.huanxung.cn

Java: LocalDate.now().plusDays(7)
来源：http://uz.lnxyls.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://le.huixinmuqiang.cn

Ruby: Time.now + 7 * 86400
来源：http://wv.newstarts.cn

C#:   DateTime.Now.AddDays(7)
来源：http://tv.shxzskj.cn

[J06] 计算两时间之差
来源：http://sa.panjiajie.cn

Py:   (end - start).total_seconds()
来源：http://th.shtwfgs.cn

PHP:  $end->diff($start)->days;
来源：http://hu.jctech888.com.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vv.asd995.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yr.bjjhwx.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ro.hahajie.cn

Go:   end.Sub(start).Hours()
来源：http://pm.yuexingan06.cn

Ruby: end - start                 # 返回秒数
来源：http://if.jianghongdianzi.cn

C#:   (end - start).TotalSeconds
来源：http://bw.yuexingan06.cn

[J07] 比较两个日期
来源：http://xr.9csxet.cn

Py:   d1 < d2;  d1 == d2
来源：http://tw.haigaiapp.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fy.yuntaijiaju.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ss.nicolike.cn

TS:   d1.getTime() < d2.getTime()
来源：http://jd.colortex.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zm.huanxung.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gx.colortex.cn

Ruby: d1 < d2;  d1 == d2
来源：http://jc.shtwfgs.cn

C#:   d1 < d2;  d1 == d2
来源：http://wq.szsharing.cn

[J08] 提取年月日与星期
来源：http://ff.yuntaijiaju.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tg.lnxyls.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wt.colortex.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gw.newstarts.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pp.huixiangedu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://we.huixiangedu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xg.521024.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://aw.shxzukj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kw.huixinmuqiang.cn

[J09] 时区处理
来源：http://oh.panjiajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kw.gzmigu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ne.yuexingan06.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fd.gzmigu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ab.newstarts.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zc.hahajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gw.gzmigu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://kb.yuntaijiaju.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yy.hahajie.cn

[J10] 取今天 / 本月第一天
来源：http://un.bookmarksfly.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ml.szxytkj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yz.newstarts.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bt.shtwfgs.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cv.yuexingan06.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zg.huixiangedu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lw.huixinmuqiang.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qb.muxihuayi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://up.huixinmuqiang.cn

================================================================================
来源：http://fv.panjiajie.cn

K. JSON 与序列化
来源：http://jp.yuexingan06.cn

================================================================================
来源：http://yz.hahajie.cn

[K01] 对象转 JSON 字符串
来源：http://pt.shxzukj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zl.hahajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xw.bjjhwx.cn

JS:   JSON.stringify(obj)
来源：http://tj.asd995.cn

TS:   JSON.stringify(obj)
来源：http://us.nszjky.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kn.chemitech.net.cn

Go:   json.Marshal(obj)
来源：http://yf.lnxyls.cn

Ruby: obj.to_json                                     // require "json"
来源：http://sn.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://aq.huanxung.cn

[K02] JSON 字符串转对象
来源：http://ig.huanxung.cn

Py:   json.loads(s)
来源：http://ki.shxzukj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cb.nicolike.cn

JS:   JSON.parse(s)
来源：http://vv.shtwfgs.cn

TS:   JSON.parse(s)
来源：http://km.asd995.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xk.gzmigu.cn

Go:   json.Unmarshal(data, &v)
来源：http://pz.chemitech.net.cn

Ruby: JSON.parse(s)
来源：http://xj.bjjhwx.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ea.9csxet.cn

[K03] JSON 美化输出（带缩进）
来源：http://ph.nicolike.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kb.hnjuh.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wg.nicolike.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://nl.szxytkj.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://il.newstarts.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lb.lnxyls.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://op.lnxyls.cn


<!-- 参考信息 -->