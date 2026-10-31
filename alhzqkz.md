代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://ou.wgjwhj.cn

Java: record User(String name, int age) {}
来源：http://kg.gzmigu.cn

Go:   type User struct { Name string; Age int }
来源：http://in.bjjhwx.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nf.szxytkj.cn

C#:   record User(string Name, int Age);
来源：http://yn.newstarts.cn

[G15] 枚举
来源：http://dt.jianghongdianzi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sn.haigaiapp.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://fu.yuexingan06.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ho.shxzskj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gj.jctech888.com.cn

Java: enum Color { RED, GREEN }
来源：http://gn.haigaiapp.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kk.shxzukj.cn

Ruby: Color = %i[red green].freeze
来源：http://wf.521024.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hg.nszjky.cn

[G16] 对象转数组 / 字典
来源：http://gj.yuexingan06.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pg.panjiajie.cn

PHP:  get_object_vars($obj);
来源：http://sh.szxytkj.cn

JS:   Object.entries(obj)
来源：http://gz.asd995.cn

TS:   Object.entries(obj)
来源：http://ow.huixiangedu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kr.huanxung.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ys.shxzukj.cn

Ruby: obj.instance_variables
来源：http://eg.szxytkj.cn

C#:   // 用反射或 System.Text.Json
来源：http://jw.shxzskj.cn

================================================================================
来源：http://xd.szsharing.cn

H. 异常与错误处理
来源：http://ui.yuntaijiaju.cn

================================================================================
来源：http://fn.wgjwhj.cn

[H01] try / catch 基础
来源：http://iu.yuntaijiaju.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lq.gzmigu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gl.newstarts.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://sc.colortex.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vr.9csxet.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yc.shtwfgs.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://iq.shxzskj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yc.shxzukj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wc.chemitech.net.cn

[H02] finally / ensure 收尾
来源：http://wl.wgjwhj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://uc.hahajie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ue.nicolike.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hf.yuexingan06.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ag.haigaiapp.cn

Java: try { f(); } finally { cleanup(); }
来源：http://sc.nszjky.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://lt.wgjwhj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ny.521024.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://iq.gzmigu.cn

[H03] 主动抛出异常
来源：http://wg.haigaiapp.cn

Py:   raise ValueError("错误信息")
来源：http://gc.asd995.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wl.gzmigu.cn

JS:   throw new Error("错误信息");
来源：http://jw.bookmarksfly.cn

TS:   throw new Error("错误信息");
来源：http://pl.szsharing.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://jb.jianghongdianzi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vp.huixinmuqiang.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wj.bookmarksfly.cn

C#:   throw new ArgumentException("错误信息");
来源：http://wo.9csxet.cn

[H04] 自定义异常类型
来源：http://ru.hnjuh.cn

Py:   class MyError(Exception): pass
来源：http://rd.chemitech.net.cn

PHP:  class MyError extends RuntimeException {}
来源：http://lm.hnjuh.cn

JS:   class MyError extends Error {}
来源：http://rd.huixinmuqiang.cn

TS:   class MyError extends Error {}
来源：http://ui.panjiajie.cn

Java: class MyException extends RuntimeException {}
来源：http://jm.bjjhwx.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zv.bjjhwx.cn

Ruby: class MyError < StandardError; end
来源：http://fr.shxzskj.cn

C#:   class MyException : Exception {}
来源：http://kn.jctech888.com.cn

[H05] 捕获特定类型
来源：http://mm.haigaiapp.cn

Py:   except ValueError as e:
来源：http://fo.colortex.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yz.szsharing.cn

JS:   if (e instanceof TypeError) {}
来源：http://at.szsharing.cn

TS:   if (e instanceof TypeError) {}
来源：http://da.newstarts.cn

Java: catch (IOException | SQLException e) {}
来源：http://nk.bookmarksfly.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ro.szsharing.cn

Ruby: rescue ArgumentError => e
来源：http://jp.hnjuh.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mo.wgjwhj.cn

[H06] 可选值 / 空值安全访问
来源：http://nu.newstarts.cn

Py:   value = d.get("k") or default
来源：http://vr.gzmigu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jy.colortex.cn

JS:   obj?.a?.b;  d ?? default
来源：http://jk.szsharing.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jc.muxihuayi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dq.colortex.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://or.huixinmuqiang.cn

Ruby: d&.dig(:a, :b)
来源：http://ef.yuntaijiaju.cn

C#:   obj?.A?.B ?? default
来源：http://wh.yuexingan06.cn

[H07] 断言
来源：http://en.haigaiapp.cn

Py:   assert x > 0, "必须为正"
来源：http://zq.nicolike.cn

PHP:  assert($x > 0);
来源：http://xq.hnjuh.cn

JS:   console.assert(x > 0);
来源：http://vi.yuntaijiaju.cn

TS:   console.assert(x > 0);
来源：http://rv.hahajie.cn

Java: assert x > 0 : "必须为正";
来源：http://ml.muxihuayi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://by.gzmigu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ky.haigaiapp.cn

C#:   Debug.Assert(x > 0);
来源：http://xm.521024.cn

[H08] 获取错误信息与堆栈
来源：http://ri.shxzukj.cn

Py:   str(e);  traceback.format_exc()
来源：http://vm.chemitech.net.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gz.gzmigu.cn

JS:   e.message;  e.stack
来源：http://mp.jianghongdianzi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://zf.521024.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://jl.panjiajie.cn

Go:   err.Error()
来源：http://al.haigaiapp.cn

Ruby: e.message;  e.backtrace
来源：http://nt.shtwfgs.cn

C#:   e.Message;  e.StackTrace
来源：http://oo.shtwfgs.cn

[H09] 带错误码的异常
来源：http://ja.gzmigu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zj.jctech888.com.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://kd.huanxung.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rt.huanxung.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zz.nszjky.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bk.huixiangedu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pv.bookmarksfly.cn

Ruby: raise MyError.new("fail", 500)
来源：http://td.newstarts.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://dc.szxytkj.cn

[H10] 资源自动释放
来源：http://vp.bjjhwx.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://fr.szxytkj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xk.yuntaijiaju.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sm.yuntaijiaju.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://on.bookmarksfly.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zv.521024.cn

Go:   defer f.Close()
来源：http://lh.haigaiapp.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hi.hnjuh.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yr.lnxyls.cn

================================================================================
来源：http://lz.jctech888.com.cn

I. 正则表达式
来源：http://ds.yuexingan06.cn

================================================================================
来源：http://ij.colortex.cn

[I01] 判断是否匹配
来源：http://qq.chemitech.net.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ck.jianghongdianzi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://mm.wgjwhj.cn

JS:   /\d+/.test(s)
来源：http://xw.szsharing.cn

TS:   /\d+/.test(s)
来源：http://kk.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yp.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ta.bookmarksfly.cn

Ruby: s.match?(/\d+/)
来源：http://wh.colortex.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ob.szsharing.cn

[I02] 提取所有匹配
来源：http://fz.huanxung.cn

Py:   re.findall(r"\d+", s)
来源：http://xr.gzmigu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zn.huixinmuqiang.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ch.muxihuayi.cn

TS:   s.match(/\d+/g)
来源：http://bj.muxihuayi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ls.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ne.colortex.cn

Ruby: s.scan(/\d+/)
来源：http://sn.nicolike.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nu.9csxet.cn

[I03] 提取捕获分组
来源：http://mv.hahajie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bn.szxytkj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://td.colortex.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zz.haigaiapp.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yv.shxzukj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ga.chemitech.net.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mf.nicolike.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ef.lnxyls.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jj.shxzukj.cn

[I04] 正则替换
来源：http://lq.gzmigu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://pa.muxihuayi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fd.bjjhwx.cn

JS:   s.replace(/\d+/g, "#")
来源：http://lk.9csxet.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ip.asd995.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ei.521024.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://yi.szsharing.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ww.9csxet.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hq.9csxet.cn

[I05] 按正则拆分
来源：http://jb.chemitech.net.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://pa.wgjwhj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pg.newstarts.cn

JS:   s.split(/\s*,\s*/)
来源：http://qi.wgjwhj.cn

TS:   s.split(/\s*,\s*/)
来源：http://do.colortex.cn

Java: s.split("\\s*,\\s*")
来源：http://mh.huanxung.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kt.colortex.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zd.jctech888.com.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pm.jianghongdianzi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://up.huixinmuqiang.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://aq.newstarts.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gt.nicolike.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://si.haigaiapp.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zy.haigaiapp.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wn.jianghongdianzi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hi.bjjhwx.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qd.shxzukj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yc.asd995.cn

[I07] 忽略大小写与多行模式
来源：http://fq.gzmigu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gs.newstarts.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://oy.asd995.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hv.hahajie.cn

TS:   /error/gim
来源：http://ek.yuntaijiaju.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xs.jianghongdianzi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zv.hnjuh.cn

Ruby: s.scan(/error/i)
来源：http://pp.panjiajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://po.nicolike.cn

[I08] 贪婪与非贪婪匹配
来源：http://as.hnjuh.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pl.521024.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://it.huixiangedu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ez.panjiajie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gx.szxytkj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ug.newstarts.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zb.colortex.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yo.yuexingan06.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uo.nszjky.cn

================================================================================
来源：http://vq.asd995.cn

J. 日期与时间
来源：http://wy.hnjuh.cn

================================================================================
来源：http://ek.huanxung.cn

[J01] 获取当前时间
来源：http://km.lnxyls.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://kp.colortex.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zf.bookmarksfly.cn

JS:   new Date();  Date.now()
来源：http://mg.haigaiapp.cn

TS:   new Date();  Date.now()
来源：http://tz.yuexingan06.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jr.9csxet.cn

Go:   time.Now()
来源：http://ui.yuexingan06.cn

Ruby: Time.now
来源：http://no.bookmarksfly.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://np.asd995.cn

[J02] 格式化输出
来源：http://jq.chemitech.net.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qw.jianghongdianzi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qi.nicolike.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ll.asd995.cn

TS:   d.toISOString()
来源：http://mq.panjiajie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xb.jctech888.com.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pq.9csxet.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lz.nszjky.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ia.wgjwhj.cn

[J03] 字符串解析为日期
来源：http://ne.szxytkj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wx.panjiajie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ii.gzmigu.cn

JS:   new Date("2024-01-02")
来源：http://hf.gzmigu.cn

TS:   new Date("2024-01-02")
来源：http://vr.huixinmuqiang.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ih.jianghongdianzi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kz.huixinmuqiang.cn

Ruby: Date.parse("2024-01-02")
来源：http://dp.newstarts.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wk.nicolike.cn

[J04] 时间戳与日期互转
来源：http://md.nicolike.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pc.panjiajie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ro.szxytkj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ee.shxzskj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ef.521024.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xw.huixiangedu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mt.nicolike.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cx.muxihuayi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://di.gzmigu.cn

[J05] 时间加减（加 7 天）
来源：http://xm.yuntaijiaju.cn

Py:   now + timedelta(days=7)
来源：http://jo.szsharing.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://dy.shtwfgs.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://uw.hahajie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xw.nszjky.cn

Java: LocalDate.now().plusDays(7)
来源：http://lq.muxihuayi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wq.jianghongdianzi.cn

Ruby: Time.now + 7 * 86400
来源：http://qx.nszjky.cn

C#:   DateTime.Now.AddDays(7)
来源：http://hw.bookmarksfly.cn

[J06] 计算两时间之差
来源：http://am.jctech888.com.cn

Py:   (end - start).total_seconds()
来源：http://mt.bjjhwx.cn

PHP:  $end->diff($start)->days;
来源：http://jw.nszjky.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jq.yuntaijiaju.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vn.szsharing.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ln.huixiangedu.cn

Go:   end.Sub(start).Hours()
来源：http://st.szsharing.cn

Ruby: end - start                 # 返回秒数
来源：http://mg.bjjhwx.cn

C#:   (end - start).TotalSeconds
来源：http://sw.huixiangedu.cn

[J07] 比较两个日期
来源：http://wx.bookmarksfly.cn

Py:   d1 < d2;  d1 == d2
来源：http://ri.panjiajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gh.lnxyls.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qm.bookmarksfly.cn

TS:   d1.getTime() < d2.getTime()
来源：http://el.colortex.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lx.panjiajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bt.9csxet.cn

Ruby: d1 < d2;  d1 == d2
来源：http://hl.huixinmuqiang.cn

C#:   d1 < d2;  d1 == d2
来源：http://xp.521024.cn

[J08] 提取年月日与星期
来源：http://xe.jianghongdianzi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cs.521024.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bk.haigaiapp.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ct.huixiangedu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tf.hnjuh.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cl.lnxyls.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://iv.jctech888.com.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gn.colortex.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ak.szxytkj.cn

[J09] 时区处理
来源：http://pn.hnjuh.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mt.haigaiapp.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mz.wgjwhj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://em.gzmigu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wf.shxzukj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qd.bjjhwx.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lr.gzmigu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xn.gzmigu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zh.huanxung.cn

[J10] 取今天 / 本月第一天
来源：http://cp.colortex.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://gk.bjjhwx.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://la.hahajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bv.bjjhwx.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ik.gzmigu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://au.szxytkj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ju.asd995.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ui.shtwfgs.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zj.colortex.cn

================================================================================
来源：http://zs.colortex.cn

K. JSON 与序列化
来源：http://sh.lnxyls.cn

================================================================================
来源：http://uh.shxzskj.cn

[K01] 对象转 JSON 字符串
来源：http://pu.wgjwhj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vv.bjjhwx.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bv.lnxyls.cn

JS:   JSON.stringify(obj)
来源：http://uz.shtwfgs.cn

TS:   JSON.stringify(obj)
来源：http://px.nicolike.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zj.panjiajie.cn

Go:   json.Marshal(obj)
来源：http://ku.panjiajie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://yb.asd995.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://kh.hnjuh.cn

[K02] JSON 字符串转对象
来源：http://us.shxzskj.cn

Py:   json.loads(s)
来源：http://kz.huixinmuqiang.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fu.huixiangedu.cn

JS:   JSON.parse(s)
来源：http://bh.hahajie.cn


<!-- 参考信息 -->