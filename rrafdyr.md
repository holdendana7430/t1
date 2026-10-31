代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://wr.jctech888.com.cn

Java: record User(String name, int age) {}
来源：http://sz.newstarts.cn

Go:   type User struct { Name string; Age int }
来源：http://hm.huanxung.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://uo.bookmarksfly.cn

C#:   record User(string Name, int Age);
来源：http://lj.nszjky.cn

[G15] 枚举
来源：http://kn.lnxyls.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dy.nszjky.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ho.yuntaijiaju.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vr.yuexingan06.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ku.asd995.cn

Java: enum Color { RED, GREEN }
来源：http://yi.lnxyls.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ys.huixinmuqiang.cn

Ruby: Color = %i[red green].freeze
来源：http://wf.muxihuayi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ai.huixinmuqiang.cn

[G16] 对象转数组 / 字典
来源：http://qm.yuntaijiaju.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uy.hahajie.cn

PHP:  get_object_vars($obj);
来源：http://if.jianghongdianzi.cn

JS:   Object.entries(obj)
来源：http://mv.shtwfgs.cn

TS:   Object.entries(obj)
来源：http://pn.szxytkj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zn.nszjky.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://qb.huixiangedu.cn

Ruby: obj.instance_variables
来源：http://mj.lnxyls.cn

C#:   // 用反射或 System.Text.Json
来源：http://hf.shtwfgs.cn

================================================================================
来源：http://ws.haigaiapp.cn

H. 异常与错误处理
来源：http://zo.huixiangedu.cn

================================================================================
来源：http://ar.hahajie.cn

[H01] try / catch 基础
来源：http://fj.panjiajie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vh.haigaiapp.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kq.colortex.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tm.9csxet.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jr.muxihuayi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ro.panjiajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pk.bjjhwx.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ny.521024.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ka.panjiajie.cn

[H02] finally / ensure 收尾
来源：http://ft.yuexingan06.cn

Py:   try: f()⏎finally: cleanup()
来源：http://hd.hnjuh.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ue.shtwfgs.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://vh.colortex.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://xt.gzmigu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://nb.521024.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://xz.huixiangedu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://by.521024.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://cg.yuntaijiaju.cn

[H03] 主动抛出异常
来源：http://el.shxzskj.cn

Py:   raise ValueError("错误信息")
来源：http://oi.szsharing.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ew.nicolike.cn

JS:   throw new Error("错误信息");
来源：http://ds.nszjky.cn

TS:   throw new Error("错误信息");
来源：http://ju.wgjwhj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://uu.nszjky.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vs.asd995.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://yj.hnjuh.cn

C#:   throw new ArgumentException("错误信息");
来源：http://me.wgjwhj.cn

[H04] 自定义异常类型
来源：http://lp.shtwfgs.cn

Py:   class MyError(Exception): pass
来源：http://zy.szxytkj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://fu.shtwfgs.cn

JS:   class MyError extends Error {}
来源：http://hf.gzmigu.cn

TS:   class MyError extends Error {}
来源：http://nm.nicolike.cn

Java: class MyException extends RuntimeException {}
来源：http://ys.yuexingan06.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fu.hnjuh.cn

Ruby: class MyError < StandardError; end
来源：http://cg.shtwfgs.cn

C#:   class MyException : Exception {}
来源：http://gf.hahajie.cn

[H05] 捕获特定类型
来源：http://ce.shxzskj.cn

Py:   except ValueError as e:
来源：http://ft.jianghongdianzi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qd.szxytkj.cn

JS:   if (e instanceof TypeError) {}
来源：http://zi.lnxyls.cn

TS:   if (e instanceof TypeError) {}
来源：http://va.huanxung.cn

Java: catch (IOException | SQLException e) {}
来源：http://vt.nszjky.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kg.wgjwhj.cn

Ruby: rescue ArgumentError => e
来源：http://ea.shxzskj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ze.szsharing.cn

[H06] 可选值 / 空值安全访问
来源：http://ez.szsharing.cn

Py:   value = d.get("k") or default
来源：http://lb.nicolike.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jm.shtwfgs.cn

JS:   obj?.a?.b;  d ?? default
来源：http://fh.haigaiapp.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xx.bookmarksfly.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zc.shxzskj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://hh.lnxyls.cn

Ruby: d&.dig(:a, :b)
来源：http://ww.colortex.cn

C#:   obj?.A?.B ?? default
来源：http://ix.shxzskj.cn

[H07] 断言
来源：http://oe.shtwfgs.cn

Py:   assert x > 0, "必须为正"
来源：http://be.521024.cn

PHP:  assert($x > 0);
来源：http://dp.colortex.cn

JS:   console.assert(x > 0);
来源：http://lv.521024.cn

TS:   console.assert(x > 0);
来源：http://cv.wgjwhj.cn

Java: assert x > 0 : "必须为正";
来源：http://xs.lnxyls.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://en.nicolike.cn

Ruby: raise "必须为正" unless x > 0
来源：http://za.szsharing.cn

C#:   Debug.Assert(x > 0);
来源：http://sw.shxzukj.cn

[H08] 获取错误信息与堆栈
来源：http://th.hnjuh.cn

Py:   str(e);  traceback.format_exc()
来源：http://ph.hnjuh.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dn.lnxyls.cn

JS:   e.message;  e.stack
来源：http://pb.panjiajie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://lb.chemitech.net.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ez.shxzskj.cn

Go:   err.Error()
来源：http://zj.nszjky.cn

Ruby: e.message;  e.backtrace
来源：http://kz.wgjwhj.cn

C#:   e.Message;  e.StackTrace
来源：http://gc.shxzukj.cn

[H09] 带错误码的异常
来源：http://mt.yuntaijiaju.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qf.shxzukj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://se.gzmigu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lo.bookmarksfly.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rf.panjiajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wi.huixiangedu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wr.wgjwhj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://iz.wgjwhj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://sx.bookmarksfly.cn

[H10] 资源自动释放
来源：http://xm.yuntaijiaju.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://os.9csxet.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nm.shxzskj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pm.nicolike.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xa.hnjuh.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qk.jianghongdianzi.cn

Go:   defer f.Close()
来源：http://ao.lnxyls.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ni.colortex.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nl.chemitech.net.cn

================================================================================
来源：http://qd.haigaiapp.cn

I. 正则表达式
来源：http://rs.newstarts.cn

================================================================================
来源：http://yw.chemitech.net.cn

[I01] 判断是否匹配
来源：http://nn.nszjky.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lp.haigaiapp.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gi.chemitech.net.cn

JS:   /\d+/.test(s)
来源：http://dw.colortex.cn

TS:   /\d+/.test(s)
来源：http://ee.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cv.jianghongdianzi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://sp.jianghongdianzi.cn

Ruby: s.match?(/\d+/)
来源：http://ai.chemitech.net.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://uw.nicolike.cn

[I02] 提取所有匹配
来源：http://hv.asd995.cn

Py:   re.findall(r"\d+", s)
来源：http://yv.nicolike.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ip.9csxet.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://le.shxzukj.cn

TS:   s.match(/\d+/g)
来源：http://as.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ih.jianghongdianzi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://uv.szxytkj.cn

Ruby: s.scan(/\d+/)
来源：http://fw.gzmigu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ey.lnxyls.cn

[I03] 提取捕获分组
来源：http://av.nszjky.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ry.bjjhwx.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fq.9csxet.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cg.hnjuh.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zf.huixiangedu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yl.521024.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ps.nicolike.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fb.hahajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ej.haigaiapp.cn

[I04] 正则替换
来源：http://wo.huanxung.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://je.haigaiapp.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wv.jctech888.com.cn

JS:   s.replace(/\d+/g, "#")
来源：http://bk.szsharing.cn

TS:   s.replace(/\d+/g, "#")
来源：http://bw.lnxyls.cn

Java: s.replaceAll("\\d+", "#")
来源：http://is.szsharing.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://kc.bjjhwx.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ha.newstarts.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fm.huixiangedu.cn

[I05] 按正则拆分
来源：http://iz.shtwfgs.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://cn.shxzukj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yy.bookmarksfly.cn

JS:   s.split(/\s*,\s*/)
来源：http://ie.asd995.cn

TS:   s.split(/\s*,\s*/)
来源：http://rl.huanxung.cn

Java: s.split("\\s*,\\s*")
来源：http://sb.colortex.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rl.jctech888.com.cn

Ruby: s.split(/\s*,\s*/)
来源：http://up.lnxyls.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ex.shxzukj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qx.szsharing.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xo.muxihuayi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ib.nszjky.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ue.colortex.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ag.newstarts.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bj.huixinmuqiang.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bf.hnjuh.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ru.521024.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pn.jctech888.com.cn

[I07] 忽略大小写与多行模式
来源：http://tw.gzmigu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fr.shtwfgs.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wf.shtwfgs.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://yo.jctech888.com.cn

TS:   /error/gim
来源：http://uz.521024.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://eo.jianghongdianzi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://li.huixinmuqiang.cn

Ruby: s.scan(/error/i)
来源：http://ca.muxihuayi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://de.nicolike.cn

[I08] 贪婪与非贪婪匹配
来源：http://pq.9csxet.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zs.wgjwhj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mq.colortex.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sm.szxytkj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://id.yuexingan06.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ko.9csxet.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zu.newstarts.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://oc.shxzskj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tq.chemitech.net.cn

================================================================================
来源：http://ty.yuntaijiaju.cn

J. 日期与时间
来源：http://tj.szsharing.cn

================================================================================
来源：http://wo.huanxung.cn

[J01] 获取当前时间
来源：http://cm.asd995.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://xz.yuntaijiaju.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yv.asd995.cn

JS:   new Date();  Date.now()
来源：http://ne.asd995.cn

TS:   new Date();  Date.now()
来源：http://eh.nicolike.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://sm.jianghongdianzi.cn

Go:   time.Now()
来源：http://io.bjjhwx.cn

Ruby: Time.now
来源：http://yj.haigaiapp.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rp.asd995.cn

[J02] 格式化输出
来源：http://gg.gzmigu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wo.wgjwhj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ek.haigaiapp.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ez.521024.cn

TS:   d.toISOString()
来源：http://dy.panjiajie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nn.yuexingan06.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pa.nicolike.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oy.jianghongdianzi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jr.521024.cn

[J03] 字符串解析为日期
来源：http://gk.shxzukj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vn.muxihuayi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ov.colortex.cn

JS:   new Date("2024-01-02")
来源：http://le.jctech888.com.cn

TS:   new Date("2024-01-02")
来源：http://vq.huanxung.cn

Java: LocalDate.parse("2024-01-02")
来源：http://rp.gzmigu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dd.gzmigu.cn

Ruby: Date.parse("2024-01-02")
来源：http://lc.colortex.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jw.muxihuayi.cn

[J04] 时间戳与日期互转
来源：http://ec.haigaiapp.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ri.9csxet.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://op.chemitech.net.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nv.nszjky.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://rj.wgjwhj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uz.huixinmuqiang.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wb.hahajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tc.colortex.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dn.huixiangedu.cn

[J05] 时间加减（加 7 天）
来源：http://yx.asd995.cn

Py:   now + timedelta(days=7)
来源：http://we.muxihuayi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://pv.bookmarksfly.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ma.haigaiapp.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xj.colortex.cn

Java: LocalDate.now().plusDays(7)
来源：http://qu.shtwfgs.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mf.nszjky.cn

Ruby: Time.now + 7 * 86400
来源：http://gv.huixinmuqiang.cn

C#:   DateTime.Now.AddDays(7)
来源：http://uk.yuntaijiaju.cn

[J06] 计算两时间之差
来源：http://ax.bookmarksfly.cn

Py:   (end - start).total_seconds()
来源：http://jz.gzmigu.cn

PHP:  $end->diff($start)->days;
来源：http://yn.newstarts.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://la.jctech888.com.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mj.huixiangedu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://yx.muxihuayi.cn

Go:   end.Sub(start).Hours()
来源：http://tg.nszjky.cn

Ruby: end - start                 # 返回秒数
来源：http://kk.gzmigu.cn

C#:   (end - start).TotalSeconds
来源：http://oa.shxzskj.cn

[J07] 比较两个日期
来源：http://si.szsharing.cn

Py:   d1 < d2;  d1 == d2
来源：http://fi.szxytkj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cm.chemitech.net.cn

JS:   d1.getTime() < d2.getTime()
来源：http://bf.bjjhwx.cn

TS:   d1.getTime() < d2.getTime()
来源：http://iy.jctech888.com.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ty.muxihuayi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tn.haigaiapp.cn

Ruby: d1 < d2;  d1 == d2
来源：http://rr.panjiajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://qd.jctech888.com.cn

[J08] 提取年月日与星期
来源：http://jo.wgjwhj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://us.nicolike.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fh.chemitech.net.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ps.yuexingan06.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nm.nicolike.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kn.lnxyls.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xe.yuexingan06.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://to.hnjuh.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bu.9csxet.cn

[J09] 时区处理
来源：http://kf.chemitech.net.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://aa.gzmigu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://eg.521024.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xi.yuexingan06.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rw.bookmarksfly.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mz.nicolike.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lj.panjiajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://uq.muxihuayi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xw.colortex.cn

[J10] 取今天 / 本月第一天
来源：http://ih.yuexingan06.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://bi.haigaiapp.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ts.hahajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rq.shxzskj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pz.nicolike.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yx.shxzskj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lu.yuexingan06.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jn.521024.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ri.szxytkj.cn

================================================================================
来源：http://jg.nszjky.cn

K. JSON 与序列化
来源：http://fe.yuexingan06.cn

================================================================================
来源：http://vf.huixinmuqiang.cn

[K01] 对象转 JSON 字符串
来源：http://rg.colortex.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ut.huanxung.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ox.nszjky.cn

JS:   JSON.stringify(obj)
来源：http://dp.szxytkj.cn

TS:   JSON.stringify(obj)
来源：http://jt.jctech888.com.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mq.muxihuayi.cn

Go:   json.Marshal(obj)
来源：http://gu.asd995.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qi.9csxet.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://tp.gzmigu.cn

[K02] JSON 字符串转对象
来源：http://kv.szxytkj.cn

Py:   json.loads(s)
来源：http://yt.hahajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cp.bjjhwx.cn

JS:   JSON.parse(s)
来源：http://hy.szsharing.cn


<!-- 参考信息 -->