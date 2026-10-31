代发 wailian999

C#:   record User(string Name, int Age);
来源：http://pe.bookmarksfly.cn

[G15] 枚举
来源：http://cm.hnjuh.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://al.shxzskj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://jw.chemitech.net.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pi.huixinmuqiang.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yf.jianghongdianzi.cn

Java: enum Color { RED, GREEN }
来源：http://zb.bjjhwx.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xm.shxzukj.cn

Ruby: Color = %i[red green].freeze
来源：http://pk.nszjky.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ot.szxytkj.cn

[G16] 对象转数组 / 字典
来源：http://rq.bjjhwx.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ac.huixiangedu.cn

PHP:  get_object_vars($obj);
来源：http://bw.szsharing.cn

JS:   Object.entries(obj)
来源：http://ut.colortex.cn

TS:   Object.entries(obj)
来源：http://wl.colortex.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://co.chemitech.net.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://fr.chemitech.net.cn

Ruby: obj.instance_variables
来源：http://oe.newstarts.cn

C#:   // 用反射或 System.Text.Json
来源：http://ug.jianghongdianzi.cn

================================================================================
来源：http://dd.szsharing.cn

H. 异常与错误处理
来源：http://ej.521024.cn

================================================================================
来源：http://mg.jctech888.com.cn

[H01] try / catch 基础
来源：http://rd.shxzukj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hu.huixinmuqiang.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vq.szxytkj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vt.gzmigu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ne.jianghongdianzi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zl.szxytkj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fx.nicolike.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fe.nicolike.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lb.huixiangedu.cn

[H02] finally / ensure 收尾
来源：http://nz.nszjky.cn

Py:   try: f()⏎finally: cleanup()
来源：http://wg.shtwfgs.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://cm.wgjwhj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ek.bookmarksfly.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://lp.chemitech.net.cn

Java: try { f(); } finally { cleanup(); }
来源：http://kb.asd995.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://go.521024.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://pc.nszjky.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ou.gzmigu.cn

[H03] 主动抛出异常
来源：http://rz.shxzskj.cn

Py:   raise ValueError("错误信息")
来源：http://xo.huixinmuqiang.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ki.hahajie.cn

JS:   throw new Error("错误信息");
来源：http://rl.huanxung.cn

TS:   throw new Error("错误信息");
来源：http://fj.nicolike.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://uc.9csxet.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ia.chemitech.net.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://pw.yuexingan06.cn

C#:   throw new ArgumentException("错误信息");
来源：http://lf.szsharing.cn

[H04] 自定义异常类型
来源：http://og.huixiangedu.cn

Py:   class MyError(Exception): pass
来源：http://es.521024.cn

PHP:  class MyError extends RuntimeException {}
来源：http://mn.wgjwhj.cn

JS:   class MyError extends Error {}
来源：http://aj.nicolike.cn

TS:   class MyError extends Error {}
来源：http://oq.bjjhwx.cn

Java: class MyException extends RuntimeException {}
来源：http://lh.yuntaijiaju.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ua.yuntaijiaju.cn

Ruby: class MyError < StandardError; end
来源：http://kd.bjjhwx.cn

C#:   class MyException : Exception {}
来源：http://cu.bjjhwx.cn

[H05] 捕获特定类型
来源：http://rx.yuntaijiaju.cn

Py:   except ValueError as e:
来源：http://cu.newstarts.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pb.panjiajie.cn

JS:   if (e instanceof TypeError) {}
来源：http://qn.9csxet.cn

TS:   if (e instanceof TypeError) {}
来源：http://mw.asd995.cn

Java: catch (IOException | SQLException e) {}
来源：http://wn.wgjwhj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yw.szxytkj.cn

Ruby: rescue ArgumentError => e
来源：http://fj.bookmarksfly.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://so.colortex.cn

[H06] 可选值 / 空值安全访问
来源：http://wx.huixiangedu.cn

Py:   value = d.get("k") or default
来源：http://nf.huixinmuqiang.cn

PHP:  $v = $d["k"] ?? null;
来源：http://zx.wgjwhj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://nt.gzmigu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://et.huixiangedu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fr.yuntaijiaju.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://yc.szsharing.cn

Ruby: d&.dig(:a, :b)
来源：http://al.nicolike.cn

C#:   obj?.A?.B ?? default
来源：http://jo.hnjuh.cn

[H07] 断言
来源：http://vk.chemitech.net.cn

Py:   assert x > 0, "必须为正"
来源：http://ft.huixinmuqiang.cn

PHP:  assert($x > 0);
来源：http://zm.chemitech.net.cn

JS:   console.assert(x > 0);
来源：http://jl.huanxung.cn

TS:   console.assert(x > 0);
来源：http://ge.gzmigu.cn

Java: assert x > 0 : "必须为正";
来源：http://nx.shxzukj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ga.panjiajie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wo.nicolike.cn

C#:   Debug.Assert(x > 0);
来源：http://bv.newstarts.cn

[H08] 获取错误信息与堆栈
来源：http://iy.bjjhwx.cn

Py:   str(e);  traceback.format_exc()
来源：http://an.bookmarksfly.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wj.huixiangedu.cn

JS:   e.message;  e.stack
来源：http://ss.asd995.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://il.yuntaijiaju.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://bh.chemitech.net.cn

Go:   err.Error()
来源：http://hz.hahajie.cn

Ruby: e.message;  e.backtrace
来源：http://gj.jctech888.com.cn

C#:   e.Message;  e.StackTrace
来源：http://fb.gzmigu.cn

[H09] 带错误码的异常
来源：http://lo.haigaiapp.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mu.yuexingan06.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://fa.muxihuayi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dp.panjiajie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cm.panjiajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://md.shxzukj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://di.newstarts.cn

Ruby: raise MyError.new("fail", 500)
来源：http://fz.gzmigu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://mo.shxzukj.cn

[H10] 资源自动释放
来源：http://oy.nszjky.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://si.yuexingan06.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jk.yuntaijiaju.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yq.hnjuh.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jw.huixinmuqiang.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vb.colortex.cn

Go:   defer f.Close()
来源：http://mt.haigaiapp.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gr.szxytkj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kj.panjiajie.cn

================================================================================
来源：http://qy.szxytkj.cn

I. 正则表达式
来源：http://qr.colortex.cn

================================================================================
来源：http://sx.huixinmuqiang.cn

[I01] 判断是否匹配
来源：http://ob.chemitech.net.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://oz.panjiajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vy.shxzukj.cn

JS:   /\d+/.test(s)
来源：http://ls.muxihuayi.cn

TS:   /\d+/.test(s)
来源：http://bh.nicolike.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nw.hahajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gy.muxihuayi.cn

Ruby: s.match?(/\d+/)
来源：http://iq.szxytkj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bi.huanxung.cn

[I02] 提取所有匹配
来源：http://rr.muxihuayi.cn

Py:   re.findall(r"\d+", s)
来源：http://uq.chemitech.net.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://av.huixinmuqiang.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xs.nszjky.cn

TS:   s.match(/\d+/g)
来源：http://te.szsharing.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://aq.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qt.haigaiapp.cn

Ruby: s.scan(/\d+/)
来源：http://bp.nicolike.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gr.yuexingan06.cn

[I03] 提取捕获分组
来源：http://hn.yuntaijiaju.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cp.9csxet.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yg.newstarts.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kg.yuexingan06.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fm.shtwfgs.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qg.newstarts.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yw.muxihuayi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jl.nszjky.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://px.jctech888.com.cn

[I04] 正则替换
来源：http://mz.wgjwhj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ev.yuntaijiaju.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vb.shxzskj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://hb.nicolike.cn

TS:   s.replace(/\d+/g, "#")
来源：http://nd.yuntaijiaju.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jf.jianghongdianzi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ee.szxytkj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://cy.gzmigu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nk.nicolike.cn

[I05] 按正则拆分
来源：http://lj.jianghongdianzi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://tj.bjjhwx.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rr.bjjhwx.cn

JS:   s.split(/\s*,\s*/)
来源：http://tz.bookmarksfly.cn

TS:   s.split(/\s*,\s*/)
来源：http://xo.panjiajie.cn

Java: s.split("\\s*,\\s*")
来源：http://gj.bjjhwx.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sg.bjjhwx.cn

Ruby: s.split(/\s*,\s*/)
来源：http://yf.huixinmuqiang.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kz.nszjky.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ox.panjiajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rj.szxytkj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fb.szsharing.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hl.lnxyls.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mg.jianghongdianzi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ym.huixiangedu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://er.hahajie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sf.lnxyls.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ya.gzmigu.cn

[I07] 忽略大小写与多行模式
来源：http://ur.yuntaijiaju.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rw.newstarts.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xo.shtwfgs.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vj.szxytkj.cn

TS:   /error/gim
来源：http://wz.wgjwhj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ob.wgjwhj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nd.wgjwhj.cn

Ruby: s.scan(/error/i)
来源：http://rc.9csxet.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://av.colortex.cn

[I08] 贪婪与非贪婪匹配
来源：http://wy.jianghongdianzi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://de.shxzskj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xf.shxzskj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://by.szsharing.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://oi.lnxyls.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bz.9csxet.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kk.bjjhwx.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://op.jianghongdianzi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ll.521024.cn

================================================================================
来源：http://xa.chemitech.net.cn

J. 日期与时间
来源：http://dh.szxytkj.cn

================================================================================
来源：http://vr.shxzskj.cn

[J01] 获取当前时间
来源：http://kj.hahajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://dn.bjjhwx.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ja.jianghongdianzi.cn

JS:   new Date();  Date.now()
来源：http://ny.bjjhwx.cn

TS:   new Date();  Date.now()
来源：http://pw.bookmarksfly.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://to.shxzskj.cn

Go:   time.Now()
来源：http://dl.szxytkj.cn

Ruby: Time.now
来源：http://zq.lnxyls.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sb.szxytkj.cn

[J02] 格式化输出
来源：http://yh.newstarts.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sg.hahajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nt.jctech888.com.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://iq.colortex.cn

TS:   d.toISOString()
来源：http://zp.bjjhwx.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ej.521024.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pi.chemitech.net.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rj.9csxet.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://aw.huixinmuqiang.cn

[J03] 字符串解析为日期
来源：http://fa.jianghongdianzi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nx.wgjwhj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wf.bookmarksfly.cn

JS:   new Date("2024-01-02")
来源：http://gl.wgjwhj.cn

TS:   new Date("2024-01-02")
来源：http://cw.colortex.cn

Java: LocalDate.parse("2024-01-02")
来源：http://pm.shtwfgs.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vx.huixinmuqiang.cn

Ruby: Date.parse("2024-01-02")
来源：http://sa.shtwfgs.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ms.wgjwhj.cn

[J04] 时间戳与日期互转
来源：http://dj.nszjky.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xc.shxzukj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rv.521024.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vd.521024.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://gn.szxytkj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rm.bjjhwx.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bq.szsharing.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gf.chemitech.net.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xp.nszjky.cn

[J05] 时间加减（加 7 天）
来源：http://yu.shxzskj.cn

Py:   now + timedelta(days=7)
来源：http://bq.szxytkj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://za.huixiangedu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xm.yuntaijiaju.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gu.nicolike.cn

Java: LocalDate.now().plusDays(7)
来源：http://fp.lnxyls.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ri.521024.cn

Ruby: Time.now + 7 * 86400
来源：http://us.521024.cn

C#:   DateTime.Now.AddDays(7)
来源：http://wx.panjiajie.cn

[J06] 计算两时间之差
来源：http://eg.shxzukj.cn

Py:   (end - start).total_seconds()
来源：http://po.521024.cn

PHP:  $end->diff($start)->days;
来源：http://ig.newstarts.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ef.muxihuayi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vv.jctech888.com.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ru.jianghongdianzi.cn

Go:   end.Sub(start).Hours()
来源：http://hu.wgjwhj.cn

Ruby: end - start                 # 返回秒数
来源：http://qd.bjjhwx.cn

C#:   (end - start).TotalSeconds
来源：http://bw.yuntaijiaju.cn

[J07] 比较两个日期
来源：http://ad.shxzskj.cn

Py:   d1 < d2;  d1 == d2
来源：http://ia.nicolike.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dh.muxihuayi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://tz.shtwfgs.cn

TS:   d1.getTime() < d2.getTime()
来源：http://sx.shxzukj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vy.gzmigu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ev.muxihuayi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://mt.huanxung.cn

C#:   d1 < d2;  d1 == d2
来源：http://yl.huixinmuqiang.cn

[J08] 提取年月日与星期
来源：http://fq.521024.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ek.yuntaijiaju.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ep.colortex.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hl.shxzukj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://si.huixinmuqiang.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mk.yuntaijiaju.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yz.haigaiapp.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://am.bookmarksfly.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xt.muxihuayi.cn

[J09] 时区处理
来源：http://fr.haigaiapp.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mk.yuexingan06.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://to.shxzskj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fy.hnjuh.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gg.huixiangedu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vn.hahajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sa.hnjuh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://bk.gzmigu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nj.huanxung.cn

[J10] 取今天 / 本月第一天
来源：http://yh.9csxet.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://iw.9csxet.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ym.jianghongdianzi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kf.nszjky.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xb.colortex.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yl.wgjwhj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yx.nszjky.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jp.szsharing.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yh.gzmigu.cn

================================================================================
来源：http://sn.szsharing.cn

K. JSON 与序列化
来源：http://xt.huixinmuqiang.cn

================================================================================
来源：http://no.asd995.cn

[K01] 对象转 JSON 字符串
来源：http://dw.colortex.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://oy.yuexingan06.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ct.huixiangedu.cn

JS:   JSON.stringify(obj)
来源：http://rv.bjjhwx.cn

TS:   JSON.stringify(obj)
来源：http://fx.haigaiapp.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ws.yuntaijiaju.cn

Go:   json.Marshal(obj)
来源：http://ky.szxytkj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ys.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://px.huixinmuqiang.cn

[K02] JSON 字符串转对象
来源：http://ax.asd995.cn

Py:   json.loads(s)
来源：http://so.colortex.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lb.nszjky.cn

JS:   JSON.parse(s)
来源：http://xa.huixiangedu.cn

TS:   JSON.parse(s)
来源：http://wn.shxzskj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vg.shtwfgs.cn

Go:   json.Unmarshal(data, &v)
来源：http://bz.colortex.cn

Ruby: JSON.parse(s)
来源：http://do.szsharing.cn


<!-- 参考信息 -->