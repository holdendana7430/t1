代发 wailian999

Py:   isinstance(u, User)
来源：http://ir.jianghongdianzi.cn

PHP:  $u instanceof User
来源：http://qj.muxihuayi.cn

JS:   u instanceof User
来源：http://ws.colortex.cn

TS:   u instanceof User
来源：http://ia.colortex.cn

Java: u instanceof User
来源：http://vo.bookmarksfly.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://xe.lnxyls.cn

Ruby: u.is_a?(User)
来源：http://ei.shtwfgs.cn

C#:   u is User
来源：http://pz.newstarts.cn

[G14] 数据类 / record
来源：http://zl.haigaiapp.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ay.yuexingan06.cn

PHP:  // 用 readonly 属性模拟
来源：http://ey.gzmigu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ac.panjiajie.cn

TS:   type User = { name: string; age: number };
来源：http://ui.yuntaijiaju.cn

Java: record User(String name, int age) {}
来源：http://lx.jianghongdianzi.cn

Go:   type User struct { Name string; Age int }
来源：http://ul.nszjky.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pw.hnjuh.cn

C#:   record User(string Name, int Age);
来源：http://ht.jianghongdianzi.cn

[G15] 枚举
来源：http://yq.hahajie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nd.521024.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ug.shtwfgs.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rp.muxihuayi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ti.hahajie.cn

Java: enum Color { RED, GREEN }
来源：http://rk.shtwfgs.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kx.jctech888.com.cn

Ruby: Color = %i[red green].freeze
来源：http://oi.nicolike.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://el.hnjuh.cn

[G16] 对象转数组 / 字典
来源：http://jf.nicolike.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dy.9csxet.cn

PHP:  get_object_vars($obj);
来源：http://mu.colortex.cn

JS:   Object.entries(obj)
来源：http://ot.nszjky.cn

TS:   Object.entries(obj)
来源：http://up.jianghongdianzi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ba.colortex.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://rf.asd995.cn

Ruby: obj.instance_variables
来源：http://aw.hahajie.cn

C#:   // 用反射或 System.Text.Json
来源：http://ng.shtwfgs.cn

================================================================================
来源：http://sj.wgjwhj.cn

H. 异常与错误处理
来源：http://sp.huixinmuqiang.cn

================================================================================
来源：http://gf.muxihuayi.cn

[H01] try / catch 基础
来源：http://sn.yuntaijiaju.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ax.wgjwhj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ab.nszjky.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ce.newstarts.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://if.shxzukj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nv.jianghongdianzi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vq.jianghongdianzi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sp.gzmigu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://aj.shxzskj.cn

[H02] finally / ensure 收尾
来源：http://af.jctech888.com.cn

Py:   try: f()⏎finally: cleanup()
来源：http://wh.szsharing.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xq.nszjky.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://jl.521024.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://bd.huixiangedu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://bj.9csxet.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ym.chemitech.net.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://gw.asd995.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://pj.lnxyls.cn

[H03] 主动抛出异常
来源：http://qc.huixiangedu.cn

Py:   raise ValueError("错误信息")
来源：http://ge.bookmarksfly.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kv.szxytkj.cn

JS:   throw new Error("错误信息");
来源：http://od.521024.cn

TS:   throw new Error("错误信息");
来源：http://xc.gzmigu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://kw.huixiangedu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gh.521024.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://vm.hahajie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ry.newstarts.cn

[H04] 自定义异常类型
来源：http://yf.shxzukj.cn

Py:   class MyError(Exception): pass
来源：http://ez.lnxyls.cn

PHP:  class MyError extends RuntimeException {}
来源：http://xk.shtwfgs.cn

JS:   class MyError extends Error {}
来源：http://nq.asd995.cn

TS:   class MyError extends Error {}
来源：http://lc.colortex.cn

Java: class MyException extends RuntimeException {}
来源：http://fh.szsharing.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://su.hnjuh.cn

Ruby: class MyError < StandardError; end
来源：http://we.gzmigu.cn

C#:   class MyException : Exception {}
来源：http://lx.muxihuayi.cn

[H05] 捕获特定类型
来源：http://kj.asd995.cn

Py:   except ValueError as e:
来源：http://ch.shtwfgs.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dj.nicolike.cn

JS:   if (e instanceof TypeError) {}
来源：http://it.szxytkj.cn

TS:   if (e instanceof TypeError) {}
来源：http://kr.huanxung.cn

Java: catch (IOException | SQLException e) {}
来源：http://hu.jctech888.com.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jb.szxytkj.cn

Ruby: rescue ArgumentError => e
来源：http://gv.9csxet.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xn.wgjwhj.cn

[H06] 可选值 / 空值安全访问
来源：http://lp.hahajie.cn

Py:   value = d.get("k") or default
来源：http://nl.shxzskj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://pk.9csxet.cn

JS:   obj?.a?.b;  d ?? default
来源：http://yi.nicolike.cn

TS:   obj?.a?.b;  d ?? default
来源：http://sy.hahajie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://sf.nicolike.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://dk.wgjwhj.cn

Ruby: d&.dig(:a, :b)
来源：http://de.jianghongdianzi.cn

C#:   obj?.A?.B ?? default
来源：http://za.panjiajie.cn

[H07] 断言
来源：http://on.chemitech.net.cn

Py:   assert x > 0, "必须为正"
来源：http://yi.haigaiapp.cn

PHP:  assert($x > 0);
来源：http://kg.bjjhwx.cn

JS:   console.assert(x > 0);
来源：http://fl.bookmarksfly.cn

TS:   console.assert(x > 0);
来源：http://rh.muxihuayi.cn

Java: assert x > 0 : "必须为正";
来源：http://uz.huanxung.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qv.wgjwhj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://og.hahajie.cn

C#:   Debug.Assert(x > 0);
来源：http://im.szxytkj.cn

[H08] 获取错误信息与堆栈
来源：http://eu.gzmigu.cn

Py:   str(e);  traceback.format_exc()
来源：http://ks.nicolike.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://il.chemitech.net.cn

JS:   e.message;  e.stack
来源：http://sl.shxzskj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://dt.hnjuh.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://kb.nicolike.cn

Go:   err.Error()
来源：http://la.asd995.cn

Ruby: e.message;  e.backtrace
来源：http://yn.muxihuayi.cn

C#:   e.Message;  e.StackTrace
来源：http://wa.panjiajie.cn

[H09] 带错误码的异常
来源：http://cc.nszjky.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tn.huanxung.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://mb.nszjky.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://go.huixiangedu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://us.yuntaijiaju.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rw.huixiangedu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uy.jianghongdianzi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://xi.yuntaijiaju.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://nf.wgjwhj.cn

[H10] 资源自动释放
来源：http://pb.huanxung.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ge.bjjhwx.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nw.521024.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rd.yuntaijiaju.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fs.asd995.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xg.muxihuayi.cn

Go:   defer f.Close()
来源：http://oh.hahajie.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cb.haigaiapp.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tb.muxihuayi.cn

================================================================================
来源：http://lg.colortex.cn

I. 正则表达式
来源：http://vu.asd995.cn

================================================================================
来源：http://eb.shxzskj.cn

[I01] 判断是否匹配
来源：http://hi.jianghongdianzi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cj.szsharing.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vv.9csxet.cn

JS:   /\d+/.test(s)
来源：http://tm.wgjwhj.cn

TS:   /\d+/.test(s)
来源：http://ld.chemitech.net.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ib.bookmarksfly.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hu.jianghongdianzi.cn

Ruby: s.match?(/\d+/)
来源：http://rq.hnjuh.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nh.bookmarksfly.cn

[I02] 提取所有匹配
来源：http://th.asd995.cn

Py:   re.findall(r"\d+", s)
来源：http://kc.521024.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yn.hnjuh.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://sn.9csxet.cn

TS:   s.match(/\d+/g)
来源：http://eo.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sf.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ul.newstarts.cn

Ruby: s.scan(/\d+/)
来源：http://zt.hnjuh.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cr.panjiajie.cn

[I03] 提取捕获分组
来源：http://kf.hahajie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://me.yuexingan06.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yz.szsharing.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dm.muxihuayi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rf.gzmigu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ea.hahajie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://oo.bookmarksfly.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fe.9csxet.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sj.yuexingan06.cn

[I04] 正则替换
来源：http://am.chemitech.net.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://dl.szxytkj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ax.muxihuayi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://kv.9csxet.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ph.newstarts.cn

Java: s.replaceAll("\\d+", "#")
来源：http://qd.newstarts.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://nu.shxzskj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://oy.hahajie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zs.shtwfgs.cn

[I05] 按正则拆分
来源：http://co.huanxung.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://zg.9csxet.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yuntaijiaju.cn

JS:   s.split(/\s*,\s*/)
来源：http://me.huixinmuqiang.cn

TS:   s.split(/\s*,\s*/)
来源：http://sz.hahajie.cn

Java: s.split("\\s*,\\s*")
来源：http://xy.521024.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://il.panjiajie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://iu.jianghongdianzi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ia.bookmarksfly.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://af.bookmarksfly.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ge.hahajie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wy.521024.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rg.9csxet.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fh.nicolike.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lx.shtwfgs.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bh.huanxung.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mb.shxzskj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sf.szxytkj.cn

[I07] 忽略大小写与多行模式
来源：http://as.colortex.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qf.jctech888.com.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zp.asd995.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ae.9csxet.cn

TS:   /error/gim
来源：http://oe.nicolike.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jl.nszjky.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lu.9csxet.cn

Ruby: s.scan(/error/i)
来源：http://ui.muxihuayi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://db.shtwfgs.cn

[I08] 贪婪与非贪婪匹配
来源：http://tx.jctech888.com.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wm.huanxung.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ih.yuexingan06.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sj.bjjhwx.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wt.shxzukj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://tg.yuntaijiaju.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://th.szsharing.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bu.asd995.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://co.lnxyls.cn

================================================================================
来源：http://np.521024.cn

J. 日期与时间
来源：http://we.yuntaijiaju.cn

================================================================================
来源：http://wa.yuntaijiaju.cn

[J01] 获取当前时间
来源：http://mv.panjiajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://nx.9csxet.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://se.jianghongdianzi.cn

JS:   new Date();  Date.now()
来源：http://xk.9csxet.cn

TS:   new Date();  Date.now()
来源：http://hs.colortex.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zt.jctech888.com.cn

Go:   time.Now()
来源：http://zc.asd995.cn

Ruby: Time.now
来源：http://du.shxzskj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ry.newstarts.cn

[J02] 格式化输出
来源：http://hc.asd995.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ha.shxzukj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wz.asd995.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hj.muxihuayi.cn

TS:   d.toISOString()
来源：http://zx.bjjhwx.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://np.bjjhwx.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zi.gzmigu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://st.shtwfgs.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ip.hnjuh.cn

[J03] 字符串解析为日期
来源：http://pg.szxytkj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xl.panjiajie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jh.nicolike.cn

JS:   new Date("2024-01-02")
来源：http://kx.muxihuayi.cn

TS:   new Date("2024-01-02")
来源：http://og.9csxet.cn

Java: LocalDate.parse("2024-01-02")
来源：http://tn.szxytkj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://iw.9csxet.cn

Ruby: Date.parse("2024-01-02")
来源：http://ev.gzmigu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mh.jianghongdianzi.cn

[J04] 时间戳与日期互转
来源：http://dd.bookmarksfly.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://de.haigaiapp.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kx.lnxyls.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cs.huanxung.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://jv.colortex.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lz.yuexingan06.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://iq.szsharing.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bv.chemitech.net.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sq.szxytkj.cn

[J05] 时间加减（加 7 天）
来源：http://yp.jctech888.com.cn

Py:   now + timedelta(days=7)
来源：http://uz.hnjuh.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xt.nszjky.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pl.nicolike.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ve.wgjwhj.cn

Java: LocalDate.now().plusDays(7)
来源：http://ev.nszjky.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ir.shxzukj.cn

Ruby: Time.now + 7 * 86400
来源：http://pc.yuexingan06.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vp.huixiangedu.cn

[J06] 计算两时间之差
来源：http://ou.bookmarksfly.cn

Py:   (end - start).total_seconds()
来源：http://rm.bookmarksfly.cn

PHP:  $end->diff($start)->days;
来源：http://bk.hnjuh.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://et.szsharing.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dq.wgjwhj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://zz.huixinmuqiang.cn

Go:   end.Sub(start).Hours()
来源：http://xl.colortex.cn

Ruby: end - start                 # 返回秒数
来源：http://zl.hahajie.cn

C#:   (end - start).TotalSeconds
来源：http://mt.jctech888.com.cn

[J07] 比较两个日期
来源：http://nl.jianghongdianzi.cn

Py:   d1 < d2;  d1 == d2
来源：http://qi.newstarts.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ri.hnjuh.cn

JS:   d1.getTime() < d2.getTime()
来源：http://oo.bjjhwx.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xy.panjiajie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ia.muxihuayi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cf.nszjky.cn

Ruby: d1 < d2;  d1 == d2
来源：http://kt.huanxung.cn

C#:   d1 < d2;  d1 == d2
来源：http://ip.wgjwhj.cn

[J08] 提取年月日与星期
来源：http://pa.hnjuh.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pl.muxihuayi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nj.wgjwhj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lk.newstarts.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vm.haigaiapp.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cy.yuexingan06.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pv.szsharing.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ko.jianghongdianzi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kw.szsharing.cn

[J09] 时区处理
来源：http://mf.hahajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://or.gzmigu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zw.jianghongdianzi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qw.hahajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://aa.nicolike.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ay.521024.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ol.lnxyls.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://lr.nszjky.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://on.lnxyls.cn

[J10] 取今天 / 本月第一天
来源：http://vx.shxzskj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://oq.yuexingan06.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cn.shxzukj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uj.asd995.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pr.szsharing.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ii.521024.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rt.huixiangedu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uv.wgjwhj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ud.huixiangedu.cn

================================================================================
来源：http://zb.hahajie.cn

K. JSON 与序列化
来源：http://bc.nszjky.cn

================================================================================
来源：http://ml.wgjwhj.cn

[K01] 对象转 JSON 字符串
来源：http://dr.hahajie.cn


<!-- 参考信息 -->