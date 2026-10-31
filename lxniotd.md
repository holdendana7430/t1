代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://ae.szxytkj.cn

Ruby: def to_s; @name; end
来源：http://rn.newstarts.cn

C#:   public override string ToString() => Name;
来源：http://jg.colortex.cn

[G13] 判断对象类型
来源：http://vp.gzmigu.cn

Py:   isinstance(u, User)
来源：http://wy.9csxet.cn

PHP:  $u instanceof User
来源：http://kg.szxytkj.cn

JS:   u instanceof User
来源：http://dz.huixinmuqiang.cn

TS:   u instanceof User
来源：http://zm.huixiangedu.cn

Java: u instanceof User
来源：http://yc.huixinmuqiang.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mt.shxzukj.cn

Ruby: u.is_a?(User)
来源：http://as.panjiajie.cn

C#:   u is User
来源：http://yn.chemitech.net.cn

[G14] 数据类 / record
来源：http://vs.521024.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zo.lnxyls.cn

PHP:  // 用 readonly 属性模拟
来源：http://vd.szxytkj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ow.9csxet.cn

TS:   type User = { name: string; age: number };
来源：http://un.asd995.cn

Java: record User(String name, int age) {}
来源：http://ag.szsharing.cn

Go:   type User struct { Name string; Age int }
来源：http://og.bjjhwx.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dk.yuexingan06.cn

C#:   record User(string Name, int Age);
来源：http://ln.jctech888.com.cn

[G15] 枚举
来源：http://ql.521024.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fy.hnjuh.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://nx.nszjky.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dz.lnxyls.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bp.shxzskj.cn

Java: enum Color { RED, GREEN }
来源：http://fz.huanxung.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://on.asd995.cn

Ruby: Color = %i[red green].freeze
来源：http://px.panjiajie.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://iu.huixinmuqiang.cn

[G16] 对象转数组 / 字典
来源：http://xz.bookmarksfly.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dq.huanxung.cn

PHP:  get_object_vars($obj);
来源：http://ot.asd995.cn

JS:   Object.entries(obj)
来源：http://tr.shxzukj.cn

TS:   Object.entries(obj)
来源：http://ky.yuntaijiaju.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gf.yuntaijiaju.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://it.yuntaijiaju.cn

Ruby: obj.instance_variables
来源：http://sz.newstarts.cn

C#:   // 用反射或 System.Text.Json
来源：http://ot.jctech888.com.cn

================================================================================
来源：http://yv.hahajie.cn

H. 异常与错误处理
来源：http://re.jianghongdianzi.cn

================================================================================
来源：http://wk.asd995.cn

[H01] try / catch 基础
来源：http://mp.newstarts.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ie.chemitech.net.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ex.szsharing.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tx.521024.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cp.hnjuh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cx.shxzukj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uf.szsharing.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ub.jianghongdianzi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://sj.muxihuayi.cn

[H02] finally / ensure 收尾
来源：http://zq.huanxung.cn

Py:   try: f()⏎finally: cleanup()
来源：http://vm.hahajie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://wj.yuntaijiaju.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://kl.nicolike.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ll.shxzskj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ah.shxzskj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ww.huixinmuqiang.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://vo.shtwfgs.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://xu.bjjhwx.cn

[H03] 主动抛出异常
来源：http://uh.bjjhwx.cn

Py:   raise ValueError("错误信息")
来源：http://fa.521024.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ft.gzmigu.cn

JS:   throw new Error("错误信息");
来源：http://lw.wgjwhj.cn

TS:   throw new Error("错误信息");
来源：http://js.bjjhwx.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://gp.lnxyls.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xk.bookmarksfly.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://yd.hahajie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ux.shxzukj.cn

[H04] 自定义异常类型
来源：http://ey.nicolike.cn

Py:   class MyError(Exception): pass
来源：http://pk.hnjuh.cn

PHP:  class MyError extends RuntimeException {}
来源：http://jg.bookmarksfly.cn

JS:   class MyError extends Error {}
来源：http://of.hnjuh.cn

TS:   class MyError extends Error {}
来源：http://ls.huixiangedu.cn

Java: class MyException extends RuntimeException {}
来源：http://fe.yuntaijiaju.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pl.lnxyls.cn

Ruby: class MyError < StandardError; end
来源：http://ax.huixinmuqiang.cn

C#:   class MyException : Exception {}
来源：http://pb.newstarts.cn

[H05] 捕获特定类型
来源：http://tt.chemitech.net.cn

Py:   except ValueError as e:
来源：http://as.bookmarksfly.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qy.lnxyls.cn

JS:   if (e instanceof TypeError) {}
来源：http://rh.gzmigu.cn

TS:   if (e instanceof TypeError) {}
来源：http://ja.szsharing.cn

Java: catch (IOException | SQLException e) {}
来源：http://lp.hahajie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cz.huanxung.cn

Ruby: rescue ArgumentError => e
来源：http://ef.nszjky.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kp.nszjky.cn

[H06] 可选值 / 空值安全访问
来源：http://yc.szxytkj.cn

Py:   value = d.get("k") or default
来源：http://rw.szsharing.cn

PHP:  $v = $d["k"] ?? null;
来源：http://fi.szxytkj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://wc.hnjuh.cn

TS:   obj?.a?.b;  d ?? default
来源：http://mi.haigaiapp.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tv.huanxung.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://mw.gzmigu.cn

Ruby: d&.dig(:a, :b)
来源：http://yf.chemitech.net.cn

C#:   obj?.A?.B ?? default
来源：http://mk.shxzskj.cn

[H07] 断言
来源：http://ed.szxytkj.cn

Py:   assert x > 0, "必须为正"
来源：http://hx.huixinmuqiang.cn

PHP:  assert($x > 0);
来源：http://mz.hahajie.cn

JS:   console.assert(x > 0);
来源：http://lc.hahajie.cn

TS:   console.assert(x > 0);
来源：http://ts.521024.cn

Java: assert x > 0 : "必须为正";
来源：http://vr.muxihuayi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://oz.huixiangedu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://qi.lnxyls.cn

C#:   Debug.Assert(x > 0);
来源：http://no.chemitech.net.cn

[H08] 获取错误信息与堆栈
来源：http://lh.yuntaijiaju.cn

Py:   str(e);  traceback.format_exc()
来源：http://io.521024.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xm.521024.cn

JS:   e.message;  e.stack
来源：http://pz.yuntaijiaju.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://yn.yuntaijiaju.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://bm.colortex.cn

Go:   err.Error()
来源：http://mg.gzmigu.cn

Ruby: e.message;  e.backtrace
来源：http://xa.shxzukj.cn

C#:   e.Message;  e.StackTrace
来源：http://wi.shxzukj.cn

[H09] 带错误码的异常
来源：http://wo.bookmarksfly.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kz.huixinmuqiang.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ns.9csxet.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ew.nszjky.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zo.gzmigu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://aa.colortex.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ik.huixinmuqiang.cn

Ruby: raise MyError.new("fail", 500)
来源：http://je.shtwfgs.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://pk.nicolike.cn

[H10] 资源自动释放
来源：http://sc.shtwfgs.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://xa.nicolike.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ai.haigaiapp.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yg.shxzskj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://da.huixiangedu.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wt.shtwfgs.cn

Go:   defer f.Close()
来源：http://mt.shxzskj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://go.szxytkj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://df.huanxung.cn

================================================================================
来源：http://jp.gzmigu.cn

I. 正则表达式
来源：http://xa.newstarts.cn

================================================================================
来源：http://ow.521024.cn

[I01] 判断是否匹配
来源：http://pj.huixinmuqiang.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pt.nszjky.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xv.huixiangedu.cn

JS:   /\d+/.test(s)
来源：http://cn.shxzukj.cn

TS:   /\d+/.test(s)
来源：http://ys.lnxyls.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zr.huixiangedu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dv.huanxung.cn

Ruby: s.match?(/\d+/)
来源：http://vz.shtwfgs.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zj.chemitech.net.cn

[I02] 提取所有匹配
来源：http://aq.hahajie.cn

Py:   re.findall(r"\d+", s)
来源：http://jp.9csxet.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hi.haigaiapp.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jz.521024.cn

TS:   s.match(/\d+/g)
来源：http://gl.jctech888.com.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zr.chemitech.net.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dr.szxytkj.cn

Ruby: s.scan(/\d+/)
来源：http://mx.shxzskj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yl.huixiangedu.cn

[I03] 提取捕获分组
来源：http://ny.asd995.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jf.huixiangedu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ci.yuexingan06.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xw.wgjwhj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://oz.huanxung.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xq.9csxet.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pb.nicolike.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://za.chemitech.net.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xd.521024.cn

[I04] 正则替换
来源：http://ks.newstarts.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://av.asd995.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nl.521024.cn

JS:   s.replace(/\d+/g, "#")
来源：http://uy.yuexingan06.cn

TS:   s.replace(/\d+/g, "#")
来源：http://yk.asd995.cn

Java: s.replaceAll("\\d+", "#")
来源：http://sv.gzmigu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://bn.hnjuh.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ri.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mu.9csxet.cn

[I05] 按正则拆分
来源：http://zu.jctech888.com.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://zz.gzmigu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ug.panjiajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://mp.colortex.cn

TS:   s.split(/\s*,\s*/)
来源：http://zw.gzmigu.cn

Java: s.split("\\s*,\\s*")
来源：http://rq.jianghongdianzi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sb.521024.cn

Ruby: s.split(/\s*,\s*/)
来源：http://sn.lnxyls.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://va.9csxet.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://uk.haigaiapp.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fy.shxzukj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://np.haigaiapp.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://re.huixinmuqiang.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fo.chemitech.net.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://et.huanxung.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jo.panjiajie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lr.bjjhwx.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ls.huixinmuqiang.cn

[I07] 忽略大小写与多行模式
来源：http://gh.szsharing.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rc.jianghongdianzi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ck.gzmigu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gd.hahajie.cn

TS:   /error/gim
来源：http://ay.wgjwhj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xz.jianghongdianzi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ic.asd995.cn

Ruby: s.scan(/error/i)
来源：http://ep.nicolike.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jg.szxytkj.cn

[I08] 贪婪与非贪婪匹配
来源：http://oe.bjjhwx.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qz.panjiajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vh.yuexingan06.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mu.wgjwhj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gl.lnxyls.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://hy.huixinmuqiang.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ad.bjjhwx.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vl.shxzukj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qs.muxihuayi.cn

================================================================================
来源：http://ki.shxzukj.cn

J. 日期与时间
来源：http://fz.gzmigu.cn

================================================================================
来源：http://of.szsharing.cn

[J01] 获取当前时间
来源：http://ah.bjjhwx.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://gm.yuexingan06.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mb.yuexingan06.cn

JS:   new Date();  Date.now()
来源：http://qa.gzmigu.cn

TS:   new Date();  Date.now()
来源：http://fc.hahajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://lw.gzmigu.cn

Go:   time.Now()
来源：http://bw.asd995.cn

Ruby: Time.now
来源：http://jj.szsharing.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vy.hnjuh.cn

[J02] 格式化输出
来源：http://mh.nszjky.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nf.bjjhwx.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gx.huanxung.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://az.bjjhwx.cn

TS:   d.toISOString()
来源：http://pz.nszjky.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ow.shtwfgs.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rd.wgjwhj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mt.shtwfgs.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://as.huixiangedu.cn

[J03] 字符串解析为日期
来源：http://qh.yuexingan06.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gz.yuexingan06.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ak.wgjwhj.cn

JS:   new Date("2024-01-02")
来源：http://tp.wgjwhj.cn

TS:   new Date("2024-01-02")
来源：http://jj.muxihuayi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://sc.chemitech.net.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rd.bjjhwx.cn

Ruby: Date.parse("2024-01-02")
来源：http://cx.szsharing.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nd.panjiajie.cn

[J04] 时间戳与日期互转
来源：http://po.haigaiapp.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rm.gzmigu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yy.haigaiapp.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yy.chemitech.net.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://hy.shxzukj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rb.huanxung.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://my.521024.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vj.yuexingan06.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xp.jianghongdianzi.cn

[J05] 时间加减（加 7 天）
来源：http://ws.lnxyls.cn

Py:   now + timedelta(days=7)
来源：http://cr.nicolike.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://jz.panjiajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mk.jctech888.com.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kw.jianghongdianzi.cn

Java: LocalDate.now().plusDays(7)
来源：http://is.colortex.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ay.chemitech.net.cn

Ruby: Time.now + 7 * 86400
来源：http://ps.shxzukj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://wt.asd995.cn

[J06] 计算两时间之差
来源：http://cq.panjiajie.cn

Py:   (end - start).total_seconds()
来源：http://zh.nszjky.cn

PHP:  $end->diff($start)->days;
来源：http://cj.huixinmuqiang.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://er.hahajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://it.lnxyls.cn

Java: Duration.between(start, end).toSeconds()
来源：http://dx.nicolike.cn

Go:   end.Sub(start).Hours()
来源：http://eq.shxzskj.cn

Ruby: end - start                 # 返回秒数
来源：http://jv.chemitech.net.cn

C#:   (end - start).TotalSeconds
来源：http://ic.szxytkj.cn

[J07] 比较两个日期
来源：http://wv.yuntaijiaju.cn

Py:   d1 < d2;  d1 == d2
来源：http://hl.huixinmuqiang.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zc.yuntaijiaju.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vs.wgjwhj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://yu.huixiangedu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nb.wgjwhj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jo.panjiajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ze.panjiajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://ww.muxihuayi.cn

[J08] 提取年月日与星期
来源：http://xv.szxytkj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vj.wgjwhj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jn.jianghongdianzi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://np.nicolike.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ua.hnjuh.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://my.colortex.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cv.521024.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nn.lnxyls.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jf.colortex.cn

[J09] 时区处理
来源：http://el.521024.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cn.szsharing.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ok.yuexingan06.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ea.jctech888.com.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zo.521024.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mh.szsharing.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ve.szxytkj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://py.wgjwhj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://di.wgjwhj.cn

[J10] 取今天 / 本月第一天
来源：http://ef.hnjuh.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://me.gzmigu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ws.szsharing.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://at.hnjuh.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://to.shxzukj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fw.szsharing.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://px.szsharing.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cd.shtwfgs.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ih.wgjwhj.cn


<!-- 参考信息 -->