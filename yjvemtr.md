代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://br.haigaiapp.cn

Ruby: def to_s; @name; end
来源：http://uc.chemitech.net.cn

C#:   public override string ToString() => Name;
来源：http://gg.chemitech.net.cn

[G13] 判断对象类型
来源：http://dx.huixinmuqiang.cn

Py:   isinstance(u, User)
来源：http://mp.jianghongdianzi.cn

PHP:  $u instanceof User
来源：http://hc.chemitech.net.cn

JS:   u instanceof User
来源：http://pp.gzmigu.cn

TS:   u instanceof User
来源：http://ps.bookmarksfly.cn

Java: u instanceof User
来源：http://ky.muxihuayi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://uy.szsharing.cn

Ruby: u.is_a?(User)
来源：http://ak.9csxet.cn

C#:   u is User
来源：http://fr.bookmarksfly.cn

[G14] 数据类 / record
来源：http://zm.jianghongdianzi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qd.szsharing.cn

PHP:  // 用 readonly 属性模拟
来源：http://qg.huanxung.cn

JS:   // 无内置：普通类或对象字面量
来源：http://co.chemitech.net.cn

TS:   type User = { name: string; age: number };
来源：http://rm.shxzukj.cn

Java: record User(String name, int age) {}
来源：http://pa.shtwfgs.cn

Go:   type User struct { Name string; Age int }
来源：http://kq.haigaiapp.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yq.521024.cn

C#:   record User(string Name, int Age);
来源：http://rg.hnjuh.cn

[G15] 枚举
来源：http://xs.9csxet.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qo.wgjwhj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://mm.huixiangedu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bj.shxzukj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mf.shtwfgs.cn

Java: enum Color { RED, GREEN }
来源：http://ta.hahajie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kj.shxzskj.cn

Ruby: Color = %i[red green].freeze
来源：http://ss.newstarts.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gr.shxzukj.cn

[G16] 对象转数组 / 字典
来源：http://au.yuexingan06.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lk.asd995.cn

PHP:  get_object_vars($obj);
来源：http://hp.huanxung.cn

JS:   Object.entries(obj)
来源：http://mf.bookmarksfly.cn

TS:   Object.entries(obj)
来源：http://ip.yuntaijiaju.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://uc.haigaiapp.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://em.haigaiapp.cn

Ruby: obj.instance_variables
来源：http://ch.panjiajie.cn

C#:   // 用反射或 System.Text.Json
来源：http://lx.jianghongdianzi.cn

================================================================================
来源：http://yt.newstarts.cn

H. 异常与错误处理
来源：http://mm.huixiangedu.cn

================================================================================
来源：http://rj.chemitech.net.cn

[H01] try / catch 基础
来源：http://zp.bookmarksfly.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mu.lnxyls.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://go.lnxyls.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://db.hnjuh.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mw.jctech888.com.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zk.hahajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jg.colortex.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bq.chemitech.net.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vf.haigaiapp.cn

[H02] finally / ensure 收尾
来源：http://ma.gzmigu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://dw.colortex.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://fl.jianghongdianzi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://xh.colortex.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ry.shxzskj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://cu.szxytkj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://wd.521024.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://jb.9csxet.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://uz.yuexingan06.cn

[H03] 主动抛出异常
来源：http://jp.shxzskj.cn

Py:   raise ValueError("错误信息")
来源：http://kg.newstarts.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tp.huixiangedu.cn

JS:   throw new Error("错误信息");
来源：http://ku.shxzskj.cn

TS:   throw new Error("错误信息");
来源：http://mw.nicolike.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ly.newstarts.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ih.lnxyls.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://nh.shxzukj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://yd.nszjky.cn

[H04] 自定义异常类型
来源：http://nm.gzmigu.cn

Py:   class MyError(Exception): pass
来源：http://kw.huixiangedu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://sc.9csxet.cn

JS:   class MyError extends Error {}
来源：http://ic.asd995.cn

TS:   class MyError extends Error {}
来源：http://iv.haigaiapp.cn

Java: class MyException extends RuntimeException {}
来源：http://jv.jianghongdianzi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ir.chemitech.net.cn

Ruby: class MyError < StandardError; end
来源：http://cr.haigaiapp.cn

C#:   class MyException : Exception {}
来源：http://fq.jctech888.com.cn

[H05] 捕获特定类型
来源：http://oz.hnjuh.cn

Py:   except ValueError as e:
来源：http://jx.yuexingan06.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nq.shxzukj.cn

JS:   if (e instanceof TypeError) {}
来源：http://ec.hnjuh.cn

TS:   if (e instanceof TypeError) {}
来源：http://gz.yuntaijiaju.cn

Java: catch (IOException | SQLException e) {}
来源：http://jz.nszjky.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qx.shxzukj.cn

Ruby: rescue ArgumentError => e
来源：http://lc.szsharing.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://it.hahajie.cn

[H06] 可选值 / 空值安全访问
来源：http://om.lnxyls.cn

Py:   value = d.get("k") or default
来源：http://kw.nicolike.cn

PHP:  $v = $d["k"] ?? null;
来源：http://tl.nicolike.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ry.521024.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ws.panjiajie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bx.9csxet.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ll.521024.cn

Ruby: d&.dig(:a, :b)
来源：http://wk.wgjwhj.cn

C#:   obj?.A?.B ?? default
来源：http://oz.haigaiapp.cn

[H07] 断言
来源：http://gw.yuntaijiaju.cn

Py:   assert x > 0, "必须为正"
来源：http://to.asd995.cn

PHP:  assert($x > 0);
来源：http://dv.jianghongdianzi.cn

JS:   console.assert(x > 0);
来源：http://en.shxzskj.cn

TS:   console.assert(x > 0);
来源：http://sn.muxihuayi.cn

Java: assert x > 0 : "必须为正";
来源：http://hp.bjjhwx.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ay.yuexingan06.cn

Ruby: raise "必须为正" unless x > 0
来源：http://lo.asd995.cn

C#:   Debug.Assert(x > 0);
来源：http://nd.szsharing.cn

[H08] 获取错误信息与堆栈
来源：http://ty.lnxyls.cn

Py:   str(e);  traceback.format_exc()
来源：http://hz.haigaiapp.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ke.chemitech.net.cn

JS:   e.message;  e.stack
来源：http://go.colortex.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pu.huixiangedu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://sv.yuexingan06.cn

Go:   err.Error()
来源：http://sa.szsharing.cn

Ruby: e.message;  e.backtrace
来源：http://zu.9csxet.cn

C#:   e.Message;  e.StackTrace
来源：http://to.huixinmuqiang.cn

[H09] 带错误码的异常
来源：http://kz.colortex.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xp.gzmigu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://cw.yuexingan06.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hh.gzmigu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://td.yuexingan06.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ky.newstarts.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tg.yuexingan06.cn

Ruby: raise MyError.new("fail", 500)
来源：http://wd.shxzukj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://mm.shxzskj.cn

[H10] 资源自动释放
来源：http://qd.nszjky.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lp.colortex.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tj.panjiajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ji.panjiajie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ur.szsharing.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://uo.chemitech.net.cn

Go:   defer f.Close()
来源：http://zy.bookmarksfly.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vl.gzmigu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://el.yuntaijiaju.cn

================================================================================
来源：http://oz.lnxyls.cn

I. 正则表达式
来源：http://uu.nszjky.cn

================================================================================
来源：http://ed.hnjuh.cn

[I01] 判断是否匹配
来源：http://kz.bookmarksfly.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jo.hnjuh.cn

PHP:  preg_match('/\d+/', $s);
来源：http://du.muxihuayi.cn

JS:   /\d+/.test(s)
来源：http://ge.muxihuayi.cn

TS:   /\d+/.test(s)
来源：http://vg.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ij.bjjhwx.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dw.lnxyls.cn

Ruby: s.match?(/\d+/)
来源：http://bu.lnxyls.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pg.wgjwhj.cn

[I02] 提取所有匹配
来源：http://gq.panjiajie.cn

Py:   re.findall(r"\d+", s)
来源：http://xs.bjjhwx.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://md.yuexingan06.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pg.yuntaijiaju.cn

TS:   s.match(/\d+/g)
来源：http://gi.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zn.521024.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tb.huixiangedu.cn

Ruby: s.scan(/\d+/)
来源：http://ba.szsharing.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tj.bookmarksfly.cn

[I03] 提取捕获分组
来源：http://ud.asd995.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ru.jctech888.com.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wz.szxytkj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dt.nszjky.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vt.bookmarksfly.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ww.colortex.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bb.jianghongdianzi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zj.szxytkj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jv.shxzukj.cn

[I04] 正则替换
来源：http://lf.bookmarksfly.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://en.hnjuh.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tv.huixinmuqiang.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pn.newstarts.cn

TS:   s.replace(/\d+/g, "#")
来源：http://wu.huixiangedu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://od.chemitech.net.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qv.huanxung.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://tw.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dt.jianghongdianzi.cn

[I05] 按正则拆分
来源：http://gf.yuexingan06.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://sm.bookmarksfly.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xv.nszjky.cn

JS:   s.split(/\s*,\s*/)
来源：http://ya.9csxet.cn

TS:   s.split(/\s*,\s*/)
来源：http://dn.chemitech.net.cn

Java: s.split("\\s*,\\s*")
来源：http://nw.gzmigu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rv.9csxet.cn

Ruby: s.split(/\s*,\s*/)
来源：http://fj.lnxyls.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rh.nszjky.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rv.yuexingan06.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dz.panjiajie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zx.gzmigu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://im.colortex.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wf.yuexingan06.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lk.bjjhwx.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fi.shxzskj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://la.shxzskj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nk.hahajie.cn

[I07] 忽略大小写与多行模式
来源：http://ay.haigaiapp.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gq.huixiangedu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ox.521024.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ol.muxihuayi.cn

TS:   /error/gim
来源：http://ru.huixinmuqiang.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bt.haigaiapp.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zd.hahajie.cn

Ruby: s.scan(/error/i)
来源：http://zy.muxihuayi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://an.asd995.cn

[I08] 贪婪与非贪婪匹配
来源：http://oq.szxytkj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://uy.nszjky.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rs.yuexingan06.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://es.nszjky.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ut.panjiajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://nr.lnxyls.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yv.muxihuayi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rl.nszjky.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pu.asd995.cn

================================================================================
来源：http://bo.panjiajie.cn

J. 日期与时间
来源：http://vv.yuntaijiaju.cn

================================================================================
来源：http://ar.wgjwhj.cn

[J01] 获取当前时间
来源：http://nu.gzmigu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://nb.521024.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gh.shxzskj.cn

JS:   new Date();  Date.now()
来源：http://oz.nszjky.cn

TS:   new Date();  Date.now()
来源：http://wp.yuexingan06.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://br.521024.cn

Go:   time.Now()
来源：http://uh.521024.cn

Ruby: Time.now
来源：http://dt.haigaiapp.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://uq.hahajie.cn

[J02] 格式化输出
来源：http://vb.panjiajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://te.huixinmuqiang.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://js.asd995.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yh.9csxet.cn

TS:   d.toISOString()
来源：http://vt.szxytkj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rg.bookmarksfly.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qs.nicolike.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gy.hahajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pv.nicolike.cn

[J03] 字符串解析为日期
来源：http://yh.hnjuh.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xx.haigaiapp.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hd.wgjwhj.cn

JS:   new Date("2024-01-02")
来源：http://ls.hahajie.cn

TS:   new Date("2024-01-02")
来源：http://cg.nicolike.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jv.huixiangedu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qi.shtwfgs.cn

Ruby: Date.parse("2024-01-02")
来源：http://fw.asd995.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://eo.huanxung.cn

[J04] 时间戳与日期互转
来源：http://py.yuntaijiaju.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gh.hnjuh.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ok.shtwfgs.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gm.szxytkj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ap.huixiangedu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sp.huanxung.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hf.yuexingan06.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ku.wgjwhj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bt.chemitech.net.cn

[J05] 时间加减（加 7 天）
来源：http://md.colortex.cn

Py:   now + timedelta(days=7)
来源：http://fk.haigaiapp.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vl.wgjwhj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://om.wgjwhj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mm.muxihuayi.cn

Java: LocalDate.now().plusDays(7)
来源：http://tz.bjjhwx.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hd.colortex.cn

Ruby: Time.now + 7 * 86400
来源：http://jd.nszjky.cn

C#:   DateTime.Now.AddDays(7)
来源：http://py.gzmigu.cn

[J06] 计算两时间之差
来源：http://rx.521024.cn

Py:   (end - start).total_seconds()
来源：http://jm.wgjwhj.cn

PHP:  $end->diff($start)->days;
来源：http://ae.hnjuh.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gr.nszjky.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fu.colortex.cn

Java: Duration.between(start, end).toSeconds()
来源：http://by.gzmigu.cn

Go:   end.Sub(start).Hours()
来源：http://my.colortex.cn

Ruby: end - start                 # 返回秒数
来源：http://ch.chemitech.net.cn

C#:   (end - start).TotalSeconds
来源：http://ry.hnjuh.cn

[J07] 比较两个日期
来源：http://um.szsharing.cn

Py:   d1 < d2;  d1 == d2
来源：http://vt.szsharing.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://iy.shtwfgs.cn

JS:   d1.getTime() < d2.getTime()
来源：http://te.panjiajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ge.nszjky.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jt.hahajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qy.asd995.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ua.lnxyls.cn

C#:   d1 < d2;  d1 == d2
来源：http://wq.521024.cn

[J08] 提取年月日与星期
来源：http://jq.asd995.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dn.gzmigu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wv.szsharing.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://uz.jianghongdianzi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pt.muxihuayi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wk.nszjky.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qf.haigaiapp.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://og.gzmigu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uq.szsharing.cn

[J09] 时区处理
来源：http://pb.bookmarksfly.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dw.shxzskj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bm.yuntaijiaju.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qh.haigaiapp.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oa.521024.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jq.521024.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://iq.nicolike.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://sd.colortex.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bu.nszjky.cn

[J10] 取今天 / 本月第一天
来源：http://gp.colortex.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://nc.huixiangedu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hg.huixinmuqiang.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xv.nszjky.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lu.wgjwhj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ql.bjjhwx.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mi.wgjwhj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fb.nicolike.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://of.nszjky.cn


<!-- 参考信息 -->