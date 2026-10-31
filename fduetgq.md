代发 wailian999

Py:   isinstance(u, User)
来源：http://je.newstarts.cn

PHP:  $u instanceof User
来源：http://hh.yuexingan06.cn

JS:   u instanceof User
来源：http://qk.newstarts.cn

TS:   u instanceof User
来源：http://en.521024.cn

Java: u instanceof User
来源：http://bm.szxytkj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://sk.nszjky.cn

Ruby: u.is_a?(User)
来源：http://nc.newstarts.cn

C#:   u is User
来源：http://ot.haigaiapp.cn

[G14] 数据类 / record
来源：http://lx.wgjwhj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gd.hnjuh.cn

PHP:  // 用 readonly 属性模拟
来源：http://ps.nicolike.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ca.szsharing.cn

TS:   type User = { name: string; age: number };
来源：http://ma.nszjky.cn

Java: record User(String name, int age) {}
来源：http://hl.jctech888.com.cn

Go:   type User struct { Name string; Age int }
来源：http://yt.haigaiapp.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://er.shtwfgs.cn

C#:   record User(string Name, int Age);
来源：http://tq.nicolike.cn

[G15] 枚举
来源：http://yd.szxytkj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://je.chemitech.net.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://xt.521024.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ko.nicolike.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ua.panjiajie.cn

Java: enum Color { RED, GREEN }
来源：http://el.yuntaijiaju.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wh.nszjky.cn

Ruby: Color = %i[red green].freeze
来源：http://sn.hahajie.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cl.bookmarksfly.cn

[G16] 对象转数组 / 字典
来源：http://xr.bookmarksfly.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ft.hnjuh.cn

PHP:  get_object_vars($obj);
来源：http://ja.szxytkj.cn

JS:   Object.entries(obj)
来源：http://fd.haigaiapp.cn

TS:   Object.entries(obj)
来源：http://ev.huixiangedu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tx.szsharing.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ej.szxytkj.cn

Ruby: obj.instance_variables
来源：http://hs.jianghongdianzi.cn

C#:   // 用反射或 System.Text.Json
来源：http://ml.newstarts.cn

================================================================================
来源：http://yg.colortex.cn

H. 异常与错误处理
来源：http://ih.szsharing.cn

================================================================================
来源：http://ru.lnxyls.cn

[H01] try / catch 基础
来源：http://xy.lnxyls.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://eb.521024.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lc.haigaiapp.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rg.newstarts.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fo.colortex.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sa.huixiangedu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://re.szxytkj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ni.hahajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://iv.muxihuayi.cn

[H02] finally / ensure 收尾
来源：http://ft.haigaiapp.cn

Py:   try: f()⏎finally: cleanup()
来源：http://tg.gzmigu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://tu.muxihuayi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://iy.hahajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://eq.521024.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ek.9csxet.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://gs.hahajie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://xe.muxihuayi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://bm.hahajie.cn

[H03] 主动抛出异常
来源：http://oc.nicolike.cn

Py:   raise ValueError("错误信息")
来源：http://be.szxytkj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qh.panjiajie.cn

JS:   throw new Error("错误信息");
来源：http://uc.asd995.cn

TS:   throw new Error("错误信息");
来源：http://uo.521024.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://kx.nicolike.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gb.gzmigu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://su.colortex.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ek.szxytkj.cn

[H04] 自定义异常类型
来源：http://mv.wgjwhj.cn

Py:   class MyError(Exception): pass
来源：http://ru.huanxung.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ky.gzmigu.cn

JS:   class MyError extends Error {}
来源：http://ym.shxzskj.cn

TS:   class MyError extends Error {}
来源：http://cr.asd995.cn

Java: class MyException extends RuntimeException {}
来源：http://dv.panjiajie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nq.yuexingan06.cn

Ruby: class MyError < StandardError; end
来源：http://pc.wgjwhj.cn

C#:   class MyException : Exception {}
来源：http://jk.newstarts.cn

[H05] 捕获特定类型
来源：http://ae.yuexingan06.cn

Py:   except ValueError as e:
来源：http://dw.jianghongdianzi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hr.gzmigu.cn

JS:   if (e instanceof TypeError) {}
来源：http://vr.shxzukj.cn

TS:   if (e instanceof TypeError) {}
来源：http://dh.yuexingan06.cn

Java: catch (IOException | SQLException e) {}
来源：http://go.asd995.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://az.hahajie.cn

Ruby: rescue ArgumentError => e
来源：http://kk.gzmigu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gb.521024.cn

[H06] 可选值 / 空值安全访问
来源：http://ir.bookmarksfly.cn

Py:   value = d.get("k") or default
来源：http://uy.szsharing.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ns.huanxung.cn

JS:   obj?.a?.b;  d ?? default
来源：http://uo.newstarts.cn

TS:   obj?.a?.b;  d ?? default
来源：http://br.huixinmuqiang.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://un.shxzukj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://xo.jianghongdianzi.cn

Ruby: d&.dig(:a, :b)
来源：http://fu.jianghongdianzi.cn

C#:   obj?.A?.B ?? default
来源：http://pt.9csxet.cn

[H07] 断言
来源：http://nn.shxzukj.cn

Py:   assert x > 0, "必须为正"
来源：http://tc.nicolike.cn

PHP:  assert($x > 0);
来源：http://zr.panjiajie.cn

JS:   console.assert(x > 0);
来源：http://dt.521024.cn

TS:   console.assert(x > 0);
来源：http://nl.wgjwhj.cn

Java: assert x > 0 : "必须为正";
来源：http://dg.muxihuayi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ru.jctech888.com.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ue.newstarts.cn

C#:   Debug.Assert(x > 0);
来源：http://ln.yuexingan06.cn

[H08] 获取错误信息与堆栈
来源：http://ik.wgjwhj.cn

Py:   str(e);  traceback.format_exc()
来源：http://gm.szxytkj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yg.hahajie.cn

JS:   e.message;  e.stack
来源：http://uf.chemitech.net.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://uq.huixinmuqiang.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ye.asd995.cn

Go:   err.Error()
来源：http://jq.huanxung.cn

Ruby: e.message;  e.backtrace
来源：http://hi.chemitech.net.cn

C#:   e.Message;  e.StackTrace
来源：http://up.9csxet.cn

[H09] 带错误码的异常
来源：http://zn.hahajie.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://br.colortex.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xi.jianghongdianzi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qe.szxytkj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vn.hahajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nm.nszjky.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vb.jianghongdianzi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://so.szsharing.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://sw.nszjky.cn

[H10] 资源自动释放
来源：http://wn.huixiangedu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://gy.bjjhwx.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jo.szsharing.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ri.colortex.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://eq.huanxung.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tx.szsharing.cn

Go:   defer f.Close()
来源：http://pe.szsharing.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zj.colortex.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kv.yuexingan06.cn

================================================================================
来源：http://li.muxihuayi.cn

I. 正则表达式
来源：http://hb.9csxet.cn

================================================================================
来源：http://at.yuexingan06.cn

[I01] 判断是否匹配
来源：http://qu.haigaiapp.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zh.wgjwhj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gk.szxytkj.cn

JS:   /\d+/.test(s)
来源：http://fh.gzmigu.cn

TS:   /\d+/.test(s)
来源：http://eu.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ri.gzmigu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ad.colortex.cn

Ruby: s.match?(/\d+/)
来源：http://zv.nszjky.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://le.huanxung.cn

[I02] 提取所有匹配
来源：http://og.wgjwhj.cn

Py:   re.findall(r"\d+", s)
来源：http://iy.asd995.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vz.newstarts.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ds.lnxyls.cn

TS:   s.match(/\d+/g)
来源：http://zk.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ku.nicolike.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ic.shxzukj.cn

Ruby: s.scan(/\d+/)
来源：http://xk.yuntaijiaju.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fr.bookmarksfly.cn

[I03] 提取捕获分组
来源：http://gs.newstarts.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sh.huixinmuqiang.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bi.gzmigu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wl.huixiangedu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qd.shxzukj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qs.shxzukj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rc.wgjwhj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qt.chemitech.net.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ps.yuexingan06.cn

[I04] 正则替换
来源：http://bw.hnjuh.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://bm.newstarts.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://oe.hnjuh.cn

JS:   s.replace(/\d+/g, "#")
来源：http://nv.shxzukj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://oj.lnxyls.cn

Java: s.replaceAll("\\d+", "#")
来源：http://kj.hahajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://dr.colortex.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://qq.panjiajie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ve.jianghongdianzi.cn

[I05] 按正则拆分
来源：http://yb.9csxet.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://yi.nszjky.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uf.asd995.cn

JS:   s.split(/\s*,\s*/)
来源：http://iz.gzmigu.cn

TS:   s.split(/\s*,\s*/)
来源：http://ar.bjjhwx.cn

Java: s.split("\\s*,\\s*")
来源：http://sr.szsharing.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wn.shxzskj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ml.lnxyls.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kf.shxzskj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wr.colortex.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ka.521024.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mi.9csxet.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zp.chemitech.net.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vf.yuexingan06.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vw.szsharing.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sk.gzmigu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://al.9csxet.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dq.gzmigu.cn

[I07] 忽略大小写与多行模式
来源：http://db.haigaiapp.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://si.newstarts.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sz.jianghongdianzi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dw.nicolike.cn

TS:   /error/gim
来源：http://tf.yuntaijiaju.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fj.huixinmuqiang.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://az.yuntaijiaju.cn

Ruby: s.scan(/error/i)
来源：http://uv.chemitech.net.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://px.huixiangedu.cn

[I08] 贪婪与非贪婪匹配
来源：http://rx.colortex.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ze.shxzskj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lr.shtwfgs.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fa.bookmarksfly.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dw.szxytkj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://dk.shxzukj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ol.huixiangedu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zy.bjjhwx.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bq.wgjwhj.cn

================================================================================
来源：http://cq.szsharing.cn

J. 日期与时间
来源：http://kc.521024.cn

================================================================================
来源：http://am.huixiangedu.cn

[J01] 获取当前时间
来源：http://zx.chemitech.net.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://gm.haigaiapp.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qz.chemitech.net.cn

JS:   new Date();  Date.now()
来源：http://bp.huixiangedu.cn

TS:   new Date();  Date.now()
来源：http://nl.jctech888.com.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ss.gzmigu.cn

Go:   time.Now()
来源：http://pq.lnxyls.cn

Ruby: Time.now
来源：http://in.shxzukj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ey.haigaiapp.cn

[J02] 格式化输出
来源：http://hr.nszjky.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qw.wgjwhj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xl.nszjky.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://au.bjjhwx.cn

TS:   d.toISOString()
来源：http://aa.shtwfgs.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jz.huixinmuqiang.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vo.huixinmuqiang.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ad.9csxet.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qy.szsharing.cn

[J03] 字符串解析为日期
来源：http://tc.haigaiapp.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://he.newstarts.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://us.nszjky.cn

JS:   new Date("2024-01-02")
来源：http://sr.asd995.cn

TS:   new Date("2024-01-02")
来源：http://rq.hnjuh.cn

Java: LocalDate.parse("2024-01-02")
来源：http://oo.shxzskj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zq.jctech888.com.cn

Ruby: Date.parse("2024-01-02")
来源：http://lb.shtwfgs.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://st.yuntaijiaju.cn

[J04] 时间戳与日期互转
来源：http://eb.newstarts.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tm.szxytkj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vn.hnjuh.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qa.nicolike.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://vh.nszjky.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dn.yuexingan06.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://um.9csxet.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tw.nicolike.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xr.muxihuayi.cn

[J05] 时间加减（加 7 天）
来源：http://ha.chemitech.net.cn

Py:   now + timedelta(days=7)
来源：http://lu.hahajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ms.szsharing.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fc.nicolike.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wn.shxzskj.cn

Java: LocalDate.now().plusDays(7)
来源：http://ev.gzmigu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ip.shxzukj.cn

Ruby: Time.now + 7 * 86400
来源：http://ni.muxihuayi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://wj.yuntaijiaju.cn

[J06] 计算两时间之差
来源：http://ex.hahajie.cn

Py:   (end - start).total_seconds()
来源：http://yj.lnxyls.cn

PHP:  $end->diff($start)->days;
来源：http://tg.haigaiapp.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qg.yuexingan06.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pr.nicolike.cn

Java: Duration.between(start, end).toSeconds()
来源：http://au.panjiajie.cn

Go:   end.Sub(start).Hours()
来源：http://gk.szsharing.cn

Ruby: end - start                 # 返回秒数
来源：http://xd.huanxung.cn

C#:   (end - start).TotalSeconds
来源：http://io.szsharing.cn

[J07] 比较两个日期
来源：http://ei.jianghongdianzi.cn

Py:   d1 < d2;  d1 == d2
来源：http://tf.hnjuh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kh.nicolike.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qk.lnxyls.cn

TS:   d1.getTime() < d2.getTime()
来源：http://zv.wgjwhj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wz.hahajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ds.huixinmuqiang.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ns.shtwfgs.cn

C#:   d1 < d2;  d1 == d2
来源：http://mn.colortex.cn

[J08] 提取年月日与星期
来源：http://yi.huixinmuqiang.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://py.szsharing.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fx.jctech888.com.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://az.chemitech.net.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://es.yuexingan06.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://na.shtwfgs.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xh.hnjuh.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gf.yuexingan06.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zn.nszjky.cn

[J09] 时区处理
来源：http://pz.jianghongdianzi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://af.shxzukj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://aa.muxihuayi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ps.asd995.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oe.szsharing.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cb.bjjhwx.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tx.huixiangedu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://jy.asd995.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wd.521024.cn

[J10] 取今天 / 本月第一天
来源：http://om.nszjky.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://av.lnxyls.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ys.hahajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sd.hahajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zb.shxzukj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://if.yuntaijiaju.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dk.nszjky.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ta.muxihuayi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bg.szsharing.cn

================================================================================
来源：http://at.521024.cn

K. JSON 与序列化
来源：http://sm.shxzukj.cn

================================================================================
来源：http://ut.asd995.cn

[K01] 对象转 JSON 字符串
来源：http://rd.huixiangedu.cn


<!-- 参考信息 -->