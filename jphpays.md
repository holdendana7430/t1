代发 wailian999

Java: u instanceof User
来源：http://yn.jianghongdianzi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://yi.jianghongdianzi.cn

Ruby: u.is_a?(User)
来源：http://kg.jianghongdianzi.cn

C#:   u is User
来源：http://po.yuexingan06.cn

[G14] 数据类 / record
来源：http://ex.hahajie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xn.szsharing.cn

PHP:  // 用 readonly 属性模拟
来源：http://kp.9csxet.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ax.huixiangedu.cn

TS:   type User = { name: string; age: number };
来源：http://ba.hnjuh.cn

Java: record User(String name, int age) {}
来源：http://or.nszjky.cn

Go:   type User struct { Name string; Age int }
来源：http://fm.shtwfgs.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://by.nszjky.cn

C#:   record User(string Name, int Age);
来源：http://je.521024.cn

[G15] 枚举
来源：http://lw.chemitech.net.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://yh.huixiangedu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://vf.muxihuayi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://sr.hahajie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://iy.lnxyls.cn

Java: enum Color { RED, GREEN }
来源：http://gq.shxzskj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lh.muxihuayi.cn

Ruby: Color = %i[red green].freeze
来源：http://wa.9csxet.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qn.szsharing.cn

[G16] 对象转数组 / 字典
来源：http://vx.huanxung.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uq.lnxyls.cn

PHP:  get_object_vars($obj);
来源：http://mr.huanxung.cn

JS:   Object.entries(obj)
来源：http://hc.haigaiapp.cn

TS:   Object.entries(obj)
来源：http://jg.haigaiapp.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tz.asd995.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://pu.szxytkj.cn

Ruby: obj.instance_variables
来源：http://ke.huanxung.cn

C#:   // 用反射或 System.Text.Json
来源：http://rj.jianghongdianzi.cn

================================================================================
来源：http://ay.9csxet.cn

H. 异常与错误处理
来源：http://se.yuexingan06.cn

================================================================================
来源：http://ou.jianghongdianzi.cn

[H01] try / catch 基础
来源：http://go.muxihuayi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://sg.jianghongdianzi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fy.hnjuh.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://iu.bjjhwx.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ls.bjjhwx.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://iz.bjjhwx.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ex.shtwfgs.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zj.muxihuayi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ir.hahajie.cn

[H02] finally / ensure 收尾
来源：http://dx.jianghongdianzi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://du.521024.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://gm.jianghongdianzi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ri.colortex.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qt.panjiajie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://fx.newstarts.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://uy.521024.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://oo.hnjuh.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://op.colortex.cn

[H03] 主动抛出异常
来源：http://uf.chemitech.net.cn

Py:   raise ValueError("错误信息")
来源：http://eo.9csxet.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dq.huanxung.cn

JS:   throw new Error("错误信息");
来源：http://tn.shtwfgs.cn

TS:   throw new Error("错误信息");
来源：http://oe.lnxyls.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ch.chemitech.net.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://oj.wgjwhj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wd.yuntaijiaju.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ih.9csxet.cn

[H04] 自定义异常类型
来源：http://au.wgjwhj.cn

Py:   class MyError(Exception): pass
来源：http://xl.hnjuh.cn

PHP:  class MyError extends RuntimeException {}
来源：http://do.jctech888.com.cn

JS:   class MyError extends Error {}
来源：http://cq.colortex.cn

TS:   class MyError extends Error {}
来源：http://jq.bookmarksfly.cn

Java: class MyException extends RuntimeException {}
来源：http://sy.newstarts.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pe.muxihuayi.cn

Ruby: class MyError < StandardError; end
来源：http://fr.chemitech.net.cn

C#:   class MyException : Exception {}
来源：http://iu.muxihuayi.cn

[H05] 捕获特定类型
来源：http://mb.lnxyls.cn

Py:   except ValueError as e:
来源：http://zs.bjjhwx.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bb.yuexingan06.cn

JS:   if (e instanceof TypeError) {}
来源：http://rr.muxihuayi.cn

TS:   if (e instanceof TypeError) {}
来源：http://br.nicolike.cn

Java: catch (IOException | SQLException e) {}
来源：http://em.nicolike.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xj.yuexingan06.cn

Ruby: rescue ArgumentError => e
来源：http://db.huixinmuqiang.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://sf.haigaiapp.cn

[H06] 可选值 / 空值安全访问
来源：http://rd.yuntaijiaju.cn

Py:   value = d.get("k") or default
来源：http://du.huixiangedu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://vt.asd995.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ug.haigaiapp.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ga.hnjuh.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://is.colortex.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://mm.chemitech.net.cn

Ruby: d&.dig(:a, :b)
来源：http://ke.yuntaijiaju.cn

C#:   obj?.A?.B ?? default
来源：http://xy.jianghongdianzi.cn

[H07] 断言
来源：http://wl.nszjky.cn

Py:   assert x > 0, "必须为正"
来源：http://zt.panjiajie.cn

PHP:  assert($x > 0);
来源：http://cs.huixiangedu.cn

JS:   console.assert(x > 0);
来源：http://gy.nicolike.cn

TS:   console.assert(x > 0);
来源：http://ct.lnxyls.cn

Java: assert x > 0 : "必须为正";
来源：http://va.huixinmuqiang.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://os.newstarts.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ja.hahajie.cn

C#:   Debug.Assert(x > 0);
来源：http://zx.huanxung.cn

[H08] 获取错误信息与堆栈
来源：http://hj.huixinmuqiang.cn

Py:   str(e);  traceback.format_exc()
来源：http://ll.muxihuayi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pg.9csxet.cn

JS:   e.message;  e.stack
来源：http://yc.muxihuayi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://bi.shtwfgs.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://wj.yuexingan06.cn

Go:   err.Error()
来源：http://yb.muxihuayi.cn

Ruby: e.message;  e.backtrace
来源：http://sm.lnxyls.cn

C#:   e.Message;  e.StackTrace
来源：http://te.hnjuh.cn

[H09] 带错误码的异常
来源：http://vh.asd995.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jr.huixinmuqiang.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ni.huixiangedu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://al.huixinmuqiang.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bp.asd995.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mu.colortex.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vc.szsharing.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ej.shtwfgs.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://al.colortex.cn

[H10] 资源自动释放
来源：http://oq.hnjuh.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://wy.chemitech.net.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kv.jianghongdianzi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://no.panjiajie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pf.huixinmuqiang.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://is.huixinmuqiang.cn

Go:   defer f.Close()
来源：http://by.huixiangedu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://sv.gzmigu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zw.shxzukj.cn

================================================================================
来源：http://dv.521024.cn

I. 正则表达式
来源：http://mp.szxytkj.cn

================================================================================
来源：http://vy.jianghongdianzi.cn

[I01] 判断是否匹配
来源：http://ls.nicolike.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hw.huanxung.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ql.jctech888.com.cn

JS:   /\d+/.test(s)
来源：http://gi.hahajie.cn

TS:   /\d+/.test(s)
来源：http://kk.lnxyls.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tb.asd995.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ye.hnjuh.cn

Ruby: s.match?(/\d+/)
来源：http://ty.bookmarksfly.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://us.bjjhwx.cn

[I02] 提取所有匹配
来源：http://hf.huixiangedu.cn

Py:   re.findall(r"\d+", s)
来源：http://we.szxytkj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://et.yuntaijiaju.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pd.521024.cn

TS:   s.match(/\d+/g)
来源：http://sd.nszjky.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xa.newstarts.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ki.shtwfgs.cn

Ruby: s.scan(/\d+/)
来源：http://ii.bookmarksfly.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gp.yuntaijiaju.cn

[I03] 提取捕获分组
来源：http://rp.9csxet.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ne.nicolike.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://be.shtwfgs.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://is.nszjky.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gp.bookmarksfly.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ys.hahajie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gf.bookmarksfly.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yy.jianghongdianzi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xk.521024.cn

[I04] 正则替换
来源：http://ih.bjjhwx.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://si.hnjuh.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yk.nicolike.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ts.bookmarksfly.cn

TS:   s.replace(/\d+/g, "#")
来源：http://gv.bookmarksfly.cn

Java: s.replaceAll("\\d+", "#")
来源：http://oo.huixinmuqiang.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://fh.muxihuayi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ij.shtwfgs.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hu.gzmigu.cn

[I05] 按正则拆分
来源：http://os.wgjwhj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://vg.nicolike.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qb.nszjky.cn

JS:   s.split(/\s*,\s*/)
来源：http://os.huanxung.cn

TS:   s.split(/\s*,\s*/)
来源：http://df.jianghongdianzi.cn

Java: s.split("\\s*,\\s*")
来源：http://lj.hnjuh.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ea.newstarts.cn

Ruby: s.split(/\s*,\s*/)
来源：http://gh.jianghongdianzi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pi.jianghongdianzi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rf.szxytkj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wc.huixiangedu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lf.haigaiapp.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qe.asd995.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xs.haigaiapp.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zu.panjiajie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dy.huanxung.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sj.shtwfgs.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vk.muxihuayi.cn

[I07] 忽略大小写与多行模式
来源：http://hc.hahajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zs.shxzskj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ok.haigaiapp.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kx.nicolike.cn

TS:   /error/gim
来源：http://nf.bjjhwx.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rw.jianghongdianzi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rp.huixinmuqiang.cn

Ruby: s.scan(/error/i)
来源：http://qc.panjiajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://re.szxytkj.cn

[I08] 贪婪与非贪婪匹配
来源：http://do.yuntaijiaju.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yn.huanxung.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zf.haigaiapp.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zq.huixinmuqiang.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ie.gzmigu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ma.nszjky.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dy.hnjuh.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://sz.asd995.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jp.hahajie.cn

================================================================================
来源：http://wz.nszjky.cn

J. 日期与时间
来源：http://uz.521024.cn

================================================================================
来源：http://ko.lnxyls.cn

[J01] 获取当前时间
来源：http://uf.wgjwhj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://sa.huanxung.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nc.muxihuayi.cn

JS:   new Date();  Date.now()
来源：http://dz.muxihuayi.cn

TS:   new Date();  Date.now()
来源：http://na.521024.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://wy.szsharing.cn

Go:   time.Now()
来源：http://zq.huixiangedu.cn

Ruby: Time.now
来源：http://zr.muxihuayi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://iz.huanxung.cn

[J02] 格式化输出
来源：http://eo.jianghongdianzi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fs.jianghongdianzi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hw.yuexingan06.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cd.asd995.cn

TS:   d.toISOString()
来源：http://vs.nicolike.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wu.newstarts.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mr.shxzskj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ir.lnxyls.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dk.jianghongdianzi.cn

[J03] 字符串解析为日期
来源：http://fv.huixiangedu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sk.nicolike.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://me.bjjhwx.cn

JS:   new Date("2024-01-02")
来源：http://iv.newstarts.cn

TS:   new Date("2024-01-02")
来源：http://uy.asd995.cn

Java: LocalDate.parse("2024-01-02")
来源：http://cv.9csxet.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ax.lnxyls.cn

Ruby: Date.parse("2024-01-02")
来源：http://bd.nszjky.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ul.shxzukj.cn

[J04] 时间戳与日期互转
来源：http://st.colortex.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wp.nicolike.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bd.panjiajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ec.chemitech.net.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://di.colortex.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hw.szsharing.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sv.521024.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tn.huixinmuqiang.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ee.panjiajie.cn

[J05] 时间加减（加 7 天）
来源：http://kw.colortex.cn

Py:   now + timedelta(days=7)
来源：http://ov.jctech888.com.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xp.jctech888.com.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qw.shxzukj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ye.hahajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://cy.asd995.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://so.shxzukj.cn

Ruby: Time.now + 7 * 86400
来源：http://sl.haigaiapp.cn

C#:   DateTime.Now.AddDays(7)
来源：http://hx.bookmarksfly.cn

[J06] 计算两时间之差
来源：http://vy.nicolike.cn

Py:   (end - start).total_seconds()
来源：http://zk.521024.cn

PHP:  $end->diff($start)->days;
来源：http://jo.panjiajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tt.shxzskj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ky.hnjuh.cn

Java: Duration.between(start, end).toSeconds()
来源：http://dd.huixiangedu.cn

Go:   end.Sub(start).Hours()
来源：http://mh.szsharing.cn

Ruby: end - start                 # 返回秒数
来源：http://af.521024.cn

C#:   (end - start).TotalSeconds
来源：http://tl.bookmarksfly.cn

[J07] 比较两个日期
来源：http://di.panjiajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://af.shtwfgs.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wk.9csxet.cn

JS:   d1.getTime() < d2.getTime()
来源：http://tg.yuntaijiaju.cn

TS:   d1.getTime() < d2.getTime()
来源：http://dn.bookmarksfly.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ak.szxytkj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://go.shxzskj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pq.panjiajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://hj.9csxet.cn

[J08] 提取年月日与星期
来源：http://uh.chemitech.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xs.colortex.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sd.panjiajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ur.gzmigu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://sz.hahajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gg.shtwfgs.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mn.newstarts.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cx.jctech888.com.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zk.jctech888.com.cn

[J09] 时区处理
来源：http://un.shxzukj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cq.muxihuayi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://za.szxytkj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xj.chemitech.net.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zx.colortex.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vb.bjjhwx.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lq.nicolike.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://os.szsharing.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jw.shxzskj.cn

[J10] 取今天 / 本月第一天
来源：http://bw.panjiajie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://hj.9csxet.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://iu.yuntaijiaju.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kq.hahajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pf.haigaiapp.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bx.newstarts.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dg.shtwfgs.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yi.huixinmuqiang.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zd.asd995.cn

================================================================================
来源：http://zo.hahajie.cn

K. JSON 与序列化
来源：http://hy.szxytkj.cn

================================================================================
来源：http://cs.nszjky.cn

[K01] 对象转 JSON 字符串
来源：http://vg.bookmarksfly.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vt.newstarts.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rm.shxzskj.cn

JS:   JSON.stringify(obj)
来源：http://xc.shxzskj.cn

TS:   JSON.stringify(obj)
来源：http://wg.wgjwhj.cn


<!-- 参考信息 -->