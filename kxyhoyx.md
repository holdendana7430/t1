代发 wailian999

Py:   isinstance(u, User)
来源：http://gn.muxihuayi.cn

PHP:  $u instanceof User
来源：http://rm.lnxyls.cn

JS:   u instanceof User
来源：http://he.asd995.cn

TS:   u instanceof User
来源：http://ug.szsharing.cn

Java: u instanceof User
来源：http://kl.szsharing.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://uo.chemitech.net.cn

Ruby: u.is_a?(User)
来源：http://ep.chemitech.net.cn

C#:   u is User
来源：http://lg.shtwfgs.cn

[G14] 数据类 / record
来源：http://la.chemitech.net.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ii.shxzskj.cn

PHP:  // 用 readonly 属性模拟
来源：http://fa.muxihuayi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://bj.huixinmuqiang.cn

TS:   type User = { name: string; age: number };
来源：http://ba.bjjhwx.cn

Java: record User(String name, int age) {}
来源：http://xx.bookmarksfly.cn

Go:   type User struct { Name string; Age int }
来源：http://qf.jctech888.com.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://uf.asd995.cn

C#:   record User(string Name, int Age);
来源：http://me.shxzukj.cn

[G15] 枚举
来源：http://ut.bjjhwx.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pj.bjjhwx.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ta.szxytkj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://df.szxytkj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kr.huanxung.cn

Java: enum Color { RED, GREEN }
来源：http://yf.jctech888.com.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yd.jctech888.com.cn

Ruby: Color = %i[red green].freeze
来源：http://hm.huixinmuqiang.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hl.jctech888.com.cn

[G16] 对象转数组 / 字典
来源：http://es.yuntaijiaju.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bm.shtwfgs.cn

PHP:  get_object_vars($obj);
来源：http://uw.hnjuh.cn

JS:   Object.entries(obj)
来源：http://bu.huixiangedu.cn

TS:   Object.entries(obj)
来源：http://ld.haigaiapp.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://et.huanxung.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://uv.yuntaijiaju.cn

Ruby: obj.instance_variables
来源：http://tl.shxzukj.cn

C#:   // 用反射或 System.Text.Json
来源：http://bj.szsharing.cn

================================================================================
来源：http://io.shxzukj.cn

H. 异常与错误处理
来源：http://xf.szxytkj.cn

================================================================================
来源：http://za.bjjhwx.cn

[H01] try / catch 基础
来源：http://jj.9csxet.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qt.newstarts.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://un.asd995.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qr.bookmarksfly.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dr.shtwfgs.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xj.shxzskj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tj.lnxyls.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gl.panjiajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pp.shxzukj.cn

[H02] finally / ensure 收尾
来源：http://jk.huanxung.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ge.521024.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://vn.gzmigu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ut.nszjky.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://bj.jctech888.com.cn

Java: try { f(); } finally { cleanup(); }
来源：http://if.shtwfgs.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://vh.bjjhwx.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://yd.hahajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://fj.haigaiapp.cn

[H03] 主动抛出异常
来源：http://lr.hahajie.cn

Py:   raise ValueError("错误信息")
来源：http://ru.yuntaijiaju.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qq.asd995.cn

JS:   throw new Error("错误信息");
来源：http://db.shtwfgs.cn

TS:   throw new Error("错误信息");
来源：http://ga.huanxung.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://tj.wgjwhj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://go.szsharing.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://im.newstarts.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ii.jctech888.com.cn

[H04] 自定义异常类型
来源：http://rd.9csxet.cn

Py:   class MyError(Exception): pass
来源：http://bk.shtwfgs.cn

PHP:  class MyError extends RuntimeException {}
来源：http://or.newstarts.cn

JS:   class MyError extends Error {}
来源：http://jd.bjjhwx.cn

TS:   class MyError extends Error {}
来源：http://an.shxzukj.cn

Java: class MyException extends RuntimeException {}
来源：http://dr.haigaiapp.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nx.shxzukj.cn

Ruby: class MyError < StandardError; end
来源：http://yc.nszjky.cn

C#:   class MyException : Exception {}
来源：http://vq.521024.cn

[H05] 捕获特定类型
来源：http://uu.jctech888.com.cn

Py:   except ValueError as e:
来源：http://vk.szxytkj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gt.szxytkj.cn

JS:   if (e instanceof TypeError) {}
来源：http://gm.nicolike.cn

TS:   if (e instanceof TypeError) {}
来源：http://ph.shtwfgs.cn

Java: catch (IOException | SQLException e) {}
来源：http://np.nicolike.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://oj.szsharing.cn

Ruby: rescue ArgumentError => e
来源：http://wr.huixinmuqiang.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kk.nicolike.cn

[H06] 可选值 / 空值安全访问
来源：http://fu.gzmigu.cn

Py:   value = d.get("k") or default
来源：http://hm.nszjky.cn

PHP:  $v = $d["k"] ?? null;
来源：http://yn.hnjuh.cn

JS:   obj?.a?.b;  d ?? default
来源：http://fh.nicolike.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ly.huanxung.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vv.colortex.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fl.szsharing.cn

Ruby: d&.dig(:a, :b)
来源：http://ne.huanxung.cn

C#:   obj?.A?.B ?? default
来源：http://xt.shxzskj.cn

[H07] 断言
来源：http://av.newstarts.cn

Py:   assert x > 0, "必须为正"
来源：http://wc.huixiangedu.cn

PHP:  assert($x > 0);
来源：http://xd.lnxyls.cn

JS:   console.assert(x > 0);
来源：http://fd.nicolike.cn

TS:   console.assert(x > 0);
来源：http://ms.jianghongdianzi.cn

Java: assert x > 0 : "必须为正";
来源：http://tl.521024.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vn.521024.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ks.muxihuayi.cn

C#:   Debug.Assert(x > 0);
来源：http://cz.szxytkj.cn

[H08] 获取错误信息与堆栈
来源：http://ux.hahajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://bh.huixiangedu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ss.hahajie.cn

JS:   e.message;  e.stack
来源：http://rt.szxytkj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://nt.shtwfgs.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://md.newstarts.cn

Go:   err.Error()
来源：http://qf.nszjky.cn

Ruby: e.message;  e.backtrace
来源：http://mh.shxzskj.cn

C#:   e.Message;  e.StackTrace
来源：http://na.shtwfgs.cn

[H09] 带错误码的异常
来源：http://lq.colortex.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vb.asd995.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ng.asd995.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yq.huanxung.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cz.jianghongdianzi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mj.9csxet.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dw.521024.cn

Ruby: raise MyError.new("fail", 500)
来源：http://em.szsharing.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://wf.colortex.cn

[H10] 资源自动释放
来源：http://tg.colortex.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://nn.jctech888.com.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dc.shxzskj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bb.haigaiapp.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nq.asd995.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rh.hahajie.cn

Go:   defer f.Close()
来源：http://zc.chemitech.net.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dy.9csxet.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dv.asd995.cn

================================================================================
来源：http://ei.wgjwhj.cn

I. 正则表达式
来源：http://jd.nicolike.cn

================================================================================
来源：http://az.yuexingan06.cn

[I01] 判断是否匹配
来源：http://dv.shtwfgs.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ue.huanxung.cn

PHP:  preg_match('/\d+/', $s);
来源：http://lp.huixiangedu.cn

JS:   /\d+/.test(s)
来源：http://nx.shxzskj.cn

TS:   /\d+/.test(s)
来源：http://jr.hnjuh.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ya.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xt.szxytkj.cn

Ruby: s.match?(/\d+/)
来源：http://cp.nicolike.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gj.szxytkj.cn

[I02] 提取所有匹配
来源：http://px.jianghongdianzi.cn

Py:   re.findall(r"\d+", s)
来源：http://yr.bookmarksfly.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tb.panjiajie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ev.chemitech.net.cn

TS:   s.match(/\d+/g)
来源：http://qp.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cr.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://uc.colortex.cn

Ruby: s.scan(/\d+/)
来源：http://xl.hahajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nq.shtwfgs.cn

[I03] 提取捕获分组
来源：http://aq.yuexingan06.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bm.wgjwhj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://od.yuexingan06.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fg.chemitech.net.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ys.szsharing.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qy.shtwfgs.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gg.bjjhwx.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ye.colortex.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://va.521024.cn

[I04] 正则替换
来源：http://qd.lnxyls.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://il.hahajie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qu.haigaiapp.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pj.newstarts.cn

TS:   s.replace(/\d+/g, "#")
来源：http://sx.huixinmuqiang.cn

Java: s.replaceAll("\\d+", "#")
来源：http://qw.9csxet.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ft.muxihuayi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://pn.szxytkj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://io.huanxung.cn

[I05] 按正则拆分
来源：http://xc.hnjuh.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://lb.hahajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wa.huixiangedu.cn

JS:   s.split(/\s*,\s*/)
来源：http://rt.jianghongdianzi.cn

TS:   s.split(/\s*,\s*/)
来源：http://xm.colortex.cn

Java: s.split("\\s*,\\s*")
来源：http://kp.szsharing.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tf.huixinmuqiang.cn

Ruby: s.split(/\s*,\s*/)
来源：http://qr.huixiangedu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ce.nszjky.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ek.huixiangedu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://oy.chemitech.net.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sm.yuntaijiaju.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ly.szxytkj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://op.9csxet.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ep.hnjuh.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ym.9csxet.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dx.shtwfgs.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zq.asd995.cn

[I07] 忽略大小写与多行模式
来源：http://yh.jianghongdianzi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qy.9csxet.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fu.hnjuh.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://eb.haigaiapp.cn

TS:   /error/gim
来源：http://pz.521024.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fz.nicolike.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ja.hahajie.cn

Ruby: s.scan(/error/i)
来源：http://mz.huixiangedu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://do.huixiangedu.cn

[I08] 贪婪与非贪婪匹配
来源：http://dz.muxihuayi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://se.9csxet.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ju.shtwfgs.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://je.jianghongdianzi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mq.huixinmuqiang.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://pw.asd995.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://iy.muxihuayi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://de.szxytkj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tl.nicolike.cn

================================================================================
来源：http://nb.chemitech.net.cn

J. 日期与时间
来源：http://cs.9csxet.cn

================================================================================
来源：http://oz.jianghongdianzi.cn

[J01] 获取当前时间
来源：http://vf.huixiangedu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://lq.newstarts.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tt.gzmigu.cn

JS:   new Date();  Date.now()
来源：http://ti.haigaiapp.cn

TS:   new Date();  Date.now()
来源：http://kh.shtwfgs.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://xk.haigaiapp.cn

Go:   time.Now()
来源：http://ko.yuexingan06.cn

Ruby: Time.now
来源：http://ry.shtwfgs.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lj.521024.cn

[J02] 格式化输出
来源：http://ga.panjiajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yn.shtwfgs.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mw.521024.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pm.hnjuh.cn

TS:   d.toISOString()
来源：http://ur.nszjky.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qi.haigaiapp.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fo.szxytkj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ty.hnjuh.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zi.wgjwhj.cn

[J03] 字符串解析为日期
来源：http://ws.jianghongdianzi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://js.wgjwhj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://sx.haigaiapp.cn

JS:   new Date("2024-01-02")
来源：http://tr.yuntaijiaju.cn

TS:   new Date("2024-01-02")
来源：http://zr.panjiajie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://vf.wgjwhj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yw.nszjky.cn

Ruby: Date.parse("2024-01-02")
来源：http://is.asd995.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ta.shxzskj.cn

[J04] 时间戳与日期互转
来源：http://st.huixiangedu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fv.9csxet.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uv.huixinmuqiang.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://eh.shxzukj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://mk.huanxung.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xz.jianghongdianzi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lm.yuexingan06.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wm.shxzskj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://it.hahajie.cn

[J05] 时间加减（加 7 天）
来源：http://ny.521024.cn

Py:   now + timedelta(days=7)
来源：http://lm.jianghongdianzi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://kz.9csxet.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tp.newstarts.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tc.haigaiapp.cn

Java: LocalDate.now().plusDays(7)
来源：http://uu.9csxet.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vw.colortex.cn

Ruby: Time.now + 7 * 86400
来源：http://ho.yuexingan06.cn

C#:   DateTime.Now.AddDays(7)
来源：http://no.newstarts.cn

[J06] 计算两时间之差
来源：http://rh.jctech888.com.cn

Py:   (end - start).total_seconds()
来源：http://vx.yuntaijiaju.cn

PHP:  $end->diff($start)->days;
来源：http://zr.nicolike.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://oy.bookmarksfly.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ef.nszjky.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ix.haigaiapp.cn

Go:   end.Sub(start).Hours()
来源：http://ma.shtwfgs.cn

Ruby: end - start                 # 返回秒数
来源：http://hx.newstarts.cn

C#:   (end - start).TotalSeconds
来源：http://ik.huixinmuqiang.cn

[J07] 比较两个日期
来源：http://mv.hnjuh.cn

Py:   d1 < d2;  d1 == d2
来源：http://if.shxzukj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xw.huanxung.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vj.yuexingan06.cn

TS:   d1.getTime() < d2.getTime()
来源：http://hl.szxytkj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ng.hahajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gy.nszjky.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xu.bookmarksfly.cn

C#:   d1 < d2;  d1 == d2
来源：http://oa.shxzukj.cn

[J08] 提取年月日与星期
来源：http://ow.nicolike.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tk.gzmigu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zd.shxzskj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zi.panjiajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kw.bjjhwx.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qy.huixiangedu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cr.colortex.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wk.huixiangedu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ui.bookmarksfly.cn

[J09] 时区处理
来源：http://gl.lnxyls.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xn.colortex.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qk.hahajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pk.jianghongdianzi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uu.shxzukj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pg.jianghongdianzi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qu.newstarts.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ni.9csxet.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ml.bookmarksfly.cn

[J10] 取今天 / 本月第一天
来源：http://nn.colortex.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zr.yuexingan06.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bc.gzmigu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://oi.bookmarksfly.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zm.jctech888.com.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hm.hnjuh.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://si.haigaiapp.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ev.huanxung.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kl.huixiangedu.cn

================================================================================
来源：http://ps.521024.cn

K. JSON 与序列化
来源：http://xb.lnxyls.cn

================================================================================
来源：http://gr.bjjhwx.cn

[K01] 对象转 JSON 字符串
来源：http://hz.nicolike.cn


<!-- 参考信息 -->