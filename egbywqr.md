代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://km.nszjky.cn

Java: record User(String name, int age) {}
来源：http://mw.newstarts.cn

Go:   type User struct { Name string; Age int }
来源：http://sa.bookmarksfly.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qq.haigaiapp.cn

C#:   record User(string Name, int Age);
来源：http://fw.szsharing.cn

[G15] 枚举
来源：http://bo.muxihuayi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lb.colortex.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://qm.chemitech.net.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://eb.9csxet.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yo.shxzukj.cn

Java: enum Color { RED, GREEN }
来源：http://rg.bookmarksfly.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xm.asd995.cn

Ruby: Color = %i[red green].freeze
来源：http://og.jctech888.com.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://we.bjjhwx.cn

[G16] 对象转数组 / 字典
来源：http://nw.shxzukj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bn.gzmigu.cn

PHP:  get_object_vars($obj);
来源：http://wp.yuexingan06.cn

JS:   Object.entries(obj)
来源：http://uu.huixiangedu.cn

TS:   Object.entries(obj)
来源：http://je.bookmarksfly.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lh.shxzskj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ro.hahajie.cn

Ruby: obj.instance_variables
来源：http://wm.muxihuayi.cn

C#:   // 用反射或 System.Text.Json
来源：http://za.hnjuh.cn

================================================================================
来源：http://jw.shtwfgs.cn

H. 异常与错误处理
来源：http://ys.521024.cn

================================================================================
来源：http://jv.gzmigu.cn

[H01] try / catch 基础
来源：http://li.9csxet.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://sd.yuntaijiaju.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://py.9csxet.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mh.shtwfgs.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zp.gzmigu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jy.panjiajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://oj.nszjky.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xn.huixiangedu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xy.haigaiapp.cn

[H02] finally / ensure 收尾
来源：http://wp.bookmarksfly.cn

Py:   try: f()⏎finally: cleanup()
来源：http://rj.hahajie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xk.colortex.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://nl.panjiajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://kx.bjjhwx.cn

Java: try { f(); } finally { cleanup(); }
来源：http://pr.jianghongdianzi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://rz.muxihuayi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://vj.521024.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://yo.wgjwhj.cn

[H03] 主动抛出异常
来源：http://sr.huixinmuqiang.cn

Py:   raise ValueError("错误信息")
来源：http://vo.chemitech.net.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vz.asd995.cn

JS:   throw new Error("错误信息");
来源：http://jg.muxihuayi.cn

TS:   throw new Error("错误信息");
来源：http://mb.hnjuh.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://yh.hahajie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sk.hahajie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://cb.szxytkj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://dz.hahajie.cn

[H04] 自定义异常类型
来源：http://ox.asd995.cn

Py:   class MyError(Exception): pass
来源：http://tn.huixiangedu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qa.nszjky.cn

JS:   class MyError extends Error {}
来源：http://np.521024.cn

TS:   class MyError extends Error {}
来源：http://uv.shxzukj.cn

Java: class MyException extends RuntimeException {}
来源：http://pk.bookmarksfly.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gv.panjiajie.cn

Ruby: class MyError < StandardError; end
来源：http://ml.yuntaijiaju.cn

C#:   class MyException : Exception {}
来源：http://ul.9csxet.cn

[H05] 捕获特定类型
来源：http://vj.szxytkj.cn

Py:   except ValueError as e:
来源：http://oi.9csxet.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vz.huixinmuqiang.cn

JS:   if (e instanceof TypeError) {}
来源：http://hv.9csxet.cn

TS:   if (e instanceof TypeError) {}
来源：http://pw.shxzukj.cn

Java: catch (IOException | SQLException e) {}
来源：http://dd.colortex.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ye.panjiajie.cn

Ruby: rescue ArgumentError => e
来源：http://sf.yuexingan06.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vj.nicolike.cn

[H06] 可选值 / 空值安全访问
来源：http://ij.huixiangedu.cn

Py:   value = d.get("k") or default
来源：http://oa.bookmarksfly.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kf.chemitech.net.cn

JS:   obj?.a?.b;  d ?? default
来源：http://wz.yuexingan06.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vl.shxzskj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nl.colortex.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fw.szsharing.cn

Ruby: d&.dig(:a, :b)
来源：http://rr.huixinmuqiang.cn

C#:   obj?.A?.B ?? default
来源：http://wx.bjjhwx.cn

[H07] 断言
来源：http://sk.bookmarksfly.cn

Py:   assert x > 0, "必须为正"
来源：http://ks.hahajie.cn

PHP:  assert($x > 0);
来源：http://rz.asd995.cn

JS:   console.assert(x > 0);
来源：http://sy.chemitech.net.cn

TS:   console.assert(x > 0);
来源：http://yf.panjiajie.cn

Java: assert x > 0 : "必须为正";
来源：http://hq.9csxet.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rz.huixinmuqiang.cn

Ruby: raise "必须为正" unless x > 0
来源：http://gw.szxytkj.cn

C#:   Debug.Assert(x > 0);
来源：http://af.szxytkj.cn

[H08] 获取错误信息与堆栈
来源：http://vz.huixinmuqiang.cn

Py:   str(e);  traceback.format_exc()
来源：http://ee.9csxet.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pz.yuexingan06.cn

JS:   e.message;  e.stack
来源：http://wo.chemitech.net.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://zj.521024.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://zs.shxzukj.cn

Go:   err.Error()
来源：http://ce.9csxet.cn

Ruby: e.message;  e.backtrace
来源：http://mh.huanxung.cn

C#:   e.Message;  e.StackTrace
来源：http://pg.shtwfgs.cn

[H09] 带错误码的异常
来源：http://vc.muxihuayi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lj.bjjhwx.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ga.shtwfgs.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rl.521024.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cs.shtwfgs.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zd.huixinmuqiang.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vh.colortex.cn

Ruby: raise MyError.new("fail", 500)
来源：http://xk.wgjwhj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://cx.hahajie.cn

[H10] 资源自动释放
来源：http://zi.shxzskj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ko.521024.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ku.shtwfgs.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://eg.chemitech.net.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qo.hnjuh.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bd.nszjky.cn

Go:   defer f.Close()
来源：http://uq.muxihuayi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ov.hnjuh.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vp.shtwfgs.cn

================================================================================
来源：http://oy.jctech888.com.cn

I. 正则表达式
来源：http://kb.huanxung.cn

================================================================================
来源：http://ud.newstarts.cn

[I01] 判断是否匹配
来源：http://zr.yuexingan06.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cv.chemitech.net.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ox.gzmigu.cn

JS:   /\d+/.test(s)
来源：http://pb.colortex.cn

TS:   /\d+/.test(s)
来源：http://xh.newstarts.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://op.521024.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://au.newstarts.cn

Ruby: s.match?(/\d+/)
来源：http://el.lnxyls.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fo.chemitech.net.cn

[I02] 提取所有匹配
来源：http://jd.nszjky.cn

Py:   re.findall(r"\d+", s)
来源：http://lk.panjiajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ud.asd995.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rl.521024.cn

TS:   s.match(/\d+/g)
来源：http://gp.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rc.hahajie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qe.shtwfgs.cn

Ruby: s.scan(/\d+/)
来源：http://vs.wgjwhj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zy.szxytkj.cn

[I03] 提取捕获分组
来源：http://lp.szxytkj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qq.9csxet.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wg.nicolike.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vc.gzmigu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hm.huanxung.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kq.haigaiapp.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wb.hnjuh.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vr.hahajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ps.wgjwhj.cn

[I04] 正则替换
来源：http://pf.jctech888.com.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ec.lnxyls.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dt.yuexingan06.cn

JS:   s.replace(/\d+/g, "#")
来源：http://nk.haigaiapp.cn

TS:   s.replace(/\d+/g, "#")
来源：http://fp.lnxyls.cn

Java: s.replaceAll("\\d+", "#")
来源：http://gk.panjiajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://vh.haigaiapp.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://up.shxzukj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kk.colortex.cn

[I05] 按正则拆分
来源：http://ex.huanxung.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://mg.yuexingan06.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ro.huixiangedu.cn

JS:   s.split(/\s*,\s*/)
来源：http://om.shxzskj.cn

TS:   s.split(/\s*,\s*/)
来源：http://rj.shtwfgs.cn

Java: s.split("\\s*,\\s*")
来源：http://eu.9csxet.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sx.jianghongdianzi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bt.yuntaijiaju.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nh.nicolike.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qr.jianghongdianzi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wy.hahajie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bo.wgjwhj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ad.panjiajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ko.jctech888.com.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gx.shtwfgs.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ve.szxytkj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zz.shxzskj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ng.huixiangedu.cn

[I07] 忽略大小写与多行模式
来源：http://zt.521024.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ld.szxytkj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cg.szsharing.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bx.nicolike.cn

TS:   /error/gim
来源：http://bl.szsharing.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jp.shxzskj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tw.9csxet.cn

Ruby: s.scan(/error/i)
来源：http://hi.asd995.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://aq.yuexingan06.cn

[I08] 贪婪与非贪婪匹配
来源：http://pu.lnxyls.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ny.asd995.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vi.shtwfgs.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bw.wgjwhj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wz.hnjuh.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zv.bjjhwx.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ff.nszjky.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kn.gzmigu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dw.huixinmuqiang.cn

================================================================================
来源：http://xz.szxytkj.cn

J. 日期与时间
来源：http://oy.shxzskj.cn

================================================================================
来源：http://ki.huixiangedu.cn

[J01] 获取当前时间
来源：http://ze.shxzskj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://kw.gzmigu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zn.huixiangedu.cn

JS:   new Date();  Date.now()
来源：http://sr.szsharing.cn

TS:   new Date();  Date.now()
来源：http://ge.muxihuayi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ky.colortex.cn

Go:   time.Now()
来源：http://hs.bookmarksfly.cn

Ruby: Time.now
来源：http://kk.shtwfgs.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zv.newstarts.cn

[J02] 格式化输出
来源：http://pa.szsharing.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uh.chemitech.net.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://sz.nicolike.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://us.lnxyls.cn

TS:   d.toISOString()
来源：http://ho.jianghongdianzi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kr.bookmarksfly.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ck.szxytkj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mn.lnxyls.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bz.nszjky.cn

[J03] 字符串解析为日期
来源：http://te.nszjky.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bx.huixinmuqiang.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ml.yuexingan06.cn

JS:   new Date("2024-01-02")
来源：http://wt.nszjky.cn

TS:   new Date("2024-01-02")
来源：http://xg.newstarts.cn

Java: LocalDate.parse("2024-01-02")
来源：http://nm.nicolike.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://im.szxytkj.cn

Ruby: Date.parse("2024-01-02")
来源：http://rt.shtwfgs.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mc.nszjky.cn

[J04] 时间戳与日期互转
来源：http://cl.yuexingan06.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xk.shtwfgs.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tn.yuexingan06.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fv.yuntaijiaju.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ta.bjjhwx.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qf.nszjky.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ke.haigaiapp.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ps.huanxung.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://po.szxytkj.cn

[J05] 时间加减（加 7 天）
来源：http://ve.521024.cn

Py:   now + timedelta(days=7)
来源：http://mm.wgjwhj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xo.shtwfgs.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xh.lnxyls.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gh.yuexingan06.cn

Java: LocalDate.now().plusDays(7)
来源：http://nx.nicolike.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://eh.colortex.cn

Ruby: Time.now + 7 * 86400
来源：http://kh.hahajie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://lk.hnjuh.cn

[J06] 计算两时间之差
来源：http://tj.shxzukj.cn

Py:   (end - start).total_seconds()
来源：http://vw.yuexingan06.cn

PHP:  $end->diff($start)->days;
来源：http://vi.bookmarksfly.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://js.hahajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sn.nicolike.cn

Java: Duration.between(start, end).toSeconds()
来源：http://pw.haigaiapp.cn

Go:   end.Sub(start).Hours()
来源：http://jt.shtwfgs.cn

Ruby: end - start                 # 返回秒数
来源：http://lb.szxytkj.cn

C#:   (end - start).TotalSeconds
来源：http://hw.hnjuh.cn

[J07] 比较两个日期
来源：http://ip.szxytkj.cn

Py:   d1 < d2;  d1 == d2
来源：http://xv.yuntaijiaju.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ur.wgjwhj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://lb.asd995.cn

TS:   d1.getTime() < d2.getTime()
来源：http://sa.nszjky.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xo.asd995.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rf.chemitech.net.cn

Ruby: d1 < d2;  d1 == d2
来源：http://tz.jianghongdianzi.cn

C#:   d1 < d2;  d1 == d2
来源：http://ob.yuntaijiaju.cn

[J08] 提取年月日与星期
来源：http://qn.asd995.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nx.colortex.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wq.nicolike.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://aa.9csxet.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xh.newstarts.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xh.haigaiapp.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vq.nicolike.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zm.panjiajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ve.jianghongdianzi.cn

[J09] 时区处理
来源：http://kq.panjiajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://by.szsharing.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rs.chemitech.net.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kf.haigaiapp.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mt.shxzskj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://iq.shtwfgs.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bg.shxzskj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cc.shtwfgs.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://di.huixiangedu.cn

[J10] 取今天 / 本月第一天
来源：http://at.shxzskj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://cv.9csxet.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bq.colortex.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fi.nicolike.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ft.yuntaijiaju.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jw.lnxyls.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dt.yuexingan06.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ye.muxihuayi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mm.hnjuh.cn

================================================================================
来源：http://sh.hahajie.cn

K. JSON 与序列化
来源：http://eo.shxzskj.cn

================================================================================
来源：http://go.yuexingan06.cn

[K01] 对象转 JSON 字符串
来源：http://yh.gzmigu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nn.yuntaijiaju.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fy.jctech888.com.cn

JS:   JSON.stringify(obj)
来源：http://oj.bookmarksfly.cn

TS:   JSON.stringify(obj)
来源：http://mu.shxzukj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vt.nszjky.cn

Go:   json.Marshal(obj)
来源：http://mr.nszjky.cn

Ruby: obj.to_json                                     // require "json"
来源：http://fb.nszjky.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://oc.bjjhwx.cn

[K02] JSON 字符串转对象
来源：http://vc.jctech888.com.cn

Py:   json.loads(s)
来源：http://ku.jctech888.com.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://it.muxihuayi.cn

JS:   JSON.parse(s)
来源：http://sy.bjjhwx.cn


<!-- 参考信息 -->