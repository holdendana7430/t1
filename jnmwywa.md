代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://pg.nicolike.cn

Ruby: def to_s; @name; end
来源：http://ku.bookmarksfly.cn

C#:   public override string ToString() => Name;
来源：http://ig.huixiangedu.cn

[G13] 判断对象类型
来源：http://oi.newstarts.cn

Py:   isinstance(u, User)
来源：http://zm.newstarts.cn

PHP:  $u instanceof User
来源：http://tm.huixiangedu.cn

JS:   u instanceof User
来源：http://sa.jianghongdianzi.cn

TS:   u instanceof User
来源：http://bk.huanxung.cn

Java: u instanceof User
来源：http://to.yuntaijiaju.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ug.gzmigu.cn

Ruby: u.is_a?(User)
来源：http://em.chemitech.net.cn

C#:   u is User
来源：http://nw.wgjwhj.cn

[G14] 数据类 / record
来源：http://dn.hnjuh.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cx.wgjwhj.cn

PHP:  // 用 readonly 属性模拟
来源：http://rw.nicolike.cn

JS:   // 无内置：普通类或对象字面量
来源：http://mn.newstarts.cn

TS:   type User = { name: string; age: number };
来源：http://qq.bookmarksfly.cn

Java: record User(String name, int age) {}
来源：http://td.huixiangedu.cn

Go:   type User struct { Name string; Age int }
来源：http://pu.yuexingan06.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jv.nszjky.cn

C#:   record User(string Name, int Age);
来源：http://ns.bookmarksfly.cn

[G15] 枚举
来源：http://yj.9csxet.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xk.chemitech.net.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ip.521024.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://sn.szsharing.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ib.nszjky.cn

Java: enum Color { RED, GREEN }
来源：http://kr.521024.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ve.panjiajie.cn

Ruby: Color = %i[red green].freeze
来源：http://jr.colortex.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://io.szsharing.cn

[G16] 对象转数组 / 字典
来源：http://zl.muxihuayi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fe.muxihuayi.cn

PHP:  get_object_vars($obj);
来源：http://uj.gzmigu.cn

JS:   Object.entries(obj)
来源：http://tf.haigaiapp.cn

TS:   Object.entries(obj)
来源：http://li.521024.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wb.wgjwhj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://rf.huixiangedu.cn

Ruby: obj.instance_variables
来源：http://tk.nszjky.cn

C#:   // 用反射或 System.Text.Json
来源：http://kz.shtwfgs.cn

================================================================================
来源：http://af.huanxung.cn

H. 异常与错误处理
来源：http://fw.nszjky.cn

================================================================================
来源：http://os.hahajie.cn

[H01] try / catch 基础
来源：http://od.hahajie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dm.lnxyls.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gi.nicolike.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://js.yuntaijiaju.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jb.chemitech.net.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dk.hahajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://bd.9csxet.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dx.huixinmuqiang.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://un.asd995.cn

[H02] finally / ensure 收尾
来源：http://dx.nicolike.cn

Py:   try: f()⏎finally: cleanup()
来源：http://wu.asd995.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://mk.huanxung.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://zz.chemitech.net.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://nb.shxzskj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://rp.szxytkj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://kb.newstarts.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://dc.hahajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ss.521024.cn

[H03] 主动抛出异常
来源：http://oe.gzmigu.cn

Py:   raise ValueError("错误信息")
来源：http://sm.huixinmuqiang.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fi.chemitech.net.cn

JS:   throw new Error("错误信息");
来源：http://kl.chemitech.net.cn

TS:   throw new Error("错误信息");
来源：http://og.hahajie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://jt.panjiajie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://un.shxzskj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wi.asd995.cn

C#:   throw new ArgumentException("错误信息");
来源：http://cj.jctech888.com.cn

[H04] 自定义异常类型
来源：http://ui.lnxyls.cn

Py:   class MyError(Exception): pass
来源：http://rv.521024.cn

PHP:  class MyError extends RuntimeException {}
来源：http://nm.haigaiapp.cn

JS:   class MyError extends Error {}
来源：http://qx.jctech888.com.cn

TS:   class MyError extends Error {}
来源：http://zy.haigaiapp.cn

Java: class MyException extends RuntimeException {}
来源：http://ex.yuntaijiaju.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ib.gzmigu.cn

Ruby: class MyError < StandardError; end
来源：http://eu.huanxung.cn

C#:   class MyException : Exception {}
来源：http://wy.bjjhwx.cn

[H05] 捕获特定类型
来源：http://kt.gzmigu.cn

Py:   except ValueError as e:
来源：http://bh.shxzukj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hw.shtwfgs.cn

JS:   if (e instanceof TypeError) {}
来源：http://cl.nicolike.cn

TS:   if (e instanceof TypeError) {}
来源：http://wo.muxihuayi.cn

Java: catch (IOException | SQLException e) {}
来源：http://nb.nicolike.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dc.muxihuayi.cn

Ruby: rescue ArgumentError => e
来源：http://pq.lnxyls.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vw.wgjwhj.cn

[H06] 可选值 / 空值安全访问
来源：http://xr.colortex.cn

Py:   value = d.get("k") or default
来源：http://so.jianghongdianzi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://cn.yuntaijiaju.cn

JS:   obj?.a?.b;  d ?? default
来源：http://yn.shtwfgs.cn

TS:   obj?.a?.b;  d ?? default
来源：http://tg.nicolike.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vi.lnxyls.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://bf.nszjky.cn

Ruby: d&.dig(:a, :b)
来源：http://dm.521024.cn

C#:   obj?.A?.B ?? default
来源：http://jk.521024.cn

[H07] 断言
来源：http://jd.newstarts.cn

Py:   assert x > 0, "必须为正"
来源：http://ji.szxytkj.cn

PHP:  assert($x > 0);
来源：http://ge.gzmigu.cn

JS:   console.assert(x > 0);
来源：http://vv.nszjky.cn

TS:   console.assert(x > 0);
来源：http://qb.bookmarksfly.cn

Java: assert x > 0 : "必须为正";
来源：http://zu.hnjuh.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uu.yuexingan06.cn

Ruby: raise "必须为正" unless x > 0
来源：http://yf.szxytkj.cn

C#:   Debug.Assert(x > 0);
来源：http://hw.bookmarksfly.cn

[H08] 获取错误信息与堆栈
来源：http://td.521024.cn

Py:   str(e);  traceback.format_exc()
来源：http://pn.jianghongdianzi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ow.bookmarksfly.cn

JS:   e.message;  e.stack
来源：http://wf.lnxyls.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://fa.jianghongdianzi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://lf.lnxyls.cn

Go:   err.Error()
来源：http://sz.newstarts.cn

Ruby: e.message;  e.backtrace
来源：http://ij.newstarts.cn

C#:   e.Message;  e.StackTrace
来源：http://vg.huanxung.cn

[H09] 带错误码的异常
来源：http://eo.bookmarksfly.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dh.haigaiapp.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://dh.newstarts.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lk.lnxyls.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xi.chemitech.net.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kx.muxihuayi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pi.haigaiapp.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ip.szsharing.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://nn.muxihuayi.cn

[H10] 资源自动释放
来源：http://je.lnxyls.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://cl.asd995.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fr.asd995.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kf.bjjhwx.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dn.colortex.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://si.shxzskj.cn

Go:   defer f.Close()
来源：http://wc.nicolike.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jw.lnxyls.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gj.hnjuh.cn

================================================================================
来源：http://nj.hahajie.cn

I. 正则表达式
来源：http://cl.szsharing.cn

================================================================================
来源：http://xv.panjiajie.cn

[I01] 判断是否匹配
来源：http://iy.szxytkj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://oa.szsharing.cn

PHP:  preg_match('/\d+/', $s);
来源：http://dw.newstarts.cn

JS:   /\d+/.test(s)
来源：http://lk.wgjwhj.cn

TS:   /\d+/.test(s)
来源：http://zx.szsharing.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wa.nszjky.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pk.huixiangedu.cn

Ruby: s.match?(/\d+/)
来源：http://al.asd995.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yt.9csxet.cn

[I02] 提取所有匹配
来源：http://vm.colortex.cn

Py:   re.findall(r"\d+", s)
来源：http://nh.yuntaijiaju.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sd.nszjky.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://uo.jctech888.com.cn

TS:   s.match(/\d+/g)
来源：http://ek.shxzskj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ib.colortex.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pr.nszjky.cn

Ruby: s.scan(/\d+/)
来源：http://nj.bookmarksfly.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ak.shxzukj.cn

[I03] 提取捕获分组
来源：http://yg.lnxyls.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mi.shtwfgs.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vv.huixinmuqiang.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dc.szsharing.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rz.szxytkj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wk.hahajie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://oy.szsharing.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xv.newstarts.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gj.hnjuh.cn

[I04] 正则替换
来源：http://pa.huixinmuqiang.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://lc.panjiajie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fo.bjjhwx.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ex.shxzskj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://wy.nszjky.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fa.jianghongdianzi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qr.hahajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://mk.huanxung.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ys.panjiajie.cn

[I05] 按正则拆分
来源：http://pz.shtwfgs.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://rw.nszjky.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://oa.panjiajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://hu.521024.cn

TS:   s.split(/\s*,\s*/)
来源：http://vo.haigaiapp.cn

Java: s.split("\\s*,\\s*")
来源：http://vi.haigaiapp.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pb.shxzskj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://lx.shxzskj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fv.521024.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jn.huixiangedu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wq.colortex.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://py.521024.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vb.jianghongdianzi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cm.huixiangedu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zu.jctech888.com.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wu.bookmarksfly.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ho.9csxet.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ku.nszjky.cn

[I07] 忽略大小写与多行模式
来源：http://zb.haigaiapp.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://aj.bjjhwx.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ey.shxzukj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fw.asd995.cn

TS:   /error/gim
来源：http://yg.colortex.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ej.gzmigu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zy.muxihuayi.cn

Ruby: s.scan(/error/i)
来源：http://gd.gzmigu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jd.asd995.cn

[I08] 贪婪与非贪婪匹配
来源：http://ut.nszjky.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zu.szxytkj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cc.lnxyls.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ip.huixinmuqiang.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ti.lnxyls.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vc.newstarts.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ef.bjjhwx.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qg.jianghongdianzi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qw.shtwfgs.cn

================================================================================
来源：http://ek.hnjuh.cn

J. 日期与时间
来源：http://sc.yuexingan06.cn

================================================================================
来源：http://fl.521024.cn

[J01] 获取当前时间
来源：http://de.gzmigu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ak.shxzukj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hj.chemitech.net.cn

JS:   new Date();  Date.now()
来源：http://li.gzmigu.cn

TS:   new Date();  Date.now()
来源：http://pr.yuexingan06.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://mp.colortex.cn

Go:   time.Now()
来源：http://wu.hnjuh.cn

Ruby: Time.now
来源：http://lr.bookmarksfly.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gp.yuntaijiaju.cn

[J02] 格式化输出
来源：http://io.bookmarksfly.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ce.hahajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hb.hnjuh.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mt.hahajie.cn

TS:   d.toISOString()
来源：http://jl.bjjhwx.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yp.bjjhwx.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zx.huanxung.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ul.jianghongdianzi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dn.wgjwhj.cn

[J03] 字符串解析为日期
来源：http://wn.newstarts.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ex.bookmarksfly.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wg.9csxet.cn

JS:   new Date("2024-01-02")
来源：http://cn.colortex.cn

TS:   new Date("2024-01-02")
来源：http://ox.wgjwhj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://aj.nicolike.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://st.huixinmuqiang.cn

Ruby: Date.parse("2024-01-02")
来源：http://bw.jianghongdianzi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dk.wgjwhj.cn

[J04] 时间戳与日期互转
来源：http://nv.lnxyls.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kb.shxzskj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dh.panjiajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://uq.bjjhwx.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ey.9csxet.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ab.newstarts.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vu.asd995.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xv.hnjuh.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zn.nszjky.cn

[J05] 时间加减（加 7 天）
来源：http://wn.shxzskj.cn

Py:   now + timedelta(days=7)
来源：http://lp.hnjuh.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://re.huixiangedu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pi.colortex.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qk.jctech888.com.cn

Java: LocalDate.now().plusDays(7)
来源：http://qc.hnjuh.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hk.jctech888.com.cn

Ruby: Time.now + 7 * 86400
来源：http://sh.huixinmuqiang.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jq.bookmarksfly.cn

[J06] 计算两时间之差
来源：http://iy.newstarts.cn

Py:   (end - start).total_seconds()
来源：http://zv.chemitech.net.cn

PHP:  $end->diff($start)->days;
来源：http://kn.wgjwhj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pu.lnxyls.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://uz.chemitech.net.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jb.wgjwhj.cn

Go:   end.Sub(start).Hours()
来源：http://de.chemitech.net.cn

Ruby: end - start                 # 返回秒数
来源：http://zq.haigaiapp.cn

C#:   (end - start).TotalSeconds
来源：http://vk.gzmigu.cn

[J07] 比较两个日期
来源：http://il.bookmarksfly.cn

Py:   d1 < d2;  d1 == d2
来源：http://vp.yuexingan06.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qn.szsharing.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ma.shtwfgs.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xj.asd995.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bv.shtwfgs.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pk.szxytkj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qm.yuexingan06.cn

C#:   d1 < d2;  d1 == d2
来源：http://dm.szsharing.cn

[J08] 提取年月日与星期
来源：http://ru.gzmigu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yj.hahajie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ic.huixinmuqiang.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nx.szxytkj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qt.shxzukj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qv.gzmigu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://av.wgjwhj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zi.yuntaijiaju.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pj.shxzukj.cn

[J09] 时区处理
来源：http://mw.bjjhwx.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ud.panjiajie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pg.asd995.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zw.haigaiapp.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eq.hahajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ul.hnjuh.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xa.lnxyls.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://zr.huanxung.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ym.yuntaijiaju.cn

[J10] 取今天 / 本月第一天
来源：http://gc.jctech888.com.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xf.jctech888.com.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zg.bookmarksfly.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mb.nszjky.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://er.jianghongdianzi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://va.colortex.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ls.chemitech.net.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wm.9csxet.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bg.shxzskj.cn


<!-- 参考信息 -->