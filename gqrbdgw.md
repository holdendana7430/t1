代发 wailian999

Py:   isinstance(u, User)
来源：http://fj.szxytkj.cn

PHP:  $u instanceof User
来源：http://wt.nszjky.cn

JS:   u instanceof User
来源：http://oh.chemitech.net.cn

TS:   u instanceof User
来源：http://rv.bjjhwx.cn

Java: u instanceof User
来源：http://tv.huanxung.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qq.shtwfgs.cn

Ruby: u.is_a?(User)
来源：http://vr.muxihuayi.cn

C#:   u is User
来源：http://ei.hahajie.cn

[G14] 数据类 / record
来源：http://xi.colortex.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yh.jianghongdianzi.cn

PHP:  // 用 readonly 属性模拟
来源：http://dg.bookmarksfly.cn

JS:   // 无内置：普通类或对象字面量
来源：http://as.9csxet.cn

TS:   type User = { name: string; age: number };
来源：http://xf.jctech888.com.cn

Java: record User(String name, int age) {}
来源：http://sm.gzmigu.cn

Go:   type User struct { Name string; Age int }
来源：http://al.bjjhwx.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zm.szsharing.cn

C#:   record User(string Name, int Age);
来源：http://gd.yuexingan06.cn

[G15] 枚举
来源：http://fo.asd995.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vw.wgjwhj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://yd.asd995.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qf.521024.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xr.chemitech.net.cn

Java: enum Color { RED, GREEN }
来源：http://ez.bookmarksfly.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mn.colortex.cn

Ruby: Color = %i[red green].freeze
来源：http://am.jctech888.com.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://as.szxytkj.cn

[G16] 对象转数组 / 字典
来源：http://te.bjjhwx.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cz.szxytkj.cn

PHP:  get_object_vars($obj);
来源：http://uc.huixinmuqiang.cn

JS:   Object.entries(obj)
来源：http://lr.wgjwhj.cn

TS:   Object.entries(obj)
来源：http://yr.lnxyls.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wk.shtwfgs.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://an.huixinmuqiang.cn

Ruby: obj.instance_variables
来源：http://ez.haigaiapp.cn

C#:   // 用反射或 System.Text.Json
来源：http://gr.newstarts.cn

================================================================================
来源：http://do.chemitech.net.cn

H. 异常与错误处理
来源：http://bp.szxytkj.cn

================================================================================
来源：http://se.huixinmuqiang.cn

[H01] try / catch 基础
来源：http://dg.szsharing.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dl.szxytkj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cp.nicolike.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ja.huanxung.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fc.huixinmuqiang.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xj.nszjky.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mc.521024.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hw.shxzskj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cz.huixinmuqiang.cn

[H02] finally / ensure 收尾
来源：http://xq.nicolike.cn

Py:   try: f()⏎finally: cleanup()
来源：http://yi.jctech888.com.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://sp.szsharing.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ep.haigaiapp.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ye.newstarts.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ug.521024.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qk.chemitech.net.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ho.colortex.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://yl.hnjuh.cn

[H03] 主动抛出异常
来源：http://cv.chemitech.net.cn

Py:   raise ValueError("错误信息")
来源：http://hf.colortex.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zz.gzmigu.cn

JS:   throw new Error("错误信息");
来源：http://wc.szsharing.cn

TS:   throw new Error("错误信息");
来源：http://eg.bookmarksfly.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ba.yuexingan06.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rs.shtwfgs.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://fi.huixiangedu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://hh.shxzskj.cn

[H04] 自定义异常类型
来源：http://td.521024.cn

Py:   class MyError(Exception): pass
来源：http://nz.huixiangedu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://jb.jctech888.com.cn

JS:   class MyError extends Error {}
来源：http://fw.9csxet.cn

TS:   class MyError extends Error {}
来源：http://cu.shtwfgs.cn

Java: class MyException extends RuntimeException {}
来源：http://dc.huixinmuqiang.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wz.lnxyls.cn

Ruby: class MyError < StandardError; end
来源：http://ur.bookmarksfly.cn

C#:   class MyException : Exception {}
来源：http://vp.huixinmuqiang.cn

[H05] 捕获特定类型
来源：http://rt.huanxung.cn

Py:   except ValueError as e:
来源：http://is.muxihuayi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fw.gzmigu.cn

JS:   if (e instanceof TypeError) {}
来源：http://vo.bookmarksfly.cn

TS:   if (e instanceof TypeError) {}
来源：http://vh.nicolike.cn

Java: catch (IOException | SQLException e) {}
来源：http://ue.panjiajie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cy.hnjuh.cn

Ruby: rescue ArgumentError => e
来源：http://wg.jctech888.com.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://el.wgjwhj.cn

[H06] 可选值 / 空值安全访问
来源：http://fw.chemitech.net.cn

Py:   value = d.get("k") or default
来源：http://km.yuntaijiaju.cn

PHP:  $v = $d["k"] ?? null;
来源：http://gs.shtwfgs.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ml.huanxung.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xl.chemitech.net.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xt.wgjwhj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://kw.haigaiapp.cn

Ruby: d&.dig(:a, :b)
来源：http://za.bookmarksfly.cn

C#:   obj?.A?.B ?? default
来源：http://iu.yuexingan06.cn

[H07] 断言
来源：http://db.521024.cn

Py:   assert x > 0, "必须为正"
来源：http://cu.9csxet.cn

PHP:  assert($x > 0);
来源：http://vc.yuexingan06.cn

JS:   console.assert(x > 0);
来源：http://xy.chemitech.net.cn

TS:   console.assert(x > 0);
来源：http://sq.bookmarksfly.cn

Java: assert x > 0 : "必须为正";
来源：http://lu.hahajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ia.wgjwhj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://rr.huixinmuqiang.cn

C#:   Debug.Assert(x > 0);
来源：http://ht.huanxung.cn

[H08] 获取错误信息与堆栈
来源：http://qd.huixinmuqiang.cn

Py:   str(e);  traceback.format_exc()
来源：http://ru.nicolike.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bm.newstarts.cn

JS:   e.message;  e.stack
来源：http://tz.bjjhwx.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ha.nicolike.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ae.shtwfgs.cn

Go:   err.Error()
来源：http://ys.chemitech.net.cn

Ruby: e.message;  e.backtrace
来源：http://rq.newstarts.cn

C#:   e.Message;  e.StackTrace
来源：http://ev.colortex.cn

[H09] 带错误码的异常
来源：http://dt.yuntaijiaju.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cx.haigaiapp.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ee.newstarts.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vo.shtwfgs.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mc.9csxet.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mw.gzmigu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gj.nicolike.cn

Ruby: raise MyError.new("fail", 500)
来源：http://gf.huixiangedu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ld.asd995.cn

[H10] 资源自动释放
来源：http://ij.asd995.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vz.521024.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://se.jianghongdianzi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qk.lnxyls.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://uu.yuntaijiaju.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://km.lnxyls.cn

Go:   defer f.Close()
来源：http://yh.hahajie.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ha.chemitech.net.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://db.521024.cn

================================================================================
来源：http://we.muxihuayi.cn

I. 正则表达式
来源：http://tt.bookmarksfly.cn

================================================================================
来源：http://vm.huixiangedu.cn

[I01] 判断是否匹配
来源：http://yr.nicolike.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tr.hahajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://lm.wgjwhj.cn

JS:   /\d+/.test(s)
来源：http://wr.chemitech.net.cn

TS:   /\d+/.test(s)
来源：http://re.bjjhwx.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cf.haigaiapp.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vy.nicolike.cn

Ruby: s.match?(/\d+/)
来源：http://on.shxzskj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ap.9csxet.cn

[I02] 提取所有匹配
来源：http://la.lnxyls.cn

Py:   re.findall(r"\d+", s)
来源：http://cv.lnxyls.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ct.hnjuh.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cq.gzmigu.cn

TS:   s.match(/\d+/g)
来源：http://il.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jn.yuexingan06.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bx.shxzukj.cn

Ruby: s.scan(/\d+/)
来源：http://eg.521024.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jj.nszjky.cn

[I03] 提取捕获分组
来源：http://rt.colortex.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ys.jctech888.com.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ly.nszjky.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lp.521024.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ie.panjiajie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yx.wgjwhj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ep.nicolike.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rm.yuntaijiaju.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ra.shxzukj.cn

[I04] 正则替换
来源：http://ik.panjiajie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://sn.wgjwhj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zy.huixiangedu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://bx.521024.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xe.lnxyls.cn

Java: s.replaceAll("\\d+", "#")
来源：http://gw.szxytkj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ne.haigaiapp.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://dw.shxzukj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bq.huixinmuqiang.cn

[I05] 按正则拆分
来源：http://jb.huanxung.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://lc.szsharing.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ls.asd995.cn

JS:   s.split(/\s*,\s*/)
来源：http://rx.521024.cn

TS:   s.split(/\s*,\s*/)
来源：http://ka.colortex.cn

Java: s.split("\\s*,\\s*")
来源：http://eo.asd995.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://iv.wgjwhj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://qx.asd995.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yj.szxytkj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://uy.nszjky.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gl.nicolike.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kb.huanxung.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://em.yuntaijiaju.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dx.shxzukj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fg.gzmigu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fu.521024.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nm.lnxyls.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ip.asd995.cn

[I07] 忽略大小写与多行模式
来源：http://ev.panjiajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jc.bookmarksfly.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fk.shxzukj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gk.chemitech.net.cn

TS:   /error/gim
来源：http://be.muxihuayi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://se.wgjwhj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jv.muxihuayi.cn

Ruby: s.scan(/error/i)
来源：http://yr.wgjwhj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dz.panjiajie.cn

[I08] 贪婪与非贪婪匹配
来源：http://in.jctech888.com.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ge.bookmarksfly.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xv.nicolike.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://km.haigaiapp.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vh.huixinmuqiang.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ds.shxzskj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qg.yuexingan06.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gn.shtwfgs.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vo.shtwfgs.cn

================================================================================
来源：http://nn.9csxet.cn

J. 日期与时间
来源：http://gy.gzmigu.cn

================================================================================
来源：http://cf.chemitech.net.cn

[J01] 获取当前时间
来源：http://il.szsharing.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://cz.shxzskj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://aj.jctech888.com.cn

JS:   new Date();  Date.now()
来源：http://uj.hnjuh.cn

TS:   new Date();  Date.now()
来源：http://lv.wgjwhj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zx.huixiangedu.cn

Go:   time.Now()
来源：http://fn.huixinmuqiang.cn

Ruby: Time.now
来源：http://gz.colortex.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fo.gzmigu.cn

[J02] 格式化输出
来源：http://ei.shxzukj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cp.huixinmuqiang.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gr.chemitech.net.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pk.newstarts.cn

TS:   d.toISOString()
来源：http://ua.szsharing.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lb.shxzukj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wt.asd995.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://us.521024.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://az.yuexingan06.cn

[J03] 字符串解析为日期
来源：http://gm.panjiajie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ka.shxzukj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tm.asd995.cn

JS:   new Date("2024-01-02")
来源：http://ew.chemitech.net.cn

TS:   new Date("2024-01-02")
来源：http://fd.yuexingan06.cn

Java: LocalDate.parse("2024-01-02")
来源：http://sa.hahajie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://uf.yuntaijiaju.cn

Ruby: Date.parse("2024-01-02")
来源：http://sp.shxzskj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kt.9csxet.cn

[J04] 时间戳与日期互转
来源：http://tj.shtwfgs.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yd.9csxet.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wo.gzmigu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vl.hahajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fo.jctech888.com.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gv.jianghongdianzi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tx.yuexingan06.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rt.wgjwhj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bs.huixinmuqiang.cn

[J05] 时间加减（加 7 天）
来源：http://dh.lnxyls.cn

Py:   now + timedelta(days=7)
来源：http://il.jctech888.com.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vi.lnxyls.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kf.wgjwhj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bk.lnxyls.cn

Java: LocalDate.now().plusDays(7)
来源：http://ro.bjjhwx.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nu.nszjky.cn

Ruby: Time.now + 7 * 86400
来源：http://to.newstarts.cn

C#:   DateTime.Now.AddDays(7)
来源：http://mc.huanxung.cn

[J06] 计算两时间之差
来源：http://bf.jctech888.com.cn

Py:   (end - start).total_seconds()
来源：http://ks.chemitech.net.cn

PHP:  $end->diff($start)->days;
来源：http://sr.yuexingan06.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gr.jianghongdianzi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ov.asd995.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ag.jianghongdianzi.cn

Go:   end.Sub(start).Hours()
来源：http://ed.hnjuh.cn

Ruby: end - start                 # 返回秒数
来源：http://ur.colortex.cn

C#:   (end - start).TotalSeconds
来源：http://ie.nicolike.cn

[J07] 比较两个日期
来源：http://mp.huixiangedu.cn

Py:   d1 < d2;  d1 == d2
来源：http://xj.nszjky.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ys.newstarts.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xw.nszjky.cn

TS:   d1.getTime() < d2.getTime()
来源：http://vq.hnjuh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://to.muxihuayi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://um.yuexingan06.cn

Ruby: d1 < d2;  d1 == d2
来源：http://kp.huixinmuqiang.cn

C#:   d1 < d2;  d1 == d2
来源：http://dj.nicolike.cn

[J08] 提取年月日与星期
来源：http://ma.9csxet.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gy.muxihuayi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rq.hnjuh.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nh.jctech888.com.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ud.shtwfgs.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sy.521024.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jx.chemitech.net.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ir.nszjky.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xl.huanxung.cn

[J09] 时区处理
来源：http://qw.newstarts.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://eh.521024.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xw.9csxet.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jx.chemitech.net.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ny.nszjky.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pp.szsharing.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://je.szsharing.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ea.szxytkj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wx.521024.cn

[J10] 取今天 / 本月第一天
来源：http://tu.nicolike.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ab.szsharing.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rf.bookmarksfly.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ji.shxzskj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rr.huixiangedu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dv.chemitech.net.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://em.newstarts.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://iv.shxzskj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://df.yuexingan06.cn

================================================================================
来源：http://ox.asd995.cn

K. JSON 与序列化
来源：http://ad.huixiangedu.cn

================================================================================
来源：http://lz.muxihuayi.cn

[K01] 对象转 JSON 字符串
来源：http://hy.wgjwhj.cn


<!-- 参考信息 -->