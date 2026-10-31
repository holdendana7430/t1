代发 wailian999

Java: u instanceof User
来源：http://nu.haigaiapp.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://wg.szsharing.cn

Ruby: u.is_a?(User)
来源：http://jw.panjiajie.cn

C#:   u is User
来源：http://tq.shxzskj.cn

[G14] 数据类 / record
来源：http://xn.huixinmuqiang.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sh.yuexingan06.cn

PHP:  // 用 readonly 属性模拟
来源：http://yd.nicolike.cn

JS:   // 无内置：普通类或对象字面量
来源：http://xe.shtwfgs.cn

TS:   type User = { name: string; age: number };
来源：http://ax.yuexingan06.cn

Java: record User(String name, int age) {}
来源：http://gy.lnxyls.cn

Go:   type User struct { Name string; Age int }
来源：http://nx.haigaiapp.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lv.muxihuayi.cn

C#:   record User(string Name, int Age);
来源：http://zn.shxzskj.cn

[G15] 枚举
来源：http://wi.jianghongdianzi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ip.huixinmuqiang.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://qu.wgjwhj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ai.521024.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fv.szsharing.cn

Java: enum Color { RED, GREEN }
来源：http://ui.asd995.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fe.colortex.cn

Ruby: Color = %i[red green].freeze
来源：http://sz.shtwfgs.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pv.szxytkj.cn

[G16] 对象转数组 / 字典
来源：http://sq.haigaiapp.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uf.szsharing.cn

PHP:  get_object_vars($obj);
来源：http://ln.nszjky.cn

JS:   Object.entries(obj)
来源：http://oi.lnxyls.cn

TS:   Object.entries(obj)
来源：http://yb.szsharing.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nl.newstarts.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://oh.hahajie.cn

Ruby: obj.instance_variables
来源：http://be.chemitech.net.cn

C#:   // 用反射或 System.Text.Json
来源：http://yn.szxytkj.cn

================================================================================
来源：http://eb.huixinmuqiang.cn

H. 异常与错误处理
来源：http://mj.szxytkj.cn

================================================================================
来源：http://ee.nicolike.cn

[H01] try / catch 基础
来源：http://py.szxytkj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lk.9csxet.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ec.yuexingan06.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qf.huixinmuqiang.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qy.huixiangedu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ft.panjiajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kx.hnjuh.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://cb.chemitech.net.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ci.panjiajie.cn

[H02] finally / ensure 收尾
来源：http://iz.asd995.cn

Py:   try: f()⏎finally: cleanup()
来源：http://zz.colortex.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://su.jctech888.com.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://qj.jianghongdianzi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://zb.gzmigu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://uw.521024.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://wn.huixinmuqiang.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://an.wgjwhj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://zp.huixiangedu.cn

[H03] 主动抛出异常
来源：http://vr.huixiangedu.cn

Py:   raise ValueError("错误信息")
来源：http://rx.shxzukj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ep.asd995.cn

JS:   throw new Error("错误信息");
来源：http://fj.hahajie.cn

TS:   throw new Error("错误信息");
来源：http://mh.huixinmuqiang.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://hm.nszjky.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mo.huixiangedu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hi.jctech888.com.cn

C#:   throw new ArgumentException("错误信息");
来源：http://wd.shxzukj.cn

[H04] 自定义异常类型
来源：http://fb.9csxet.cn

Py:   class MyError(Exception): pass
来源：http://nt.colortex.cn

PHP:  class MyError extends RuntimeException {}
来源：http://cq.9csxet.cn

JS:   class MyError extends Error {}
来源：http://br.colortex.cn

TS:   class MyError extends Error {}
来源：http://qw.huixiangedu.cn

Java: class MyException extends RuntimeException {}
来源：http://kg.yuntaijiaju.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nu.panjiajie.cn

Ruby: class MyError < StandardError; end
来源：http://ec.nszjky.cn

C#:   class MyException : Exception {}
来源：http://ki.bjjhwx.cn

[H05] 捕获特定类型
来源：http://je.shxzukj.cn

Py:   except ValueError as e:
来源：http://bi.haigaiapp.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jm.szxytkj.cn

JS:   if (e instanceof TypeError) {}
来源：http://kf.muxihuayi.cn

TS:   if (e instanceof TypeError) {}
来源：http://ph.yuntaijiaju.cn

Java: catch (IOException | SQLException e) {}
来源：http://et.hahajie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rq.yuntaijiaju.cn

Ruby: rescue ArgumentError => e
来源：http://zp.jianghongdianzi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zr.haigaiapp.cn

[H06] 可选值 / 空值安全访问
来源：http://oz.haigaiapp.cn

Py:   value = d.get("k") or default
来源：http://yj.panjiajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://sq.yuexingan06.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ew.colortex.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ya.shxzskj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rv.colortex.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://me.jctech888.com.cn

Ruby: d&.dig(:a, :b)
来源：http://uy.hahajie.cn

C#:   obj?.A?.B ?? default
来源：http://th.jctech888.com.cn

[H07] 断言
来源：http://wl.huanxung.cn

Py:   assert x > 0, "必须为正"
来源：http://bn.jianghongdianzi.cn

PHP:  assert($x > 0);
来源：http://nu.wgjwhj.cn

JS:   console.assert(x > 0);
来源：http://ex.jctech888.com.cn

TS:   console.assert(x > 0);
来源：http://xq.bjjhwx.cn

Java: assert x > 0 : "必须为正";
来源：http://ay.lnxyls.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wd.yuntaijiaju.cn

Ruby: raise "必须为正" unless x > 0
来源：http://sh.panjiajie.cn

C#:   Debug.Assert(x > 0);
来源：http://by.huixinmuqiang.cn

[H08] 获取错误信息与堆栈
来源：http://dr.huixiangedu.cn

Py:   str(e);  traceback.format_exc()
来源：http://ej.muxihuayi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pv.shtwfgs.cn

JS:   e.message;  e.stack
来源：http://wc.shxzskj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://yz.yuexingan06.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://gd.gzmigu.cn

Go:   err.Error()
来源：http://oy.hahajie.cn

Ruby: e.message;  e.backtrace
来源：http://qn.nszjky.cn

C#:   e.Message;  e.StackTrace
来源：http://it.szxytkj.cn

[H09] 带错误码的异常
来源：http://qh.bjjhwx.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yq.haigaiapp.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://wg.panjiajie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://px.newstarts.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ec.yuntaijiaju.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sx.lnxyls.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vv.nszjky.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jr.hnjuh.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ae.yuntaijiaju.cn

[H10] 资源自动释放
来源：http://re.muxihuayi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ep.wgjwhj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rp.bookmarksfly.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ho.nszjky.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mv.muxihuayi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://yq.huixiangedu.cn

Go:   defer f.Close()
来源：http://wm.bjjhwx.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zc.521024.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ap.nszjky.cn

================================================================================
来源：http://ue.shxzskj.cn

I. 正则表达式
来源：http://xi.hnjuh.cn

================================================================================
来源：http://gu.shxzukj.cn

[I01] 判断是否匹配
来源：http://wr.haigaiapp.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ux.szxytkj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://th.bjjhwx.cn

JS:   /\d+/.test(s)
来源：http://pg.9csxet.cn

TS:   /\d+/.test(s)
来源：http://sm.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ku.wgjwhj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ix.huixinmuqiang.cn

Ruby: s.match?(/\d+/)
来源：http://js.szxytkj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://av.shxzskj.cn

[I02] 提取所有匹配
来源：http://je.shxzskj.cn

Py:   re.findall(r"\d+", s)
来源：http://eo.haigaiapp.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lb.szxytkj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cx.yuntaijiaju.cn

TS:   s.match(/\d+/g)
来源：http://ao.newstarts.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://uv.jianghongdianzi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ld.yuntaijiaju.cn

Ruby: s.scan(/\d+/)
来源：http://jl.hnjuh.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pv.521024.cn

[I03] 提取捕获分组
来源：http://ye.haigaiapp.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vu.nszjky.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jq.shtwfgs.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://is.jianghongdianzi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dk.521024.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nq.szsharing.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://om.nicolike.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qm.jianghongdianzi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dm.huixinmuqiang.cn

[I04] 正则替换
来源：http://gm.huanxung.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ci.panjiajie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://eo.jianghongdianzi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://lb.muxihuayi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://nj.nicolike.cn

Java: s.replaceAll("\\d+", "#")
来源：http://iz.521024.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://cp.muxihuayi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://kr.shxzskj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pw.haigaiapp.cn

[I05] 按正则拆分
来源：http://wb.huixinmuqiang.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://rk.shxzskj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kl.shtwfgs.cn

JS:   s.split(/\s*,\s*/)
来源：http://og.colortex.cn

TS:   s.split(/\s*,\s*/)
来源：http://ti.lnxyls.cn

Java: s.split("\\s*,\\s*")
来源：http://gl.muxihuayi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ic.hnjuh.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bv.bjjhwx.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jv.huixinmuqiang.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vn.lnxyls.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rz.9csxet.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://oe.asd995.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ee.huanxung.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zf.shtwfgs.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xs.muxihuayi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ha.9csxet.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://be.nicolike.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bu.chemitech.net.cn

[I07] 忽略大小写与多行模式
来源：http://hs.521024.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lh.jctech888.com.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uh.9csxet.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://td.jctech888.com.cn

TS:   /error/gim
来源：http://ao.bookmarksfly.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ro.shxzskj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qn.shxzskj.cn

Ruby: s.scan(/error/i)
来源：http://lb.jianghongdianzi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://oe.huanxung.cn

[I08] 贪婪与非贪婪匹配
来源：http://fe.colortex.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jv.panjiajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tf.bjjhwx.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uw.gzmigu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pb.yuexingan06.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://sh.hnjuh.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ms.wgjwhj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ch.asd995.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gv.yuntaijiaju.cn

================================================================================
来源：http://rl.panjiajie.cn

J. 日期与时间
来源：http://sb.521024.cn

================================================================================
来源：http://yv.nszjky.cn

[J01] 获取当前时间
来源：http://hx.colortex.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://sf.lnxyls.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gg.yuexingan06.cn

JS:   new Date();  Date.now()
来源：http://jh.huixinmuqiang.cn

TS:   new Date();  Date.now()
来源：http://as.yuntaijiaju.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://bf.newstarts.cn

Go:   time.Now()
来源：http://ys.panjiajie.cn

Ruby: Time.now
来源：http://qu.nszjky.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ee.521024.cn

[J02] 格式化输出
来源：http://ku.panjiajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wj.yuexingan06.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zk.colortex.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lr.chemitech.net.cn

TS:   d.toISOString()
来源：http://rt.9csxet.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lk.muxihuayi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yi.bjjhwx.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hb.szxytkj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rr.hahajie.cn

[J03] 字符串解析为日期
来源：http://zv.newstarts.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://il.nicolike.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://en.bookmarksfly.cn

JS:   new Date("2024-01-02")
来源：http://kl.muxihuayi.cn

TS:   new Date("2024-01-02")
来源：http://yo.shxzskj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qv.nszjky.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://og.lnxyls.cn

Ruby: Date.parse("2024-01-02")
来源：http://uq.huixiangedu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sm.bjjhwx.cn

[J04] 时间戳与日期互转
来源：http://ns.shtwfgs.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qx.gzmigu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gc.521024.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gg.yuntaijiaju.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://gt.lnxyls.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://so.9csxet.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zw.hahajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xx.bjjhwx.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://or.nicolike.cn

[J05] 时间加减（加 7 天）
来源：http://jd.szxytkj.cn

Py:   now + timedelta(days=7)
来源：http://sp.chemitech.net.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://sg.panjiajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wn.szxytkj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bo.huixinmuqiang.cn

Java: LocalDate.now().plusDays(7)
来源：http://oc.muxihuayi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dq.shxzskj.cn

Ruby: Time.now + 7 * 86400
来源：http://ct.haigaiapp.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ly.asd995.cn

[J06] 计算两时间之差
来源：http://qn.newstarts.cn

Py:   (end - start).total_seconds()
来源：http://kt.9csxet.cn

PHP:  $end->diff($start)->days;
来源：http://zm.nicolike.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://er.521024.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://il.yuexingan06.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qk.asd995.cn

Go:   end.Sub(start).Hours()
来源：http://yh.chemitech.net.cn

Ruby: end - start                 # 返回秒数
来源：http://ao.jianghongdianzi.cn

C#:   (end - start).TotalSeconds
来源：http://ws.shtwfgs.cn

[J07] 比较两个日期
来源：http://nk.yuntaijiaju.cn

Py:   d1 < d2;  d1 == d2
来源：http://ix.panjiajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hb.newstarts.cn

JS:   d1.getTime() < d2.getTime()
来源：http://sj.nszjky.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ar.jctech888.com.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lj.haigaiapp.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jp.yuexingan06.cn

Ruby: d1 < d2;  d1 == d2
来源：http://fz.hahajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://ou.521024.cn

[J08] 提取年月日与星期
来源：http://uj.shtwfgs.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xy.yuntaijiaju.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fr.521024.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ve.muxihuayi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zc.hahajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dc.nszjky.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ab.huixinmuqiang.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xx.shxzskj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qc.jctech888.com.cn

[J09] 时区处理
来源：http://rt.9csxet.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://oa.gzmigu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wm.huixiangedu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ns.newstarts.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://io.huixinmuqiang.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zk.wgjwhj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kj.shxzukj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://gx.nicolike.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zu.jianghongdianzi.cn

[J10] 取今天 / 本月第一天
来源：http://pc.yuexingan06.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://hi.nicolike.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zx.haigaiapp.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://io.yuntaijiaju.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cl.nszjky.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dt.shxzukj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://oz.haigaiapp.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mu.9csxet.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://sf.gzmigu.cn

================================================================================
来源：http://pc.nicolike.cn

K. JSON 与序列化
来源：http://wz.bookmarksfly.cn

================================================================================
来源：http://vn.yuexingan06.cn

[K01] 对象转 JSON 字符串
来源：http://sy.hnjuh.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://iv.nicolike.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yb.bookmarksfly.cn

JS:   JSON.stringify(obj)
来源：http://zs.newstarts.cn

TS:   JSON.stringify(obj)
来源：http://tp.yuntaijiaju.cn


<!-- 参考信息 -->