代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://nm.newstarts.cn

Ruby: def to_s; @name; end
来源：http://lj.bjjhwx.cn

C#:   public override string ToString() => Name;
来源：http://mq.yuntaijiaju.cn

[G13] 判断对象类型
来源：http://wz.jctech888.com.cn

Py:   isinstance(u, User)
来源：http://wf.huixinmuqiang.cn

PHP:  $u instanceof User
来源：http://xw.shxzskj.cn

JS:   u instanceof User
来源：http://dt.huixiangedu.cn

TS:   u instanceof User
来源：http://mi.huixinmuqiang.cn

Java: u instanceof User
来源：http://yd.shxzukj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://gi.hnjuh.cn

Ruby: u.is_a?(User)
来源：http://pp.jctech888.com.cn

C#:   u is User
来源：http://la.colortex.cn

[G14] 数据类 / record
来源：http://da.szsharing.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mg.yuexingan06.cn

PHP:  // 用 readonly 属性模拟
来源：http://lr.asd995.cn

JS:   // 无内置：普通类或对象字面量
来源：http://dg.huixiangedu.cn

TS:   type User = { name: string; age: number };
来源：http://qz.yuntaijiaju.cn

Java: record User(String name, int age) {}
来源：http://ju.hahajie.cn

Go:   type User struct { Name string; Age int }
来源：http://zq.szxytkj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hq.newstarts.cn

C#:   record User(string Name, int Age);
来源：http://ho.newstarts.cn

[G15] 枚举
来源：http://as.yuntaijiaju.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ja.haigaiapp.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rr.shxzskj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kr.newstarts.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nz.muxihuayi.cn

Java: enum Color { RED, GREEN }
来源：http://ub.wgjwhj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://je.panjiajie.cn

Ruby: Color = %i[red green].freeze
来源：http://ku.panjiajie.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ta.muxihuayi.cn

[G16] 对象转数组 / 字典
来源：http://zw.yuntaijiaju.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ux.szsharing.cn

PHP:  get_object_vars($obj);
来源：http://xi.yuexingan06.cn

JS:   Object.entries(obj)
来源：http://uc.shxzukj.cn

TS:   Object.entries(obj)
来源：http://pf.nicolike.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kn.colortex.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://dq.chemitech.net.cn

Ruby: obj.instance_variables
来源：http://jf.szxytkj.cn

C#:   // 用反射或 System.Text.Json
来源：http://cz.asd995.cn

================================================================================
来源：http://av.szsharing.cn

H. 异常与错误处理
来源：http://dj.colortex.cn

================================================================================
来源：http://bg.huanxung.cn

[H01] try / catch 基础
来源：http://zp.szxytkj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ds.shtwfgs.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://il.shxzukj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yx.gzmigu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pz.bookmarksfly.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ks.shxzukj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kk.jctech888.com.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dl.bjjhwx.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lz.huixinmuqiang.cn

[H02] finally / ensure 收尾
来源：http://pu.bjjhwx.cn

Py:   try: f()⏎finally: cleanup()
来源：http://eq.haigaiapp.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://zo.jctech888.com.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://lg.hnjuh.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://cl.chemitech.net.cn

Java: try { f(); } finally { cleanup(); }
来源：http://vd.szsharing.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://cn.9csxet.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hn.hnjuh.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://wl.hahajie.cn

[H03] 主动抛出异常
来源：http://ti.huanxung.cn

Py:   raise ValueError("错误信息")
来源：http://jw.lnxyls.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mf.lnxyls.cn

JS:   throw new Error("错误信息");
来源：http://se.bjjhwx.cn

TS:   throw new Error("错误信息");
来源：http://lf.lnxyls.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ku.521024.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lo.colortex.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://eu.521024.cn

C#:   throw new ArgumentException("错误信息");
来源：http://iq.panjiajie.cn

[H04] 自定义异常类型
来源：http://fk.shxzukj.cn

Py:   class MyError(Exception): pass
来源：http://cl.jctech888.com.cn

PHP:  class MyError extends RuntimeException {}
来源：http://wd.jianghongdianzi.cn

JS:   class MyError extends Error {}
来源：http://tr.jctech888.com.cn

TS:   class MyError extends Error {}
来源：http://tb.nszjky.cn

Java: class MyException extends RuntimeException {}
来源：http://eg.asd995.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://eu.yuntaijiaju.cn

Ruby: class MyError < StandardError; end
来源：http://jr.newstarts.cn

C#:   class MyException : Exception {}
来源：http://wm.hahajie.cn

[H05] 捕获特定类型
来源：http://yj.hnjuh.cn

Py:   except ValueError as e:
来源：http://se.szsharing.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ok.521024.cn

JS:   if (e instanceof TypeError) {}
来源：http://wc.haigaiapp.cn

TS:   if (e instanceof TypeError) {}
来源：http://td.asd995.cn

Java: catch (IOException | SQLException e) {}
来源：http://tz.jctech888.com.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ed.shtwfgs.cn

Ruby: rescue ArgumentError => e
来源：http://nk.bjjhwx.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vv.yuntaijiaju.cn

[H06] 可选值 / 空值安全访问
来源：http://ah.nszjky.cn

Py:   value = d.get("k") or default
来源：http://ur.huixinmuqiang.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ou.wgjwhj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://gp.asd995.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ay.shxzukj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yx.szxytkj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://yr.huixiangedu.cn

Ruby: d&.dig(:a, :b)
来源：http://hx.jctech888.com.cn

C#:   obj?.A?.B ?? default
来源：http://ke.yuntaijiaju.cn

[H07] 断言
来源：http://cq.bjjhwx.cn

Py:   assert x > 0, "必须为正"
来源：http://kd.nicolike.cn

PHP:  assert($x > 0);
来源：http://zs.huixinmuqiang.cn

JS:   console.assert(x > 0);
来源：http://dg.9csxet.cn

TS:   console.assert(x > 0);
来源：http://wk.yuntaijiaju.cn

Java: assert x > 0 : "必须为正";
来源：http://ji.jianghongdianzi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://py.haigaiapp.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ny.nicolike.cn

C#:   Debug.Assert(x > 0);
来源：http://vv.asd995.cn

[H08] 获取错误信息与堆栈
来源：http://oo.9csxet.cn

Py:   str(e);  traceback.format_exc()
来源：http://jp.yuntaijiaju.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://oq.muxihuayi.cn

JS:   e.message;  e.stack
来源：http://yl.lnxyls.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://py.hnjuh.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://lk.shtwfgs.cn

Go:   err.Error()
来源：http://wh.szsharing.cn

Ruby: e.message;  e.backtrace
来源：http://an.colortex.cn

C#:   e.Message;  e.StackTrace
来源：http://yw.hahajie.cn

[H09] 带错误码的异常
来源：http://wh.chemitech.net.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cn.bookmarksfly.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ej.shtwfgs.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mi.colortex.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hl.yuexingan06.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ln.chemitech.net.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://am.521024.cn

Ruby: raise MyError.new("fail", 500)
来源：http://tp.colortex.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ke.szxytkj.cn

[H10] 资源自动释放
来源：http://ig.bjjhwx.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://hn.lnxyls.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tn.hahajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zr.huixiangedu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://oy.9csxet.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pz.chemitech.net.cn

Go:   defer f.Close()
来源：http://bo.jianghongdianzi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://st.nszjky.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ps.lnxyls.cn

================================================================================
来源：http://nt.asd995.cn

I. 正则表达式
来源：http://sp.nszjky.cn

================================================================================
来源：http://cv.chemitech.net.cn

[I01] 判断是否匹配
来源：http://dn.huixiangedu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pg.shtwfgs.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gb.shxzskj.cn

JS:   /\d+/.test(s)
来源：http://lf.521024.cn

TS:   /\d+/.test(s)
来源：http://yj.chemitech.net.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ru.muxihuayi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://po.shtwfgs.cn

Ruby: s.match?(/\d+/)
来源：http://ne.shtwfgs.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://uo.colortex.cn

[I02] 提取所有匹配
来源：http://nc.yuexingan06.cn

Py:   re.findall(r"\d+", s)
来源：http://nb.szxytkj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://km.huixinmuqiang.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ab.bookmarksfly.cn

TS:   s.match(/\d+/g)
来源：http://tw.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xx.huixiangedu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ot.hnjuh.cn

Ruby: s.scan(/\d+/)
来源：http://gx.shxzskj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ew.asd995.cn

[I03] 提取捕获分组
来源：http://hi.yuexingan06.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rf.szxytkj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xu.huanxung.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nf.panjiajie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fe.shxzskj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://aj.huixinmuqiang.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jp.panjiajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lg.huixinmuqiang.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qe.newstarts.cn

[I04] 正则替换
来源：http://em.521024.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jt.bjjhwx.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sz.jianghongdianzi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://sh.chemitech.net.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xp.hahajie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://dj.huixiangedu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://sc.colortex.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://tv.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vy.jctech888.com.cn

[I05] 按正则拆分
来源：http://nd.chemitech.net.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://bj.shxzukj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yj.huixiangedu.cn

JS:   s.split(/\s*,\s*/)
来源：http://pb.muxihuayi.cn

TS:   s.split(/\s*,\s*/)
来源：http://cs.colortex.cn

Java: s.split("\\s*,\\s*")
来源：http://qt.521024.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rq.nszjky.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ki.hahajie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ke.muxihuayi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xh.newstarts.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yx.jianghongdianzi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jb.shtwfgs.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zt.haigaiapp.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://el.colortex.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xb.shtwfgs.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nh.9csxet.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ga.yuntaijiaju.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tu.huixinmuqiang.cn

[I07] 忽略大小写与多行模式
来源：http://db.nicolike.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mq.hnjuh.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wm.shtwfgs.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sj.panjiajie.cn

TS:   /error/gim
来源：http://qt.wgjwhj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pd.bjjhwx.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://np.newstarts.cn

Ruby: s.scan(/error/i)
来源：http://km.newstarts.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gv.yuntaijiaju.cn

[I08] 贪婪与非贪婪匹配
来源：http://an.haigaiapp.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ok.bookmarksfly.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://il.nszjky.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ph.lnxyls.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hy.newstarts.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ci.chemitech.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yo.yuntaijiaju.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mx.nszjky.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hj.jianghongdianzi.cn

================================================================================
来源：http://hm.521024.cn

J. 日期与时间
来源：http://mx.huixinmuqiang.cn

================================================================================
来源：http://hk.panjiajie.cn

[J01] 获取当前时间
来源：http://ts.jctech888.com.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ww.shtwfgs.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dr.jctech888.com.cn

JS:   new Date();  Date.now()
来源：http://gj.haigaiapp.cn

TS:   new Date();  Date.now()
来源：http://ym.521024.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rr.jianghongdianzi.cn

Go:   time.Now()
来源：http://bk.lnxyls.cn

Ruby: Time.now
来源：http://gv.shxzskj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mj.wgjwhj.cn

[J02] 格式化输出
来源：http://hq.jctech888.com.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ww.lnxyls.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ih.jianghongdianzi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zj.yuntaijiaju.cn

TS:   d.toISOString()
来源：http://iz.colortex.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xj.hahajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bj.shtwfgs.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bf.newstarts.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ge.newstarts.cn

[J03] 字符串解析为日期
来源：http://dp.jctech888.com.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://uk.lnxyls.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://aq.jctech888.com.cn

JS:   new Date("2024-01-02")
来源：http://ra.panjiajie.cn

TS:   new Date("2024-01-02")
来源：http://jz.shxzukj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zx.chemitech.net.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://sa.yuexingan06.cn

Ruby: Date.parse("2024-01-02")
来源：http://vp.lnxyls.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wo.yuntaijiaju.cn

[J04] 时间戳与日期互转
来源：http://jb.newstarts.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qx.wgjwhj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://og.bjjhwx.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ba.hnjuh.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://nd.colortex.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rv.shxzukj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xk.wgjwhj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lf.newstarts.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bm.yuexingan06.cn

[J05] 时间加减（加 7 天）
来源：http://qd.colortex.cn

Py:   now + timedelta(days=7)
来源：http://ls.hnjuh.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://zz.nszjky.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vt.huixinmuqiang.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://eq.yuntaijiaju.cn

Java: LocalDate.now().plusDays(7)
来源：http://gu.bookmarksfly.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ng.nicolike.cn

Ruby: Time.now + 7 * 86400
来源：http://fh.huixinmuqiang.cn

C#:   DateTime.Now.AddDays(7)
来源：http://wo.huixiangedu.cn

[J06] 计算两时间之差
来源：http://rl.bjjhwx.cn

Py:   (end - start).total_seconds()
来源：http://dh.huanxung.cn

PHP:  $end->diff($start)->days;
来源：http://yq.yuntaijiaju.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ir.wgjwhj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lm.newstarts.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bh.521024.cn

Go:   end.Sub(start).Hours()
来源：http://ez.521024.cn

Ruby: end - start                 # 返回秒数
来源：http://ni.lnxyls.cn

C#:   (end - start).TotalSeconds
来源：http://vu.lnxyls.cn

[J07] 比较两个日期
来源：http://df.yuntaijiaju.cn

Py:   d1 < d2;  d1 == d2
来源：http://tj.nszjky.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cd.bjjhwx.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ir.muxihuayi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://rj.huixiangedu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kp.yuntaijiaju.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fz.9csxet.cn

Ruby: d1 < d2;  d1 == d2
来源：http://yf.asd995.cn

C#:   d1 < d2;  d1 == d2
来源：http://ai.newstarts.cn

[J08] 提取年月日与星期
来源：http://na.szsharing.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pj.hnjuh.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mh.huixiangedu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lx.hnjuh.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://oz.hahajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ch.jctech888.com.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nv.colortex.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jn.huixinmuqiang.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nj.szsharing.cn

[J09] 时区处理
来源：http://kt.nicolike.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qa.521024.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://up.newstarts.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nq.hahajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tb.yuexingan06.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ew.nszjky.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://si.lnxyls.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ak.521024.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://oi.9csxet.cn

[J10] 取今天 / 本月第一天
来源：http://xz.hahajie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ep.521024.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pv.nicolike.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://np.hahajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ju.muxihuayi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lp.haigaiapp.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://id.yuntaijiaju.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wu.shxzskj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ke.shxzskj.cn


<!-- 参考信息 -->