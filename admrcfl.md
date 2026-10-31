代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://vd.huanxung.cn

Ruby: def to_s; @name; end
来源：http://rs.chemitech.net.cn

C#:   public override string ToString() => Name;
来源：http://ud.shxzukj.cn

[G13] 判断对象类型
来源：http://kb.yuexingan06.cn

Py:   isinstance(u, User)
来源：http://ny.bookmarksfly.cn

PHP:  $u instanceof User
来源：http://gx.szxytkj.cn

JS:   u instanceof User
来源：http://ii.bjjhwx.cn

TS:   u instanceof User
来源：http://dm.huanxung.cn

Java: u instanceof User
来源：http://vc.bookmarksfly.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://nr.521024.cn

Ruby: u.is_a?(User)
来源：http://pw.hnjuh.cn

C#:   u is User
来源：http://li.haigaiapp.cn

[G14] 数据类 / record
来源：http://tn.huixiangedu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://us.shxzskj.cn

PHP:  // 用 readonly 属性模拟
来源：http://fi.huanxung.cn

JS:   // 无内置：普通类或对象字面量
来源：http://xu.521024.cn

TS:   type User = { name: string; age: number };
来源：http://po.gzmigu.cn

Java: record User(String name, int age) {}
来源：http://aw.gzmigu.cn

Go:   type User struct { Name string; Age int }
来源：http://rc.jianghongdianzi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://it.shxzukj.cn

C#:   record User(string Name, int Age);
来源：http://yt.huixinmuqiang.cn

[G15] 枚举
来源：http://hv.hahajie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://or.shtwfgs.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ze.newstarts.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://eq.521024.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jv.huixiangedu.cn

Java: enum Color { RED, GREEN }
来源：http://er.wgjwhj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mo.huixiangedu.cn

Ruby: Color = %i[red green].freeze
来源：http://bk.muxihuayi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://iq.gzmigu.cn

[G16] 对象转数组 / 字典
来源：http://na.shxzukj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://re.bjjhwx.cn

PHP:  get_object_vars($obj);
来源：http://xc.yuntaijiaju.cn

JS:   Object.entries(obj)
来源：http://ik.bookmarksfly.cn

TS:   Object.entries(obj)
来源：http://rm.hahajie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fw.chemitech.net.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ro.bjjhwx.cn

Ruby: obj.instance_variables
来源：http://tf.shxzskj.cn

C#:   // 用反射或 System.Text.Json
来源：http://ns.colortex.cn

================================================================================
来源：http://id.huixiangedu.cn

H. 异常与错误处理
来源：http://ur.muxihuayi.cn

================================================================================
来源：http://hy.muxihuayi.cn

[H01] try / catch 基础
来源：http://og.jianghongdianzi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qy.haigaiapp.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yd.bookmarksfly.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jj.lnxyls.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ig.hnjuh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gf.jianghongdianzi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://su.9csxet.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kx.gzmigu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ap.shxzskj.cn

[H02] finally / ensure 收尾
来源：http://ho.hnjuh.cn

Py:   try: f()⏎finally: cleanup()
来源：http://nq.huixiangedu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://cw.shxzskj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://pk.hahajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ei.asd995.cn

Java: try { f(); } finally { cleanup(); }
来源：http://km.yuntaijiaju.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://by.muxihuayi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://se.yuexingan06.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://tb.szsharing.cn

[H03] 主动抛出异常
来源：http://zb.huixinmuqiang.cn

Py:   raise ValueError("错误信息")
来源：http://ax.hnjuh.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hj.521024.cn

JS:   throw new Error("错误信息");
来源：http://ad.lnxyls.cn

TS:   throw new Error("错误信息");
来源：http://lv.gzmigu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qn.hahajie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ea.muxihuayi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://sl.shxzukj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://xs.shxzskj.cn

[H04] 自定义异常类型
来源：http://gx.huanxung.cn

Py:   class MyError(Exception): pass
来源：http://rd.shxzukj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ho.hnjuh.cn

JS:   class MyError extends Error {}
来源：http://af.huixinmuqiang.cn

TS:   class MyError extends Error {}
来源：http://lf.chemitech.net.cn

Java: class MyException extends RuntimeException {}
来源：http://ak.szsharing.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://we.muxihuayi.cn

Ruby: class MyError < StandardError; end
来源：http://bw.bookmarksfly.cn

C#:   class MyException : Exception {}
来源：http://fc.bjjhwx.cn

[H05] 捕获特定类型
来源：http://fd.huixiangedu.cn

Py:   except ValueError as e:
来源：http://qz.wgjwhj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zn.jianghongdianzi.cn

JS:   if (e instanceof TypeError) {}
来源：http://np.shxzskj.cn

TS:   if (e instanceof TypeError) {}
来源：http://cm.bookmarksfly.cn

Java: catch (IOException | SQLException e) {}
来源：http://os.jianghongdianzi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qd.bookmarksfly.cn

Ruby: rescue ArgumentError => e
来源：http://ht.nszjky.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.bjjhwx.cn

[H06] 可选值 / 空值安全访问
来源：http://jx.9csxet.cn

Py:   value = d.get("k") or default
来源：http://cg.nszjky.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rg.wgjwhj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ik.shxzskj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://un.9csxet.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://oj.muxihuayi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://it.lnxyls.cn

Ruby: d&.dig(:a, :b)
来源：http://kr.521024.cn

C#:   obj?.A?.B ?? default
来源：http://gh.huixiangedu.cn

[H07] 断言
来源：http://mt.panjiajie.cn

Py:   assert x > 0, "必须为正"
来源：http://tb.shxzukj.cn

PHP:  assert($x > 0);
来源：http://bl.colortex.cn

JS:   console.assert(x > 0);
来源：http://oj.huixinmuqiang.cn

TS:   console.assert(x > 0);
来源：http://cb.lnxyls.cn

Java: assert x > 0 : "必须为正";
来源：http://oz.huanxung.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vh.bjjhwx.cn

Ruby: raise "必须为正" unless x > 0
来源：http://mz.9csxet.cn

C#:   Debug.Assert(x > 0);
来源：http://vy.lnxyls.cn

[H08] 获取错误信息与堆栈
来源：http://xd.shxzskj.cn

Py:   str(e);  traceback.format_exc()
来源：http://pb.bookmarksfly.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cl.yuexingan06.cn

JS:   e.message;  e.stack
来源：http://gc.huanxung.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://zy.newstarts.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://xm.shxzukj.cn

Go:   err.Error()
来源：http://yf.jianghongdianzi.cn

Ruby: e.message;  e.backtrace
来源：http://ex.lnxyls.cn

C#:   e.Message;  e.StackTrace
来源：http://eo.colortex.cn

[H09] 带错误码的异常
来源：http://nf.bjjhwx.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bz.gzmigu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ia.hnjuh.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cy.hahajie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://to.szsharing.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sf.521024.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kz.9csxet.cn

Ruby: raise MyError.new("fail", 500)
来源：http://pk.chemitech.net.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://wx.shxzskj.cn

[H10] 资源自动释放
来源：http://mw.lnxyls.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://of.jctech888.com.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bk.jianghongdianzi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://py.jianghongdianzi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rl.asd995.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://iu.jctech888.com.cn

Go:   defer f.Close()
来源：http://al.shxzskj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ag.muxihuayi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wk.9csxet.cn

================================================================================
来源：http://uv.huixiangedu.cn

I. 正则表达式
来源：http://aw.gzmigu.cn

================================================================================
来源：http://on.gzmigu.cn

[I01] 判断是否匹配
来源：http://ct.muxihuayi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lx.bjjhwx.cn

PHP:  preg_match('/\d+/', $s);
来源：http://oy.panjiajie.cn

JS:   /\d+/.test(s)
来源：http://ck.szxytkj.cn

TS:   /\d+/.test(s)
来源：http://yo.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://df.asd995.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tk.nicolike.cn

Ruby: s.match?(/\d+/)
来源：http://ka.521024.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sn.bjjhwx.cn

[I02] 提取所有匹配
来源：http://xg.haigaiapp.cn

Py:   re.findall(r"\d+", s)
来源：http://qi.gzmigu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dv.hnjuh.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://uj.huixiangedu.cn

TS:   s.match(/\d+/g)
来源：http://zh.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dc.hahajie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://os.bookmarksfly.cn

Ruby: s.scan(/\d+/)
来源：http://wv.jctech888.com.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bc.colortex.cn

[I03] 提取捕获分组
来源：http://ys.newstarts.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vm.huixiangedu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mi.yuntaijiaju.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zp.gzmigu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://le.asd995.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gq.nicolike.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rg.jctech888.com.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://is.jianghongdianzi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sx.bookmarksfly.cn

[I04] 正则替换
来源：http://on.hnjuh.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hv.lnxyls.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hf.9csxet.cn

JS:   s.replace(/\d+/g, "#")
来源：http://hg.muxihuayi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://qt.huixinmuqiang.cn

Java: s.replaceAll("\\d+", "#")
来源：http://kd.huixinmuqiang.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://nd.colortex.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://yv.muxihuayi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ug.bookmarksfly.cn

[I05] 按正则拆分
来源：http://qo.jctech888.com.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://mj.jctech888.com.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://py.colortex.cn

JS:   s.split(/\s*,\s*/)
来源：http://ho.muxihuayi.cn

TS:   s.split(/\s*,\s*/)
来源：http://kn.bjjhwx.cn

Java: s.split("\\s*,\\s*")
来源：http://db.bjjhwx.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lg.wgjwhj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://co.gzmigu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tm.huanxung.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lj.colortex.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rj.hnjuh.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gf.colortex.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qr.shtwfgs.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ub.hahajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wk.panjiajie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://od.huanxung.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cg.yuexingan06.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pl.colortex.cn

[I07] 忽略大小写与多行模式
来源：http://sb.jctech888.com.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yt.chemitech.net.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uw.bookmarksfly.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pk.521024.cn

TS:   /error/gim
来源：http://md.521024.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cn.newstarts.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pq.wgjwhj.cn

Ruby: s.scan(/error/i)
来源：http://is.colortex.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://uz.hnjuh.cn

[I08] 贪婪与非贪婪匹配
来源：http://pm.nszjky.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vt.lnxyls.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dl.chemitech.net.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yi.huixinmuqiang.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lt.huixinmuqiang.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://wj.hnjuh.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://va.gzmigu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://em.nszjky.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://oz.huixinmuqiang.cn

================================================================================
来源：http://in.shxzskj.cn

J. 日期与时间
来源：http://ei.hahajie.cn

================================================================================
来源：http://rw.gzmigu.cn

[J01] 获取当前时间
来源：http://ip.szsharing.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ob.szxytkj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jt.newstarts.cn

JS:   new Date();  Date.now()
来源：http://qn.asd995.cn

TS:   new Date();  Date.now()
来源：http://ys.yuexingan06.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rt.bjjhwx.cn

Go:   time.Now()
来源：http://uc.chemitech.net.cn

Ruby: Time.now
来源：http://jb.nicolike.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fj.wgjwhj.cn

[J02] 格式化输出
来源：http://ax.huixinmuqiang.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://te.newstarts.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fd.hahajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xd.szsharing.cn

TS:   d.toISOString()
来源：http://kw.shtwfgs.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rn.wgjwhj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lz.hnjuh.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cq.asd995.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xq.gzmigu.cn

[J03] 字符串解析为日期
来源：http://fa.hahajie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xi.panjiajie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ol.chemitech.net.cn

JS:   new Date("2024-01-02")
来源：http://xj.huixiangedu.cn

TS:   new Date("2024-01-02")
来源：http://kw.newstarts.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ct.yuexingan06.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rp.szsharing.cn

Ruby: Date.parse("2024-01-02")
来源：http://af.haigaiapp.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pp.huixiangedu.cn

[J04] 时间戳与日期互转
来源：http://wn.bjjhwx.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mp.hahajie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jl.yuntaijiaju.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zt.huanxung.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fm.huixiangedu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pj.lnxyls.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jv.bjjhwx.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wa.yuntaijiaju.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hu.chemitech.net.cn

[J05] 时间加减（加 7 天）
来源：http://vt.lnxyls.cn

Py:   now + timedelta(days=7)
来源：http://zh.521024.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vz.gzmigu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lb.muxihuayi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://po.huixiangedu.cn

Java: LocalDate.now().plusDays(7)
来源：http://vv.gzmigu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yq.haigaiapp.cn

Ruby: Time.now + 7 * 86400
来源：http://fp.asd995.cn

C#:   DateTime.Now.AddDays(7)
来源：http://tb.hahajie.cn

[J06] 计算两时间之差
来源：http://ds.hnjuh.cn

Py:   (end - start).total_seconds()
来源：http://vo.huanxung.cn

PHP:  $end->diff($start)->days;
来源：http://lt.huanxung.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ey.haigaiapp.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dt.lnxyls.cn

Java: Duration.between(start, end).toSeconds()
来源：http://at.panjiajie.cn

Go:   end.Sub(start).Hours()
来源：http://mx.jianghongdianzi.cn

Ruby: end - start                 # 返回秒数
来源：http://xk.panjiajie.cn

C#:   (end - start).TotalSeconds
来源：http://wj.hnjuh.cn

[J07] 比较两个日期
来源：http://yz.nszjky.cn

Py:   d1 < d2;  d1 == d2
来源：http://xp.huixiangedu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yx.asd995.cn

JS:   d1.getTime() < d2.getTime()
来源：http://km.shxzskj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://rj.shtwfgs.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://am.nszjky.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ld.lnxyls.cn

Ruby: d1 < d2;  d1 == d2
来源：http://kq.wgjwhj.cn

C#:   d1 < d2;  d1 == d2
来源：http://vq.9csxet.cn

[J08] 提取年月日与星期
来源：http://ru.jianghongdianzi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gn.yuntaijiaju.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://do.wgjwhj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ak.bookmarksfly.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qx.szxytkj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ag.huixinmuqiang.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fb.nicolike.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tk.colortex.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jo.gzmigu.cn

[J09] 时区处理
来源：http://ve.shxzukj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qk.huanxung.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xc.shxzskj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dh.bookmarksfly.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rd.shtwfgs.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://og.lnxyls.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fj.yuntaijiaju.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qp.muxihuayi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jh.jctech888.com.cn

[J10] 取今天 / 本月第一天
来源：http://hw.huixiangedu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://kv.bjjhwx.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wd.huixinmuqiang.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pl.hnjuh.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kn.nicolike.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hq.muxihuayi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dm.wgjwhj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ay.chemitech.net.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mj.huixinmuqiang.cn


<!-- 参考信息 -->